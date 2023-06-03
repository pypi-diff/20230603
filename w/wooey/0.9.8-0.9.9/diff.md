# Comparing `tmp/wooey-0.9.8.tar.gz` & `tmp/wooey-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wooey-0.9.8.tar", last modified: Mon Jan  2 03:00:18 2017, max compression
+gzip compressed data, was "dist/wooey-0.9.9.tar", last modified: Thu Sep  7 03:13:22 2017, max compression
```

## Comparing `wooey-0.9.8.tar` & `wooey-0.9.9.tar`

### file list

```diff
@@ -1,199 +1,198 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/
--rw-rw-r--   0 chris     (1000) chris     (1000)       59 2017-01-02 03:00:18.000000 wooey-0.9.8/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)     1458 2017-01-02 03:00:01.000000 wooey-0.9.8/setup.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      193 2016-10-16 14:27:05.000000 wooey-0.9.8/MANIFEST.in
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/scripts/
--rw-rw-r--   0 chris     (1000) chris     (1000)      188 2017-01-01 21:45:05.000000 wooey-0.9.8/scripts/wooify
--rw-rw-r--   0 chris     (1000) chris     (1000)      916 2017-01-02 03:00:18.000000 wooey-0.9.8/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     1260 2016-10-16 14:27:05.000000 wooey-0.9.8/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/tests/
--rw-------   0 chris     (1000) chris     (1000)       21 2016-05-15 13:47:03.000000 wooey-0.9.8/tests/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1558 2016-10-16 14:27:05.000000 wooey-0.9.8/tests/test_project.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/models/
--rw-rw-r--   0 chris     (1000) chris     (1000)    23016 2016-10-16 14:47:38.000000 wooey-0.9.8/wooey/models/core.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1209 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/models/favorite.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1832 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/models/mixins.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      771 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/models/fields.py
--rw-rw-r--   0 chris     (1000) chris     (1000)       83 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/models/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2288 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/signals.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2541 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/test_settings.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      152 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/docs_settings.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/locale/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/locale/ja/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 chris     (1000) chris     (1000)    12130 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/locale/ja/LC_MESSAGES/django.po
--rw-rw-r--   0 chris     (1000) chris     (1000)     7258 2017-01-01 17:57:55.000000 wooey-0.9.8/wooey/locale/ja/LC_MESSAGES/django.mo
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/locale/nl/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 chris     (1000) chris     (1000)     7144 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/locale/nl/LC_MESSAGES/django.po
--rw-rw-r--   0 chris     (1000) chris     (1000)     4105 2017-01-01 17:57:55.000000 wooey-0.9.8/wooey/locale/nl/LC_MESSAGES/django.mo
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/locale/de/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/locale/de/LC_MESSAGES/
--rw-rw-r--   0 chris     (1000) chris     (1000)     7274 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 chris     (1000) chris     (1000)     4229 2017-01-01 17:57:55.000000 wooey-0.9.8/wooey/locale/de/LC_MESSAGES/django.mo
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/locale/fr/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 chris     (1000) chris     (1000)     7286 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 chris     (1000) chris     (1000)     4244 2017-01-01 17:57:55.000000 wooey-0.9.8/wooey/locale/fr/LC_MESSAGES/django.mo
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/locale/zh_Hans/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/locale/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 chris     (1000) chris     (1000)     8529 2017-01-01 17:57:45.000000 wooey-0.9.8/wooey/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-r--   0 chris     (1000) chris     (1000)     4827 2017-01-01 17:57:55.000000 wooey-0.9.8/wooey/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-r--   0 chris     (1000) chris     (1000)      525 2017-01-01 21:45:05.000000 wooey-0.9.8/wooey/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/views/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1986 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/views/favorite.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2983 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/views/authentication.py
--rw-------   0 chris     (1000) chris     (1000)     1736 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/views/mixins.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      164 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/views/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10455 2016-11-28 23:17:47.000000 wooey-0.9.8/wooey/views/wooey_celery.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10947 2016-11-28 23:17:40.000000 wooey-0.9.8/wooey/views/views.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/templates/
--rw-------   0 chris     (1000) chris     (1000)      333 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/templates/404.html
--rw-------   0 chris     (1000) chris     (1000)      333 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/templates/500.html
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/templates/wooey/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/templates/wooey/jobs/
--rw-rw-r--   0 chris     (1000) chris     (1000)    13235 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/templates/wooey/jobs/job_view.html
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/templates/wooey/jobs/results/
--rw-rw-r--   0 chris     (1000) chris     (1000)      667 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/templates/wooey/jobs/results/table_row.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     2704 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/templates/wooey/jobs/job_list.html
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/templates/wooey/scripts/
--rw-rw-r--   0 chris     (1000) chris     (1000)    12853 2017-01-01 17:10:02.000000 wooey-0.9.8/wooey/templates/wooey/scripts/script_view.html
--rw-------   0 chris     (1000) chris     (1000)      129 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/templates/wooey/scripts/scriptgroup_view.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     3046 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/templates/wooey/scripts/script_panel.html
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/templates/wooey/profile/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1056 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/templates/wooey/profile/profile.html
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/templates/wooey/preview/
--rw-------   0 chris     (1000) chris     (1000)      371 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/templates/wooey/preview/image.html
--rw-------   0 chris     (1000) chris     (1000)     1273 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/templates/wooey/preview/tabular.html
--rw-------   0 chris     (1000) chris     (1000)      245 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/templates/wooey/preview/fasta.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     1712 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/templates/wooey/preview/base.html
--rw-------   0 chris     (1000) chris     (1000)     1143 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/templates/wooey/scrapbook.html
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/templates/wooey/registration/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1644 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/templates/wooey/registration/login.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     2806 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/templates/wooey/registration/register.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      939 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/templates/wooey/registration/login_header.html
--rw-rw-r--   0 chris     (1000) chris     (1000)    21568 2017-01-01 21:45:06.000000 wooey-0.9.8/wooey/templates/wooey/base.html
--rw-rw-r--   0 chris     (1000) chris     (1000)     2117 2017-01-01 16:28:59.000000 wooey-0.9.8/wooey/templates/wooey/home.html
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/templates/wooey/modals/
--rw-------   0 chris     (1000) chris     (1000)      843 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/templates/wooey/modals/base_modal.html
--rw-------   0 chris     (1000) chris     (1000)      452 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/templates/wooey/modals/resubmit_modal.html
--rw-rw-r--   0 chris     (1000) chris     (1000)      589 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/templates/wooey/modals/permalink_modal.html
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/templatetags/
--rw-------   0 chris     (1000) chris     (1000)       21 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/templatetags/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6290 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/templatetags/wooey_tags.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/management/
--rw-------   0 chris     (1000) chris     (1000)       21 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/management/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/management/commands/
--rw-------   0 chris     (1000) chris     (1000)       21 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/management/commands/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3461 2017-01-01 17:15:36.000000 wooey-0.9.8/wooey/management/commands/addscript.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/forms/
--rw-rw-r--   0 chris     (1000) chris     (1000)      485 2016-11-28 23:17:40.000000 wooey-0.9.8/wooey/forms/fields.py
--rw-------   0 chris     (1000) chris     (1000)      106 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/forms/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)       96 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/forms/config.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      392 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/forms/scripts.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10011 2017-01-01 16:12:16.000000 wooey-0.9.8/wooey/forms/factory.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1536 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/django_compat.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/backend/
--rw-rw-r--   0 chris     (1000) chris     (1000)    30133 2017-01-01 16:12:16.000000 wooey-0.9.8/wooey/backend/utils.py
--rw-------   0 chris     (1000) chris     (1000)       39 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/backend/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4908 2017-01-01 18:32:03.000000 wooey-0.9.8/wooey/backend/command_line.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      356 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/test_urls.py
--rw-------   0 chris     (1000) chris     (1000)     2071 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/wooeystorage.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1204 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/settings.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3487 2017-01-01 21:45:05.000000 wooey-0.9.8/wooey/urls.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)     5979 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/test_models.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8415 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/test_views.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/tests/scripts/
--rwxrwxr-x   0 chris     (1000) chris     (1000)     3183 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/scripts/translate.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      329 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/scripts/command_order.py
--rwxrwxr-x   0 chris     (1000) chris     (1000)     1803 2016-06-30 12:42:18.000000 wooey-0.9.8/wooey/tests/scripts/heatmap.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      247 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/scripts/without_args.py
--rw-------   0 chris     (1000) chris     (1000)       21 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/tests/scripts/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3639 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/scripts/nested_heatmap.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      815 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/scripts/choices_2.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      809 2016-12-19 00:22:03.000000 wooey-0.9.8/wooey/tests/scripts/choices.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1788 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/scripts/mandlebrot.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      576 2016-09-02 14:29:52.000000 wooey-0.9.8/wooey/tests/scripts/threaded_prints.py
--rwxrwxr-x   0 chris     (1000) chris     (1000)     1851 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/scripts/fetch_cats.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      389 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/scripts/multi_output.py
--rwxrwxr-x   0 chris     (1000) chris     (1000)      959 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/scripts/gaussian.py
--rwxrwxr-x   0 chris     (1000) chris     (1000)     1082 2017-01-01 16:12:16.000000 wooey-0.9.8/wooey/tests/scripts/crop.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1061 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/test_commands.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2587 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/mixins.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1352 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/test_tasks.py
--rw-------   0 chris     (1000) chris     (1000)       62 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/tests/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4886 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/test_scripts.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2642 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/test_utils.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1517 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/config.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6540 2017-01-01 16:12:16.000000 wooey-0.9.8/wooey/tests/test_forms.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1519 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/factories.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1023 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tests/test_template_tags.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      584 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/version.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/static/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/static/wooey/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/static/wooey/js/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/static/wooey/js/admin/
--rw-rw-r--   0 chris     (1000) chris     (1000)      811 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/static/wooey/js/admin/script.js
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/static/wooey/css/
--rw-rw-r--   0 chris     (1000) chris     (1000)     6550 2017-01-02 02:55:56.000000 wooey-0.9.8/wooey/static/wooey/css/base.css
--rw-rw-r--   0 chris     (1000) chris     (1000)     1880 2017-01-01 21:45:05.000000 wooey-0.9.8/wooey/static/wooey/css/simple-sidebar.css
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/static/wooey/images/
--rw-------   0 chris     (1000) chris     (1000)      817 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/static/wooey/images/pinstripe.png
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/migrations/
--rw-------   0 chris     (1000) chris     (1000)      353 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/migrations/0002_remove_scriptparameter_output_path.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      414 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0016_wooeyfile_checksum.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      414 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0025_remove_script_parameter_sv.py
--rw-------   0 chris     (1000) chris     (1000)      921 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/migrations/0003_populate_from_slug.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1835 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0021_fix_verbose_names.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1507 2016-07-03 18:08:16.000000 wooey-0.9.8/wooey/migrations/0028_auto_20160703_1808.py
--rw-------   0 chris     (1000) chris     (1000)      438 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/migrations/0004_choice_limits.py
--rw-------   0 chris     (1000) chris     (1000)        0 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/migrations/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      959 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0018_userfile.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      584 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0022_add_collapse_arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      821 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0023_script_parameter_m2m.py
--rw-------   0 chris     (1000) chris     (1000)      431 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/migrations/0006_script_group_defaults.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      592 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0012_wooeyjob_uuid.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7166 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0019_userfile_data.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      416 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0007_script_documentation.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      479 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0014_wooeyjob_uuid_finalise.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      597 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0024_script_parameter_m2m_data.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1882 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0009_script_versioning.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      429 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0008_short_param_admin.py
--rw-------   0 chris     (1000) chris     (1000)     1220 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/migrations/0005_size_bytes.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1883 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0010_script_versioning_data_migration.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      517 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0013_wooeyjob_uuid_populate.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      459 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0026_rename_script_parameter_sv.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      582 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0015_hidden_parameters.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1554 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0011_script_versioning_cleanup.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      454 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0020_userfile_finalize.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      627 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0017_wooeyfile_generate_checksums.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      720 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/migrations/0027_parameter_order.py
--rw-------   0 chris     (1000) chris     (1000)     7445 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/migrations/0001_initial.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      245 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/apps.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/conf/
--rw-------   0 chris     (1000) chris     (1000)       21 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/conf/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/conf/project_template/
--rw-------   0 chris     (1000) chris     (1000)      432 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/conf/project_template/wooey_celery_app.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      360 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/conf/project_template/middleware.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/conf/project_template/settings/
--rw-rw-r--   0 chris     (1000) chris     (1000)      856 2017-01-01 21:45:05.000000 wooey-0.9.8/wooey/conf/project_template/settings/wooey_settings.py
--rw-------   0 chris     (1000) chris     (1000)       29 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/conf/project_template/settings/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3942 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/conf/project_template/settings/user_settings.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey/conf/project_template/urls/
--rw-------   0 chris     (1000) chris     (1000)      353 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/conf/project_template/urls/user_urls.py
--rw-------   0 chris     (1000) chris     (1000)       25 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/conf/project_template/urls/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      175 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/conf/project_template/urls/wooey_urls.py
--rw-------   0 chris     (1000) chris     (1000)      197 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/conf/project_template/__init__.py
--rw-------   0 chris     (1000) chris     (1000)      115 2016-05-15 13:47:03.000000 wooey-0.9.8/wooey/conf/project_template/requirements.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     1532 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/admin.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7713 2016-10-16 14:27:05.000000 wooey-0.9.8/wooey/tasks.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1468 2016-10-16 14:27:05.000000 wooey-0.9.8/LICENSE
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)       86 2017-01-02 03:00:13.000000 wooey-0.9.8/wooey.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      916 2017-01-02 03:00:13.000000 wooey-0.9.8/wooey.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     5189 2017-01-02 03:00:18.000000 wooey-0.9.8/wooey.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       12 2017-01-02 03:00:13.000000 wooey-0.9.8/wooey.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2017-01-02 03:00:13.000000 wooey-0.9.8/wooey.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       65 2017-01-02 03:00:13.000000 wooey-0.9.8/wooey.egg-info/entry_points.txt
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       59 2017-09-07 03:13:22.000000 wooey-0.9.9/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1458 2017-09-05 00:57:39.000000 wooey-0.9.9/setup.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      193 2016-10-16 14:27:05.000000 wooey-0.9.9/MANIFEST.in
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/scripts/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      188 2017-04-15 22:31:33.000000 wooey-0.9.9/scripts/wooify
+-rw-rw-r--   0 chris     (1000) chris     (1000)      916 2017-09-07 03:13:22.000000 wooey-0.9.9/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1260 2016-10-16 14:27:05.000000 wooey-0.9.9/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/tests/
+-rw-------   0 chris     (1000) chris     (1000)       21 2016-05-15 13:47:03.000000 wooey-0.9.9/tests/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1558 2016-10-16 14:27:05.000000 wooey-0.9.9/tests/test_project.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/models/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    23016 2017-09-04 22:56:02.000000 wooey-0.9.9/wooey/models/core.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1209 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/models/favorite.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1832 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/models/mixins.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      771 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/models/fields.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)       83 2017-06-04 12:43:47.000000 wooey-0.9.9/wooey/models/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2288 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/signals.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3047 2017-05-26 12:39:04.000000 wooey-0.9.9/wooey/test_settings.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      152 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/docs_settings.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/locale/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/locale/ja/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12130 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/locale/ja/LC_MESSAGES/django.po
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7258 2017-01-01 17:57:55.000000 wooey-0.9.9/wooey/locale/ja/LC_MESSAGES/django.mo
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/locale/nl/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7144 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/locale/nl/LC_MESSAGES/django.po
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4105 2017-01-01 17:57:55.000000 wooey-0.9.9/wooey/locale/nl/LC_MESSAGES/django.mo
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/locale/de/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7274 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4229 2017-01-01 17:57:55.000000 wooey-0.9.9/wooey/locale/de/LC_MESSAGES/django.mo
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/locale/fr/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7286 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4244 2017-01-01 17:57:55.000000 wooey-0.9.9/wooey/locale/fr/LC_MESSAGES/django.mo
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/locale/zh_Hans/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8529 2017-04-15 22:31:33.000000 wooey-0.9.9/wooey/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4827 2017-04-15 22:31:33.000000 wooey-0.9.9/wooey/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-r--   0 chris     (1000) chris     (1000)      525 2017-04-15 22:31:33.000000 wooey-0.9.9/wooey/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/views/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1986 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/views/favorite.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2983 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/views/authentication.py
+-rw-------   0 chris     (1000) chris     (1000)     1736 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/views/mixins.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      164 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/views/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10455 2017-04-15 22:31:33.000000 wooey-0.9.9/wooey/views/wooey_celery.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10947 2016-11-28 23:17:40.000000 wooey-0.9.9/wooey/views/views.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/templates/
+-rw-------   0 chris     (1000) chris     (1000)      333 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/templates/404.html
+-rw-------   0 chris     (1000) chris     (1000)      333 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/templates/500.html
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/templates/wooey/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/templates/wooey/jobs/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    13235 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/templates/wooey/jobs/job_view.html
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/templates/wooey/jobs/results/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      667 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/templates/wooey/jobs/results/table_row.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2704 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/templates/wooey/jobs/job_list.html
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/templates/wooey/scripts/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12853 2017-09-04 22:56:02.000000 wooey-0.9.9/wooey/templates/wooey/scripts/script_view.html
+-rw-------   0 chris     (1000) chris     (1000)      129 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/templates/wooey/scripts/scriptgroup_view.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3046 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/templates/wooey/scripts/script_panel.html
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/templates/wooey/profile/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1056 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/templates/wooey/profile/profile.html
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/templates/wooey/preview/
+-rw-------   0 chris     (1000) chris     (1000)      371 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/templates/wooey/preview/image.html
+-rw-------   0 chris     (1000) chris     (1000)     1273 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/templates/wooey/preview/tabular.html
+-rw-------   0 chris     (1000) chris     (1000)      245 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/templates/wooey/preview/fasta.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1712 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/templates/wooey/preview/base.html
+-rw-------   0 chris     (1000) chris     (1000)     1143 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/templates/wooey/scrapbook.html
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/templates/wooey/registration/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1644 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/templates/wooey/registration/login.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2806 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/templates/wooey/registration/register.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      939 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/templates/wooey/registration/login_header.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)    21568 2017-04-15 22:31:33.000000 wooey-0.9.9/wooey/templates/wooey/base.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2117 2017-01-01 16:28:59.000000 wooey-0.9.9/wooey/templates/wooey/home.html
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/templates/wooey/modals/
+-rw-------   0 chris     (1000) chris     (1000)      843 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/templates/wooey/modals/base_modal.html
+-rw-------   0 chris     (1000) chris     (1000)      452 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/templates/wooey/modals/resubmit_modal.html
+-rw-rw-r--   0 chris     (1000) chris     (1000)      589 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/templates/wooey/modals/permalink_modal.html
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/templatetags/
+-rw-------   0 chris     (1000) chris     (1000)       21 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/templatetags/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6290 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/templatetags/wooey_tags.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/management/
+-rw-------   0 chris     (1000) chris     (1000)       21 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/management/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/management/commands/
+-rw-------   0 chris     (1000) chris     (1000)       21 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/management/commands/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3461 2017-01-01 17:15:36.000000 wooey-0.9.9/wooey/management/commands/addscript.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/forms/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      485 2016-11-28 23:17:40.000000 wooey-0.9.9/wooey/forms/fields.py
+-rw-------   0 chris     (1000) chris     (1000)      106 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/forms/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)       96 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/forms/config.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      392 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/forms/scripts.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10011 2017-09-04 22:56:02.000000 wooey-0.9.9/wooey/forms/factory.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1543 2017-05-26 12:39:04.000000 wooey-0.9.9/wooey/django_compat.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/backend/
+-rw-rw-r--   0 chris     (1000) chris     (1000)    30133 2017-09-04 22:56:02.000000 wooey-0.9.9/wooey/backend/utils.py
+-rw-------   0 chris     (1000) chris     (1000)       39 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/backend/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5091 2017-05-26 12:39:04.000000 wooey-0.9.9/wooey/backend/command_line.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      457 2017-05-26 12:39:04.000000 wooey-0.9.9/wooey/test_urls.py
+-rw-------   0 chris     (1000) chris     (1000)     2071 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/wooeystorage.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1204 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/settings.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3487 2017-04-15 22:31:33.000000 wooey-0.9.9/wooey/urls.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5950 2017-05-26 12:39:04.000000 wooey-0.9.9/wooey/tests/test_models.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8415 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/test_views.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/tests/scripts/
+-rwxrwxr-x   0 chris     (1000) chris     (1000)     3183 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/scripts/translate.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      329 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/scripts/command_order.py
+-rwxrwxr-x   0 chris     (1000) chris     (1000)     1803 2016-06-30 12:42:18.000000 wooey-0.9.9/wooey/tests/scripts/heatmap.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      247 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/scripts/without_args.py
+-rw-------   0 chris     (1000) chris     (1000)       21 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/tests/scripts/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3639 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/scripts/nested_heatmap.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      815 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/scripts/choices_2.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      809 2016-12-19 00:22:03.000000 wooey-0.9.9/wooey/tests/scripts/choices.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1788 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/scripts/mandlebrot.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      576 2016-09-02 14:29:52.000000 wooey-0.9.9/wooey/tests/scripts/threaded_prints.py
+-rwxrwxr-x   0 chris     (1000) chris     (1000)     1851 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/scripts/fetch_cats.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      389 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/scripts/multi_output.py
+-rwxrwxr-x   0 chris     (1000) chris     (1000)      959 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/scripts/gaussian.py
+-rwxrwxr-x   0 chris     (1000) chris     (1000)     1082 2017-04-15 22:31:33.000000 wooey-0.9.9/wooey/tests/scripts/crop.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1061 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/test_commands.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2587 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/mixins.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1352 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/test_tasks.py
+-rw-------   0 chris     (1000) chris     (1000)       62 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/tests/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4886 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/test_scripts.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2642 2017-03-05 21:19:27.000000 wooey-0.9.9/wooey/tests/test_utils.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1517 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/config.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6540 2017-04-15 22:31:33.000000 wooey-0.9.9/wooey/tests/test_forms.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1519 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/factories.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1023 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tests/test_template_tags.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      614 2017-05-26 12:39:04.000000 wooey-0.9.9/wooey/version.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/static/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/static/wooey/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/static/wooey/js/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/static/wooey/js/admin/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      811 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/static/wooey/js/admin/script.js
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/static/wooey/css/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6550 2017-09-04 22:56:02.000000 wooey-0.9.9/wooey/static/wooey/css/base.css
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1880 2017-04-15 22:31:33.000000 wooey-0.9.9/wooey/static/wooey/css/simple-sidebar.css
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/static/wooey/images/
+-rw-------   0 chris     (1000) chris     (1000)      817 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/static/wooey/images/pinstripe.png
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/migrations/
+-rw-------   0 chris     (1000) chris     (1000)      353 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/migrations/0002_remove_scriptparameter_output_path.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      414 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0016_wooeyfile_checksum.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      414 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0025_remove_script_parameter_sv.py
+-rw-------   0 chris     (1000) chris     (1000)      921 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/migrations/0003_populate_from_slug.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1835 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0021_fix_verbose_names.py
+-rw-------   0 chris     (1000) chris     (1000)      438 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/migrations/0004_choice_limits.py
+-rw-------   0 chris     (1000) chris     (1000)        0 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/migrations/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      959 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0018_userfile.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      584 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0022_add_collapse_arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      821 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0023_script_parameter_m2m.py
+-rw-------   0 chris     (1000) chris     (1000)      431 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/migrations/0006_script_group_defaults.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      592 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0012_wooeyjob_uuid.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7166 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0019_userfile_data.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      416 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0007_script_documentation.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      479 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0014_wooeyjob_uuid_finalise.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      597 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0024_script_parameter_m2m_data.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1882 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0009_script_versioning.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      429 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0008_short_param_admin.py
+-rw-------   0 chris     (1000) chris     (1000)     1220 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/migrations/0005_size_bytes.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1883 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0010_script_versioning_data_migration.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      517 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0013_wooeyjob_uuid_populate.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      459 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0026_rename_script_parameter_sv.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      582 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0015_hidden_parameters.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1554 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0011_script_versioning_cleanup.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      454 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0020_userfile_finalize.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      627 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0017_wooeyfile_generate_checksums.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      720 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/migrations/0027_parameter_order.py
+-rw-------   0 chris     (1000) chris     (1000)     7445 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/migrations/0001_initial.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      245 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/apps.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/conf/
+-rw-------   0 chris     (1000) chris     (1000)       21 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/conf/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/conf/project_template/
+-rw-------   0 chris     (1000) chris     (1000)      432 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/conf/project_template/wooey_celery_app.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      536 2017-05-26 12:39:04.000000 wooey-0.9.9/wooey/conf/project_template/middleware.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/conf/project_template/settings/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1179 2017-05-26 12:39:04.000000 wooey-0.9.9/wooey/conf/project_template/settings/wooey_settings.py
+-rw-------   0 chris     (1000) chris     (1000)       29 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/conf/project_template/settings/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4014 2017-05-26 12:39:04.000000 wooey-0.9.9/wooey/conf/project_template/settings/user_settings.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey/conf/project_template/urls/
+-rw-------   0 chris     (1000) chris     (1000)      353 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/conf/project_template/urls/user_urls.py
+-rw-------   0 chris     (1000) chris     (1000)       25 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/conf/project_template/urls/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      175 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/conf/project_template/urls/wooey_urls.py
+-rw-------   0 chris     (1000) chris     (1000)      197 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/conf/project_template/__init__.py
+-rw-------   0 chris     (1000) chris     (1000)      115 2016-05-15 13:47:03.000000 wooey-0.9.9/wooey/conf/project_template/requirements.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1532 2017-06-04 12:43:47.000000 wooey-0.9.9/wooey/admin.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7713 2016-10-16 14:27:05.000000 wooey-0.9.9/wooey/tasks.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1468 2016-10-16 14:27:05.000000 wooey-0.9.9/LICENSE
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       86 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      916 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5145 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       12 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       65 2017-09-07 03:13:22.000000 wooey-0.9.9/wooey.egg-info/entry_points.txt
```

### Comparing `wooey-0.9.8/setup.py` & `wooey-0.9.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,19 +5,19 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='wooey',
-    version='0.9.8',
+    version='0.9.9',
     packages=find_packages(),
     scripts=['scripts/wooify'],
     entry_points={'console_scripts': ['wooify = wooey.backend.command_line:bootstrap', ]},
-    install_requires = ['Django>=1.6,<1.10', 'django-autoslug', 'django-celery', 'six', 'clinto>=0.1.3', 'celery>=3.1.15,<4.0'],
+    install_requires = ['Django>=1.6,<1.10', 'django-autoslug', 'django-celery', 'six', 'clinto>=0.1.4', 'celery>=3.1.15,<4.0'],
     include_package_data=True,
     description='A Django app which creates a web GUI and task interface for argparse scripts',
     url='http://www.github.com/wooey/wooey',
     author='Chris Mitchell <chris.mit7@gmail.com>, Martin Fitzpatrick <martin.fitzpatrick@gmail.com>',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
```

### Comparing `wooey-0.9.8/PKG-INFO` & `wooey-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wooey
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Django app which creates a web GUI and task interface for argparse scripts
 Home-page: http://www.github.com/wooey/wooey
 Author: Chris Mitchell <chris.mit7@gmail.com>, Martin Fitzpatrick <martin.fitzpatrick@gmail.com>
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `wooey-0.9.8/README.md` & `wooey-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/tests/test_project.py` & `wooey-0.9.9/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/models/core.py` & `wooey-0.9.9/wooey/models/core.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/models/favorite.py` & `wooey-0.9.9/wooey/models/favorite.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/models/mixins.py` & `wooey-0.9.9/wooey/models/mixins.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/models/fields.py` & `wooey-0.9.9/wooey/models/fields.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/signals.py` & `wooey-0.9.9/wooey/signals.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/test_settings.py` & `wooey-0.9.9/wooey/test_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,29 +35,46 @@
     'django.contrib.staticfiles.finders.AppDirectoriesFinder',
 ]
 
 STATIC_URL = '/static/'
 
 STATIC_ROOT = os.path.join(TEST_DIR, 'static')
 
+TEMPLATES = [
+    {
+        'BACKEND': 'django.template.backends.django.DjangoTemplates',
+        'DIRS': [],
+        'APP_DIRS': True,
+        'OPTIONS': {
+            'context_processors': [
+                'django.template.context_processors.debug',
+                'django.template.context_processors.request',
+                'django.contrib.auth.context_processors.auth',
+                'django.contrib.messages.context_processors.messages',
+            ],
+        },
+    },
+]
+
 MEDIA_URL = '/files/'
 MEDIA_ROOT = os.path.join(TEST_DIR, 'media')
 
 if django.VERSION[:2] < (1, 6):
     TEST_RUNNER = 'discover_runner.DiscoverRunner'
 
 SECRET_KEY = "iufoj=mibkpdz*%bob952x(%49rqgv8gg45k36kjcg76&-y5=!"
 
 PASSWORD_HASHERS = (
     'django.contrib.auth.hashers.UnsaltedMD5PasswordHasher',
 )
 
 MIDDLEWARE_CLASSES = []
+MIDDLEWARE = []
 
-ROOT_URLCONF = 'wooey.urls'
+ROOT_URLCONF = 'wooey.test_urls'
 
 WOOEY_EPHEMERAL_FILES = True
 WOOEY_CELERY = False
 WOOEY_FILE_DIR = 'wooey_test'
 
 if os.environ.get('WOOEY_TEST_S3'):
     STATICFILES_STORAGE = DEFAULT_FILE_STORAGE = 'wooey.wooeystorage.CachedS3BotoStorage'
```

### Comparing `wooey-0.9.8/wooey/locale/ja/LC_MESSAGES/django.po` & `wooey-0.9.9/wooey/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/locale/ja/LC_MESSAGES/django.mo` & `wooey-0.9.9/wooey/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/locale/nl/LC_MESSAGES/django.po` & `wooey-0.9.9/wooey/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/locale/nl/LC_MESSAGES/django.mo` & `wooey-0.9.9/wooey/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/locale/de/LC_MESSAGES/django.po` & `wooey-0.9.9/wooey/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/locale/de/LC_MESSAGES/django.mo` & `wooey-0.9.9/wooey/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/locale/fr/LC_MESSAGES/django.po` & `wooey-0.9.9/wooey/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/locale/fr/LC_MESSAGES/django.mo` & `wooey-0.9.9/wooey/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/locale/zh_Hans/LC_MESSAGES/django.po` & `wooey-0.9.9/wooey/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/locale/zh_Hans/LC_MESSAGES/django.mo` & `wooey-0.9.9/wooey/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/__init__.py` & `wooey-0.9.9/wooey/__init__.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/views/favorite.py` & `wooey-0.9.9/wooey/views/favorite.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/views/authentication.py` & `wooey-0.9.9/wooey/views/authentication.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/views/mixins.py` & `wooey-0.9.9/wooey/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/views/wooey_celery.py` & `wooey-0.9.9/wooey/views/wooey_celery.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/views/views.py` & `wooey-0.9.9/wooey/views/views.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/jobs/job_view.html` & `wooey-0.9.9/wooey/templates/wooey/jobs/job_view.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/jobs/results/table_row.html` & `wooey-0.9.9/wooey/templates/wooey/jobs/results/table_row.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/jobs/job_list.html` & `wooey-0.9.9/wooey/templates/wooey/jobs/job_list.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/scripts/script_view.html` & `wooey-0.9.9/wooey/templates/wooey/scripts/script_view.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/scripts/script_panel.html` & `wooey-0.9.9/wooey/templates/wooey/scripts/script_panel.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/profile/profile.html` & `wooey-0.9.9/wooey/templates/wooey/profile/profile.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/preview/tabular.html` & `wooey-0.9.9/wooey/templates/wooey/preview/tabular.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/preview/base.html` & `wooey-0.9.9/wooey/templates/wooey/preview/base.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/scrapbook.html` & `wooey-0.9.9/wooey/templates/wooey/scrapbook.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/registration/login.html` & `wooey-0.9.9/wooey/templates/wooey/registration/login.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/registration/register.html` & `wooey-0.9.9/wooey/templates/wooey/registration/register.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/registration/login_header.html` & `wooey-0.9.9/wooey/templates/wooey/registration/login_header.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/base.html` & `wooey-0.9.9/wooey/templates/wooey/base.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/home.html` & `wooey-0.9.9/wooey/templates/wooey/home.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/modals/base_modal.html` & `wooey-0.9.9/wooey/templates/wooey/modals/base_modal.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templates/wooey/modals/permalink_modal.html` & `wooey-0.9.9/wooey/templates/wooey/modals/permalink_modal.html`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/templatetags/wooey_tags.py` & `wooey-0.9.9/wooey/templatetags/wooey_tags.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/management/commands/addscript.py` & `wooey-0.9.9/wooey/management/commands/addscript.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/forms/factory.py` & `wooey-0.9.9/wooey/forms/factory.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/django_compat.py` & `wooey-0.9.9/wooey/django_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . version import DJANGO_VERSION, DJ18, DJ17, DJ16, DJ19
+from . version import DJANGO_VERSION, DJ18, DJ17, DJ16, DJ19, DJ110
 from django.conf import settings
 
 try:
     settings.configure()
 except RuntimeError:
     pass
```

### Comparing `wooey-0.9.8/wooey/backend/utils.py` & `wooey-0.9.9/wooey/backend/utils.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/backend/command_line.py` & `wooey-0.9.9/wooey/backend/command_line.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 import os
 import subprocess
 import shutil
 from argparse import ArgumentParser
 from django.template import Context
 
 # This is needed on django 1.9
-from .. version import DJANGO_VERSION, DJ19
+from .. version import DJANGO_VERSION, DJ19, DJ110
 if DJANGO_VERSION >= DJ19:
     from django.conf import settings
     import django
-    settings.configure()
+    extra_settings = {}
+    if DJANGO_VERSION >= DJ110:
+        extra_settings['TEMPLATES'] = [{'BACKEND': 'django.template.backends.django.DjangoTemplates',}]
+    settings.configure(**extra_settings)
     django.setup()
 
 import wooey
 
 from .. import django_compat
```

### Comparing `wooey-0.9.8/wooey/wooeystorage.py` & `wooey-0.9.9/wooey/wooeystorage.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/settings.py` & `wooey-0.9.9/wooey/settings.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/urls.py` & `wooey-0.9.9/wooey/urls.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/test_models.py` & `wooey-0.9.9/wooey/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 class ScriptGroupTestCase(TestCase):
 
     def test_script_group_creation(self):
         group = factories.ScriptGroupFactory()
 
 
 class TestJob(mixins.ScriptFactoryMixin, mixins.FileCleanupMixin, mixins.FileMixin, TestCase):
-    urls = 'wooey.test_urls'
 
     def get_local_url(self, fileinfo):
         from ..backend import utils
         local_storage = utils.get_storage(local=True)
         return local_storage.url(fileinfo['object'].filepath.name)
 
     def test_jobs(self):
```

### Comparing `wooey-0.9.8/wooey/tests/test_views.py` & `wooey-0.9.9/wooey/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/scripts/translate.py` & `wooey-0.9.9/wooey/tests/scripts/translate.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/scripts/heatmap.py` & `wooey-0.9.9/wooey/tests/scripts/heatmap.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/scripts/nested_heatmap.py` & `wooey-0.9.9/wooey/tests/scripts/nested_heatmap.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/scripts/choices_2.py` & `wooey-0.9.9/wooey/tests/scripts/choices_2.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/scripts/choices.py` & `wooey-0.9.9/wooey/tests/scripts/choices.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/scripts/mandlebrot.py` & `wooey-0.9.9/wooey/tests/scripts/mandlebrot.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/scripts/threaded_prints.py` & `wooey-0.9.9/wooey/tests/scripts/threaded_prints.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/scripts/fetch_cats.py` & `wooey-0.9.9/wooey/tests/scripts/fetch_cats.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/scripts/gaussian.py` & `wooey-0.9.9/wooey/tests/scripts/gaussian.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/scripts/crop.py` & `wooey-0.9.9/wooey/tests/scripts/crop.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/test_commands.py` & `wooey-0.9.9/wooey/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/mixins.py` & `wooey-0.9.9/wooey/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/test_tasks.py` & `wooey-0.9.9/wooey/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/test_scripts.py` & `wooey-0.9.9/wooey/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/test_utils.py` & `wooey-0.9.9/wooey/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/config.py` & `wooey-0.9.9/wooey/tests/config.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/test_forms.py` & `wooey-0.9.9/wooey/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/factories.py` & `wooey-0.9.9/wooey/tests/factories.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tests/test_template_tags.py` & `wooey-0.9.9/wooey/tests/test_template_tags.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/version.py` & `wooey-0.9.9/wooey/version.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 
 from django import get_version
 from distutils.version import StrictVersion
 DJANGO_VERSION = StrictVersion(get_version())
+DJ110 = StrictVersion('1.10')
 DJ19 = StrictVersion('1.9')
 DJ18 = StrictVersion('1.8')
 DJ17 = StrictVersion('1.7')
 DJ16 = StrictVersion('1.6')
 
 PY_FULL_VERSION = StrictVersion('{}.{}.{}'.format(sys.version_info.major, sys.version_info.minor, sys.version_info.micro))
 PY_MINOR_VERSION = StrictVersion('{}.{}'.format(sys.version_info.major, sys.version_info.minor))
```

### Comparing `wooey-0.9.8/wooey/static/wooey/js/admin/script.js` & `wooey-0.9.9/wooey/static/wooey/js/admin/script.js`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/static/wooey/css/base.css` & `wooey-0.9.9/wooey/static/wooey/css/base.css`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/static/wooey/css/simple-sidebar.css` & `wooey-0.9.9/wooey/static/wooey/css/simple-sidebar.css`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/static/wooey/images/pinstripe.png` & `wooey-0.9.9/wooey/static/wooey/images/pinstripe.png`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0003_populate_from_slug.py` & `wooey-0.9.9/wooey/migrations/0003_populate_from_slug.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0021_fix_verbose_names.py` & `wooey-0.9.9/wooey/migrations/0021_fix_verbose_names.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0018_userfile.py` & `wooey-0.9.9/wooey/migrations/0018_userfile.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0022_add_collapse_arguments.py` & `wooey-0.9.9/wooey/migrations/0022_add_collapse_arguments.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0023_script_parameter_m2m.py` & `wooey-0.9.9/wooey/migrations/0023_script_parameter_m2m.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0012_wooeyjob_uuid.py` & `wooey-0.9.9/wooey/migrations/0012_wooeyjob_uuid.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0019_userfile_data.py` & `wooey-0.9.9/wooey/migrations/0019_userfile_data.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0024_script_parameter_m2m_data.py` & `wooey-0.9.9/wooey/migrations/0024_script_parameter_m2m_data.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0009_script_versioning.py` & `wooey-0.9.9/wooey/migrations/0009_script_versioning.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0005_size_bytes.py` & `wooey-0.9.9/wooey/migrations/0005_size_bytes.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0010_script_versioning_data_migration.py` & `wooey-0.9.9/wooey/migrations/0010_script_versioning_data_migration.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0013_wooeyjob_uuid_populate.py` & `wooey-0.9.9/wooey/migrations/0013_wooeyjob_uuid_populate.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0015_hidden_parameters.py` & `wooey-0.9.9/wooey/migrations/0015_hidden_parameters.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0011_script_versioning_cleanup.py` & `wooey-0.9.9/wooey/migrations/0011_script_versioning_cleanup.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0017_wooeyfile_generate_checksums.py` & `wooey-0.9.9/wooey/migrations/0017_wooeyfile_generate_checksums.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0027_parameter_order.py` & `wooey-0.9.9/wooey/migrations/0027_parameter_order.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/migrations/0001_initial.py` & `wooey-0.9.9/wooey/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/conf/project_template/settings/wooey_settings.py` & `wooey-0.9.9/wooey/conf/project_template/settings/wooey_settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 from .django_settings import *
-from wooey.version import DJANGO_VERSION, DJ17
+from wooey.version import DJANGO_VERSION, DJ17, DJ110
 from django.utils.translation import ugettext_lazy as _
 
 INSTALLED_APPS += (
     # 'corsheaders',
     'wooey',
 )
 
+if DJANGO_VERSION < DJ110:
+    MIDDLEWARE_CLASSES = list(MIDDLEWARE_CLASSES)
+    MIDDLEWARE_CLASSES.append('{{ project_name }}.middleware.ProcessExceptionMiddleware')
+else:
+    # Using Django 1.10 +
+    MIDDLEWARE = list(MIDDLEWARE)
+    MIDDLEWARE.append('{{ project_name }}.middleware.ProcessExceptionMiddleware')
+
 LANGUAGES = [
   ('de', _('German')),
   ('en', _('English')),
   ('fr', _('French')),
   ('ja', _('Japanese')),
   ('nl', _('Dutch')),
   ('zh-hans' if DJANGO_VERSION >= DJ17 else 'zh-cn', _('Simplified Chinese')),
```

### Comparing `wooey-0.9.8/wooey/conf/project_template/settings/user_settings.py` & `wooey-0.9.9/wooey/conf/project_template/settings/user_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 #
 # INSTALLED_APPS += (
 #     'storages',
 #     'collectfast',
 # )
 
 ## We have user authentication -- we need to use https (django-sslify)
+## NOTE: This is MIDDLEWARE and not MIDDLEWARE_CLASSES in Django 1.10+!
 # if not DEBUG:
 #     MIDDLEWARE_CLASSES = ['sslify.middleware.SSLifyMiddleware']+list(MIDDLEWARE_CLASSES)
 #     SECURE_PROXY_SSL_HEADER = ('HTTP_X_FORWARDED_PROTO', 'https')
 #
 # ALLOWED_HOSTS = (
 #     'localhost',
 #     '127.0.0.1',
```

### Comparing `wooey-0.9.8/wooey/admin.py` & `wooey-0.9.9/wooey/admin.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey/tasks.py` & `wooey-0.9.9/wooey/tasks.py`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/LICENSE` & `wooey-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wooey-0.9.8/wooey.egg-info/PKG-INFO` & `wooey-0.9.9/wooey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wooey
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Django app which creates a web GUI and task interface for argparse scripts
 Home-page: http://www.github.com/wooey/wooey
 Author: Chris Mitchell <chris.mit7@gmail.com>, Martin Fitzpatrick <martin.fitzpatrick@gmail.com>
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `wooey-0.9.8/wooey.egg-info/SOURCES.txt` & `wooey-0.9.9/wooey.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 wooey/migrations/0021_fix_verbose_names.py
 wooey/migrations/0022_add_collapse_arguments.py
 wooey/migrations/0023_script_parameter_m2m.py
 wooey/migrations/0024_script_parameter_m2m_data.py
 wooey/migrations/0025_remove_script_parameter_sv.py
 wooey/migrations/0026_rename_script_parameter_sv.py
 wooey/migrations/0027_parameter_order.py
-wooey/migrations/0028_auto_20160703_1808.py
 wooey/migrations/__init__.py
 wooey/models/__init__.py
 wooey/models/core.py
 wooey/models/favorite.py
 wooey/models/fields.py
 wooey/models/mixins.py
 wooey/static/wooey/css/base.css
```

