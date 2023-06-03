# Comparing `tmp/django-admin-datta-1.0.8.tar.gz` & `tmp/django-admin-datta-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-datta-1.0.8.tar", last modified: Wed May 31 07:35:09 2023, max compression
+gzip compressed data, was "django-admin-datta-1.0.9.tar", last modified: Fri Jun  2 13:54:12 2023, max compression
```

## Comparing `django-admin-datta-1.0.8.tar` & `django-admin-datta-1.0.9.tar`

### file list

```diff
@@ -1,248 +1,248 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.452172 django-admin-datta-1.0.8/
--rw-rw-rw-   0        0        0     1113 2022-09-27 05:30:21.000000 django-admin-datta-1.0.8/LICENSE.md
--rw-rw-rw-   0        0        0      144 2023-02-09 15:44:00.000000 django-admin-datta-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7277 2023-05-31 07:35:09.449159 django-admin-datta-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6182 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.742652 django-admin-datta-1.0.8/admin_datta/
--rw-rw-rw-   0        0        0       78 2022-09-27 05:30:21.000000 django-admin-datta-1.0.8/admin_datta/__init__.py
--rw-rw-rw-   0        0        0       78 2022-09-27 05:30:21.000000 django-admin-datta-1.0.8/admin_datta/admin.py
--rw-rw-rw-   0        0        0      235 2023-02-09 15:45:05.000000 django-admin-datta-1.0.8/admin_datta/apps.py
--rw-rw-rw-   0        0        0     2601 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/forms.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.744622 django-admin-datta-1.0.8/admin_datta/static/
--rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-datta-1.0.8/admin_datta/static/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.679965 django-admin-datta-1.0.8/admin_datta/static/assets/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.778479 django-admin-datta-1.0.8/admin_datta/static/assets/css/
--rw-rw-rw-   0        0        0     3610 2023-02-28 04:48:58.000000 django-admin-datta-1.0.8/admin_datta/static/assets/css/dark.css
--rw-rw-rw-   0        0        0     9732 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/css/forms.css
--rw-rw-rw-   0        0        0   325947 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/css/style.css
--rw-rw-rw-   0        0        0    12595 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/css/widgets.css
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.646331 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.781490 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/
--rw-rw-rw-   0        0        0     1623 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/datta-icon.css
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.792042 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/
--rw-rw-rw-   0        0        0     2548 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.eot
--rw-rw-rw-   0        0        0     2553 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.svg
--rw-rw-rw-   0        0        0     2400 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.ttf
--rw-rw-rw-   0        0        0     1544 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.woff
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.645334 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.794041 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/css/
--rw-rw-rw-   0        0        0    12312 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/css/feather.css
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.845343 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/
--rw-rw-rw-   0        0        0    55828 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.eot
--rw-rw-rw-   0        0        0   192354 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.svg
--rw-rw-rw-   0        0        0    55664 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.ttf
--rw-rw-rw-   0        0        0    26432 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.woff
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.647330 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.847344 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/css/
--rw-rw-rw-   0        0        0    41069 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/css/fontawesome-all.min.css
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.911785 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/
--rw-rw-rw-   0        0        0   111620 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.eot
--rw-rw-rw-   0        0        0   600938 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.svg
--rw-rw-rw-   0        0        0   111384 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0        0        0    71560 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff
--rw-rw-rw-   0        0        0    61336 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0        0        0    31272 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.eot
--rw-rw-rw-   0        0        0   105078 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.svg
--rw-rw-rw-   0        0        0    31044 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0        0        0    14724 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff
--rw-rw-rw-   0        0        0    12188 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0        0        0   133140 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.eot
--rw-rw-rw-   0        0        0   490291 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.svg
--rw-rw-rw-   0        0        0   132920 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0        0        0    63836 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff
--rw-rw-rw-   0        0        0    50372 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.994316 django-admin-datta-1.0.8/admin_datta/static/assets/images/
--rw-rw-rw-   0        0        0    45568 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/Thumbs.db
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.021776 django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/
--rw-rw-rw-   0        0        0    23040 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/Thumbs.db
--rw-rw-rw-   0        0        0     3822 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/chrome.png
--rw-rw-rw-   0        0        0     4809 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/firefox.png
--rw-rw-rw-   0        0        0     4359 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/ie.png
--rw-rw-rw-   0        0        0     3379 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/opera.png
--rw-rw-rw-   0        0        0     4915 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/safari.png
--rw-rw-rw-   0        0        0     1150 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/favicon.ico
--rw-rw-rw-   0        0        0      334 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-addlink.svg
--rw-rw-rw-   0        0        0     1095 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-calendar.svg
--rw-rw-rw-   0        0        0      383 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-changelink.svg
--rw-rw-rw-   0        0        0      686 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-clock.svg
--rw-rw-rw-   0        0        0      395 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-deletelink.svg
--rw-rw-rw-   0        0        0      563 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-no.svg
--rw-rw-rw-   0        0        0      658 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-unknown-alt.svg
--rw-rw-rw-   0        0        0      658 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-unknown.svg
--rw-rw-rw-   0        0        0      584 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-viewlink.svg
--rw-rw-rw-   0        0        0      439 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-yes.svg
--rw-rw-rw-   0        0        0      563 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/inline-delete.svg
--rw-rw-rw-   0        0        0     2091 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/logo-dark.png
--rw-rw-rw-   0        0        0     1529 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/logo-thumb.png
--rw-rw-rw-   0        0        0     2131 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/logo.png
--rw-rw-rw-   0        0        0      461 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/search.svg
--rw-rw-rw-   0        0        0     3325 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/selector-icons.svg
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.044887 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/
--rw-rw-rw-   0        0        0    31417 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-1.jpg
--rw-rw-rw-   0        0        0    66369 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-2.jpg
--rw-rw-rw-   0        0        0    22071 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-3.jpg
--rw-rw-rw-   0        0        0    21820 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-4.jpg
--rw-rw-rw-   0        0        0    33652 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-5.jpg
--rw-rw-rw-   0        0        0   246009 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img1.jpg
--rw-rw-rw-   0        0        0   165567 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img2.jpg
--rw-rw-rw-   0        0        0   168914 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img3.jpg
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.068790 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/
--rw-rw-rw-   0        0        0    24576 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/Thumbs.db
--rw-rw-rw-   0        0        0     9287 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-1.jpg
--rw-rw-rw-   0        0        0     9372 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-2.jpg
--rw-rw-rw-   0        0        0     9408 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-3.jpg
--rw-rw-rw-   0        0        0     8489 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-4.jpg
--rw-rw-rw-   0        0        0     9350 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-5.jpg
--rw-rw-rw-   0        0        0     1662 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/user-1.png
--rw-rw-rw-   0        0        0     1560 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/user-2.png
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.102031 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/
--rw-rw-rw-   0        0        0   120832 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/Thumbs.db
--rw-rw-rw-   0        0        0   104704 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-1.png
--rw-rw-rw-   0        0        0   170223 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-2.png
--rw-rw-rw-   0        0        0   115557 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-3.png
--rw-rw-rw-   0        0        0    14068 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-4.png
--rw-rw-rw-   0        0        0     6239 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-5.png
--rw-rw-rw-   0        0        0     8193 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-6.png
--rw-rw-rw-   0        0        0   111459 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/emoticon.png
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.128429 django-admin-datta-1.0.8/admin_datta/static/assets/js/
--rw-rw-rw-   0        0        0     2141 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/js/dark-mode.js
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.134329 django-admin-datta-1.0.8/admin_datta/static/assets/js/pages/
--rw-rw-rw-   0        0        0     8008 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/js/pages/chart-morris-custom.js
--rw-rw-rw-   0        0        0     4360 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/js/pages/google-maps.js
--rw-rw-rw-   0        0        0    15247 2023-02-28 04:46:45.000000 django-admin-datta-1.0.8/admin_datta/static/assets/js/pcoded.min.js
--rw-rw-rw-   0        0        0   117122 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/js/vendor-all.min.js
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.678967 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.667291 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.183090 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/
--rw-rw-rw-   0        0        0   209489 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/amcharts.js
--rw-rw-rw-   0        0        0   168766 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/ammap.min.js
--rw-rw-rw-   0        0        0    12860 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/gauge.js
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.189173 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/images/
--rw-rw-rw-   0        0        0      679 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/images/dragIconRoundBig.svg
--rw-rw-rw-   0        0        0      539 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/images/lens.svg
--rw-rw-rw-   0        0        0     2916 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/light.js
--rw-rw-rw-   0        0        0    14700 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/pie.min.js
--rw-rw-rw-   0        0        0     6464 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/radar.js
--rw-rw-rw-   0        0        0    49491 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/serial.js
--rw-rw-rw-   0        0        0    30336 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/usaLow.js
--rw-rw-rw-   0        0        0   130785 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/worldLow.js
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.669450 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/animation/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.191213 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/animation/css/
--rw-rw-rw-   0        0        0    57908 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/animation/css/animate.min.css
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.671454 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.197213 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/css/
--rw-rw-rw-   0        0        0   182626 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.css
--rw-rw-rw-   0        0        0   140893 2023-02-28 04:49:50.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.209029 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/js/
--rw-rw-rw-   0        0        0   127709 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.js
--rw-rw-rw-   0        0        0    50698 2023-02-28 04:49:34.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.min.js
--rw-rw-rw-   0        0        0    19213 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/js/popover.js
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.673455 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.213032 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/css/
--rw-rw-rw-   0        0        0      435 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/css/morris.css
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.218554 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/js/
--rw-rw-rw-   0        0        0    35658 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/js/morris.min.js
--rw-rw-rw-   0        0        0    92631 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/js/raphael.min.js
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.674453 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/google-maps/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.222563 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/google-maps/js/
--rw-rw-rw-   0        0        0    46138 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/google-maps/js/gmaps.js
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.678967 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.239612 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery/js/
--rw-rw-rw-   0        0        0    86929 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery/js/jquery.min.js
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.676452 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-scrollbar/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.226563 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-scrollbar/css/
--rw-rw-rw-   0        0        0     2851 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.229084 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-scrollbar/js/
--rw-rw-rw-   0        0        0    11662 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.677958 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-ui/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.232086 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-ui/js/
--rw-rw-rw-   0        0        0   477536 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-ui/js/jquery-ui.js
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.243623 django-admin-datta-1.0.8/admin_datta/static/assets/scss/
--rw-rw-rw-   0        0        0     3741 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/scss/dark.scss
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.248134 django-admin-datta-1.0.8/admin_datta/templates/
--rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-datta-1.0.8/admin_datta/templates/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.280315 django-admin-datta-1.0.8/admin_datta/templates/accounts/
--rw-rw-rw-   0        0        0     1479 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-change-password.html
--rw-rw-rw-   0        0        0      963 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-change-done.html
--rw-rw-rw-   0        0        0      994 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-reset-complete.html
--rw-rw-rw-   0        0        0     1494 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-reset-confirm.html
--rw-rw-rw-   0        0        0     1028 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-reset-done.html
--rw-rw-rw-   0        0        0     1494 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-reset-password.html
--rw-rw-rw-   0        0        0     2184 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-signin.html
--rw-rw-rw-   0        0        0     2288 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-signup.html
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.322087 django-admin-datta-1.0.8/admin_datta/templates/admin/
--rw-rw-rw-   0        0        0        0 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/.gitkeep
--rw-rw-rw-   0        0        0     1743 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/actions.html
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.682974 django-admin-datta-1.0.8/admin_datta/templates/admin/auth/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.326603 django-admin-datta-1.0.8/admin_datta/templates/admin/auth/user/
--rw-rw-rw-   0        0        0      471 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/auth/user/add_form.html
--rw-rw-rw-   0        0        0     5360 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/auth/user/change_password.html
--rw-rw-rw-   0        0        0     4438 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/change_form.html
--rw-rw-rw-   0        0        0      691 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/change_form_object_tools.html
--rw-rw-rw-   0        0        0     4508 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/change_list.html
--rw-rw-rw-   0        0        0      605 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/change_list_object_tools.html
--rw-rw-rw-   0        0        0     3232 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/change_list_results.html
--rw-rw-rw-   0        0        0     5853 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/delete_confirmation.html
--rw-rw-rw-   0        0        0     6198 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/delete_selected_confirmation.html
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.332170 django-admin-datta-1.0.8/admin_datta/templates/admin/edit_inline/
--rw-rw-rw-   0        0        0     3893 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/edit_inline/stacked.html
--rw-rw-rw-   0        0        0     7788 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/edit_inline/tabular.html
--rw-rw-rw-   0        0        0      643 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/filter.html
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.337172 django-admin-datta-1.0.8/admin_datta/templates/admin/includes/
--rw-rw-rw-   0        0        0     2572 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/includes/fieldset.html
--rw-rw-rw-   0        0        0      339 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/includes/object_delete_summary.html
--rw-rw-rw-   0        0        0    28386 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/index.html
--rw-rw-rw-   0        0        0     2724 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/invalid_setup.html
--rw-rw-rw-   0        0        0     3365 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/login.html
--rw-rw-rw-   0        0        0     2818 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/object_history.html
--rw-rw-rw-   0        0        0     2317 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/pagination.html
--rw-rw-rw-   0        0        0     2155 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/search_form.html
--rw-rw-rw-   0        0        0     1616 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/submit_line.html
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.349212 django-admin-datta-1.0.8/admin_datta/templates/includes/
--rw-rw-rw-   0        0        0      735 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/includes/breadcrumb.html
--rw-rw-rw-   0        0        0     1758 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/includes/head.html
--rw-rw-rw-   0        0        0     6727 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/includes/navigation.html
--rw-rw-rw-   0        0        0      168 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/includes/pre-loader.html
--rw-rw-rw-   0        0        0      323 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/includes/scripts.html
--rw-rw-rw-   0        0        0     8551 2023-02-27 06:26:13.000000 django-admin-datta-1.0.8/admin_datta/templates/includes/sidebar.html
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.368246 django-admin-datta-1.0.8/admin_datta/templates/layouts/
--rw-rw-rw-   0        0        0      306 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/layouts/base-auth.html
--rw-rw-rw-   0        0        0     1428 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/templates/layouts/base.html
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.398208 django-admin-datta-1.0.8/admin_datta/templates/pages/
--rw-rw-rw-   0        0        0     2857 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/chart-morris.html
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.422661 django-admin-datta-1.0.8/admin_datta/templates/pages/components/
--rw-rw-rw-   0        0        0     1907 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_badges.html
--rw-rw-rw-   0        0        0     4650 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_breadcrumb-pagination.html
--rw-rw-rw-   0        0        0    12079 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_button.html
--rw-rw-rw-   0        0        0     6970 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_collapse.html
--rw-rw-rw-   0        0        0    10818 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_tabs.html
--rw-rw-rw-   0        0        0     9952 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_typography.html
--rw-rw-rw-   0        0        0     5996 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/components/icon-feather.html
--rw-rw-rw-   0        0        0    15591 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/form_elements.html
--rw-rw-rw-   0        0        0    28386 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/index.html
--rw-rw-rw-   0        0        0     5101 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/map-google.html
--rw-rw-rw-   0        0        0     3810 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/profile.html
--rw-rw-rw-   0        0        0      945 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/sample-page.html
--rw-rw-rw-   0        0        0     4635 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/tbl_bootstrap.html
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.430123 django-admin-datta-1.0.8/admin_datta/templates/registration/
--rw-rw-rw-   0        0        0        0 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/registration/.gitkeep
--rw-rw-rw-   0        0        0     1458 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/registration/logged_out.html
--rw-rw-rw-   0        0        0     1971 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/registration/password_change_done.html
--rw-rw-rw-   0        0        0     3308 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/registration/password_change_form.html
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.437086 django-admin-datta-1.0.8/admin_datta/templatetags/
--rw-rw-rw-   0        0        0        0 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templatetags/__init__.py
--rw-rw-rw-   0        0        0     2550 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templatetags/admin_datta.py
--rw-rw-rw-   0        0        0      178 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templatetags/replace_value.py
--rw-rw-rw-   0        0        0     2342 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/urls.py
--rw-rw-rw-   0        0        0    16593 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/utils.py
--rw-rw-rw-   0        0        0     4313 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/views.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.445647 django-admin-datta-1.0.8/django_admin_datta.egg-info/
--rw-rw-rw-   0        0        0     7277 2023-05-31 07:35:07.000000 django-admin-datta-1.0.8/django_admin_datta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9583 2023-05-31 07:35:08.000000 django-admin-datta-1.0.8/django_admin_datta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 07:35:07.000000 django-admin-datta-1.0.8/django_admin_datta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 05:41:21.000000 django-admin-datta-1.0.8/django_admin_datta.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-05-31 07:35:07.000000 django-admin-datta-1.0.8/django_admin_datta.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.446644 django-admin-datta-1.0.8/docs/
--rw-rw-rw-   0        0        0       13 2022-09-27 05:30:21.000000 django-admin-datta-1.0.8/docs/blank.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 07:35:09.452172 django-admin-datta-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1343 2023-05-31 07:34:09.000000 django-admin-datta-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.457375 django-admin-datta-1.0.9/
+-rw-rw-rw-   0        0        0     1113 2022-09-27 05:30:21.000000 django-admin-datta-1.0.9/LICENSE.md
+-rw-rw-rw-   0        0        0      144 2023-02-09 15:44:00.000000 django-admin-datta-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     7277 2023-06-02 13:54:12.455344 django-admin-datta-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6182 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.775995 django-admin-datta-1.0.9/admin_datta/
+-rw-rw-rw-   0        0        0       78 2022-09-27 05:30:21.000000 django-admin-datta-1.0.9/admin_datta/__init__.py
+-rw-rw-rw-   0        0        0       78 2022-09-27 05:30:21.000000 django-admin-datta-1.0.9/admin_datta/admin.py
+-rw-rw-rw-   0        0        0      235 2023-02-09 15:45:05.000000 django-admin-datta-1.0.9/admin_datta/apps.py
+-rw-rw-rw-   0        0        0     2601 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/forms.py
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.800122 django-admin-datta-1.0.9/admin_datta/static/
+-rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-datta-1.0.9/admin_datta/static/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.679284 django-admin-datta-1.0.9/admin_datta/static/assets/
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.895445 django-admin-datta-1.0.9/admin_datta/static/assets/css/
+-rw-rw-rw-   0        0        0     3610 2023-02-28 04:48:58.000000 django-admin-datta-1.0.9/admin_datta/static/assets/css/dark.css
+-rw-rw-rw-   0        0        0     9732 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/css/forms.css
+-rw-rw-rw-   0        0        0   325947 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/css/style.css
+-rw-rw-rw-   0        0        0    12595 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/css/widgets.css
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.588302 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.897437 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/datta/
+-rw-rw-rw-   0        0        0     1623 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/datta/datta-icon.css
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.912574 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/datta/fonts/
+-rw-rw-rw-   0        0        0     2548 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/datta/fonts/pct.eot
+-rw-rw-rw-   0        0        0     2553 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/datta/fonts/pct.svg
+-rw-rw-rw-   0        0        0     2400 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/datta/fonts/pct.ttf
+-rw-rw-rw-   0        0        0     1544 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/datta/fonts/pct.woff
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.587302 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/feather/
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.926978 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/feather/css/
+-rw-rw-rw-   0        0        0    12312 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/feather/css/feather.css
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.993808 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/feather/fonts/
+-rw-rw-rw-   0        0        0    55828 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/feather/fonts/feather.eot
+-rw-rw-rw-   0        0        0   192354 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/feather/fonts/feather.svg
+-rw-rw-rw-   0        0        0    55664 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/feather/fonts/feather.ttf
+-rw-rw-rw-   0        0        0    26432 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/feather/fonts/feather.woff
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.608428 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.997808 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/css/
+-rw-rw-rw-   0        0        0    41069 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/css/fontawesome-all.min.css
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:11.292840 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/
+-rw-rw-rw-   0        0        0   111620 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.eot
+-rw-rw-rw-   0        0        0   600938 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.svg
+-rw-rw-rw-   0        0        0   111384 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0        0        0    71560 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff
+-rw-rw-rw-   0        0        0    61336 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0        0        0    31272 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.eot
+-rw-rw-rw-   0        0        0   105078 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.svg
+-rw-rw-rw-   0        0        0    31044 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0        0        0    14724 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff
+-rw-rw-rw-   0        0        0    12188 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0        0        0   133140 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.eot
+-rw-rw-rw-   0        0        0   490291 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.svg
+-rw-rw-rw-   0        0        0   132920 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0        0        0    63836 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff
+-rw-rw-rw-   0        0        0    50372 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:11.404652 django-admin-datta-1.0.9/admin_datta/static/assets/images/
+-rw-rw-rw-   0        0        0    45568 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/Thumbs.db
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:11.563951 django-admin-datta-1.0.9/admin_datta/static/assets/images/browser/
+-rw-rw-rw-   0        0        0    23040 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/browser/Thumbs.db
+-rw-rw-rw-   0        0        0     3822 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/browser/chrome.png
+-rw-rw-rw-   0        0        0     4809 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/browser/firefox.png
+-rw-rw-rw-   0        0        0     4359 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/browser/ie.png
+-rw-rw-rw-   0        0        0     3379 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/browser/opera.png
+-rw-rw-rw-   0        0        0     4915 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/browser/safari.png
+-rw-rw-rw-   0        0        0     1150 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/favicon.ico
+-rw-rw-rw-   0        0        0      334 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-addlink.svg
+-rw-rw-rw-   0        0        0     1095 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-calendar.svg
+-rw-rw-rw-   0        0        0      383 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-changelink.svg
+-rw-rw-rw-   0        0        0      686 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-clock.svg
+-rw-rw-rw-   0        0        0      395 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-deletelink.svg
+-rw-rw-rw-   0        0        0      563 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-no.svg
+-rw-rw-rw-   0        0        0      658 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-unknown-alt.svg
+-rw-rw-rw-   0        0        0      658 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-unknown.svg
+-rw-rw-rw-   0        0        0      584 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-viewlink.svg
+-rw-rw-rw-   0        0        0      439 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-yes.svg
+-rw-rw-rw-   0        0        0      563 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/inline-delete.svg
+-rw-rw-rw-   0        0        0     2091 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/logo-dark.png
+-rw-rw-rw-   0        0        0     1529 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/logo-thumb.png
+-rw-rw-rw-   0        0        0     2131 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/logo.png
+-rw-rw-rw-   0        0        0      461 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/search.svg
+-rw-rw-rw-   0        0        0     3325 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/selector-icons.svg
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:11.607135 django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/
+-rw-rw-rw-   0        0        0    31417 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img-slide-1.jpg
+-rw-rw-rw-   0        0        0    66369 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img-slide-2.jpg
+-rw-rw-rw-   0        0        0    22071 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img-slide-3.jpg
+-rw-rw-rw-   0        0        0    21820 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img-slide-4.jpg
+-rw-rw-rw-   0        0        0    33652 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img-slide-5.jpg
+-rw-rw-rw-   0        0        0   246009 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img1.jpg
+-rw-rw-rw-   0        0        0   165567 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img2.jpg
+-rw-rw-rw-   0        0        0   168914 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img3.jpg
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:11.717537 django-admin-datta-1.0.9/admin_datta/static/assets/images/user/
+-rw-rw-rw-   0        0        0    24576 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/user/Thumbs.db
+-rw-rw-rw-   0        0        0     9287 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/user/avatar-1.jpg
+-rw-rw-rw-   0        0        0     9372 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/user/avatar-2.jpg
+-rw-rw-rw-   0        0        0     9408 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/user/avatar-3.jpg
+-rw-rw-rw-   0        0        0     8489 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/user/avatar-4.jpg
+-rw-rw-rw-   0        0        0     9350 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/user/avatar-5.jpg
+-rw-rw-rw-   0        0        0     1662 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/user/user-1.png
+-rw-rw-rw-   0        0        0     1560 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/user/user-2.png
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:11.746187 django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/
+-rw-rw-rw-   0        0        0   120832 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/Thumbs.db
+-rw-rw-rw-   0        0        0   104704 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/dashborad-1.png
+-rw-rw-rw-   0        0        0   170223 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/dashborad-2.png
+-rw-rw-rw-   0        0        0   115557 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/dashborad-3.png
+-rw-rw-rw-   0        0        0    14068 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/dashborad-4.png
+-rw-rw-rw-   0        0        0     6239 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/dashborad-5.png
+-rw-rw-rw-   0        0        0     8193 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/dashborad-6.png
+-rw-rw-rw-   0        0        0   111459 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/emoticon.png
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:11.794603 django-admin-datta-1.0.9/admin_datta/static/assets/js/
+-rw-rw-rw-   0        0        0     2141 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/js/dark-mode.js
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:11.799602 django-admin-datta-1.0.9/admin_datta/static/assets/js/pages/
+-rw-rw-rw-   0        0        0     8008 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/js/pages/chart-morris-custom.js
+-rw-rw-rw-   0        0        0     4360 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/js/pages/google-maps.js
+-rw-rw-rw-   0        0        0    15247 2023-02-28 04:46:45.000000 django-admin-datta-1.0.9/admin_datta/static/assets/js/pcoded.min.js
+-rw-rw-rw-   0        0        0   117122 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/js/vendor-all.min.js
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.677284 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.658230 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:11.829794 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/
+-rw-rw-rw-   0        0        0   209489 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/amcharts.js
+-rw-rw-rw-   0        0        0   168766 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/ammap.min.js
+-rw-rw-rw-   0        0        0    12860 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/gauge.js
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:11.836964 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/images/
+-rw-rw-rw-   0        0        0      679 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/images/dragIconRoundBig.svg
+-rw-rw-rw-   0        0        0      539 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/images/lens.svg
+-rw-rw-rw-   0        0        0     2916 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/light.js
+-rw-rw-rw-   0        0        0    14700 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/pie.min.js
+-rw-rw-rw-   0        0        0     6464 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/radar.js
+-rw-rw-rw-   0        0        0    49491 2023-02-11 11:10:18.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/serial.js
+-rw-rw-rw-   0        0        0    30336 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/usaLow.js
+-rw-rw-rw-   0        0        0   130785 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/worldLow.js
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.660815 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/animation/
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:11.839954 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/animation/css/
+-rw-rw-rw-   0        0        0    57908 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/animation/css/animate.min.css
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.663761 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/bootstrap/
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:11.847472 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/bootstrap/css/
+-rw-rw-rw-   0        0        0   182626 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0        0        0   140893 2023-02-28 04:49:50.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:11.921974 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/bootstrap/js/
+-rw-rw-rw-   0        0        0   127709 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0        0        0    50698 2023-02-28 04:49:34.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0    19213 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/bootstrap/js/popover.js
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.666757 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/chart-morris/
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:11.971585 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/chart-morris/css/
+-rw-rw-rw-   0        0        0      435 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/chart-morris/css/morris.css
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.020669 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/chart-morris/js/
+-rw-rw-rw-   0        0        0    35658 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/chart-morris/js/morris.min.js
+-rw-rw-rw-   0        0        0    92631 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/chart-morris/js/raphael.min.js
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.668753 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/google-maps/
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.070944 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/google-maps/js/
+-rw-rw-rw-   0        0        0    46138 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/google-maps/js/gmaps.js
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.678285 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery/
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.115100 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery/js/
+-rw-rw-rw-   0        0        0    86929 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery/js/jquery.min.js
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.672273 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery-scrollbar/
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.103052 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery-scrollbar/css/
+-rw-rw-rw-   0        0        0     2851 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.106046 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery-scrollbar/js/
+-rw-rw-rw-   0        0        0    11662 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.676286 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery-ui/
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.108056 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery-ui/js/
+-rw-rw-rw-   0        0        0   477536 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery-ui/js/jquery-ui.js
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.119104 django-admin-datta-1.0.9/admin_datta/static/assets/scss/
+-rw-rw-rw-   0        0        0     3741 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/static/assets/scss/dark.scss
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.138645 django-admin-datta-1.0.9/admin_datta/templates/
+-rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-datta-1.0.9/admin_datta/templates/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.170848 django-admin-datta-1.0.9/admin_datta/templates/accounts/
+-rw-rw-rw-   0        0        0     1479 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-change-password.html
+-rw-rw-rw-   0        0        0      963 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-password-change-done.html
+-rw-rw-rw-   0        0        0      994 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-password-reset-complete.html
+-rw-rw-rw-   0        0        0     1494 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-password-reset-confirm.html
+-rw-rw-rw-   0        0        0     1028 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-password-reset-done.html
+-rw-rw-rw-   0        0        0     1494 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-reset-password.html
+-rw-rw-rw-   0        0        0     2184 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-signin.html
+-rw-rw-rw-   0        0        0     2288 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-signup.html
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.231515 django-admin-datta-1.0.9/admin_datta/templates/admin/
+-rw-rw-rw-   0        0        0        0 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/.gitkeep
+-rw-rw-rw-   0        0        0     1743 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/actions.html
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:10.685820 django-admin-datta-1.0.9/admin_datta/templates/admin/auth/
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.235921 django-admin-datta-1.0.9/admin_datta/templates/admin/auth/user/
+-rw-rw-rw-   0        0        0      471 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/auth/user/add_form.html
+-rw-rw-rw-   0        0        0     5360 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/auth/user/change_password.html
+-rw-rw-rw-   0        0        0     4438 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/change_form.html
+-rw-rw-rw-   0        0        0      691 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/change_form_object_tools.html
+-rw-rw-rw-   0        0        0     4508 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/change_list.html
+-rw-rw-rw-   0        0        0      605 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/change_list_object_tools.html
+-rw-rw-rw-   0        0        0     3232 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/change_list_results.html
+-rw-rw-rw-   0        0        0     5853 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/delete_confirmation.html
+-rw-rw-rw-   0        0        0     6198 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/delete_selected_confirmation.html
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.241485 django-admin-datta-1.0.9/admin_datta/templates/admin/edit_inline/
+-rw-rw-rw-   0        0        0     3893 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/edit_inline/stacked.html
+-rw-rw-rw-   0        0        0     7788 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/edit_inline/tabular.html
+-rw-rw-rw-   0        0        0      643 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/filter.html
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.247495 django-admin-datta-1.0.9/admin_datta/templates/admin/includes/
+-rw-rw-rw-   0        0        0     2572 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/includes/fieldset.html
+-rw-rw-rw-   0        0        0      339 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/includes/object_delete_summary.html
+-rw-rw-rw-   0        0        0    28386 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/index.html
+-rw-rw-rw-   0        0        0     2724 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/invalid_setup.html
+-rw-rw-rw-   0        0        0     3365 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/login.html
+-rw-rw-rw-   0        0        0     2818 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/object_history.html
+-rw-rw-rw-   0        0        0     2317 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/pagination.html
+-rw-rw-rw-   0        0        0     2155 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/search_form.html
+-rw-rw-rw-   0        0        0     1616 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/admin/submit_line.html
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.264529 django-admin-datta-1.0.9/admin_datta/templates/includes/
+-rw-rw-rw-   0        0        0      735 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/includes/breadcrumb.html
+-rw-rw-rw-   0        0        0     1758 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/includes/head.html
+-rw-rw-rw-   0        0        0     6705 2023-06-02 13:52:34.000000 django-admin-datta-1.0.9/admin_datta/templates/includes/navigation.html
+-rw-rw-rw-   0        0        0      168 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/includes/pre-loader.html
+-rw-rw-rw-   0        0        0      323 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/includes/scripts.html
+-rw-rw-rw-   0        0        0     8551 2023-02-27 06:26:13.000000 django-admin-datta-1.0.9/admin_datta/templates/includes/sidebar.html
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.286869 django-admin-datta-1.0.9/admin_datta/templates/layouts/
+-rw-rw-rw-   0        0        0      306 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/layouts/base-auth.html
+-rw-rw-rw-   0        0        0     1428 2023-05-31 07:29:40.000000 django-admin-datta-1.0.9/admin_datta/templates/layouts/base.html
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.331183 django-admin-datta-1.0.9/admin_datta/templates/pages/
+-rw-rw-rw-   0        0        0     2857 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/pages/chart-morris.html
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.410516 django-admin-datta-1.0.9/admin_datta/templates/pages/components/
+-rw-rw-rw-   0        0        0     1907 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/pages/components/bc_badges.html
+-rw-rw-rw-   0        0        0     4650 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/pages/components/bc_breadcrumb-pagination.html
+-rw-rw-rw-   0        0        0    12079 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/pages/components/bc_button.html
+-rw-rw-rw-   0        0        0     6970 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/pages/components/bc_collapse.html
+-rw-rw-rw-   0        0        0    10818 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/pages/components/bc_tabs.html
+-rw-rw-rw-   0        0        0     9952 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/pages/components/bc_typography.html
+-rw-rw-rw-   0        0        0     5996 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/pages/components/icon-feather.html
+-rw-rw-rw-   0        0        0    15591 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/pages/form_elements.html
+-rw-rw-rw-   0        0        0    28386 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/pages/index.html
+-rw-rw-rw-   0        0        0     5101 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/pages/map-google.html
+-rw-rw-rw-   0        0        0     3810 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/pages/profile.html
+-rw-rw-rw-   0        0        0      945 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/pages/sample-page.html
+-rw-rw-rw-   0        0        0     4635 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/pages/tbl_bootstrap.html
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.418234 django-admin-datta-1.0.9/admin_datta/templates/registration/
+-rw-rw-rw-   0        0        0        0 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/registration/.gitkeep
+-rw-rw-rw-   0        0        0     1458 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/registration/logged_out.html
+-rw-rw-rw-   0        0        0     1971 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/registration/password_change_done.html
+-rw-rw-rw-   0        0        0     3308 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templates/registration/password_change_form.html
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.443815 django-admin-datta-1.0.9/admin_datta/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     2550 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templatetags/admin_datta.py
+-rw-rw-rw-   0        0        0      178 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/templatetags/replace_value.py
+-rw-rw-rw-   0        0        0     2342 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/urls.py
+-rw-rw-rw-   0        0        0    16593 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/utils.py
+-rw-rw-rw-   0        0        0     4313 2023-02-11 11:10:19.000000 django-admin-datta-1.0.9/admin_datta/views.py
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.452332 django-admin-datta-1.0.9/django_admin_datta.egg-info/
+-rw-rw-rw-   0        0        0     7277 2023-06-02 13:54:08.000000 django-admin-datta-1.0.9/django_admin_datta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9583 2023-06-02 13:54:10.000000 django-admin-datta-1.0.9/django_admin_datta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 13:54:09.000000 django-admin-datta-1.0.9/django_admin_datta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 05:41:21.000000 django-admin-datta-1.0.9/django_admin_datta.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-06-02 13:54:09.000000 django-admin-datta-1.0.9/django_admin_datta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 13:54:12.453338 django-admin-datta-1.0.9/docs/
+-rw-rw-rw-   0        0        0       13 2022-09-27 05:30:21.000000 django-admin-datta-1.0.9/docs/blank.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 13:54:12.458352 django-admin-datta-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1343 2023-06-02 13:52:47.000000 django-admin-datta-1.0.9/setup.py
```

### Comparing `django-admin-datta-1.0.8/LICENSE.md` & `django-admin-datta-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/PKG-INFO` & `django-admin-datta-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-datta
-Version: 1.0.8
+Version: 1.0.9
 Summary: Modern template for Django admin interface
 Home-page: https://appseed.us/product/datta-able/django/
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `django-admin-datta-1.0.8/README.md` & `django-admin-datta-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/forms.py` & `django-admin-datta-1.0.9/admin_datta/forms.py`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/css/dark.css` & `django-admin-datta-1.0.9/admin_datta/static/assets/css/dark.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/css/forms.css` & `django-admin-datta-1.0.9/admin_datta/static/assets/css/forms.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/css/style.css` & `django-admin-datta-1.0.9/admin_datta/static/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/css/widgets.css` & `django-admin-datta-1.0.9/admin_datta/static/assets/css/widgets.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/datta-icon.css` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/datta/datta-icon.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.eot` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/datta/fonts/pct.eot`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/datta/fonts/pct.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.ttf` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/datta/fonts/pct.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.woff` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/datta/fonts/pct.woff`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/css/feather.css` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/feather/css/feather.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.eot` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/feather/fonts/feather.eot`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/feather/fonts/feather.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.ttf` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/feather/fonts/feather.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.woff` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/feather/fonts/feather.woff`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/css/fontawesome-all.min.css` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/css/fontawesome-all.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.eot` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.eot` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.eot` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2` & `django-admin-datta-1.0.9/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/Thumbs.db` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/Thumbs.db`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/Thumbs.db` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/browser/Thumbs.db`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/chrome.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/browser/chrome.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/firefox.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/browser/firefox.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/ie.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/browser/ie.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/opera.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/browser/opera.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/safari.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/browser/safari.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/favicon.ico` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-calendar.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-calendar.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-clock.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-clock.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-no.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-no.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-unknown-alt.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-unknown-alt.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-unknown.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-unknown.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-viewlink.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/icon-viewlink.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/inline-delete.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/inline-delete.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/logo-dark.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/logo-dark.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/logo-thumb.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/logo-thumb.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/logo.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/selector-icons.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/selector-icons.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-1.jpg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img-slide-1.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-2.jpg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img-slide-2.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-3.jpg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img-slide-3.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-4.jpg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img-slide-4.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-5.jpg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img-slide-5.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img1.jpg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img1.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img2.jpg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img2.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img3.jpg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/slider/img3.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/Thumbs.db` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/user/Thumbs.db`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-1.jpg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/user/avatar-1.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-2.jpg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/user/avatar-2.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-3.jpg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/user/avatar-3.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-4.jpg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/user/avatar-4.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-5.jpg` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/user/avatar-5.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/user-1.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/user/user-1.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/user-2.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/user/user-2.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/Thumbs.db` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/Thumbs.db`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-1.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/dashborad-1.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-2.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/dashborad-2.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-3.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/dashborad-3.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-4.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/dashborad-4.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-5.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/dashborad-5.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-6.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/dashborad-6.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/emoticon.png` & `django-admin-datta-1.0.9/admin_datta/static/assets/images/widget/emoticon.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/js/dark-mode.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/js/dark-mode.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/js/pages/chart-morris-custom.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/js/pages/chart-morris-custom.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/js/pages/google-maps.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/js/pages/google-maps.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/js/pcoded.min.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/js/pcoded.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/js/vendor-all.min.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/js/vendor-all.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/amcharts.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/amcharts.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/ammap.min.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/ammap.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/gauge.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/gauge.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/images/dragIconRoundBig.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/images/dragIconRoundBig.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/images/lens.svg` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/images/lens.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/light.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/light.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/pie.min.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/pie.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/radar.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/radar.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/serial.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/serial.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/usaLow.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/usaLow.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/worldLow.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/amchart/js/worldLow.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/animation/css/animate.min.css` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/animation/css/animate.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.css` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.min.css` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.min.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/js/popover.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/bootstrap/js/popover.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/js/morris.min.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/chart-morris/js/morris.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/js/raphael.min.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/chart-morris/js/raphael.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/google-maps/js/gmaps.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/google-maps/js/gmaps.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery/js/jquery.min.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-ui/js/jquery-ui.js` & `django-admin-datta-1.0.9/admin_datta/static/assets/plugins/jquery-ui/js/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/static/assets/scss/dark.scss` & `django-admin-datta-1.0.9/admin_datta/static/assets/scss/dark.scss`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-change-password.html` & `django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-change-password.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-change-done.html` & `django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-password-change-done.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-reset-complete.html` & `django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-password-reset-complete.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-reset-confirm.html` & `django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-password-reset-confirm.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-reset-done.html` & `django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-password-reset-done.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-reset-password.html` & `django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-reset-password.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-signin.html` & `django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-signin.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-signup.html` & `django-admin-datta-1.0.9/admin_datta/templates/accounts/auth-signup.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/actions.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/auth/user/change_password.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/change_form.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/change_form_object_tools.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/change_list.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/change_list_object_tools.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/change_list_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/change_list_results.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/delete_confirmation.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/delete_selected_confirmation.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/edit_inline/stacked.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/edit_inline/tabular.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/filter.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/includes/fieldset.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/index.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/invalid_setup.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/invalid_setup.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/login.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/object_history.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/pagination.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/search_form.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/admin/submit_line.html` & `django-admin-datta-1.0.9/admin_datta/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/includes/breadcrumb.html` & `django-admin-datta-1.0.9/admin_datta/templates/includes/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/includes/head.html` & `django-admin-datta-1.0.9/admin_datta/templates/includes/head.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/includes/navigation.html` & `django-admin-datta-1.0.9/admin_datta/templates/includes/navigation.html`

 * *Files 1% similar despite different names*

```diff
@@ -118,21 +118,21 @@
                 <a href="{% url 'logout' %}" class="dud-logout" title="Logout">
                 {% endif %}
                   <i class="feather icon-log-out"></i>
                 </a>
               {% endif %}
             </div>
             <ul class="pro-body">
-              <li><a href="javascript;" class="dropdown-item"><i class="feather icon-settings"></i>
+              <li><a href="#" class="dropdown-item"><i class="feather icon-settings"></i>
                   Settings</a></li>
-              <li><a href="javascript;" class="dropdown-item"><i class="feather icon-user"></i>
+              <li><a href="{% url 'profile' %}" class="dropdown-item"><i class="feather icon-user"></i>
                   Profile</a></li>
-              <li><a href="javascript;" class="dropdown-item"><i class="feather icon-mail"></i> My
+              <li><a href="#" class="dropdown-item"><i class="feather icon-mail"></i> My
                   Messages</a></li>
-              <li><a href="javascript;" class="dropdown-item"><i class="feather icon-lock"></i> Lock
+              <li><a href="#" class="dropdown-item"><i class="feather icon-lock"></i> Lock
                   Screen</a></li>
               {% if request.user.is_authenticated %}
               <li>
                 {% if request.user.is_superuser %}
                 <a href="{% url 'admin:password_change' %}" class="dropdown-item">
                 {% else %}
                 <a href="{% url 'password_change' %}" class="dropdown-item">
```

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/includes/sidebar.html` & `django-admin-datta-1.0.9/admin_datta/templates/includes/sidebar.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/layouts/base.html` & `django-admin-datta-1.0.9/admin_datta/templates/layouts/base.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/pages/chart-morris.html` & `django-admin-datta-1.0.9/admin_datta/templates/pages/chart-morris.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_badges.html` & `django-admin-datta-1.0.9/admin_datta/templates/pages/components/bc_badges.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_breadcrumb-pagination.html` & `django-admin-datta-1.0.9/admin_datta/templates/pages/components/bc_breadcrumb-pagination.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_button.html` & `django-admin-datta-1.0.9/admin_datta/templates/pages/components/bc_button.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_collapse.html` & `django-admin-datta-1.0.9/admin_datta/templates/pages/components/bc_collapse.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_tabs.html` & `django-admin-datta-1.0.9/admin_datta/templates/pages/components/bc_tabs.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_typography.html` & `django-admin-datta-1.0.9/admin_datta/templates/pages/components/bc_typography.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/pages/components/icon-feather.html` & `django-admin-datta-1.0.9/admin_datta/templates/pages/components/icon-feather.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/pages/form_elements.html` & `django-admin-datta-1.0.9/admin_datta/templates/pages/form_elements.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/pages/index.html` & `django-admin-datta-1.0.9/admin_datta/templates/pages/index.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/pages/map-google.html` & `django-admin-datta-1.0.9/admin_datta/templates/pages/map-google.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/pages/profile.html` & `django-admin-datta-1.0.9/admin_datta/templates/pages/profile.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/pages/sample-page.html` & `django-admin-datta-1.0.9/admin_datta/templates/pages/sample-page.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/pages/tbl_bootstrap.html` & `django-admin-datta-1.0.9/admin_datta/templates/pages/tbl_bootstrap.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/registration/logged_out.html` & `django-admin-datta-1.0.9/admin_datta/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/registration/password_change_done.html` & `django-admin-datta-1.0.9/admin_datta/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templates/registration/password_change_form.html` & `django-admin-datta-1.0.9/admin_datta/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/templatetags/admin_datta.py` & `django-admin-datta-1.0.9/admin_datta/templatetags/admin_datta.py`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/urls.py` & `django-admin-datta-1.0.9/admin_datta/urls.py`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/utils.py` & `django-admin-datta-1.0.9/admin_datta/utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/admin_datta/views.py` & `django-admin-datta-1.0.9/admin_datta/views.py`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/django_admin_datta.egg-info/PKG-INFO` & `django-admin-datta-1.0.9/django_admin_datta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-datta
-Version: 1.0.8
+Version: 1.0.9
 Summary: Modern template for Django admin interface
 Home-page: https://appseed.us/product/datta-able/django/
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `django-admin-datta-1.0.8/django_admin_datta.egg-info/SOURCES.txt` & `django-admin-datta-1.0.9/django_admin_datta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.8/setup.py` & `django-admin-datta-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
 name='django-admin-datta',
-version='1.0.8',
+version='1.0.9',
 zip_safe=False,
 packages=find_packages(),
 include_package_data=True,
 description='Modern template for Django admin interface',
 long_description=README,
 long_description_content_type="text/markdown",
 url='https://appseed.us/product/datta-able/django/',
```

