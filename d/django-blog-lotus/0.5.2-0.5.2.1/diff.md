# Comparing `tmp/django-blog-lotus-0.5.2.tar.gz` & `tmp/django-blog-lotus-0.5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-blog-lotus-0.5.2.tar", last modified: Tue Apr  4 12:50:03 2023, max compression
+gzip compressed data, was "django-blog-lotus-0.5.2.1.tar", last modified: Sat Jun  3 01:20:31 2023, max compression
```

## Comparing `django-blog-lotus-0.5.2.tar` & `django-blog-lotus-0.5.2.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.378416 django-blog-lotus-0.5.2/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1070 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/LICENCE.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      304 2021-05-29 23:54:08.000000 django-blog-lotus-0.5.2/MANIFEST.in
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2573 2023-04-04 12:50:03.378416 django-blog-lotus-0.5.2/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1330 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/README.rst
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.370416 django-blog-lotus-0.5.2/django_blog_lotus.egg-info/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2573 2023-04-04 12:50:03.000000 django-blog-lotus-0.5.2/django_blog_lotus.egg-info/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2721 2023-04-04 12:50:03.000000 django-blog-lotus-0.5.2/django_blog_lotus.egg-info/SOURCES.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-04-04 12:50:03.000000 django-blog-lotus-0.5.2/django_blog_lotus.egg-info/dependency_links.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      322 2023-04-04 12:50:03.000000 django-blog-lotus-0.5.2/django_blog_lotus.egg-info/requires.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       14 2023-04-04 12:50:03.000000 django-blog-lotus-0.5.2/django_blog_lotus.egg-info/top_level.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-04-04 10:02:08.000000 django-blog-lotus-0.5.2/django_blog_lotus.egg-info/zip-safe
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.370416 django-blog-lotus-0.5.2/lotus/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      152 2022-12-19 01:25:34.000000 django-blog-lotus-0.5.2/lotus/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.370416 django-blog-lotus-0.5.2/lotus/admin/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      258 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/admin/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4001 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/admin/article.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2612 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/admin/category.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1418 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/admin/translated.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      231 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2/lotus/apps.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      785 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/choices.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.370416 django-blog-lotus-0.5.2/lotus/contrib/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/contrib/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1667 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2/lotus/contrib/django_configuration.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      330 2023-01-21 14:51:37.000000 django-blog-lotus-0.5.2/lotus/exceptions.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.374416 django-blog-lotus-0.5.2/lotus/factories/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      376 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/factories/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     7596 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/factories/article.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1573 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/factories/author.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2520 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/factories/category.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1592 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/factories/tag.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.374416 django-blog-lotus-0.5.2/lotus/forms/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      367 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/forms/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5662 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/forms/article.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3464 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2/lotus/forms/category.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1285 2021-10-25 23:19:15.000000 django-blog-lotus-0.5.2/lotus/forms/translated.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.374416 django-blog-lotus-0.5.2/lotus/locale/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.366416 django-blog-lotus-0.5.2/lotus/locale/de/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.374416 django-blog-lotus-0.5.2/lotus/locale/de/LC_MESSAGES/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      380 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2/lotus/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     8674 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2/lotus/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     8627 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2/lotus/locale/django.pot
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.366416 django-blog-lotus-0.5.2/lotus/locale/en/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.374416 django-blog-lotus-0.5.2/lotus/locale/en/LC_MESSAGES/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      380 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2/lotus/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     8674 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2/lotus/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.366416 django-blog-lotus-0.5.2/lotus/locale/fr/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.374416 django-blog-lotus-0.5.2/lotus/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     7232 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2/lotus/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    11353 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2/lotus/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4091 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/lookups.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.374416 django-blog-lotus-0.5.2/lotus/management/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/management/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.374416 django-blog-lotus-0.5.2/lotus/management/commands/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/management/commands/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    22425 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/management/commands/lotus_demo.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5480 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2/lotus/managers.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.374416 django-blog-lotus-0.5.2/lotus/migrations/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    12526 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/migrations/0001_initial.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-01-01 21:16:12.000000 django-blog-lotus-0.5.2/lotus/migrations/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.374416 django-blog-lotus-0.5.2/lotus/models/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      148 2021-05-29 23:54:08.000000 django-blog-lotus-0.5.2/lotus/models/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    12914 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2/lotus/models/article.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1599 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/models/author.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3232 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/models/category.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      551 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/models/translated.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      194 2022-07-04 12:22:57.000000 django-blog-lotus-0.5.2/lotus/responses.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2733 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/settings.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.366416 django-blog-lotus-0.5.2/lotus/templates/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.366416 django-blog-lotus-0.5.2/lotus/templates/admin/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.366416 django-blog-lotus-0.5.2/lotus/templates/admin/lotus/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.374416 django-blog-lotus-0.5.2/lotus/templates/admin/lotus/article/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4914 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/templates/admin/lotus/article/change_form.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1515 2023-01-16 21:53:43.000000 django-blog-lotus-0.5.2/lotus/templates/admin/lotus/article/translate_original.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.374416 django-blog-lotus-0.5.2/lotus/templates/admin/lotus/category/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1633 2022-07-04 12:22:57.000000 django-blog-lotus-0.5.2/lotus/templates/admin/lotus/category/change_form.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1519 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2/lotus/templates/admin/lotus/category/translate_original.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.378416 django-blog-lotus-0.5.2/lotus/templates/lotus/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.378416 django-blog-lotus-0.5.2/lotus/templates/lotus/article/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     9789 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/article/detail.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      752 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/article/list.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.378416 django-blog-lotus-0.5.2/lotus/templates/lotus/article/partials/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2798 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/article/partials/item.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      383 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/article/partials/siblings.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.378416 django-blog-lotus-0.5.2/lotus/templates/lotus/author/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      738 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/author/detail.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      717 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/author/list.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.378416 django-blog-lotus-0.5.2/lotus/templates/lotus/author/partials/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      340 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/author/partials/item.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      164 2022-01-02 21:03:15.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/base.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.378416 django-blog-lotus-0.5.2/lotus/templates/lotus/category/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1514 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/category/detail.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      751 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/category/list.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.378416 django-blog-lotus-0.5.2/lotus/templates/lotus/category/partials/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      587 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/category/partials/item.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      387 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/category/partials/siblings.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      613 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/pagination.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      544 2022-12-18 14:29:13.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/preview_switch.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.378416 django-blog-lotus-0.5.2/lotus/templates/lotus/tag/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      726 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/tag/detail.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      951 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/templates/lotus/tag/list.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.378416 django-blog-lotus-0.5.2/lotus/templatetags/
--rw-r--r--   0 emencia   (1001) emencia   (1001)        0 2021-07-04 20:57:38.000000 django-blog-lotus-0.5.2/lotus/templatetags/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    11813 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/templatetags/lotus.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1659 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/urls.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.378416 django-blog-lotus-0.5.2/lotus/utils/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2021-05-29 23:54:08.000000 django-blog-lotus-0.5.2/lotus/utils/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1719 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/utils/factory.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    13239 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/utils/imaging.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     8329 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2/lotus/utils/tests.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.378416 django-blog-lotus-0.5.2/lotus/views/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      768 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2/lotus/views/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 12:50:03.378416 django-blog-lotus-0.5.2/lotus/views/admin/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      300 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2/lotus/views/admin/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      295 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2/lotus/views/admin/article.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      299 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2/lotus/views/admin/category.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3770 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2/lotus/views/admin/mixins.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4610 2023-03-19 17:30:54.000000 django-blog-lotus-0.5.2/lotus/views/article.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3156 2022-12-18 15:40:32.000000 django-blog-lotus-0.5.2/lotus/views/author.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3148 2022-12-18 15:40:43.000000 django-blog-lotus-0.5.2/lotus/views/category.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5633 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2/lotus/views/mixins.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2614 2022-07-04 12:22:57.000000 django-blog-lotus-0.5.2/lotus/views/preview.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5347 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2/lotus/views/tag.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2097 2023-04-04 12:50:03.382416 django-blog-lotus-0.5.2/setup.cfg
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2021-05-29 23:54:08.000000 django-blog-lotus-0.5.2/setup.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1070 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/LICENCE.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      304 2021-05-29 23:54:08.000000 django-blog-lotus-0.5.2.1/MANIFEST.in
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2575 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1330 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/README.rst
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2575 2023-06-03 01:20:31.000000 django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2721 2023-06-03 01:20:31.000000 django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/SOURCES.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-06-03 01:20:31.000000 django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/dependency_links.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      322 2023-06-03 01:20:31.000000 django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/requires.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       14 2023-06-03 01:20:31.000000 django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/top_level.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-05-03 20:30:50.000000 django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/zip-safe
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/lotus/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      152 2022-12-19 01:25:34.000000 django-blog-lotus-0.5.2.1/lotus/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/lotus/admin/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      258 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/admin/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4001 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/admin/article.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2612 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/admin/category.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1418 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/admin/translated.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      231 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/apps.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      785 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/choices.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/lotus/contrib/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/contrib/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1667 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2.1/lotus/contrib/django_configuration.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      330 2023-01-21 14:51:37.000000 django-blog-lotus-0.5.2.1/lotus/exceptions.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/lotus/factories/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      376 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/factories/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     7596 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/factories/article.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1573 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/factories/author.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2520 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/factories/category.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1592 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/factories/tag.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/lotus/forms/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      367 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/forms/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5662 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/forms/article.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3464 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/forms/category.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1285 2021-10-25 23:19:15.000000 django-blog-lotus-0.5.2.1/lotus/forms/translated.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/lotus/locale/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.508260 django-blog-lotus-0.5.2.1/lotus/locale/de/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/lotus/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      380 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     8674 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     8627 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/locale/django.pot
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.508260 django-blog-lotus-0.5.2.1/lotus/locale/en/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      380 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     8674 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.508260 django-blog-lotus-0.5.2.1/lotus/locale/fr/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     7232 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    11353 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4091 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/lookups.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/management/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/management/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/management/commands/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/management/commands/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    22425 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/management/commands/lotus_demo.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5480 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2.1/lotus/managers.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/migrations/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    12384 2023-06-03 01:20:11.000000 django-blog-lotus-0.5.2.1/lotus/migrations/0001_initial.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-01-01 21:16:12.000000 django-blog-lotus-0.5.2.1/lotus/migrations/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/models/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      148 2021-05-29 23:54:08.000000 django-blog-lotus-0.5.2.1/lotus/models/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    12914 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2.1/lotus/models/article.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1599 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/models/author.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3232 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/models/category.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      551 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/models/translated.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      194 2022-07-04 12:22:57.000000 django-blog-lotus-0.5.2.1/lotus/responses.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2733 2023-06-03 01:07:36.000000 django-blog-lotus-0.5.2.1/lotus/settings.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.508260 django-blog-lotus-0.5.2.1/lotus/templates/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.508260 django-blog-lotus-0.5.2.1/lotus/templates/admin/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.508260 django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/article/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4914 2023-05-03 20:48:05.000000 django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/article/change_form.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1515 2023-01-16 21:53:43.000000 django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/article/translate_original.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/category/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1633 2022-07-04 12:22:57.000000 django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/category/change_form.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1519 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/category/translate_original.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     9789 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/detail.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      752 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/list.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/partials/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2798 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/partials/item.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      383 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/partials/siblings.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/author/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      738 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/author/detail.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      717 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/author/list.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/author/partials/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      340 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/author/partials/item.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      164 2022-01-02 21:03:15.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/base.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1514 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/detail.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      751 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/list.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/partials/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      587 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/partials/item.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      387 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/partials/siblings.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      613 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/pagination.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      544 2022-12-18 14:29:13.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/preview_switch.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/tag/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      726 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/tag/detail.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      951 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/tag/list.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/lotus/templatetags/
+-rw-r--r--   0 emencia   (1001) emencia   (1001)        0 2021-07-04 20:57:38.000000 django-blog-lotus-0.5.2.1/lotus/templatetags/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    11813 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templatetags/lotus.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1659 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/urls.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/lotus/utils/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2021-05-29 23:54:08.000000 django-blog-lotus-0.5.2.1/lotus/utils/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1719 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/utils/factory.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    13239 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/utils/imaging.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     8329 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/utils/tests.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/lotus/views/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      768 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2.1/lotus/views/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/lotus/views/admin/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      300 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/views/admin/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      295 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/views/admin/article.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      299 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/views/admin/category.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3770 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/views/admin/mixins.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4610 2023-03-19 17:30:54.000000 django-blog-lotus-0.5.2.1/lotus/views/article.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3156 2022-12-18 15:40:32.000000 django-blog-lotus-0.5.2.1/lotus/views/author.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3148 2022-12-18 15:40:43.000000 django-blog-lotus-0.5.2.1/lotus/views/category.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5633 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2.1/lotus/views/mixins.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2614 2022-07-04 12:22:57.000000 django-blog-lotus-0.5.2.1/lotus/views/preview.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5347 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2.1/lotus/views/tag.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2099 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/setup.cfg
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2021-05-29 23:54:08.000000 django-blog-lotus-0.5.2.1/setup.py
```

### Comparing `django-blog-lotus-0.5.2/LICENCE.txt` & `django-blog-lotus-0.5.2.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/PKG-INFO` & `django-blog-lotus-0.5.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-blog-lotus
-Version: 0.5.2
+Version: 0.5.2.1
 Summary: A weblog application with Django.
 Home-page: https://github.com/emencia/django-blog-lotus
 Author: Emencia
 Author-email: support@emencia.com
 License: MIT
 Project-URL: Source Code, https://github.com/emencia/django-blog-lotus
 Project-URL: Issue Tracker, https://github.com/emencia/django-blog-lotus/issues
```

### Comparing `django-blog-lotus-0.5.2/README.rst` & `django-blog-lotus-0.5.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/django_blog_lotus.egg-info/PKG-INFO` & `django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-blog-lotus
-Version: 0.5.2
+Version: 0.5.2.1
 Summary: A weblog application with Django.
 Home-page: https://github.com/emencia/django-blog-lotus
 Author: Emencia
 Author-email: support@emencia.com
 License: MIT
 Project-URL: Source Code, https://github.com/emencia/django-blog-lotus
 Project-URL: Issue Tracker, https://github.com/emencia/django-blog-lotus/issues
```

### Comparing `django-blog-lotus-0.5.2/django_blog_lotus.egg-info/SOURCES.txt` & `django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/admin/article.py` & `django-blog-lotus-0.5.2.1/lotus/admin/article.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/admin/category.py` & `django-blog-lotus-0.5.2.1/lotus/admin/category.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/admin/translated.py` & `django-blog-lotus-0.5.2.1/lotus/admin/translated.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/choices.py` & `django-blog-lotus-0.5.2.1/lotus/choices.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/contrib/django_configuration.py` & `django-blog-lotus-0.5.2.1/lotus/contrib/django_configuration.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/factories/article.py` & `django-blog-lotus-0.5.2.1/lotus/factories/article.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/factories/author.py` & `django-blog-lotus-0.5.2.1/lotus/factories/author.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/factories/category.py` & `django-blog-lotus-0.5.2.1/lotus/factories/category.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/factories/tag.py` & `django-blog-lotus-0.5.2.1/lotus/factories/tag.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/forms/article.py` & `django-blog-lotus-0.5.2.1/lotus/forms/article.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/forms/category.py` & `django-blog-lotus-0.5.2.1/lotus/forms/category.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/forms/translated.py` & `django-blog-lotus-0.5.2.1/lotus/forms/translated.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/locale/de/LC_MESSAGES/django.po` & `django-blog-lotus-0.5.2.1/lotus/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/locale/django.pot` & `django-blog-lotus-0.5.2.1/lotus/locale/django.pot`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/locale/en/LC_MESSAGES/django.po` & `django-blog-lotus-0.5.2.1/lotus/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/locale/fr/LC_MESSAGES/django.mo` & `django-blog-lotus-0.5.2.1/lotus/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/locale/fr/LC_MESSAGES/django.po` & `django-blog-lotus-0.5.2.1/lotus/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/lookups.py` & `django-blog-lotus-0.5.2.1/lotus/lookups.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/management/commands/lotus_demo.py` & `django-blog-lotus-0.5.2.1/lotus/management/commands/lotus_demo.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/managers.py` & `django-blog-lotus-0.5.2.1/lotus/managers.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/migrations/0001_initial.py` & `django-blog-lotus-0.5.2.1/lotus/migrations/0001_initial.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from django.db import migrations, models
 import django.db.models.deletion
 import django.utils.timezone
 import smart_media.mixins
 import smart_media.modelfields
 import taggit.managers
 
+from ..choices import (
+    get_status_choices, get_status_default, get_language_choices, get_language_default
+)
+
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
         ("auth", "0012_alter_user_first_name_max_length"),
@@ -43,21 +47,17 @@
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 (
                     "language",
                     models.CharField(
-                        choices=[
-                            ("en", "English"),
-                            ("fr", "Français"),
-                            ("de", "Deutsche"),
-                        ],
+                        choices=get_language_choices(),
                         db_index=True,
-                        default="en",
+                        default=get_language_default(),
                         max_length=8,
                         verbose_name="language",
                     ),
                 ),
                 (
                     "title",
                     models.CharField(default="", max_length=255, verbose_name="title"),
@@ -115,31 +115,27 @@
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
                 (
                     "language",
                     models.CharField(
-                        choices=[
-                            ("en", "English"),
-                            ("fr", "Français"),
-                            ("de", "Deutsche"),
-                        ],
+                        choices=get_language_choices(),
                         db_index=True,
-                        default="en",
+                        default=get_language_default(),
                         max_length=8,
                         verbose_name="language",
                     ),
                 ),
                 (
                     "status",
                     models.SmallIntegerField(
-                        choices=[(0, "draft"), (10, "available")],
+                        choices=get_status_choices(),
                         db_index=True,
-                        default=0,
+                        default=get_status_default(),
                         help_text="Publication status.",
                         verbose_name="status",
                     ),
                 ),
                 (
                     "featured",
                     models.BooleanField(
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-blog-lotus-0.5.2/lotus/models/article.py` & `django-blog-lotus-0.5.2.1/lotus/models/article.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/models/author.py` & `django-blog-lotus-0.5.2.1/lotus/models/author.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/models/category.py` & `django-blog-lotus-0.5.2.1/lotus/models/category.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/models/translated.py` & `django-blog-lotus-0.5.2.1/lotus/models/translated.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/settings.py` & `django-blog-lotus-0.5.2.1/lotus/settings.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/admin/lotus/article/change_form.html` & `django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/article/change_form.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/admin/lotus/article/translate_original.html` & `django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/article/translate_original.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/admin/lotus/category/change_form.html` & `django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/category/change_form.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/admin/lotus/category/translate_original.html` & `django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/category/translate_original.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/lotus/article/detail.html` & `django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/detail.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/lotus/article/list.html` & `django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/list.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/lotus/article/partials/item.html` & `django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/partials/item.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/lotus/author/detail.html` & `django-blog-lotus-0.5.2.1/lotus/templates/lotus/author/detail.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/lotus/author/list.html` & `django-blog-lotus-0.5.2.1/lotus/templates/lotus/author/list.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/lotus/category/detail.html` & `django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/detail.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/lotus/category/list.html` & `django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/list.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/lotus/category/partials/item.html` & `django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/partials/item.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/lotus/pagination.html` & `django-blog-lotus-0.5.2.1/lotus/templates/lotus/pagination.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/lotus/preview_switch.html` & `django-blog-lotus-0.5.2.1/lotus/templates/lotus/preview_switch.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/lotus/tag/detail.html` & `django-blog-lotus-0.5.2.1/lotus/templates/lotus/tag/detail.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templates/lotus/tag/list.html` & `django-blog-lotus-0.5.2.1/lotus/templates/lotus/tag/list.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/templatetags/lotus.py` & `django-blog-lotus-0.5.2.1/lotus/templatetags/lotus.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/urls.py` & `django-blog-lotus-0.5.2.1/lotus/urls.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/utils/factory.py` & `django-blog-lotus-0.5.2.1/lotus/utils/factory.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/utils/imaging.py` & `django-blog-lotus-0.5.2.1/lotus/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/utils/tests.py` & `django-blog-lotus-0.5.2.1/lotus/utils/tests.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/views/__init__.py` & `django-blog-lotus-0.5.2.1/lotus/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/views/admin/mixins.py` & `django-blog-lotus-0.5.2.1/lotus/views/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/views/article.py` & `django-blog-lotus-0.5.2.1/lotus/views/article.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/views/author.py` & `django-blog-lotus-0.5.2.1/lotus/views/author.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/views/category.py` & `django-blog-lotus-0.5.2.1/lotus/views/category.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/views/mixins.py` & `django-blog-lotus-0.5.2.1/lotus/views/mixins.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/views/preview.py` & `django-blog-lotus-0.5.2.1/lotus/views/preview.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/lotus/views/tag.py` & `django-blog-lotus-0.5.2.1/lotus/views/tag.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2/setup.cfg` & `django-blog-lotus-0.5.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-blog-lotus
-version = 0.5.2
+version = 0.5.2.1
 description = A weblog application with Django.
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = Emencia
 author_email = support@emencia.com
 url = https://github.com/emencia/django-blog-lotus
 project_urls =
```

