# Comparing `tmp/Bigsansar-1.6.1.tar.gz` & `tmp/Bigsansar-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-1.6.1.tar", last modified: Fri Jun  2 15:21:34 2023, max compression
+gzip compressed data, was "Bigsansar-1.6.2.tar", last modified: Sat Jun  3 02:28:31 2023, max compression
```

## Comparing `Bigsansar-1.6.1.tar` & `Bigsansar-1.6.2.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.674381 Bigsansar-1.6.1/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.124381 Bigsansar-1.6.1/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3992 2023-06-02 15:21:34.000000 Bigsansar-1.6.1/Bigsansar.egg-info/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13745 2023-06-02 15:21:34.000000 Bigsansar-1.6.1/Bigsansar.egg-info/SOURCES.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-06-02 15:21:34.000000 Bigsansar-1.6.1/Bigsansar.egg-info/dependency_links.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-06-02 15:21:34.000000 Bigsansar-1.6.1/Bigsansar.egg-info/entry_points.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       98 2023-06-02 15:21:34.000000 Bigsansar-1.6.1/Bigsansar.egg-info/requires.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-06-02 15:21:34.000000 Bigsansar-1.6.1/Bigsansar.egg-info/top_level.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-29 06:46:12.000000 Bigsansar-1.6.1/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3992 2023-06-02 15:21:34.674381 Bigsansar-1.6.1/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3411 2023-06-02 15:20:47.000000 Bigsansar-1.6.1/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.134381 Bigsansar-1.6.1/bigsansar/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.134381 Bigsansar-1.6.1/bigsansar/contrib/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.154381 Bigsansar-1.6.1/bigsansar/contrib/account/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/account/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/account/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/account/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.154381 Bigsansar-1.6.1/bigsansar/contrib/account/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/account/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/account/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/account/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.154381 Bigsansar-1.6.1/bigsansar/contrib/account/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/account/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/account/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/account/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.164381 Bigsansar-1.6.1/bigsansar/contrib/advance/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.6.1/bigsansar/contrib/advance/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      291 2023-05-13 03:12:35.000000 Bigsansar-1.6.1/bigsansar/contrib/advance/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      202 2023-05-08 12:23:18.000000 Bigsansar-1.6.1/bigsansar/contrib/advance/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.174381 Bigsansar-1.6.1/bigsansar/contrib/advance/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1000 2023-05-08 12:29:40.000000 Bigsansar-1.6.1/bigsansar/contrib/advance/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-05-13 02:56:41.000000 Bigsansar-1.6.1/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1050 2023-05-13 03:08:43.000000 Bigsansar-1.6.1/bigsansar/contrib/advance/migrations/0003_javascript.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      386 2023-05-13 03:14:07.000000 Bigsansar-1.6.1/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.6.1/bigsansar/contrib/advance/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2023-05-13 04:58:52.000000 Bigsansar-1.6.1/bigsansar/contrib/advance/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-05-08 12:18:38.000000 Bigsansar-1.6.1/bigsansar/contrib/advance/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-05-08 12:18:38.000000 Bigsansar-1.6.1/bigsansar/contrib/advance/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.184381 Bigsansar-1.6.1/bigsansar/contrib/blogs/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/blogs/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      531 2023-06-02 13:13:25.000000 Bigsansar-1.6.1/bigsansar/contrib/blogs/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/blogs/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.194381 Bigsansar-1.6.1/bigsansar/contrib/blogs/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2261 2023-05-29 10:57:40.000000 Bigsansar-1.6.1/bigsansar/contrib/blogs/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-06-02 13:13:53.000000 Bigsansar-1.6.1/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 10:57:14.000000 Bigsansar-1.6.1/bigsansar/contrib/blogs/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2152 2023-06-02 13:13:06.000000 Bigsansar-1.6.1/bigsansar/contrib/blogs/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.194381 Bigsansar-1.6.1/bigsansar/contrib/blogs/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-20 12:33:35.000000 Bigsansar-1.6.1/bigsansar/contrib/blogs/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1511 2023-06-02 15:12:56.000000 Bigsansar-1.6.1/bigsansar/contrib/blogs/templatetags/blogs.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/blogs/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/blogs/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.194381 Bigsansar-1.6.1/bigsansar/contrib/sites/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/sites/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1733 2023-06-02 12:05:41.000000 Bigsansar-1.6.1/bigsansar/contrib/sites/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/sites/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3041 2023-05-17 09:58:25.000000 Bigsansar-1.6.1/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.194381 Bigsansar-1.6.1/bigsansar/contrib/sites/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1847 2023-05-02 12:46:38.000000 Bigsansar-1.6.1/bigsansar/contrib/sites/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:46:31.000000 Bigsansar-1.6.1/bigsansar/contrib/sites/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1899 2023-05-17 10:15:27.000000 Bigsansar-1.6.1/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.204381 Bigsansar-1.6.1/bigsansar/contrib/sites/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/sites/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/sites/templatetags/pages.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/sites/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/contrib/sites/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.204381 Bigsansar-1.6.1/bigsansar/core/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/core/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/core/host.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    10679 2023-05-27 06:38:55.000000 Bigsansar-1.6.1/bigsansar/core/init.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/main.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.204381 Bigsansar-1.6.1/bigsansar/management/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.204381 Bigsansar-1.6.1/bigsansar/management/commands/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/management/commands/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.6.1/bigsansar/management/commands/createuser.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.204381 Bigsansar-1.6.1/bigsansar/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.214381 Bigsansar-1.6.1/bigsansar/static/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/static/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.084381 Bigsansar-1.6.1/bigsansar/static/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.084381 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.104381 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.214381 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.214381 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2361 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/codesnippet.js
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.214381 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      532 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/codesnippet.png
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.214381 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1046 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/codesnippet.png
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.314381 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      509 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ar.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      455 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/az.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      512 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/bg.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      452 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ca.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      431 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/cs.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      415 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/da.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      438 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/de-ch.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      435 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/de.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      581 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/el.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/en-au.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/en-gb.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      424 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/en.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      413 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/eo.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/es-mx.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/es.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      411 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/et.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      420 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/eu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      453 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fa.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      479 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fr-ca.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      439 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      471 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/gl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      455 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/he.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      433 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/hr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      434 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/hu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/id.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      468 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/it.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      486 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ja.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      487 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/km.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      451 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ko.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ku.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      441 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/lt.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      431 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/lv.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      415 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/nb.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      407 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/nl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/no.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      440 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/oc.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      418 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/pl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      470 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/pt-br.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      465 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/pt.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      438 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ro.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      478 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ru.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      415 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      446 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sq.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      425 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sr-latn.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      488 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      410 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sv.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      541 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/th.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      428 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/tr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/tt.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      482 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ug.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      502 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/uk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      437 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/vi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      420 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/zh-cn.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      435 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/zh.js
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.094381 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.314381 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    29367 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/CHANGES.md
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1498 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4682 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.md
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     7534 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.ru.md
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    30210 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/highlight.pack.js
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.564381 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2354 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/arta.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      806 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ascetic.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1719 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1733 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.light.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1744 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1753 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.light.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1743 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.light.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1765 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1774 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.light.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1755 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1764 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.light.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1791 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_paper.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    18198 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_papersq.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1762 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2651 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/default.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1776 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/docco.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1903 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/far.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1582 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/foundation.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1684 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/github.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2162 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/googlecode.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/idea.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1462 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ir_black.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1928 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/magula.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      899 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/mono-blue.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2014 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2336 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai_sublime.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2316 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/obsidian.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1493 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1494 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.light.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1641 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.jpg
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2554 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/railscasts.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1595 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/rainbow.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1983 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      486 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1602 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_dark.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1602 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_light.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2238 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/sunburst.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1603 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-blue.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1533 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-bright.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1537 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-eighties.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1600 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1429 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1561 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/vs.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2294 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/xcode.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1856 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/zenburn.css
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    15468 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/plugin.js
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.564381 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/samples/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     8267 2023-03-22 09:50:46.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/samples/codesnippet.html
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.564381 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.564381 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1258 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1165 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.654381 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1337 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1654 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1209 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1078 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1514 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1049 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1084 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1103 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      960 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1051 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1250 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1166 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1106 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1195 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1229 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1047 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1064 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1120 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1151 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1178 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1564 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1173 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1206 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1538 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1067 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      916 2021-03-31 11:22:53.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13371 2021-03-31 14:36:18.000000 Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/static/logo.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-02 15:21:34.674381 Bigsansar-1.6.1/bigsansar/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/templates/404.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/templates/acc_active_email.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1521 2023-05-05 10:08:59.000000 Bigsansar-1.6.1/bigsansar/templates/base.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1326 2023-05-20 05:28:14.000000 Bigsansar-1.6.1/bigsansar/templates/blog_preview.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/templates/default.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/templates/defaultpage.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/templates/parking.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-05-20 05:28:14.000000 Bigsansar-1.6.1/bigsansar/templates/sitemap.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.1/bigsansar/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1155 2023-05-20 14:08:47.000000 Bigsansar-1.6.1/bigsansar/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4445 2023-06-02 12:16:08.000000 Bigsansar-1.6.1/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-06-02 15:21:34.674381 Bigsansar-1.6.1/setup.cfg
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2056 2023-06-02 15:21:02.000000 Bigsansar-1.6.1/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.812105 Bigsansar-1.6.2/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.602105 Bigsansar-1.6.2/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3992 2023-06-03 02:28:31.000000 Bigsansar-1.6.2/Bigsansar.egg-info/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13745 2023-06-03 02:28:31.000000 Bigsansar-1.6.2/Bigsansar.egg-info/SOURCES.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-06-03 02:28:31.000000 Bigsansar-1.6.2/Bigsansar.egg-info/dependency_links.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-06-03 02:28:31.000000 Bigsansar-1.6.2/Bigsansar.egg-info/entry_points.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       98 2023-06-03 02:28:31.000000 Bigsansar-1.6.2/Bigsansar.egg-info/requires.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-06-03 02:28:31.000000 Bigsansar-1.6.2/Bigsansar.egg-info/top_level.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-29 06:46:12.000000 Bigsansar-1.6.2/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3992 2023-06-03 02:28:31.812105 Bigsansar-1.6.2/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3411 2023-06-02 15:23:37.000000 Bigsansar-1.6.2/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.602105 Bigsansar-1.6.2/bigsansar/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.602105 Bigsansar-1.6.2/bigsansar/contrib/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.602105 Bigsansar-1.6.2/bigsansar/contrib/account/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/account/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/account/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/account/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.602105 Bigsansar-1.6.2/bigsansar/contrib/account/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/account/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/account/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/account/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.602105 Bigsansar-1.6.2/bigsansar/contrib/account/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/account/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/account/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/account/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.602105 Bigsansar-1.6.2/bigsansar/contrib/advance/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.6.2/bigsansar/contrib/advance/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      291 2023-05-13 03:12:35.000000 Bigsansar-1.6.2/bigsansar/contrib/advance/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      202 2023-05-08 12:23:18.000000 Bigsansar-1.6.2/bigsansar/contrib/advance/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.612105 Bigsansar-1.6.2/bigsansar/contrib/advance/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1000 2023-05-08 12:29:40.000000 Bigsansar-1.6.2/bigsansar/contrib/advance/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-05-13 02:56:41.000000 Bigsansar-1.6.2/bigsansar/contrib/advance/migrations/0002_alter_css_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1050 2023-05-13 03:08:43.000000 Bigsansar-1.6.2/bigsansar/contrib/advance/migrations/0003_javascript.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      386 2023-05-13 03:14:07.000000 Bigsansar-1.6.2/bigsansar/contrib/advance/migrations/0004_alter_javascript_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-08 12:18:38.000000 Bigsansar-1.6.2/bigsansar/contrib/advance/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2023-05-13 04:58:52.000000 Bigsansar-1.6.2/bigsansar/contrib/advance/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-05-08 12:18:38.000000 Bigsansar-1.6.2/bigsansar/contrib/advance/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-05-08 12:18:38.000000 Bigsansar-1.6.2/bigsansar/contrib/advance/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.612105 Bigsansar-1.6.2/bigsansar/contrib/blogs/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/blogs/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      531 2023-06-02 13:13:25.000000 Bigsansar-1.6.2/bigsansar/contrib/blogs/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/blogs/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.612105 Bigsansar-1.6.2/bigsansar/contrib/blogs/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2261 2023-05-29 10:57:40.000000 Bigsansar-1.6.2/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      367 2023-06-02 13:13:53.000000 Bigsansar-1.6.2/bigsansar/contrib/blogs/migrations/0002_post_visitor.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-29 10:57:14.000000 Bigsansar-1.6.2/bigsansar/contrib/blogs/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2152 2023-06-02 13:13:06.000000 Bigsansar-1.6.2/bigsansar/contrib/blogs/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.612105 Bigsansar-1.6.2/bigsansar/contrib/blogs/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-20 12:33:35.000000 Bigsansar-1.6.2/bigsansar/contrib/blogs/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1511 2023-06-02 15:12:56.000000 Bigsansar-1.6.2/bigsansar/contrib/blogs/templatetags/blogs.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/blogs/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.612105 Bigsansar-1.6.2/bigsansar/contrib/sites/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/sites/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1733 2023-06-02 12:05:41.000000 Bigsansar-1.6.2/bigsansar/contrib/sites/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/sites/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3579 2023-06-03 02:16:10.000000 Bigsansar-1.6.2/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.612105 Bigsansar-1.6.2/bigsansar/contrib/sites/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1847 2023-05-02 12:46:38.000000 Bigsansar-1.6.2/bigsansar/contrib/sites/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:46:31.000000 Bigsansar-1.6.2/bigsansar/contrib/sites/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1899 2023-05-17 10:15:27.000000 Bigsansar-1.6.2/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.612105 Bigsansar-1.6.2/bigsansar/contrib/sites/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/sites/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/sites/templatetags/pages.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/sites/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/contrib/sites/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.612105 Bigsansar-1.6.2/bigsansar/core/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/core/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/core/host.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    10679 2023-05-27 06:38:55.000000 Bigsansar-1.6.2/bigsansar/core/init.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/main.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.612105 Bigsansar-1.6.2/bigsansar/management/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.612105 Bigsansar-1.6.2/bigsansar/management/commands/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/management/commands/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.6.2/bigsansar/management/commands/createuser.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.622105 Bigsansar-1.6.2/bigsansar/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.622105 Bigsansar-1.6.2/bigsansar/static/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/static/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.592105 Bigsansar-1.6.2/bigsansar/static/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.592105 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.592105 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.622105 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.622105 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2361 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/codesnippet.js
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.622105 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      532 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/codesnippet.png
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.632105 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1046 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/codesnippet.png
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.692105 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      509 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ar.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      455 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/az.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      512 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/bg.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      452 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ca.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      431 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/cs.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      415 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/da.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      438 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/de-ch.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      435 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/de.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      581 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/el.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/en-au.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/en-gb.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      424 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/en.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      413 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/eo.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/es-mx.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/es.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      411 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/et.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      420 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/eu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      453 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fa.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      479 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fr-ca.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      439 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/fr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      471 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/gl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      455 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/he.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      433 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/hr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      434 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/hu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/id.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      468 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/it.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      486 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ja.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      487 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/km.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      451 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ko.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ku.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      441 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/lt.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      431 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/lv.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      415 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/nb.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      407 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/nl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/no.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      440 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/oc.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      418 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/pl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      470 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/pt-br.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      465 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/pt.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      438 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ro.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      478 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ru.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      415 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      446 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sq.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      425 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sr-latn.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      488 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      410 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/sv.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      541 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/th.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      428 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/tr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      474 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/tt.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      482 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/ug.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      502 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/uk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      437 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/vi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      420 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/zh-cn.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      435 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/zh.js
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.592105 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.702105 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    29367 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/CHANGES.md
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1498 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4682 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.md
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     7534 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.ru.md
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    30210 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/highlight.pack.js
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.742105 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2354 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/arta.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      806 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ascetic.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1719 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1733 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.light.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1744 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1753 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.light.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1743 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.light.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1765 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1774 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.light.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1755 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1764 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.light.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1791 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_paper.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    18198 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_papersq.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1762 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2651 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/default.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1776 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/docco.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1903 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/far.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1582 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/foundation.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1684 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/github.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2162 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/googlecode.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/idea.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1462 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ir_black.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1928 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/magula.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      899 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/mono-blue.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2014 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2336 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai_sublime.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2316 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/obsidian.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1493 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1494 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.light.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1641 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.jpg
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2554 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/railscasts.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1595 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/rainbow.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1983 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      486 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1602 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_dark.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1602 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_light.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2238 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/sunburst.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1603 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-blue.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1533 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-bright.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1537 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-eighties.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1600 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1429 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1561 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/vs.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2294 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/xcode.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1856 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/zenburn.css
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    15468 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/plugin.js
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.752105 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/samples/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     8267 2023-03-22 09:50:46.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/samples/codesnippet.html
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.752105 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.752105 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1258 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1165 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.792105 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1337 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1654 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1209 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1078 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1514 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1049 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1084 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1103 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1186 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      960 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1051 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1250 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1166 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1106 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1195 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1229 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1059 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1047 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1064 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1120 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1151 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1178 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1564 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1173 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1206 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1538 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1067 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      916 2021-03-31 11:22:53.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)    13371 2021-03-31 14:36:18.000000 Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/static/logo.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-06-03 02:28:31.802105 Bigsansar-1.6.2/bigsansar/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/templates/404.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/templates/acc_active_email.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1521 2023-05-05 10:08:59.000000 Bigsansar-1.6.2/bigsansar/templates/base.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1326 2023-05-20 05:28:14.000000 Bigsansar-1.6.2/bigsansar/templates/blog_preview.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/templates/default.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/templates/defaultpage.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/templates/parking.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      427 2023-05-20 05:28:14.000000 Bigsansar-1.6.2/bigsansar/templates/sitemap.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.6.2/bigsansar/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1155 2023-05-20 14:08:47.000000 Bigsansar-1.6.2/bigsansar/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     4445 2023-06-02 12:16:08.000000 Bigsansar-1.6.2/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-06-03 02:28:31.812105 Bigsansar-1.6.2/setup.cfg
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2056 2023-06-03 02:10:45.000000 Bigsansar-1.6.2/setup.py
```

### Comparing `Bigsansar-1.6.1/Bigsansar.egg-info/PKG-INFO` & `Bigsansar-1.6.2/Bigsansar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.6.1
+Version: 1.6.2
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
@@ -51,24 +51,24 @@
 
 # After you install bigsansar
 Type `bigsansar init` command for **automatically** setup server .
 
 # How to access admin pannel in local env
 Go to [localhost:8000](http://localhost:8000) 
 
-# How to change admin ulr in server side with domain 
+# How to change admin URL in server side with domain 
 go to **VirtualHost.py** file and change **localhost:8000** with your subdomain 
 ## Some usefull commands:
 
 `python3 manage.py createuser` - get unlimited users.
 
 ## templatetags for extends and include 
 
-{{% extends '<domain_name>/<page_slug>.html' %}
-% include '<domain_name>/<page_slug>.html' %}
+{% extends '<domain_name>/<page_slug>.html' %}
+{% include '<domain_name>/<page_slug>.html' %}
 
 
 
 ## load blog list in templates
 
 `{% load blogs %}
 {% get_blog as bloglist %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 1.6.1 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 1.6.2 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 bigsansar.com Author: Bikash Pokhrel Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN Project-URL: Bug Tracker, https://github.com/pokhrelb9/
 bigsansar/issues Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django
 flatpages Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
@@ -22,18 +22,18 @@
 bugs before an official release. Get it using this shell command, which
 requires [Git](https://git-scm.com/): `git clone https://github.com/pokhrelb9/
 bigsansar.git` You can also download a [gzipped tarball](https://pypi.org/
 project/Bigsansar/#files) of the development version. This archive is updated
 every time we commit code. # After you install bigsansar Type `bigsansar init`
 command for **automatically** setup server . # How to access admin pannel in
 local env Go to [localhost:8000](http://localhost:8000) # How to change admin
-ulr in server side with domain go to **VirtualHost.py** file and change
+URL in server side with domain go to **VirtualHost.py** file and change
 **localhost:8000** with your subdomain ## Some usefull commands: `python3
 manage.py createuser` - get unlimited users. ## templatetags for extends and
-include {{% extends '/.html' %} % include '/.html' %} ## load blog list in
+include {% extends '/.html' %} {% include '/.html' %} ## load blog list in
 templates `{% load blogs %} {% get_blog as bloglist %} {% for list in bloglist
 %}
 ** {{list.title}} - {{ list.domain }} **
 {{list.body|slice:":100"}} - {{ list.publish_date }}
 Read_More
 {% endfor %}` ## get single blog objects `{% load blogs %} {% get_blog_object
 as get_blog %} {{ get_blog.title }} {{ get_blog.thumbnails }} {
```

### Comparing `Bigsansar-1.6.1/Bigsansar.egg-info/SOURCES.txt` & `Bigsansar-1.6.2/Bigsansar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/LICENSE` & `Bigsansar-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/PKG-INFO` & `Bigsansar-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.6.1
+Version: 1.6.2
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
@@ -51,24 +51,24 @@
 
 # After you install bigsansar
 Type `bigsansar init` command for **automatically** setup server .
 
 # How to access admin pannel in local env
 Go to [localhost:8000](http://localhost:8000) 
 
-# How to change admin ulr in server side with domain 
+# How to change admin URL in server side with domain 
 go to **VirtualHost.py** file and change **localhost:8000** with your subdomain 
 ## Some usefull commands:
 
 `python3 manage.py createuser` - get unlimited users.
 
 ## templatetags for extends and include 
 
-{{% extends '<domain_name>/<page_slug>.html' %}
-% include '<domain_name>/<page_slug>.html' %}
+{% extends '<domain_name>/<page_slug>.html' %}
+{% include '<domain_name>/<page_slug>.html' %}
 
 
 
 ## load blog list in templates
 
 `{% load blogs %}
 {% get_blog as bloglist %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Bigsansar Version: 1.6.1 Summary: Build one in
+Metadata-Version: 2.1 Name: Bigsansar Version: 1.6.2 Summary: Build one in
 minutes with bigsansar - a visual site building tool! Home-page: https://
 bigsansar.com Author: Bikash Pokhrel Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN Project-URL: Bug Tracker, https://github.com/pokhrelb9/
 bigsansar/issues Project-URL: Documentations, https://docs.bigsansar.com/
 Keywords: python,django host,bigsansar,django,django sites framework,django
 flatpages Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
@@ -22,18 +22,18 @@
 bugs before an official release. Get it using this shell command, which
 requires [Git](https://git-scm.com/): `git clone https://github.com/pokhrelb9/
 bigsansar.git` You can also download a [gzipped tarball](https://pypi.org/
 project/Bigsansar/#files) of the development version. This archive is updated
 every time we commit code. # After you install bigsansar Type `bigsansar init`
 command for **automatically** setup server . # How to access admin pannel in
 local env Go to [localhost:8000](http://localhost:8000) # How to change admin
-ulr in server side with domain go to **VirtualHost.py** file and change
+URL in server side with domain go to **VirtualHost.py** file and change
 **localhost:8000** with your subdomain ## Some usefull commands: `python3
 manage.py createuser` - get unlimited users. ## templatetags for extends and
-include {{% extends '/.html' %} % include '/.html' %} ## load blog list in
+include {% extends '/.html' %} {% include '/.html' %} ## load blog list in
 templates `{% load blogs %} {% get_blog as bloglist %} {% for list in bloglist
 %}
 ** {{list.title}} - {{ list.domain }} **
 {{list.body|slice:":100"}} - {{ list.publish_date }}
 Read_More
 {% endfor %}` ## get single blog objects `{% load blogs %} {% get_blog_object
 as get_blog %} {{ get_blog.title }} {{ get_blog.thumbnails }} {
```

### Comparing `Bigsansar-1.6.1/README.md` & `Bigsansar-1.6.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,24 +32,24 @@
 
 # After you install bigsansar
 Type `bigsansar init` command for **automatically** setup server .
 
 # How to access admin pannel in local env
 Go to [localhost:8000](http://localhost:8000) 
 
-# How to change admin ulr in server side with domain 
+# How to change admin URL in server side with domain 
 go to **VirtualHost.py** file and change **localhost:8000** with your subdomain 
 ## Some usefull commands:
 
 `python3 manage.py createuser` - get unlimited users.
 
 ## templatetags for extends and include 
 
-{{% extends '<domain_name>/<page_slug>.html' %}
-% include '<domain_name>/<page_slug>.html' %}
+{% extends '<domain_name>/<page_slug>.html' %}
+{% include '<domain_name>/<page_slug>.html' %}
 
 
 
 ## load blog list in templates
 
 `{% load blogs %}
 {% get_blog as bloglist %}
```

#### html2text {}

```diff
@@ -13,18 +13,18 @@
 before an official release. Get it using this shell command, which requires
 [Git](https://git-scm.com/): `git clone https://github.com/pokhrelb9/
 bigsansar.git` You can also download a [gzipped tarball](https://pypi.org/
 project/Bigsansar/#files) of the development version. This archive is updated
 every time we commit code. # After you install bigsansar Type `bigsansar init`
 command for **automatically** setup server . # How to access admin pannel in
 local env Go to [localhost:8000](http://localhost:8000) # How to change admin
-ulr in server side with domain go to **VirtualHost.py** file and change
+URL in server side with domain go to **VirtualHost.py** file and change
 **localhost:8000** with your subdomain ## Some usefull commands: `python3
 manage.py createuser` - get unlimited users. ## templatetags for extends and
-include {{% extends '/.html' %} % include '/.html' %} ## load blog list in
+include {% extends '/.html' %} {% include '/.html' %} ## load blog list in
 templates `{% load blogs %} {% get_blog as bloglist %} {% for list in bloglist
 %}
 ** {{list.title}} - {{ list.domain }} **
 {{list.body|slice:":100"}} - {{ list.publish_date }}
 Read_More
 {% endfor %}` ## get single blog objects `{% load blogs %} {% get_blog_object
 as get_blog %} {{ get_blog.title }} {{ get_blog.thumbnails }} {
```

### Comparing `Bigsansar-1.6.1/bigsansar/contrib/account/forms.py` & `Bigsansar-1.6.2/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/contrib/account/migrations/0001_initial.py` & `Bigsansar-1.6.2/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/contrib/account/models.py` & `Bigsansar-1.6.2/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/contrib/advance/migrations/0001_initial.py` & `Bigsansar-1.6.2/bigsansar/contrib/advance/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/contrib/advance/migrations/0003_javascript.py` & `Bigsansar-1.6.2/bigsansar/contrib/advance/migrations/0003_javascript.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/contrib/advance/models.py` & `Bigsansar-1.6.2/bigsansar/contrib/advance/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/contrib/blogs/admin.py` & `Bigsansar-1.6.2/bigsansar/contrib/blogs/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/contrib/blogs/migrations/0001_initial.py` & `Bigsansar-1.6.2/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/contrib/blogs/models.py` & `Bigsansar-1.6.2/bigsansar/contrib/blogs/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/contrib/blogs/templatetags/blogs.py` & `Bigsansar-1.6.2/bigsansar/contrib/blogs/templatetags/blogs.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/contrib/sites/admin.py` & `Bigsansar-1.6.2/bigsansar/contrib/sites/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/contrib/sites/forms.py` & `Bigsansar-1.6.2/bigsansar/contrib/sites/forms.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from typing import Any, Dict
 
 from django import forms
 from django.core.exceptions import ValidationError
 from django.core.validators import RegexValidator
 from django.utils.translation import gettext_lazy as _
 from bigsansar.contrib.sites.models import domains, pages
 from www.settings import BASE_DIR
@@ -13,14 +14,28 @@
         RegexValidator('^[a-z0-9.]+\.[a-z0-9]{1,5}$', message='Please enter your correct domain name')],
                              widget=forms.TextInput(attrs={'autofocus': True, 'class': 'form-control', }))
 
     class Meta:
         model = domains
         fields = ('domain', 'Description', 'user',)
 
+    def clean(self):
+        getdir = 'templates'
+        gethost = self.cleaned_data.get('domain')
+        mkdir = getdir + '/' + str(gethost)
+        try:
+            final_directory = os.path.join(BASE_DIR, mkdir)
+            if not os.path.exists(final_directory):
+                os.makedirs(final_directory)
+        except:
+            raise ValidationError(
+                _(final_directory + ' Directory not created "Permission Denied"'),
+            )
+
+        return super().clean()
 
 class customaddpageform(forms.ModelForm):
     class Meta:
         model = pages
         fields = '__all__'
         exclude = ('body',)
         widgets = {'slug': forms.HiddenInput(), 'visitor': forms.HiddenInput()}
```

### Comparing `Bigsansar-1.6.1/bigsansar/contrib/sites/migrations/0001_initial.py` & `Bigsansar-1.6.2/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/contrib/sites/models.py` & `Bigsansar-1.6.2/bigsansar/contrib/sites/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/core/__init__.py` & `Bigsansar-1.6.2/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/core/init.py` & `Bigsansar-1.6.2/bigsansar/core/init.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/management/commands/createuser.py` & `Bigsansar-1.6.2/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/codesnippet.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/dialogs/codesnippet.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/codesnippet.png` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/codesnippet.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/codesnippet.png` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/icons/hidpi/codesnippet.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/bg.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/bg.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/el.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/el.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/th.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lang/th.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/CHANGES.md` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/CHANGES.md`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/LICENSE` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.md` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.md`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.ru.md` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/README.ru.md`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/highlight.pack.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/arta.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/arta.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ascetic.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ascetic.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.dark.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.light.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-dune.light.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.dark.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.light.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-forest.light.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.dark.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.light.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-heath.light.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.dark.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.light.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-lakeside.light.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.dark.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.light.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/atelier-seaside.light.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_paper.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_paper.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_papersq.png` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/brown_papersq.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/dark.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/default.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/default.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/docco.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/docco.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/far.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/far.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/foundation.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/foundation.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/github.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/github.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/googlecode.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/googlecode.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/idea.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/idea.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ir_black.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/ir_black.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/magula.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/magula.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/mono-blue.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/mono-blue.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai_sublime.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/monokai_sublime.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/obsidian.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/obsidian.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.dark.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.light.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/paraiso.light.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.jpg` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/pojoaque.jpg`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/railscasts.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/railscasts.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/rainbow.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/rainbow.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/school_book.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_dark.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_dark.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_light.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/solarized_light.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/sunburst.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/sunburst.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-blue.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-blue.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-bright.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-bright.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-eighties.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night-eighties.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow-night.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/tomorrow.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/vs.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/vs.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/xcode.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/xcode.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/zenburn.css` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/lib/highlight/styles/zenburn.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/plugin.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/plugin.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/samples/codesnippet.html` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/codesnippet/samples/codesnippet.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon-hdpi.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/images/icon.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ar.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/bg.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/cs.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/de.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/el.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/en.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/es.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/et.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/eu.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fi.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/fr.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/he.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/hu.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/it.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ja.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ko.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nb.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nl.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/nn.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pl.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/pt.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/ru.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/sk.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/tr.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/uk.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/vi.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/lang/zh.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js` & `Bigsansar-1.6.2/bigsansar/static/ckeditor/ckeditor/plugins/youtube/plugin.js`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/logo.png` & `Bigsansar-1.6.2/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/static/style.css` & `Bigsansar-1.6.2/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/templates/404.html` & `Bigsansar-1.6.2/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/templates/base.html` & `Bigsansar-1.6.2/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/templates/blog_preview.html` & `Bigsansar-1.6.2/bigsansar/templates/blog_preview.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/templates/default.html` & `Bigsansar-1.6.2/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/templates/defaultpage.html` & `Bigsansar-1.6.2/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/templates/parking.html` & `Bigsansar-1.6.2/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/urls.py` & `Bigsansar-1.6.2/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/bigsansar/views.py` & `Bigsansar-1.6.2/bigsansar/views.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.6.1/setup.py` & `Bigsansar-1.6.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="1.6.1",
+    version="1.6.2",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bigsansar.com",
     project_urls={
```

