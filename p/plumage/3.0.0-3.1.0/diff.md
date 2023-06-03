# Comparing `tmp/plumage-3.0.0.tar.gz` & `tmp/plumage-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plumage-3.0.0.tar", max compression
+gzip compressed data, was "plumage-3.1.0.tar", max compression
```

## Comparing `plumage-3.0.0.tar` & `plumage-3.1.0.tar`

### file list

```diff
@@ -1,92 +1,89 @@
--rw-r--r--   0        0        0     1613 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/__init__.py
--rw-r--r--   0        0        0     2175 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/config.py
--rw-r--r--   0        0        0     4274 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/dom_transforms.py
--rw-r--r--   0        0        0     2440 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/favicon.py
--rw-r--r--   0        0        0    31893 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/package-lock.json
--rw-r--r--   0        0        0      233 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/package.json
--rw-r--r--   0        0        0       73 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/postcss.config.js
--rw-r--r--   0        0        0        0 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/py.typed
--rw-r--r--   0        0        0     2765 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/code.scss
--rw-r--r--   0        0        0     2143 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/main.scss
--rw-r--r--   0        0        0      720 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/mglass.scss
--rw-r--r--   0        0        0     4514 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/abap.css
--rw-r--r--   0        0        0     4690 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/algol.css
--rw-r--r--   0        0        0     4600 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/algol_nu.css
--rw-r--r--   0        0        0     4761 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/arduino.css
--rw-r--r--   0        0        0     5240 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/autumn.css
--rw-r--r--   0        0        0     4470 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/borland.css
--rw-r--r--   0        0        0     3195 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/bw.css
--rw-r--r--   0        0        0     6160 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/colorful.css
--rw-r--r--   0        0        0     5823 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/default.css
--rw-r--r--   0        0        0     5612 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/emacs.css
--rw-r--r--   0        0        0     5974 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/friendly.css
--rw-r--r--   0        0        0     6587 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/fruity.css
--rw-r--r--   0        0        0     2905 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/igor.css
--rw-r--r--   0        0        0     6144 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/inkpot.css
--rw-r--r--   0        0        0     5727 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/lovelace.css
--rw-r--r--   0        0        0     5678 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/manni.css
--rw-r--r--   0        0        0     5596 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/monokai.css
--rw-r--r--   0        0        0     6113 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/murphy.css
--rw-r--r--   0        0        0     6390 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/native.css
--rw-r--r--   0        0        0     5972 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/paraiso-dark.css
--rw-r--r--   0        0        0     6044 2023-03-08 07:31:13.551524 plumage-3.0.0/plumage/static/css/pygments/paraiso-light.css
--rw-r--r--   0        0        0     6130 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/pastie.css
--rw-r--r--   0        0        0     5516 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/perldoc.css
--rw-r--r--   0        0        0     6078 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/rainbow_dash.css
--rw-r--r--   0        0        0     2988 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/rrt.css
--rw-r--r--   0        0        0     5044 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/sas.css
--rw-r--r--   0        0        0     6733 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/solarized-dark.css
--rw-r--r--   0        0        0     6811 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/solarized-light.css
--rw-r--r--   0        0        0     4513 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/stata-dark.css
--rw-r--r--   0        0        0     4485 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/stata-light.css
--rw-r--r--   0        0        0     4203 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/stata.css
--rw-r--r--   0        0        0     6480 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/tango.css
--rw-r--r--   0        0        0     5292 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/trac.css
--rw-r--r--   0        0        0     5715 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/vim.css
--rw-r--r--   0        0        0     2956 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/vs.css
--rw-r--r--   0        0        0     4703 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/css/pygments/xcode.css
--rw-r--r--   0        0        0     1369 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/favicon/android-chrome-192x192.png
--rw-r--r--   0        0        0     3279 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/favicon/android-chrome-512x512.png
--rw-r--r--   0        0        0     1035 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/favicon/apple-touch-icon.png
--rw-r--r--   0        0        0      246 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/favicon/browserconfig.xml
--rw-r--r--   0        0        0      260 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/favicon/favicon-16x16.png
--rw-r--r--   0        0        0      388 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/favicon/favicon-32x32.png
--rw-r--r--   0        0        0    15086 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/favicon/favicon.ico
--rw-r--r--   0        0        0     1115 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/favicon/mstile-144x144.png
--rw-r--r--   0        0        0     1007 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/favicon/mstile-150x150.png
--rw-r--r--   0        0        0     1022 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/favicon/mstile-310x150.png
--rw-r--r--   0        0        0     1848 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/favicon/mstile-310x310.png
--rw-r--r--   0        0        0      843 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/favicon/mstile-70x70.png
--rw-r--r--   0        0        0     2152 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/favicon/safari-pinned-tab.svg
--rw-r--r--   0        0        0      426 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/favicon/site.webmanifest
--rw-r--r--   0        0        0     1655 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/img/creampaper.jpeg
--rw-r--r--   0        0        0     1074 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/img/fabric_plaid.jpeg
--rw-r--r--   0        0        0      641 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/img/feather-alt-solid.svg
--rw-r--r--   0        0        0     1211 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/img/magnifier.png
--rw-r--r--   0        0        0     3588 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/img/play-button.png
--rw-r--r--   0        0        0     3113 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/js/application.js
--rw-r--r--   0        0        0     2366 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/js/jquery.mglass.js
--rw-r--r--   0        0        0    33168 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/js/tipuesearch.js
--rw-r--r--   0        0        0     3042 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/static/js/tipuesearch_set.js
--rw-r--r--   0        0        0      387 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/analytics.html
--rw-r--r--   0        0        0     3493 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/archives.html
--rw-r--r--   0        0        0     7667 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/article.html
--rw-r--r--   0        0        0      317 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/author.html
--rw-r--r--   0        0        0     1076 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/authors.html
--rw-r--r--   0        0        0    17925 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/base.html
--rw-r--r--   0        0        0     1117 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/categories.html
--rw-r--r--   0        0        0      715 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/category.html
--rw-r--r--   0        0        0      780 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/index.html
--rw-r--r--   0        0        0     2048 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/macros.html
--rw-r--r--   0        0        0      477 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/page.html
--rw-r--r--   0        0        0     2920 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/pagination.html
--rw-r--r--   0        0        0     1159 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/period_archives.html
--rw-r--r--   0        0        0     6982 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/projects.html
--rw-r--r--   0        0        0      695 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/tag.html
--rw-r--r--   0        0        0     1581 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/tags.html
--rw-r--r--   0        0        0      285 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/templates/translations.html
--rw-r--r--   0        0        0     3865 2023-03-08 07:31:13.555524 plumage-3.0.0/plumage/webassets.py
--rw-r--r--   0        0        0     2229 2023-03-08 07:31:13.555524 plumage-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    26901 2023-03-08 07:31:13.555524 plumage-3.0.0/readme.md
--rw-r--r--   0        0        0    28439 1970-01-01 00:00:00.000000 plumage-3.0.0/setup.py
--rw-r--r--   0        0        0    28794 1970-01-01 00:00:00.000000 plumage-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1613 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/__init__.py
+-rw-r--r--   0        0        0     2175 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/config.py
+-rw-r--r--   0        0        0     3703 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/dom_transforms.py
+-rw-r--r--   0        0        0     2440 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/favicon.py
+-rw-r--r--   0        0        0    33129 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/package-lock.json
+-rw-r--r--   0        0        0      260 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/package.json
+-rw-r--r--   0        0        0       73 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/postcss.config.js
+-rw-r--r--   0        0        0        0 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/py.typed
+-rw-r--r--   0        0        0     2765 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/code.scss
+-rw-r--r--   0        0        0     5479 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/main.scss
+-rw-r--r--   0        0        0      724 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/mglass.scss
+-rw-r--r--   0        0        0     4514 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/abap.css
+-rw-r--r--   0        0        0     4690 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/algol.css
+-rw-r--r--   0        0        0     4600 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/algol_nu.css
+-rw-r--r--   0        0        0     4761 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/arduino.css
+-rw-r--r--   0        0        0     5240 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/autumn.css
+-rw-r--r--   0        0        0     4470 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/borland.css
+-rw-r--r--   0        0        0     3195 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/bw.css
+-rw-r--r--   0        0        0     6160 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/colorful.css
+-rw-r--r--   0        0        0     5823 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/default.css
+-rw-r--r--   0        0        0     5612 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/emacs.css
+-rw-r--r--   0        0        0     5974 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/friendly.css
+-rw-r--r--   0        0        0     6587 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/fruity.css
+-rw-r--r--   0        0        0     2905 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/igor.css
+-rw-r--r--   0        0        0     6144 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/inkpot.css
+-rw-r--r--   0        0        0     5727 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/lovelace.css
+-rw-r--r--   0        0        0     5678 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/manni.css
+-rw-r--r--   0        0        0     5596 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/monokai.css
+-rw-r--r--   0        0        0     6113 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/murphy.css
+-rw-r--r--   0        0        0     6390 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/native.css
+-rw-r--r--   0        0        0     5972 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/paraiso-dark.css
+-rw-r--r--   0        0        0     6044 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/paraiso-light.css
+-rw-r--r--   0        0        0     6130 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/pastie.css
+-rw-r--r--   0        0        0     5516 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/perldoc.css
+-rw-r--r--   0        0        0     6078 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/rainbow_dash.css
+-rw-r--r--   0        0        0     2988 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/rrt.css
+-rw-r--r--   0        0        0     5044 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/sas.css
+-rw-r--r--   0        0        0     6733 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/solarized-dark.css
+-rw-r--r--   0        0        0     6811 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/solarized-light.css
+-rw-r--r--   0        0        0     4513 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/stata-dark.css
+-rw-r--r--   0        0        0     4485 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/stata-light.css
+-rw-r--r--   0        0        0     4203 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/stata.css
+-rw-r--r--   0        0        0     6480 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/tango.css
+-rw-r--r--   0        0        0     5292 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/trac.css
+-rw-r--r--   0        0        0     5715 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/vim.css
+-rw-r--r--   0        0        0     2956 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/vs.css
+-rw-r--r--   0        0        0     4703 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/css/pygments/xcode.css
+-rw-r--r--   0        0        0     1369 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/android-chrome-192x192.png
+-rw-r--r--   0        0        0     3279 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/android-chrome-512x512.png
+-rw-r--r--   0        0        0     1035 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/apple-touch-icon.png
+-rw-r--r--   0        0        0      246 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/browserconfig.xml
+-rw-r--r--   0        0        0      260 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/favicon-16x16.png
+-rw-r--r--   0        0        0      388 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/favicon-32x32.png
+-rw-r--r--   0        0        0    15086 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/favicon.ico
+-rw-r--r--   0        0        0     1115 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/mstile-144x144.png
+-rw-r--r--   0        0        0     1007 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/mstile-150x150.png
+-rw-r--r--   0        0        0     1022 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/mstile-310x150.png
+-rw-r--r--   0        0        0     1848 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/mstile-310x310.png
+-rw-r--r--   0        0        0      843 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/mstile-70x70.png
+-rw-r--r--   0        0        0     2152 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      426 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/favicon/site.webmanifest
+-rw-r--r--   0        0        0     1655 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/img/creampaper.jpeg
+-rw-r--r--   0        0        0     1074 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/img/fabric_plaid.jpeg
+-rw-r--r--   0        0        0      641 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/img/feather-alt-solid.svg
+-rw-r--r--   0        0        0     1211 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/img/magnifier.png
+-rw-r--r--   0        0        0     3588 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/img/play-button.png
+-rw-r--r--   0        0        0     2543 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/js/application.js
+-rw-r--r--   0        0        0     2366 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/static/js/jquery.mglass.js
+-rw-r--r--   0        0        0      387 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/analytics.html
+-rw-r--r--   0        0        0     3493 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/archives.html
+-rw-r--r--   0        0        0     7667 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/article.html
+-rw-r--r--   0        0        0      317 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/author.html
+-rw-r--r--   0        0        0     1076 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/authors.html
+-rw-r--r--   0        0        0    17390 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/base.html
+-rw-r--r--   0        0        0     1117 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/categories.html
+-rw-r--r--   0        0        0      715 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/category.html
+-rw-r--r--   0        0        0      780 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/index.html
+-rw-r--r--   0        0        0     2048 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/macros.html
+-rw-r--r--   0        0        0      477 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/page.html
+-rw-r--r--   0        0        0     2920 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/pagination.html
+-rw-r--r--   0        0        0     1159 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/period_archives.html
+-rw-r--r--   0        0        0     6982 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/projects.html
+-rw-r--r--   0        0        0      695 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/tag.html
+-rw-r--r--   0        0        0     1581 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/tags.html
+-rw-r--r--   0        0        0      285 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/templates/translations.html
+-rw-r--r--   0        0        0     3864 2023-06-03 09:26:24.073969 plumage-3.1.0/plumage/webassets.py
+-rw-r--r--   0        0        0     2250 2023-06-03 09:26:24.077968 plumage-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    24824 2023-06-03 09:26:24.077968 plumage-3.1.0/readme.md
+-rw-r--r--   0        0        0    26875 1970-01-01 00:00:00.000000 plumage-3.1.0/PKG-INFO
```

### Comparing `plumage-3.0.0/plumage/__init__.py` & `plumage-3.1.0/plumage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 import logging
 from pathlib import Path
 
-__version__ = "3.0.0"
+__version__ = "3.1.0"
 
 """ Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
     __version__ = "1.2.3.dev1"  # Development release 1
     __version__ = "1.2.3a1"  # Alpha Release 1
     __version__ = "1.2.3b1"  # Beta Release 1
```

### Comparing `plumage-3.0.0/plumage/config.py` & `plumage-3.1.0/plumage/config.py`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/dom_transforms.py` & `plumage-3.1.0/plumage/dom_transforms.py`

 * *Files 20% similar despite different names*

```diff
@@ -54,15 +54,17 @@
         return True
 
     doc(main_images_selector).filter(exclude_external_images).add_class(
         "image-process-article-photo"
     )
 
     # Style blockquotes in the way Bootstrap does.
-    doc("blockquote").add_class("blockquote border-start border-primary-subtle bg-dark-subtle fs-6 border-4 ps-2")
+    doc("blockquote").add_class(
+        "blockquote border-start border-primary-subtle bg-dark-subtle fs-6 border-4 ps-2"
+    )
     doc("blockquote p").add_class("p-2")
 
     # Style code boxes.
     doc(".codehilite, .highlight").add_class(
         f"pygments-style-{context.get('CODE_STYLE')} rounded shadow-sm mb-3"
     )
 
@@ -81,20 +83,10 @@
         "light": {"light"},
         "dark": {"dark"},
     }
     for bootstrap_class, admo_classes in admo_map.items():
         for admo_class in admo_classes:
             doc(f".admonition.{admo_class}").add_class(f"alert-{bootstrap_class}")
 
-    # Tipue Search results styling.
-    doc("#tipue_search_results_count").add_class("text-body-secondary small float-end")
-    doc("#tipue_search_image_modal").add_class("d-none")
-    doc(".tipue_search_result").add_class("border-bottom border-secondary mb-4 pb-3")
-    doc(".tipue_search_content_title").add_class("h3")
-    doc(".tipue_search_content_bold").add_class("bg-warning rounded px-1")
-    doc(".tipue_search_content_url").add_class("small text-info")
-    doc(".tipue_search_image").add_class("float-start border rounded")
-    doc(".tipue_search_note").add_class("d-none")
-
     # Save result.
     with open(path, "w") as source:
         source.write(doc.outerHtml())
```

### Comparing `plumage-3.0.0/plumage/favicon.py` & `plumage-3.1.0/plumage/favicon.py`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/package-lock.json` & `plumage-3.1.0/plumage/package-lock.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953675881410257%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'autoprefixer': '^10.4.14', 'postcss': '^8.4.24', "*

 * *               "'bootstrap': '^5.3.0'}}, 'node_modules/autoprefixer': {'version': '10.4.14', "*

 * *               "'resolved': 'https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.14.tgz', "*

 * *               "'integrity': "*

 * *               "'sha512-FQzyfOsTlwVzjHxKEqRIAdJx9niO6VCBCoEwax/VLSoQF29ggECcPuBqUMZ+u8jCZOPSy8b8/8KnuFbp0SaFZQ==', "*

 * *               "'dependencies': {'browserslist': '^4.21.5', 'caniuse-lite': '^ […]*

```diff
@@ -1,15 +1,16 @@
 {
     "lockfileVersion": 3,
     "name": "plumage-webassets-pipeline",
     "packages": {
         "": {
             "dependencies": {
-                "autoprefixer": "^10.4.13",
-                "postcss": "^8.4.21",
+                "autoprefixer": "^10.4.14",
+                "bootstrap": "^5.3.0",
+                "postcss": "^8.4.24",
                 "postcss-cli": "^10.1.0"
             },
             "name": "plumage-webassets-pipeline"
         },
         "node_modules/@nodelib/fs.scandir": {
             "dependencies": {
                 "@nodelib/fs.stat": "2.0.5",
@@ -38,14 +39,24 @@
             "engines": {
                 "node": ">= 8"
             },
             "integrity": "sha512-oGB+UxlgWcgQkgwo8GcEGwemoTFt3FIO9ababBmaGwXIoBKZ+GTy0pP185beGg7Llih/NSHSV2XAs1lnznocSg==",
             "resolved": "https://registry.npmjs.org/@nodelib/fs.walk/-/fs.walk-1.2.8.tgz",
             "version": "1.2.8"
         },
+        "node_modules/@popperjs/core": {
+            "funding": {
+                "type": "opencollective",
+                "url": "https://opencollective.com/popperjs"
+            },
+            "integrity": "sha512-P1st0aksCrn9sGZhp8GMYwBnQsbvAWsZAX44oXNNvLHGqAOcoVxmjZiohstwQ7SqKnbR47akdNi+uleWD8+g6A==",
+            "peer": true,
+            "resolved": "https://registry.npmjs.org/@popperjs/core/-/core-2.11.8.tgz",
+            "version": "2.11.8"
+        },
         "node_modules/ansi-regex": {
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-quJQXlTSUGL2LH9SUXo8VwsY4soanhgo6LNSm84E1LBcE8s3O0wpdiRzyR9z/ZZJMlMWv37qOOb9pdJlMUEKFQ==",
             "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-5.0.1.tgz",
             "version": "5.0.1"
@@ -77,16 +88,16 @@
             "version": "3.1.3"
         },
         "node_modules/autoprefixer": {
             "bin": {
                 "autoprefixer": "bin/autoprefixer"
             },
             "dependencies": {
-                "browserslist": "^4.21.4",
-                "caniuse-lite": "^1.0.30001426",
+                "browserslist": "^4.21.5",
+                "caniuse-lite": "^1.0.30001464",
                 "fraction.js": "^4.2.0",
                 "normalize-range": "^0.1.2",
                 "picocolors": "^1.0.0",
                 "postcss-value-parser": "^4.2.0"
             },
             "engines": {
                 "node": "^10 || ^12 || >=14"
@@ -97,29 +108,47 @@
                     "url": "https://opencollective.com/postcss/"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/autoprefixer"
                 }
             ],
-            "integrity": "sha512-49vKpMqcZYsJjwotvt4+h/BCjJVnhGwcLpDt5xkcaOG3eLrG/HUYLagrihYsQ+qrIBgIzX1Rw7a6L8I/ZA1Atg==",
+            "integrity": "sha512-FQzyfOsTlwVzjHxKEqRIAdJx9niO6VCBCoEwax/VLSoQF29ggECcPuBqUMZ+u8jCZOPSy8b8/8KnuFbp0SaFZQ==",
             "peerDependencies": {
                 "postcss": "^8.1.0"
             },
-            "resolved": "https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.13.tgz",
-            "version": "10.4.13"
+            "resolved": "https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.14.tgz",
+            "version": "10.4.14"
         },
         "node_modules/binary-extensions": {
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-jDctJ/IVQbZoJykoeHbhXpOlNBqGNcwXJKJog42E5HDPUwQTSdjCHdihjj0DlnheQ7blbT6dHOafNAiS8ooQKA==",
             "resolved": "https://registry.npmjs.org/binary-extensions/-/binary-extensions-2.2.0.tgz",
             "version": "2.2.0"
         },
+        "node_modules/bootstrap": {
+            "funding": [
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/twbs"
+                },
+                {
+                    "type": "opencollective",
+                    "url": "https://opencollective.com/bootstrap"
+                }
+            ],
+            "integrity": "sha512-UnBV3E3v4STVNQdms6jSGO2CvOkjUMdDAVR2V5N4uCMdaIkaQjbcEAMqRimDHIs4uqBYzDAKCQwCB+97tJgHQw==",
+            "peerDependencies": {
+                "@popperjs/core": "^2.11.7"
+            },
+            "resolved": "https://registry.npmjs.org/bootstrap/-/bootstrap-5.3.0.tgz",
+            "version": "5.3.0"
+        },
         "node_modules/braces": {
             "dependencies": {
                 "fill-range": "^7.0.1"
             },
             "engines": {
                 "node": ">=8"
             },
@@ -161,17 +190,17 @@
                     "url": "https://opencollective.com/browserslist"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/caniuse-lite"
                 }
             ],
-            "integrity": "sha512-XFHJY5dUgmpMV25UqaD4kVq2LsiaU5rS8fb0f17pCoXQiQslzmFgnfOxfvo1bTpTqf7dwG/N/05CnLCnOEKmzA==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001456.tgz",
-            "version": "1.0.30001456"
+            "integrity": "sha512-oww27MtUmusatpRpCGSOneQk2/l5czXANDSFvsc7VuOQ86s3ANhZetpwXNf1zY/zdfP63Xvjz325DAdAoES13g==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001464.tgz",
+            "version": "1.0.30001464"
         },
         "node_modules/chokidar": {
             "dependencies": {
                 "anymatch": "~3.1.2",
                 "braces": "~3.0.2",
                 "glob-parent": "~5.1.2",
                 "is-binary-path": "~2.1.0",
@@ -493,17 +522,23 @@
         "node_modules/nanoid": {
             "bin": {
                 "nanoid": "bin/nanoid.cjs"
             },
             "engines": {
                 "node": "^10 || ^12 || ^13.7 || ^14 || >=15.0.1"
             },
-            "integrity": "sha512-MqBkQh/OHTS2egovRtLk45wEyNXwF+cokD+1YPf9u5VfJiRdAiRwB2froX5Co9Rh20xs4siNPm8naNotSD6RBw==",
-            "resolved": "https://registry.npmjs.org/nanoid/-/nanoid-3.3.4.tgz",
-            "version": "3.3.4"
+            "funding": [
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/ai"
+                }
+            ],
+            "integrity": "sha512-BGcqMMJuToF7i1rt+2PWSNVnWIkGCU78jBG3RxO/bZlnZPK2Cmi2QaffxGO/2RvWi9sL+FAiRiXMgsyxQ1DIDA==",
+            "resolved": "https://registry.npmjs.org/nanoid/-/nanoid-3.3.6.tgz",
+            "version": "3.3.6"
         },
         "node_modules/node-releases": {
             "integrity": "sha512-5GFldHPXVG/YZmFzJvKK2zDSzPKhEp0+ZR5SVaoSag9fsL5YgHbUHDfnG5494ISANDcK4KwPXAx2xqVEydmd7w==",
             "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-2.0.10.tgz",
             "version": "2.0.10"
         },
         "node_modules/normalize-path": {
@@ -552,34 +587,38 @@
             },
             "integrity": "sha512-udgsAY+fTnvv7kI7aaxbqwWNb0AHiB0qBO89PZKPkoTmGOgdbrHDKD+0B2X4uTfJ/FT1R09r9gTsjUjNJotuog==",
             "resolved": "https://registry.npmjs.org/pify/-/pify-2.3.0.tgz",
             "version": "2.3.0"
         },
         "node_modules/postcss": {
             "dependencies": {
-                "nanoid": "^3.3.4",
+                "nanoid": "^3.3.6",
                 "picocolors": "^1.0.0",
                 "source-map-js": "^1.0.2"
             },
             "engines": {
                 "node": "^10 || ^12 || >=14"
             },
             "funding": [
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/postcss/"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/postcss"
+                },
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-tP7u/Sn/dVxK2NnruI4H9BG+x+Wxz6oeZ1cJ8P6G/PZY0IKk4k/63TDsQf2kQq3+qoJeLm2kIBUNlZe3zgb4Zg==",
-            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.21.tgz",
-            "version": "8.4.21"
+            "integrity": "sha512-M0RzbcI0sO/XJNucsGjvWU9ERWxb/ytp1w6dKtxTKgixdtQDq4rmx/g8W1hnaheq9jgwL/oyEdH5Bc4WwJKMqg==",
+            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.24.tgz",
+            "version": "8.4.24"
         },
         "node_modules/postcss-cli": {
             "bin": {
                 "postcss": "index.js"
             },
             "dependencies": {
                 "chokidar": "^3.3.0",
@@ -858,17 +897,17 @@
             "resolved": "https://registry.npmjs.org/y18n/-/y18n-5.0.8.tgz",
             "version": "5.0.8"
         },
         "node_modules/yaml": {
             "engines": {
                 "node": ">= 14"
             },
-            "integrity": "sha512-e0WHiYql7+9wr4cWMx3TVQrNwejKaEe7/rHNmQmqRjazfOP5W8PB6Jpebb5o6fIapbz9o9+2ipcaTM2ZwDI6lw==",
-            "resolved": "https://registry.npmjs.org/yaml/-/yaml-2.2.1.tgz",
-            "version": "2.2.1"
+            "integrity": "sha512-CBKFWExMn46Foo4cldiChEzn7S7SRV+wqiluAb6xmueD/fGyRHIhX8m14vVGgeFWjN540nKCNVj6P21eQjgTuA==",
+            "resolved": "https://registry.npmjs.org/yaml/-/yaml-2.2.2.tgz",
+            "version": "2.2.2"
         },
         "node_modules/yargs": {
             "dependencies": {
                 "cliui": "^8.0.1",
                 "escalade": "^3.1.1",
                 "get-caller-file": "^2.0.5",
                 "require-directory": "^2.1.1",
```

### Comparing `plumage-3.0.0/plumage/static/css/code.scss` & `plumage-3.1.0/plumage/static/css/code.scss`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/mglass.scss` & `plumage-3.1.0/plumage/static/css/mglass.scss`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 .mglass {
   background-color: rgba(0, 0, 0, 0.3);
-  background-image: url(/theme/img/magnifier.png);
+  background-image: url("/theme/img/magnifier.png");
   background-position: center;
   background-repeat: no-repeat;
 
   box-shadow: 0 0 10rem 0 #000 inset;
   cursor: zoom-in;
   opacity: 0;
   position: absolute;
   z-index: 10;
 
   &:hover {
     opacity: 1;
   }
 
   #content .video & {
-    background-image: url(/theme/img/play-button.png);
+    background-image: url("/theme/img/play-button.png");
   }
 }
 
 .mfp-with-zoom {
   .mfp-container,
   &.mfp-bg {
     backface-visibility: hidden;
```

### Comparing `plumage-3.0.0/plumage/static/css/pygments/abap.css` & `plumage-3.1.0/plumage/static/css/pygments/abap.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/algol.css` & `plumage-3.1.0/plumage/static/css/pygments/algol.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/algol_nu.css` & `plumage-3.1.0/plumage/static/css/pygments/algol_nu.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/arduino.css` & `plumage-3.1.0/plumage/static/css/pygments/arduino.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/autumn.css` & `plumage-3.1.0/plumage/static/css/pygments/autumn.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/borland.css` & `plumage-3.1.0/plumage/static/css/pygments/borland.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/bw.css` & `plumage-3.1.0/plumage/static/css/pygments/bw.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/colorful.css` & `plumage-3.1.0/plumage/static/css/pygments/colorful.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/default.css` & `plumage-3.1.0/plumage/static/css/pygments/default.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/emacs.css` & `plumage-3.1.0/plumage/static/css/pygments/emacs.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/friendly.css` & `plumage-3.1.0/plumage/static/css/pygments/friendly.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/fruity.css` & `plumage-3.1.0/plumage/static/css/pygments/fruity.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/igor.css` & `plumage-3.1.0/plumage/static/css/pygments/igor.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/inkpot.css` & `plumage-3.1.0/plumage/static/css/pygments/inkpot.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/lovelace.css` & `plumage-3.1.0/plumage/static/css/pygments/lovelace.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/manni.css` & `plumage-3.1.0/plumage/static/css/pygments/manni.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/monokai.css` & `plumage-3.1.0/plumage/static/css/pygments/monokai.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/murphy.css` & `plumage-3.1.0/plumage/static/css/pygments/murphy.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/native.css` & `plumage-3.1.0/plumage/static/css/pygments/native.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/paraiso-dark.css` & `plumage-3.1.0/plumage/static/css/pygments/paraiso-dark.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/paraiso-light.css` & `plumage-3.1.0/plumage/static/css/pygments/paraiso-light.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/pastie.css` & `plumage-3.1.0/plumage/static/css/pygments/pastie.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/perldoc.css` & `plumage-3.1.0/plumage/static/css/pygments/perldoc.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/rainbow_dash.css` & `plumage-3.1.0/plumage/static/css/pygments/rainbow_dash.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/rrt.css` & `plumage-3.1.0/plumage/static/css/pygments/rrt.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/sas.css` & `plumage-3.1.0/plumage/static/css/pygments/sas.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/solarized-dark.css` & `plumage-3.1.0/plumage/static/css/pygments/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/solarized-light.css` & `plumage-3.1.0/plumage/static/css/pygments/solarized-light.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/stata-dark.css` & `plumage-3.1.0/plumage/static/css/pygments/stata-dark.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/stata-light.css` & `plumage-3.1.0/plumage/static/css/pygments/stata-light.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/stata.css` & `plumage-3.1.0/plumage/static/css/pygments/stata.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/tango.css` & `plumage-3.1.0/plumage/static/css/pygments/tango.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/trac.css` & `plumage-3.1.0/plumage/static/css/pygments/trac.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/vim.css` & `plumage-3.1.0/plumage/static/css/pygments/vim.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/vs.css` & `plumage-3.1.0/plumage/static/css/pygments/vs.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/css/pygments/xcode.css` & `plumage-3.1.0/plumage/static/css/pygments/xcode.css`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/favicon/android-chrome-192x192.png` & `plumage-3.1.0/plumage/static/favicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/favicon/android-chrome-512x512.png` & `plumage-3.1.0/plumage/static/favicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/favicon/apple-touch-icon.png` & `plumage-3.1.0/plumage/static/favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/favicon/favicon.ico` & `plumage-3.1.0/plumage/static/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/favicon/mstile-144x144.png` & `plumage-3.1.0/plumage/static/favicon/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/favicon/mstile-150x150.png` & `plumage-3.1.0/plumage/static/favicon/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/favicon/mstile-310x150.png` & `plumage-3.1.0/plumage/static/favicon/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/favicon/mstile-310x310.png` & `plumage-3.1.0/plumage/static/favicon/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/favicon/mstile-70x70.png` & `plumage-3.1.0/plumage/static/favicon/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/favicon/safari-pinned-tab.svg` & `plumage-3.1.0/plumage/static/favicon/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/img/creampaper.jpeg` & `plumage-3.1.0/plumage/static/img/creampaper.jpeg`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/img/fabric_plaid.jpeg` & `plumage-3.1.0/plumage/static/img/fabric_plaid.jpeg`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/img/feather-alt-solid.svg` & `plumage-3.1.0/plumage/static/img/feather-alt-solid.svg`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/img/magnifier.png` & `plumage-3.1.0/plumage/static/img/magnifier.png`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/img/play-button.png` & `plumage-3.1.0/plumage/static/img/play-button.png`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/static/js/application.js` & `plumage-3.1.0/plumage/static/js/application.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -23,24 +23,14 @@
             } else if (scrollTop <= navTop && isFixed) {
                 isFixed = 0
                 $nav.removeClass('fixed-top').addClass('rounded-3 d-block')
                 $brand.addClass('d-none')
             }
         };
 
-        // Tipue Search results styling.
-        $("#tipue_search_results_count").addClass('text-body-secondary small float-end');
-        $("#tipue_search_image_modal").addClass('d-none');
-        $(".tipue_search_result").addClass('border-bottom border-secondary mb-4 pb-3');
-        $(".tipue_search_content_title").addClass('h3');
-        $(".tipue_search_content_bold").addClass('bg-warning rounded px-1');
-        $(".tipue_search_content_url").addClass('small text-info');
-        $(".tipue_search_image").addClass('float-start border rounded');
-        $(".tipue_search_note").addClass('d-none');
-
         // YouTube URL parser. Source: https://stackoverflow.com/questions/2964678/jquery-youtube-url-validation-with-regex/10315969#10315969
         function parse_youtube_url(url) {
             var p = /^(?:https?:\/\/)?(?:www\.)?(?:youtu\.be\/|youtube\.com\/(?:embed\/|v\/|watch\?v=|watch\?.+&v=))((\w|-){11})(?:\S+)?$/;
             return (url.match(p)) ? RegExp.$1 : false;
         };
 
         // Activate zoom on content images in the main column and add an icon overlay
```

### Comparing `plumage-3.0.0/plumage/static/js/jquery.mglass.js` & `plumage-3.1.0/plumage/static/js/jquery.mglass.js`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/templates/archives.html` & `plumage-3.1.0/plumage/templates/archives.html`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/templates/article.html` & `plumage-3.1.0/plumage/templates/article.html`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/templates/authors.html` & `plumage-3.1.0/plumage/templates/authors.html`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/templates/base.html` & `plumage-3.1.0/plumage/templates/base.html`

 * *Files 4% similar despite different names*

```diff
@@ -13,33 +13,29 @@
         <title>
             {% block title %}
                 Home
             {% endblock title %}
         | {{ SITENAME|e }}</title>
         <meta name="author" content="{{ AUTHOR|e }}" />
         <meta name="generator" content="Pelican v{{ PELICAN_VERSION }}" />
-        <link rel="stylesheet"
-              href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.0-alpha1/css/bootstrap.min.css"
-              integrity="sha512-72OVeAaPeV8n3BdZj7hOkaPSEk/uwpDkaGyP4W2jSzAC8tfiO4LMEDWoL3uFp5mcZu+8Eehb4GhZWFwvrss69Q=="
-              crossorigin="anonymous"
-              referrerpolicy="no-referrer" />
+        {% assets filters="libsass,postcss,cssmin", output="css/main.min.css",
+            "css/mglass.scss", "css/main.scss", "css/pygments/" + CODE_STYLE + ".css", "css/code.scss" %}
+            <link rel="stylesheet" href="{{ SITEURL }}/{{ ASSET_URL }}" />
+        {% endassets %}
         <link rel="stylesheet"
               href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.3.0/css/all.min.css"
               integrity="sha512-SzlrxWUlpfuzQ+pcUCosxcglQRNAq/DZjVsC0lE40xsADsfeQoEypE+enwcOiGjk/bSuGGKHEyjSoQ1zVisanQ=="
               crossorigin="anonymous"
               referrerpolicy="no-referrer"/>
         <link rel="stylesheet"
               href="https://cdnjs.cloudflare.com/ajax/libs/magnific-popup.js/1.1.0/magnific-popup.min.css"
               integrity="sha512-+EoPw+Fiwh6eSeRK7zwIKG2MA8i3rV/DGa3tdttQGgWyatG/SkncT53KHQaS5Jh9MNOT3dmFL0FjTY08And/Cw=="
               crossorigin="anonymous"
               referrerpolicy="no-referrer"/>
-        {% assets filters="libsass,postcss,cssmin", output="css/main.min.css",
-            "css/mglass.scss", "css/main.scss", "css/pygments/" + CODE_STYLE + ".css", "css/code.scss" %}
-            <link rel="stylesheet" href="{{ SITEURL }}/{{ ASSET_URL }}" />
-        {% endassets %}
+        {% block extra_css %}{% endblock %}
         {% include "analytics.html" %}
         <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.3/jquery.min.js"
                 integrity="sha512-STof4xm1wgkfm7heWqFJVn58Hm3EtS31XFaagaa8VMReCXAkQnJZ+jEy8PCC/iT18dFy95WcExNHFTqLyp72eQ=="
                 crossorigin="anonymous"
                 referrerpolicy="no-referrer"></script>
         <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.0-alpha1/js/bootstrap.bundle.min.js"
                 integrity="sha512-Sct/LCTfkoqr7upmX9VZKEzXuRk5YulFoDTunGapYJdlCwA+Rl4RhgcPCLf7awTNLmIVrszTPNUFu4MSesep5Q=="
@@ -162,34 +158,22 @@
                                         {{ c.name }}
                                         {% if active_category %}<span class="visually-hidden">(current)</span>{% endif %}
                                     </a>
                                 </li>
                             {% endfor %}
                         {% endif %}
                     </ul>
-                    {% if TIPUE_SEARCH %}
-                        <form class="d-flex my-lg-0"
-                              role="search"
-                              action="{{ SITEURL }}/search.html"
-                              onsubmit="return validateForm(this.elements['q'].value);">
+                    {% if STORK_SEARCH %}
+                        <div class="position-relative dropdown">
                             <div class="input-group">
-                                <input
-                                    type="search"
-                                    name="q"
-                                    class="form-control border-secondary-subtle"
-                                    id="tipue_search_input"
-                                    placeholder="Search"
-                                    aria-label="Search"
-                                    aria-describedby="tipue_search_submit"
-                                    required/>
-                                <button class="btn btn-outline-secondary border-secondary-subtle" id="tipue_search_submit" type="submit">
-                                    <i class="fas fa-search fa-fw"></i>
-                                </button>
+                                <label class="input-group-text" for="sitesearch-input"><i class="fas fa-search fa-fw"></i></label>
+                                <input data-stork="sitesearch" id="sitesearch-input" class="form-control dropdown-toggle" placeholder="Search" data-bs-toggle="dropdown" aria-expanded="false" />
+                                <div data-stork="sitesearch-output" class="dropdown-menu dropdown-menu-end shadow"></div>
                             </div>
-                        </form>
+                        </div>
                     {% endif %}
                 </div>
             </nav>
         </div>
         <div class="container mt-5">
             {% set has_left_content = has_left or LEFT_SIDEBAR is defined %}
             {% set has_right_content = has_right or RIGHT_SIDEBAR is defined %}
@@ -201,19 +185,19 @@
             <div class="row">
                 {% if LAYOUT != 'full-width' and has_left_content %}
                     <div class="col-md-3">
                         {% block left_sidebar %}{% endblock %}
                         {{ LEFT_SIDEBAR }}
                     </div>
                 {% endif %}
-                <div id="content"
+                <main id="content"
                      role="main"
                      class=" {% if LAYOUT == 'full-width' %} offset-md-1 {% elif has_left_content and has_right_content %} col-md-6 {% elif has_left_content or has_right_content %} col-md-9 {% else %} col-md-12 {% endif %}">
                     {% block content %}{% endblock %}
-                </div>
+                </main>
                 {% if LAYOUT != 'full-width' and has_right_content %}
                     <div class="col-md-3">
                         {% block right_sidebar %}{% endblock %}
                         {{ RIGHT_SIDEBAR }}
                     </div>
                 {% endif %}
             </div>
@@ -319,9 +303,15 @@
                     theme by <a class="text-dark" href="https://kevin.deldycke.com">Kevin Deldycke</a>.
                 </div>
                 <div class="col-3 text-end d-flex flex-column">
                     <a class="mt-auto" href="#"><i class="fas fa-arrow-up"></i> Back to top</a>
                 </div>
             </div>
         </footer>
+        {% if STORK_SEARCH %}
+            <script src="https://files.stork-search.net/releases/v1.6.0/stork.js"></script>
+            <script>
+                stork.register("sitesearch", "{{ SITEURL }}/search-index.st")
+            </script>
+        {% endif %}
     </body>
 </html>
```

#### html2text {}

```diff
@@ -2,21 +2,20 @@
 
 
  {% if (page in hidden_articles) or (page in drafts) or (page in hidden_pages)
 or (page in draft_pages) %}
  {% else %}
  {% endif %}
 
-
-
-
  {% assets filters="libsass,postcss,cssmin", output="css/main.min.css", "css/
 mglass.scss", "css/main.scss", "css/pygments/" + CODE_STYLE + ".css", "css/
 code.scss" %}
- {% endassets %} {% include "analytics.html" %}
+ {% endassets %}
+
+ {% block extra_css %}{% endblock %} {% include "analytics.html" %}
  {% assets filters="closure_js", output="js/main.min.js", "js/
 jquery.mglass.js", "js/application.js" %}
  {% endassets %} {% block extra_js %}{% endblock %}
 
 
 
 
@@ -56,25 +55,24 @@
     * {% endfor %} {% if DISPLAY_PAGES_ON_MENU %} {% for p in pages %} {% set
       active_page = (p == page) -%}
     * {{_p.title_}}_{%_if_active_page_%}(current){%_endif_%}
     * {% endfor %} {% endif %} {% if DISPLAY_CATEGORIES_ON_MENU %} {% for c,
       null in categories %} {% set active_category = (c == category) -%}
     * {{_c.name_}}_{%_if_active_category_%}(current){%_endif_%}
     * {% endfor %} {% endif %}
-{% if TIPUE_SEARCH %}
-[Unknown INPUT type]
+{% if STORK_SEARCH %}
+ [                    ]
 {% endif %}
 {% set has_left_content = has_left or LEFT_SIDEBAR is defined %} {% set
 has_right_content = has_right or RIGHT_SIDEBAR is defined %}
 {% block top_center %}{% endblock %}
 {% if LAYOUT != 'full-width' and has_left_content %}
 {% block left_sidebar %}{% endblock %} {{ LEFT_SIDEBAR }}
-{% endif %}
-{% block content %}{% endblock %}
-{% if LAYOUT != 'full-width' and has_right_content %}
+{% endif %}  {% block content %}{% endblock %}  {% if LAYOUT != 'full-width'
+and has_right_content %}
 {% block right_sidebar %}{% endblock %} {{ RIGHT_SIDEBAR }}
 {% endif %}
 {# TODO: make footer sticky #}
 {% set SOCIAL_WIDGET_NAME = SOCIAL_WIDGET_NAME or 'Social' %} {% set
 LINKS_WIDGET_NAME = LINKS_WIDGET_NAME or 'Links' %} {% for group_title,
 group_links in ((SOCIAL_WIDGET_NAME, SOCIAL), (LINKS_WIDGET_NAME, LINKS)) %}
 {% if group_links %}
@@ -112,7 +110,9 @@
     * {% for feed in all_feeds %}
     *  {{_feed.name_}}_({{_feed.kind_}})
     * {% endfor %}
 {% endif %}
 Site generated by Pelican.
 Plumage theme by Kevin_Deldycke.
  Back_to_top
+ {% if STORK_SEARCH %}
+ {% endif %}
```

### Comparing `plumage-3.0.0/plumage/templates/categories.html` & `plumage-3.1.0/plumage/templates/categories.html`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/templates/category.html` & `plumage-3.1.0/plumage/templates/category.html`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/templates/index.html` & `plumage-3.1.0/plumage/templates/index.html`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/templates/macros.html` & `plumage-3.1.0/plumage/templates/macros.html`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/templates/pagination.html` & `plumage-3.1.0/plumage/templates/pagination.html`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/templates/period_archives.html` & `plumage-3.1.0/plumage/templates/period_archives.html`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/templates/projects.html` & `plumage-3.1.0/plumage/templates/projects.html`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/templates/tag.html` & `plumage-3.1.0/plumage/templates/tag.html`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/templates/tags.html` & `plumage-3.1.0/plumage/templates/tags.html`

 * *Files identical despite different names*

### Comparing `plumage-3.0.0/plumage/webassets.py` & `plumage-3.1.0/plumage/webassets.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     # No need to force a compressed rendering, a minification pass is applied
     # at the end of the pipeline. See:
     # https://webassets.readthedocs.io/en/latest/builtin_filters.html#webassets.filter.libsass.LibSass
     # "LIBSASS_STYLE": "compressed",
 }
 """Default configuration for `webassets <https://github.com/miracle2k/webassets>`_.
 
-See the `list of configuration parameters for each filter
-<https://webassets.readthedocs.io/en/latest/builtin_filters.html>`_.
+See the
+`list of configuration parameters for each filter<https://webassets.readthedocs.io/en/latest/builtin_filters.html>`_.
 """
 
 
 CLI_NAME = "postcss"
 """Name of the PostCSS CLI binary."""
```

### Comparing `plumage-3.0.0/pyproject.toml` & `plumage-3.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "plumage"
-version = "3.0.0"
+version = "3.1.0"
 description = "Clean and tidy theme for Pelican."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/plumage'
 repository = 'https://github.com/kdeldycke/plumage'
 documentation = 'https://github.com/kdeldycke/plumage#settings'
 keywords = [
     'pelican',
     'pelican-theme',
-    'tipue-search',
+    'stork',
+    'static-search',
     'masonry',
     'theme',
     'bootstrap',
     'jquery',
     'font-awesome',
 ]
 classifiers = [
@@ -39,29 +40,29 @@
 "Funding" = "https://github.com/sponsors/kdeldycke"
 "Issues" = "https://github.com/kdeldycke/plumage/issues"
 "Changelog" = "https://github.com/kdeldycke/plumage/blob/main/changelog.md#changelog"
 
 [tool.poetry.dependencies]
 # List of python versions and their support status:
 # https://en.wikipedia.org/wiki/History_of_Python#Support
-python = "^3.11"
-closure = "^20191111"         # XXX Unmaintained!
-cssmin = "^0.2.0"             # XXX Unmaintained!
+python = "^3.8"
+closure = "^20191111"          # XXX Unmaintained!
+cssmin = "^0.2.0"              # XXX Unmaintained!
 libsass = "^0.22.0"
 Markdown = "^3.4.1"
 pelican = "^4.8.0"
 pelican-webassets = "^2.0.0"
 pygments = "^2.14.0"
-pymdown-extensions = "^9.9.2"
+pymdown-extensions = "^10.0.1"
 pynpm = "^0.1.2"
 pyquery = "^2.0.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 bump2version = "^1.0.1"
-djlint = "^1.19.16"
+djlint = "^1.30.2"
 mypy = "^1.1"
 types-Pygments = "^2.14.0"
 
 [tool.mypy]
 warn_unused_configs = true
 warn_redundant_casts = true
 warn_unused_ignores = true
```

### Comparing `plumage-3.0.0/readme.md` & `plumage-3.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,52 @@
+Metadata-Version: 2.1
+Name: plumage
+Version: 3.1.0
+Summary: Clean and tidy theme for Pelican.
+Home-page: https://github.com/kdeldycke/plumage
+License: GPL-2.0-or-later
+Keywords: pelican,pelican-theme,stork,static-search,masonry,theme,bootstrap,jquery,font-awesome
+Author: Kevin Deldycke
+Author-email: kevin@deldycke.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Plugins
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Pelican :: Themes
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Other
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Text Processing :: Markup :: HTML
+Classifier: Typing :: Typed
+Requires-Dist: Markdown (>=3.4.1,<4.0.0)
+Requires-Dist: closure (>=20191111,<20191112)
+Requires-Dist: cssmin (>=0.2.0,<0.3.0)
+Requires-Dist: libsass (>=0.22.0,<0.23.0)
+Requires-Dist: pelican (>=4.8.0,<5.0.0)
+Requires-Dist: pelican-webassets (>=2.0.0,<3.0.0)
+Requires-Dist: pygments (>=2.14.0,<3.0.0)
+Requires-Dist: pymdown-extensions (>=10.0.1,<11.0.0)
+Requires-Dist: pynpm (>=0.1.2,<0.2.0)
+Requires-Dist: pyquery (>=2.0.0,<3.0.0)
+Project-URL: Changelog, https://github.com/kdeldycke/plumage/blob/main/changelog.md#changelog
+Project-URL: Documentation, https://github.com/kdeldycke/plumage#settings
+Project-URL: Funding, https://github.com/sponsors/kdeldycke
+Project-URL: Issues, https://github.com/kdeldycke/plumage/issues
+Project-URL: Repository, https://github.com/kdeldycke/plumage
+Description-Content-Type: text/markdown
+
 <p align="center">
   <a href="https://github.com/kdeldycke/plumage/">
     <img src="https://github.com/kdeldycke/plumage/raw/main/screenshots/plumage-header-logo.jpeg" alt="Plumage, a Pelican theme">
   </a>
 </p>
 
 Plumage is a clean and tidy theme for [Pelican](https://getpelican.com), a
@@ -28,15 +73,15 @@
   | :--------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------: |
   | Code showcase ([source](https://github.com/kdeldycke/kevin-deldycke-blog/blob/ebe0d17a59730457c3016dff77fdfa799a80d756/content/templates/code.html)) | Videos showcase ([source](https://github.com/kdeldycke/kevin-deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/videos.html)) | Themes showcase ([source](https://github.com/kdeldycke/kevin-deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/themes.html)) |
 
 - Based on [Bootstrap v4](https://getbootstrap.com).
 
 - [Code syntax highlighting](#code-syntax-highlighting) with [30+ styles](https://github.com/pygments/pygments/tree/master/pygments/styles).
 
-- Site-wide static search via [Tipue-search](https://web.archive.org/web/20200703134724/https://tipue.com/search/).
+- Site-wide static search via [Stork](https://stork-search.net).
 
 - Bare YouTube links in articles gets rendered as embedded videos:
 
   ![Plumage YouTube link](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/youtube-link.jpeg)
 
 - Direct link to edit articles on GitHub:
 
@@ -60,15 +105,15 @@
 
 | Plugin name                                                                                                      | Type               | Status   | Notes                                                                                                         |
 | :--------------------------------------------------------------------------------------------------------------- | :----------------- | :------- | :------------------------------------------------------------------------------------------------------------ |
 | [`pelican-image-process`](https://github.com/pelican-plugins/image-process)                                      | Pelican plugin     | Optional | Embed a hack to [fix parsing of external images](https://github.com/pelican-plugins/image-process/issues/33). |
 | [`pelican-neighbors`](https://github.com/pelican-plugins/neighbors)                                              | Pelican plugin     | Optional |                                                                                                               |
 | [`pelican-related-posts`](https://github.com/pelican-plugins/related-posts)                                      | Pelican plugin     | Optional |                                                                                                               |
 | [`pelican-similar-posts`](https://github.com/pelican-plugins/similar-posts)                                      | Pelican plugin     | Optional |                                                                                                               |
-| [`pelican-tipue-search`](https://github.com/pelican-plugins/tipue-search)                                        | Pelican plugin     | Optional |                                                                                                               |
+| [`pelican-search`](https://github.com/pelican-plugins/search)                                                    | Pelican plugin     | Optional |                                                                                                               |
 | [`pelican-webassets`](https://github.com/pelican-plugins/webassets)                                              | Pelican plugin     | Required |                                                                                                               |
 | [`markdown.extensions.admonition`](https://python-markdown.github.io/extensions/admonition/)                     | Markdown extension | Optional | Re-style admonitions into [alerts](https://getbootstrap.com/docs/4.5/components/alerts/).                     |
 | [`markdown.extensions.codehilite`](https://python-markdown.github.io/extensions/code_hilite/)                    | Markdown extension | Optional | Style highlighted code with Pygment style.                                                                    |
 | [`markdown.extensions.toc`](https://python-markdown.github.io/extensions/toc/#usage)                             | Markdown extension | Optional | Adds permalink anchors to article's subtitles.                                                                |
 | [`pymdownx.emoji`](https://facelessuser.github.io/pymdown-extensions/extensions/emoji/#default-emoji-generators) | Markdown extension | Optional | Style `emojione` set for proper integration into text.                                                        |
 | [`pymdownx.highlight`](https://facelessuser.github.io/pymdown-extensions/extensions/highlight/)                  | Markdown extension | Optional | Style highlighted code with Pygment style.                                                                    |
 | [`typogrify`](https://pypi.python.org/pypi/typogrify)                                                            | Pelican builtin    | Optional | Style ampersands.                                                                                             |
@@ -131,35 +176,35 @@
 ```
 
 ## Settings
 
 Plumage can be customized by adding these optionnal parameters to your
 `pelicanconf.py` file:
 
-| Setting name                                                                                  | Default value | Description                                                                                                                                                                                                                           |
-| :-------------------------------------------------------------------------------------------- | :------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
-| `ARTICLE_EDIT_LINK`                                                                           |               | Generate an edit link besides each article. Can use `%(slug)s` to include dynamic article's slug in the link.                                                                                                                         |
-| `CODE_STYLE`                                                                                  | `"monokai"`   | Pygments' style ID. Choose one from `poetry run pygmentize -L styles`.                                                                                                                                                                |
-| `COPYRIGHT`                                                                                   |               | Additional copyright statement to add in the third column of the footer.                                                                                                                                                              |
-| `DISCLAIMER`                                                                                  |               | Overide the disclaimer notice that gets displayed at the fourth column of the footer.                                                                                                                                                 |
-| [`DISQUS_SITENAME`](http://docs.getpelican.com/en/stable/settings.html#DISQUS_SITENAME)       |               | Pelican can handle Disqus comments. Specify the Disqus sitename identifier here.                                                                                                                                                      |
-| `FAVICON_LINKS`                                                                               | `True`        | Fetch link's icons from [Google's favicons webservice](https://www.google.com/s2/favicons).                                                                                                                                           |
-| [`GOOGLE_ANALYTICS`](http://docs.getpelican.com/en/stable/settings.html#GOOGLE_ANALYTICS)     |               | Set to `UA-XXXXXX-Y` Property's tracking ID to activate Google Analytics.                                                                                                                                                             |
-| `LEFT_SIDEBAR`                                                                                |               | HTML content to put as-is in the left sidebar.                                                                                                                                                                                        |
-| [`LINKS_WIDGET_NAME`](http://docs.getpelican.com/en/stable/settings.html#LINKS_WIDGET_NAME)   | `"Links"`     | Allows override of the name of the links widget.                                                                                                                                                                                      |
-| [`LINKS`](http://docs.getpelican.com/en/stable/settings.html#LINKS)                           |               | A list of tuples (Title, URL) for links to appear in the second column of the footer.                                                                                                                                                 |
-| [`MANUAL_LINKS`](http://docs.getpelican.com/en/stable/settings.html#MANUAL_LINKS)             |               | When enabling this, you must pass the links (in LINKS & SOCIAL settins) not as tuples anymore, but as list, where every entry is formatted as you like                                                                                |
-| [`MENUITEMS`](http://docs.getpelican.com/en/stable/settings.html#MENUITEMS)                   |               | A list of tuples (Title, URL) for additional menu items to appear at the beginning of the main menu.                                                                                                                                  |
-| `RIGHT_SIDEBAR`                                                                               |               | HTML content to put as-is in the right sidebar.                                                                                                                                                                                       |
-| [`SITESUBTITLE`](http://docs.getpelican.com/en/stable/settings.html#SITESUBTITLE)             |               | A subtitle to appear in the header.                                                                                                                                                                                                   |
-| `SITE_THUMBNAIL_TEXT`                                                                         |               | Text displayed behind site's thumbnail.                                                                                                                                                                                               |
-| `SITE_THUMBNAIL`                                                                              |               | Site's thumbnail URL as displayed in the header. Should be a square image of at least 80x80 pixels.                                                                                                                                   |
-| [`SOCIAL_WIDGET_NAME`](http://docs.getpelican.com/en/stable/settings.html#SOCIAL_WIDGET_NAME) | `"Social"`    | Allows override of the name of the “social” widget.                                                                                                                                                                                   |
-| [`SOCIAL`](http://docs.getpelican.com/en/stable/settings.html#SOCIAL)                         |               | A list of tuples (Title, URL) to appear in the first columns of the footer.                                                                                                                                                           |
-| `TIPUE_SEARCH`                                                                                | `False`       | Activate [Tipue Search](https://web.archive.org/web/20200703134724/https://tipue.com/search/) (javascript static search engine) into the site. Requires the [`tipue_search`](https://github.com/pelican-plugins/tipue-search) plugin. |
+| Setting name                                                                                  | Default value | Description                                                                                                                                                    |
+| :-------------------------------------------------------------------------------------------- | :------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `ARTICLE_EDIT_LINK`                                                                           |               | Generate an edit link besides each article. Can use `%(slug)s` to include dynamic article's slug in the link.                                                  |
+| `CODE_STYLE`                                                                                  | `"monokai"`   | Pygments' style ID. Choose one from `poetry run pygmentize -L styles`.                                                                                         |
+| `COPYRIGHT`                                                                                   |               | Additional copyright statement to add in the third column of the footer.                                                                                       |
+| `DISCLAIMER`                                                                                  |               | Overide the disclaimer notice that gets displayed at the fourth column of the footer.                                                                          |
+| [`DISQUS_SITENAME`](http://docs.getpelican.com/en/stable/settings.html#DISQUS_SITENAME)       |               | Pelican can handle Disqus comments. Specify the Disqus sitename identifier here.                                                                               |
+| `FAVICON_LINKS`                                                                               | `True`        | Fetch link's icons from [Google's favicons webservice](https://www.google.com/s2/favicons).                                                                    |
+| [`GOOGLE_ANALYTICS`](http://docs.getpelican.com/en/stable/settings.html#GOOGLE_ANALYTICS)     |               | Set to `UA-XXXXXX-Y` Property's tracking ID to activate Google Analytics.                                                                                      |
+| `LEFT_SIDEBAR`                                                                                |               | HTML content to put as-is in the left sidebar.                                                                                                                 |
+| [`LINKS_WIDGET_NAME`](http://docs.getpelican.com/en/stable/settings.html#LINKS_WIDGET_NAME)   | `"Links"`     | Allows override of the name of the links widget.                                                                                                               |
+| [`LINKS`](http://docs.getpelican.com/en/stable/settings.html#LINKS)                           |               | A list of tuples (Title, URL) for links to appear in the second column of the footer.                                                                          |
+| [`MANUAL_LINKS`](http://docs.getpelican.com/en/stable/settings.html#MANUAL_LINKS)             |               | When enabling this, you must pass the links (in LINKS & SOCIAL settins) not as tuples anymore, but as list, where every entry is formatted as you like         |
+| [`MENUITEMS`](http://docs.getpelican.com/en/stable/settings.html#MENUITEMS)                   |               | A list of tuples (Title, URL) for additional menu items to appear at the beginning of the main menu.                                                           |
+| `RIGHT_SIDEBAR`                                                                               |               | HTML content to put as-is in the right sidebar.                                                                                                                |
+| [`SITESUBTITLE`](http://docs.getpelican.com/en/stable/settings.html#SITESUBTITLE)             |               | A subtitle to appear in the header.                                                                                                                            |
+| `SITE_THUMBNAIL_TEXT`                                                                         |               | Text displayed behind site's thumbnail.                                                                                                                        |
+| `SITE_THUMBNAIL`                                                                              |               | Site's thumbnail URL as displayed in the header. Should be a square image of at least 80x80 pixels.                                                            |
+| [`SOCIAL_WIDGET_NAME`](http://docs.getpelican.com/en/stable/settings.html#SOCIAL_WIDGET_NAME) | `"Social"`    | Allows override of the name of the “social” widget.                                                                                                            |
+| [`SOCIAL`](http://docs.getpelican.com/en/stable/settings.html#SOCIAL)                         |               | A list of tuples (Title, URL) to appear in the first columns of the footer.                                                                                    |
+| `STORK_SEARCH`                                                                                | `False`       | Activate [Stork](https://stork-search.net) static search engine. Requires the [official Pelican's `search` plugin](https://github.com/pelican-plugins/search). |
 
 Most of these [parameters are similar to `notmyidea`'s
 ](https://docs.getpelican.com/en/latest/settings.html#themes) (Pelican's default
 theme). For usage example, please have a look into [my own `pelicanconf.py`
 ](https://github.com/kdeldycke/kevin-deldycke-blog/blob/main/pelicanconf.py).
 
 The theme is also sensible to this list of [standard Pelican parameters
@@ -330,35 +375,18 @@
 
 ```markdown
 ![Image title](/folder/image.png){: .noZoom}
 ```
 
 ### Why is the search not working?
 
-The [`tipue-search`](https://github.com/pelican-plugins/tipue-search) needs to
-be installed then have an additional template file registered in your
-`pelicanconf.py`.
-
-There are two alternatives:
-
-- update the `TEMPLATE_PAGES` variable:
-
-  ```python
-  TEMPLATE_PAGES = {
-      (…)
-      "search.html": "search.html",
-   }
-  ```
-
-- or `DIRECT_TEMPLATES`:
-  ([example](https://github.com/kdeldycke/kevin-deldycke-blog/commit/cd4bf8d1f4c55d835d7bfe1d7233cffe48e67a8a)):
-
-  ```python
-  DIRECT_TEMPLATES = [(…), "search"]
-  ```
+The [official Pelican's `search` plugin](https://github.com/pelican-plugins/search) needs to
+be installed.
+
+TODO: Activate search field automaticcaly if the plugin is present.
 
 ## License
 
 This software is licensed under the [GNU General Public License v2 or later
 (GPLv2+)](https://github.com/kdeldycke/plumage/blob/main/LICENSE).
 
 Copyright (C) 2012-2020 [Kevin Deldycke](https://kevin.deldycke.com) and
@@ -366,21 +394,14 @@
 
 ## Third-party assets
 
 The theme embed copies of some external softwares, scripts, libraries and
 artworks:
 
 ```text
-Tipue Search v7.1
-Copyright (c) 2019 Tipue
-Distributed under a MIT license
-Source: https://web.archive.org/web/20200703134724/https://www.tipue.com/search/tipuesearch.zip
-```
-
-```text
 jQuery MGlass v1.1
 Copyright (c) 2012 Younès El Biache
 Distributed under a MIT license
 Source: https://github.com/younes0/jQuery-MGlass
 ```
 
 ```text
@@ -404,7 +425,8 @@
 Source: https://fontawesome.com/icons/feather-alt?style=solid
 ```
 
 ```text
 Macro shot of White Feather
 Source: https://unsplash.com/photos/Sw7f58YJbc0
 ```
+
```

#### html2text {}

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1 Name: plumage Version: 3.1.0 Summary: Clean and tidy
+theme for Pelican. Home-page: https://github.com/kdeldycke/plumage License:
+GPL-2.0-or-later Keywords: pelican,pelican-theme,stork,static-
+search,masonry,theme,bootstrap,jquery,font-awesome Author: Kevin Deldycke
+Author-email: kevin@deldycke.com Requires-Python: >=3.8,<4.0 Classifier:
+Development Status :: 5 - Production/Stable Classifier: Environment :: Plugins
+Classifier: Environment :: Web Environment Classifier: Framework :: Pelican ::
+Themes Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Information Technology Classifier: License :: OSI Approved :: GNU
+General Public License v2 or later (GPLv2+) Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: JavaScript Classifier:
+Programming Language :: Other Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Internet :: WWW/HTTP Classifier: Topic :: Text Processing :: Markup :: HTML
+Classifier: Typing :: Typed Requires-Dist: Markdown (>=3.4.1,<4.0.0) Requires-
+Dist: closure (>=20191111,<20191112) Requires-Dist: cssmin (>=0.2.0,<0.3.0)
+Requires-Dist: libsass (>=0.22.0,<0.23.0) Requires-Dist: pelican
+(>=4.8.0,<5.0.0) Requires-Dist: pelican-webassets (>=2.0.0,<3.0.0) Requires-
+Dist: pygments (>=2.14.0,<3.0.0) Requires-Dist: pymdown-extensions
+(>=10.0.1,<11.0.0) Requires-Dist: pynpm (>=0.1.2,<0.2.0) Requires-Dist: pyquery
+(>=2.0.0,<3.0.0) Project-URL: Changelog, https://github.com/kdeldycke/plumage/
+blob/main/changelog.md#changelog Project-URL: Documentation, https://
+github.com/kdeldycke/plumage#settings Project-URL: Funding, https://github.com/
+sponsors/kdeldycke Project-URL: Issues, https://github.com/kdeldycke/plumage/
+issues Project-URL: Repository, https://github.com/kdeldycke/plumage
+Description-Content-Type: text/markdown
                           [Plumage,_a_Pelican_theme]
 Plumage is a clean and tidy theme for [Pelican](https://getpelican.com), a
 static site generator. I initially created this theme for [my blog](https://
 kevin.deldycke.com), but it is now generic enough to be used by anyone. ##
 Features - Standard Pelican views: | ![Plumage article view](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/article.jpeg) | !
 [Plumage categories view](https://raw.githubusercontent.com/kdeldycke/plumage/
@@ -36,45 +64,44 @@
 code.html)) | Videos showcase ([source](https://github.com/kdeldycke/kevin-
 deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/
 videos.html)) | Themes showcase ([source](https://github.com/kdeldycke/kevin-
 deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/
 themes.html)) | - Based on [Bootstrap v4](https://getbootstrap.com). - [Code
 syntax highlighting](#code-syntax-highlighting) with [30+ styles](https://
 github.com/pygments/pygments/tree/master/pygments/styles). - Site-wide static
-search via [Tipue-search](https://web.archive.org/web/20200703134724/https://
-tipue.com/search/). - Bare YouTube links in articles gets rendered as embedded
-videos: ![Plumage YouTube link](https://raw.githubusercontent.com/kdeldycke/
-plumage/main/screenshots/youtube-link.jpeg) - Direct link to edit articles on
-GitHub: ![Plumage GitHub edit link](https://raw.githubusercontent.com/
-kdeldycke/plumage/main/screenshots/github-edit-link.jpeg) - Magnifying glass
-overlays on images and zoom: ![Plumage image magnifying glass](https://
-raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/magnifying-
-glass.jpeg) ![Plumage image zoom](https://raw.githubusercontent.com/kdeldycke/
-plumage/main/screenshots/zoom.jpeg) - External assets (Bootstrap, Jquery,
-etc...) uses [CDNjs ](https://cdnjs.com/about). - Disqus integration: ![Plumage
-disqus comments](https://raw.githubusercontent.com/kdeldycke/plumage/main/
-screenshots/disqus.jpeg) ## Plugins Plumage has built-in support for the
-following plugins and extensions: | Plugin name | Type | Status | Notes | | :--
--------------------------------------------------------------------------------
------------------------------- | :----------------- | :------- | :-------------
--------------------------------------------------------------------------------
----------------- | | [`pelican-image-process`](https://github.com/pelican-
-plugins/image-process) | Pelican plugin | Optional | Embed a hack to [fix
-parsing of external images](https://github.com/pelican-plugins/image-process/
-issues/33). | | [`pelican-neighbors`](https://github.com/pelican-plugins/
-neighbors) | Pelican plugin | Optional | | | [`pelican-related-posts`](https://
-github.com/pelican-plugins/related-posts) | Pelican plugin | Optional | | |
-[`pelican-similar-posts`](https://github.com/pelican-plugins/similar-posts) |
-Pelican plugin | Optional | | | [`pelican-tipue-search`](https://github.com/
-pelican-plugins/tipue-search) | Pelican plugin | Optional | | | [`pelican-
-webassets`](https://github.com/pelican-plugins/webassets) | Pelican plugin |
-Required | | | [`markdown.extensions.admonition`](https://python-
-markdown.github.io/extensions/admonition/) | Markdown extension | Optional |
-Re-style admonitions into [alerts](https://getbootstrap.com/docs/4.5/
-components/alerts/). | | [`markdown.extensions.codehilite`](https://python-
+search via [Stork](https://stork-search.net). - Bare YouTube links in articles
+gets rendered as embedded videos: ![Plumage YouTube link](https://
+raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/youtube-link.jpeg)
+- Direct link to edit articles on GitHub: ![Plumage GitHub edit link](https://
+raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/github-edit-
+link.jpeg) - Magnifying glass overlays on images and zoom: ![Plumage image
+magnifying glass](https://raw.githubusercontent.com/kdeldycke/plumage/main/
+screenshots/magnifying-glass.jpeg) ![Plumage image zoom](https://
+raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/zoom.jpeg) -
+External assets (Bootstrap, Jquery, etc...) uses [CDNjs ](https://cdnjs.com/
+about). - Disqus integration: ![Plumage disqus comments](https://
+raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/disqus.jpeg) ##
+Plugins Plumage has built-in support for the following plugins and extensions:
+| Plugin name | Type | Status | Notes | | :------------------------------------
+--------------------------------------------------------------------------- | :
+----------------- | :------- | :-----------------------------------------------
+------------------------------------------------------------- | | [`pelican-
+image-process`](https://github.com/pelican-plugins/image-process) | Pelican
+plugin | Optional | Embed a hack to [fix parsing of external images](https://
+github.com/pelican-plugins/image-process/issues/33). | | [`pelican-neighbors`]
+(https://github.com/pelican-plugins/neighbors) | Pelican plugin | Optional | |
+| [`pelican-related-posts`](https://github.com/pelican-plugins/related-posts) |
+Pelican plugin | Optional | | | [`pelican-similar-posts`](https://github.com/
+pelican-plugins/similar-posts) | Pelican plugin | Optional | | | [`pelican-
+search`](https://github.com/pelican-plugins/search) | Pelican plugin | Optional
+| | | [`pelican-webassets`](https://github.com/pelican-plugins/webassets) |
+Pelican plugin | Required | | | [`markdown.extensions.admonition`](https://
+python-markdown.github.io/extensions/admonition/) | Markdown extension |
+Optional | Re-style admonitions into [alerts](https://getbootstrap.com/docs/
+4.5/components/alerts/). | | [`markdown.extensions.codehilite`](https://python-
 markdown.github.io/extensions/code_hilite/) | Markdown extension | Optional |
 Style highlighted code with Pygment style. | | [`markdown.extensions.toc`]
 (https://python-markdown.github.io/extensions/toc/#usage) | Markdown extension
 | Optional | Adds permalink anchors to article's subtitles. | |
 [`pymdownx.emoji`](https://facelessuser.github.io/pymdown-extensions/
 extensions/emoji/#default-emoji-generators) | Markdown extension | Optional |
 Style `emojione` set for proper integration into text. | |
@@ -105,31 +132,30 @@
 up to date, audited 96 packages in 984ms found 0 vulnerabilities -> postcss CLI
 found at (â¦)/plumage/node_modules/.bin/postcss (â¦) ``` ## Settings Plumage
 can be customized by adding these optionnal parameters to your `pelicanconf.py`
 file: | Setting name | Default value | Description | | :-----------------------
 --------------------------------------------------------------------- | :------
 ------ | :---------------------------------------------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------------
-- | | `ARTICLE_EDIT_LINK` | | Generate an edit link besides each article. Can
-use `%(slug)s` to include dynamic article's slug in the link. | | `CODE_STYLE`
-| `"monokai"` | Pygments' style ID. Choose one from `poetry run pygmentize -
-L styles`. | | `COPYRIGHT` | | Additional copyright statement to add in the
-third column of the footer. | | `DISCLAIMER` | | Overide the disclaimer notice
-that gets displayed at the fourth column of the footer. | | [`DISQUS_SITENAME`]
-(http://docs.getpelican.com/en/stable/settings.html#DISQUS_SITENAME) | |
-Pelican can handle Disqus comments. Specify the Disqus sitename identifier
-here. | | `FAVICON_LINKS` | `True` | Fetch link's icons from [Google's favicons
-webservice](https://www.google.com/s2/favicons). | | [`GOOGLE_ANALYTICS`](http:
-//docs.getpelican.com/en/stable/settings.html#GOOGLE_ANALYTICS) | | Set to `UA-
-XXXXXX-Y` Property's tracking ID to activate Google Analytics. | |
-`LEFT_SIDEBAR` | | HTML content to put as-is in the left sidebar. | |
-[`LINKS_WIDGET_NAME`](http://docs.getpelican.com/en/stable/
-settings.html#LINKS_WIDGET_NAME) | `"Links"` | Allows override of the name of
-the links widget. | | [`LINKS`](http://docs.getpelican.com/en/stable/
+--------- | | `ARTICLE_EDIT_LINK` | | Generate an edit link besides each
+article. Can use `%(slug)s` to include dynamic article's slug in the link. | |
+`CODE_STYLE` | `"monokai"` | Pygments' style ID. Choose one from `poetry run
+pygmentize -L styles`. | | `COPYRIGHT` | | Additional copyright statement to
+add in the third column of the footer. | | `DISCLAIMER` | | Overide the
+disclaimer notice that gets displayed at the fourth column of the footer. | |
+[`DISQUS_SITENAME`](http://docs.getpelican.com/en/stable/
+settings.html#DISQUS_SITENAME) | | Pelican can handle Disqus comments. Specify
+the Disqus sitename identifier here. | | `FAVICON_LINKS` | `True` | Fetch
+link's icons from [Google's favicons webservice](https://www.google.com/s2/
+favicons). | | [`GOOGLE_ANALYTICS`](http://docs.getpelican.com/en/stable/
+settings.html#GOOGLE_ANALYTICS) | | Set to `UA-XXXXXX-Y` Property's tracking ID
+to activate Google Analytics. | | `LEFT_SIDEBAR` | | HTML content to put as-is
+in the left sidebar. | | [`LINKS_WIDGET_NAME`](http://docs.getpelican.com/en/
+stable/settings.html#LINKS_WIDGET_NAME) | `"Links"` | Allows override of the
+name of the links widget. | | [`LINKS`](http://docs.getpelican.com/en/stable/
 settings.html#LINKS) | | A list of tuples (Title, URL) for links to appear in
 the second column of the footer. | | [`MANUAL_LINKS`](http://
 docs.getpelican.com/en/stable/settings.html#MANUAL_LINKS) | | When enabling
 this, you must pass the links (in LINKS & SOCIAL settins) not as tuples
 anymore, but as list, where every entry is formatted as you like | |
 [`MENUITEMS`](http://docs.getpelican.com/en/stable/settings.html#MENUITEMS) | |
 A list of tuples (Title, URL) for additional menu items to appear at the
@@ -138,25 +164,24 @@
 stable/settings.html#SITESUBTITLE) | | A subtitle to appear in the header. | |
 `SITE_THUMBNAIL_TEXT` | | Text displayed behind site's thumbnail. | |
 `SITE_THUMBNAIL` | | Site's thumbnail URL as displayed in the header. Should be
 a square image of at least 80x80 pixels. | | [`SOCIAL_WIDGET_NAME`](http://
 docs.getpelican.com/en/stable/settings.html#SOCIAL_WIDGET_NAME) | `"Social"` |
 Allows override of the name of the âsocialâ widget. | | [`SOCIAL`](http://
 docs.getpelican.com/en/stable/settings.html#SOCIAL) | | A list of tuples
-(Title, URL) to appear in the first columns of the footer. | | `TIPUE_SEARCH` |
-`False` | Activate [Tipue Search](https://web.archive.org/web/20200703134724/
-https://tipue.com/search/) (javascript static search engine) into the site.
-Requires the [`tipue_search`](https://github.com/pelican-plugins/tipue-search)
-plugin. | Most of these [parameters are similar to `notmyidea`'s ](https://
-docs.getpelican.com/en/latest/settings.html#themes) (Pelican's default theme).
-For usage example, please have a look into [my own `pelicanconf.py` ](https://
-github.com/kdeldycke/kevin-deldycke-blog/blob/main/pelicanconf.py). The theme
-is also sensible to this list of [standard Pelican parameters ](https://
-docs.getpelican.com/en/latest/settings.html): - `ARCHIVES_SAVE_AS` - `AUTHOR` -
-`AUTHOR_SAVE_AS` - `AUTHORS_SAVE_AS` - `CATEGORIES_SAVE_AS` -
+(Title, URL) to appear in the first columns of the footer. | | `STORK_SEARCH` |
+`False` | Activate [Stork](https://stork-search.net) static search engine.
+Requires the [official Pelican's `search` plugin](https://github.com/pelican-
+plugins/search). | Most of these [parameters are similar to `notmyidea`'s ]
+(https://docs.getpelican.com/en/latest/settings.html#themes) (Pelican's default
+theme). For usage example, please have a look into [my own `pelicanconf.py` ]
+(https://github.com/kdeldycke/kevin-deldycke-blog/blob/main/pelicanconf.py).
+The theme is also sensible to this list of [standard Pelican parameters ]
+(https://docs.getpelican.com/en/latest/settings.html): - `ARCHIVES_SAVE_AS` -
+`AUTHOR` - `AUTHOR_SAVE_AS` - `AUTHORS_SAVE_AS` - `CATEGORIES_SAVE_AS` -
 `CATEGORY_FEED_ATOM` - `CATEGORY_FEED_RSS` - `DEFAULT_LANG` -
 `DEFAULT_PAGINATION` - `DISPLAY_PAGES_ON_MENU` - `DISPLAY_CATEGORIES_ON_MENU` -
 `FEED_ALL_ATOM` - `FEED_ALL_RSS` - `FEED_ATOM` - `FEED_DOMAIN` - `FEED_RSS` -
 `PAGINATION_PATTERNS` - `SITENAME` - `SITEURL` - `TAG_FEED_ATOM` -
 `TAG_FEED_RSS` - `TAGS_SAVE_AS` ## Code Syntax Highlighting There is two
 alternatives, all relying on [Pygments syntax highlighter](https://
 pygments.org), sharing most features, with some differences: | Feature |
@@ -201,33 +226,26 @@
 Extensions' Highlight rendering](https://raw.githubusercontent.com/kdeldycke/
 plumage/main/screenshots/highlight-rendering.jpeg) ## FAQ ### How can I disable
 the zoom on images? All images of an article are zoomable by default. You can
 deactivate the magnifying glass per-image by adding a `noZoom` CSS class. So
 instead of the following Markdown code: ```markdown ![Image title](/folder/
 image.png) ``` You have to use the following template to deactivate the zoom of
 an image: ```markdown ![Image title](/folder/image.png){: .noZoom} ``` ### Why
-is the search not working? The [`tipue-search`](https://github.com/pelican-
-plugins/tipue-search) needs to be installed then have an additional template
-file registered in your `pelicanconf.py`. There are two alternatives: - update
-the `TEMPLATE_PAGES` variable: ```python TEMPLATE_PAGES = { (â¦)
-"search.html": "search.html", } ``` - or `DIRECT_TEMPLATES`: ([example](https:/
-/github.com/kdeldycke/kevin-deldycke-blog/commit/
-cd4bf8d1f4c55d835d7bfe1d7233cffe48e67a8a)): ```python DIRECT_TEMPLATES = [
-(â¦), "search"] ``` ## License This software is licensed under the [GNU
-General Public License v2 or later (GPLv2+)](https://github.com/kdeldycke/
-plumage/blob/main/LICENSE). Copyright (C) 2012-2020 [Kevin Deldycke](https://
-kevin.deldycke.com) and [contributors](https://github.com/kdeldycke/plumage/
-graphs/contributors). ## Third-party assets The theme embed copies of some
-external softwares, scripts, libraries and artworks: ```text Tipue Search v7.1
-Copyright (c) 2019 Tipue Distributed under a MIT license Source: https://
-web.archive.org/web/20200703134724/https://www.tipue.com/search/tipuesearch.zip
-``` ```text jQuery MGlass v1.1 Copyright (c) 2012 YounÃ¨s El Biache Distributed
-under a MIT license Source: https://github.com/younes0/jQuery-MGlass ```
-```text Fabric (Plaid) Copyright (c) 2012 James Basoo Distributed under a
-Creative Commons Attribution-ShareAlike 3.0 Unported license Source: https://
-subtlepatterns.com/fabric-plaid/ ``` ```text Cream paper Copyright (c) 2012
-Devin Holmes Distributed under a Creative Commons Attribution-ShareAlike 3.0
-Unported license Source: https://subtlepatterns.com/cream-paper/ ``` ```text
-Feather-alt icon v5.1.0 Copyright (c) 2020 Font Awesome project Distributed
-under a Creative Commons Attribution 4.0 International license Source: https://
+is the search not working? The [official Pelican's `search` plugin](https://
+github.com/pelican-plugins/search) needs to be installed. TODO: Activate search
+field automaticcaly if the plugin is present. ## License This software is
+licensed under the [GNU General Public License v2 or later (GPLv2+)](https://
+github.com/kdeldycke/plumage/blob/main/LICENSE). Copyright (C) 2012-2020 [Kevin
+Deldycke](https://kevin.deldycke.com) and [contributors](https://github.com/
+kdeldycke/plumage/graphs/contributors). ## Third-party assets The theme embed
+copies of some external softwares, scripts, libraries and artworks: ```text
+jQuery MGlass v1.1 Copyright (c) 2012 YounÃ¨s El Biache Distributed under a MIT
+license Source: https://github.com/younes0/jQuery-MGlass ``` ```text Fabric
+(Plaid) Copyright (c) 2012 James Basoo Distributed under a Creative Commons
+Attribution-ShareAlike 3.0 Unported license Source: https://subtlepatterns.com/
+fabric-plaid/ ``` ```text Cream paper Copyright (c) 2012 Devin Holmes
+Distributed under a Creative Commons Attribution-ShareAlike 3.0 Unported
+license Source: https://subtlepatterns.com/cream-paper/ ``` ```text Feather-alt
+icon v5.1.0 Copyright (c) 2020 Font Awesome project Distributed under a
+Creative Commons Attribution 4.0 International license Source: https://
 fontawesome.com/icons/feather-alt?style=solid ``` ```text Macro shot of White
 Feather Source: https://unsplash.com/photos/Sw7f58YJbc0 ```
```

### Comparing `plumage-3.0.0/PKG-INFO` & `plumage-3.1.0/readme.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,7 @@
-Metadata-Version: 2.1
-Name: plumage
-Version: 3.0.0
-Summary: Clean and tidy theme for Pelican.
-Home-page: https://github.com/kdeldycke/plumage
-License: GPL-2.0-or-later
-Keywords: pelican,pelican-theme,tipue-search,masonry,theme,bootstrap,jquery,font-awesome
-Author: Kevin Deldycke
-Author-email: kevin@deldycke.com
-Requires-Python: >=3.11,<4.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Plugins
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Pelican :: Themes
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Other
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Text Processing :: Markup :: HTML
-Classifier: Typing :: Typed
-Requires-Dist: Markdown (>=3.4.1,<4.0.0)
-Requires-Dist: closure (>=20191111,<20191112)
-Requires-Dist: cssmin (>=0.2.0,<0.3.0)
-Requires-Dist: libsass (>=0.22.0,<0.23.0)
-Requires-Dist: pelican (>=4.8.0,<5.0.0)
-Requires-Dist: pelican-webassets (>=2.0.0,<3.0.0)
-Requires-Dist: pygments (>=2.14.0,<3.0.0)
-Requires-Dist: pymdown-extensions (>=9.9.2,<10.0.0)
-Requires-Dist: pynpm (>=0.1.2,<0.2.0)
-Requires-Dist: pyquery (>=2.0.0,<3.0.0)
-Project-URL: Changelog, https://github.com/kdeldycke/plumage/blob/main/changelog.md#changelog
-Project-URL: Documentation, https://github.com/kdeldycke/plumage#settings
-Project-URL: Funding, https://github.com/sponsors/kdeldycke
-Project-URL: Issues, https://github.com/kdeldycke/plumage/issues
-Project-URL: Repository, https://github.com/kdeldycke/plumage
-Description-Content-Type: text/markdown
-
 <p align="center">
   <a href="https://github.com/kdeldycke/plumage/">
     <img src="https://github.com/kdeldycke/plumage/raw/main/screenshots/plumage-header-logo.jpeg" alt="Plumage, a Pelican theme">
   </a>
 </p>
 
 Plumage is a clean and tidy theme for [Pelican](https://getpelican.com), a
@@ -70,15 +28,15 @@
   | :--------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------: |
   | Code showcase ([source](https://github.com/kdeldycke/kevin-deldycke-blog/blob/ebe0d17a59730457c3016dff77fdfa799a80d756/content/templates/code.html)) | Videos showcase ([source](https://github.com/kdeldycke/kevin-deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/videos.html)) | Themes showcase ([source](https://github.com/kdeldycke/kevin-deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/themes.html)) |
 
 - Based on [Bootstrap v4](https://getbootstrap.com).
 
 - [Code syntax highlighting](#code-syntax-highlighting) with [30+ styles](https://github.com/pygments/pygments/tree/master/pygments/styles).
 
-- Site-wide static search via [Tipue-search](https://web.archive.org/web/20200703134724/https://tipue.com/search/).
+- Site-wide static search via [Stork](https://stork-search.net).
 
 - Bare YouTube links in articles gets rendered as embedded videos:
 
   ![Plumage YouTube link](https://raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/youtube-link.jpeg)
 
 - Direct link to edit articles on GitHub:
 
@@ -102,15 +60,15 @@
 
 | Plugin name                                                                                                      | Type               | Status   | Notes                                                                                                         |
 | :--------------------------------------------------------------------------------------------------------------- | :----------------- | :------- | :------------------------------------------------------------------------------------------------------------ |
 | [`pelican-image-process`](https://github.com/pelican-plugins/image-process)                                      | Pelican plugin     | Optional | Embed a hack to [fix parsing of external images](https://github.com/pelican-plugins/image-process/issues/33). |
 | [`pelican-neighbors`](https://github.com/pelican-plugins/neighbors)                                              | Pelican plugin     | Optional |                                                                                                               |
 | [`pelican-related-posts`](https://github.com/pelican-plugins/related-posts)                                      | Pelican plugin     | Optional |                                                                                                               |
 | [`pelican-similar-posts`](https://github.com/pelican-plugins/similar-posts)                                      | Pelican plugin     | Optional |                                                                                                               |
-| [`pelican-tipue-search`](https://github.com/pelican-plugins/tipue-search)                                        | Pelican plugin     | Optional |                                                                                                               |
+| [`pelican-search`](https://github.com/pelican-plugins/search)                                                    | Pelican plugin     | Optional |                                                                                                               |
 | [`pelican-webassets`](https://github.com/pelican-plugins/webassets)                                              | Pelican plugin     | Required |                                                                                                               |
 | [`markdown.extensions.admonition`](https://python-markdown.github.io/extensions/admonition/)                     | Markdown extension | Optional | Re-style admonitions into [alerts](https://getbootstrap.com/docs/4.5/components/alerts/).                     |
 | [`markdown.extensions.codehilite`](https://python-markdown.github.io/extensions/code_hilite/)                    | Markdown extension | Optional | Style highlighted code with Pygment style.                                                                    |
 | [`markdown.extensions.toc`](https://python-markdown.github.io/extensions/toc/#usage)                             | Markdown extension | Optional | Adds permalink anchors to article's subtitles.                                                                |
 | [`pymdownx.emoji`](https://facelessuser.github.io/pymdown-extensions/extensions/emoji/#default-emoji-generators) | Markdown extension | Optional | Style `emojione` set for proper integration into text.                                                        |
 | [`pymdownx.highlight`](https://facelessuser.github.io/pymdown-extensions/extensions/highlight/)                  | Markdown extension | Optional | Style highlighted code with Pygment style.                                                                    |
 | [`typogrify`](https://pypi.python.org/pypi/typogrify)                                                            | Pelican builtin    | Optional | Style ampersands.                                                                                             |
@@ -173,35 +131,35 @@
 ```
 
 ## Settings
 
 Plumage can be customized by adding these optionnal parameters to your
 `pelicanconf.py` file:
 
-| Setting name                                                                                  | Default value | Description                                                                                                                                                                                                                           |
-| :-------------------------------------------------------------------------------------------- | :------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
-| `ARTICLE_EDIT_LINK`                                                                           |               | Generate an edit link besides each article. Can use `%(slug)s` to include dynamic article's slug in the link.                                                                                                                         |
-| `CODE_STYLE`                                                                                  | `"monokai"`   | Pygments' style ID. Choose one from `poetry run pygmentize -L styles`.                                                                                                                                                                |
-| `COPYRIGHT`                                                                                   |               | Additional copyright statement to add in the third column of the footer.                                                                                                                                                              |
-| `DISCLAIMER`                                                                                  |               | Overide the disclaimer notice that gets displayed at the fourth column of the footer.                                                                                                                                                 |
-| [`DISQUS_SITENAME`](http://docs.getpelican.com/en/stable/settings.html#DISQUS_SITENAME)       |               | Pelican can handle Disqus comments. Specify the Disqus sitename identifier here.                                                                                                                                                      |
-| `FAVICON_LINKS`                                                                               | `True`        | Fetch link's icons from [Google's favicons webservice](https://www.google.com/s2/favicons).                                                                                                                                           |
-| [`GOOGLE_ANALYTICS`](http://docs.getpelican.com/en/stable/settings.html#GOOGLE_ANALYTICS)     |               | Set to `UA-XXXXXX-Y` Property's tracking ID to activate Google Analytics.                                                                                                                                                             |
-| `LEFT_SIDEBAR`                                                                                |               | HTML content to put as-is in the left sidebar.                                                                                                                                                                                        |
-| [`LINKS_WIDGET_NAME`](http://docs.getpelican.com/en/stable/settings.html#LINKS_WIDGET_NAME)   | `"Links"`     | Allows override of the name of the links widget.                                                                                                                                                                                      |
-| [`LINKS`](http://docs.getpelican.com/en/stable/settings.html#LINKS)                           |               | A list of tuples (Title, URL) for links to appear in the second column of the footer.                                                                                                                                                 |
-| [`MANUAL_LINKS`](http://docs.getpelican.com/en/stable/settings.html#MANUAL_LINKS)             |               | When enabling this, you must pass the links (in LINKS & SOCIAL settins) not as tuples anymore, but as list, where every entry is formatted as you like                                                                                |
-| [`MENUITEMS`](http://docs.getpelican.com/en/stable/settings.html#MENUITEMS)                   |               | A list of tuples (Title, URL) for additional menu items to appear at the beginning of the main menu.                                                                                                                                  |
-| `RIGHT_SIDEBAR`                                                                               |               | HTML content to put as-is in the right sidebar.                                                                                                                                                                                       |
-| [`SITESUBTITLE`](http://docs.getpelican.com/en/stable/settings.html#SITESUBTITLE)             |               | A subtitle to appear in the header.                                                                                                                                                                                                   |
-| `SITE_THUMBNAIL_TEXT`                                                                         |               | Text displayed behind site's thumbnail.                                                                                                                                                                                               |
-| `SITE_THUMBNAIL`                                                                              |               | Site's thumbnail URL as displayed in the header. Should be a square image of at least 80x80 pixels.                                                                                                                                   |
-| [`SOCIAL_WIDGET_NAME`](http://docs.getpelican.com/en/stable/settings.html#SOCIAL_WIDGET_NAME) | `"Social"`    | Allows override of the name of the “social” widget.                                                                                                                                                                                   |
-| [`SOCIAL`](http://docs.getpelican.com/en/stable/settings.html#SOCIAL)                         |               | A list of tuples (Title, URL) to appear in the first columns of the footer.                                                                                                                                                           |
-| `TIPUE_SEARCH`                                                                                | `False`       | Activate [Tipue Search](https://web.archive.org/web/20200703134724/https://tipue.com/search/) (javascript static search engine) into the site. Requires the [`tipue_search`](https://github.com/pelican-plugins/tipue-search) plugin. |
+| Setting name                                                                                  | Default value | Description                                                                                                                                                    |
+| :-------------------------------------------------------------------------------------------- | :------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `ARTICLE_EDIT_LINK`                                                                           |               | Generate an edit link besides each article. Can use `%(slug)s` to include dynamic article's slug in the link.                                                  |
+| `CODE_STYLE`                                                                                  | `"monokai"`   | Pygments' style ID. Choose one from `poetry run pygmentize -L styles`.                                                                                         |
+| `COPYRIGHT`                                                                                   |               | Additional copyright statement to add in the third column of the footer.                                                                                       |
+| `DISCLAIMER`                                                                                  |               | Overide the disclaimer notice that gets displayed at the fourth column of the footer.                                                                          |
+| [`DISQUS_SITENAME`](http://docs.getpelican.com/en/stable/settings.html#DISQUS_SITENAME)       |               | Pelican can handle Disqus comments. Specify the Disqus sitename identifier here.                                                                               |
+| `FAVICON_LINKS`                                                                               | `True`        | Fetch link's icons from [Google's favicons webservice](https://www.google.com/s2/favicons).                                                                    |
+| [`GOOGLE_ANALYTICS`](http://docs.getpelican.com/en/stable/settings.html#GOOGLE_ANALYTICS)     |               | Set to `UA-XXXXXX-Y` Property's tracking ID to activate Google Analytics.                                                                                      |
+| `LEFT_SIDEBAR`                                                                                |               | HTML content to put as-is in the left sidebar.                                                                                                                 |
+| [`LINKS_WIDGET_NAME`](http://docs.getpelican.com/en/stable/settings.html#LINKS_WIDGET_NAME)   | `"Links"`     | Allows override of the name of the links widget.                                                                                                               |
+| [`LINKS`](http://docs.getpelican.com/en/stable/settings.html#LINKS)                           |               | A list of tuples (Title, URL) for links to appear in the second column of the footer.                                                                          |
+| [`MANUAL_LINKS`](http://docs.getpelican.com/en/stable/settings.html#MANUAL_LINKS)             |               | When enabling this, you must pass the links (in LINKS & SOCIAL settins) not as tuples anymore, but as list, where every entry is formatted as you like         |
+| [`MENUITEMS`](http://docs.getpelican.com/en/stable/settings.html#MENUITEMS)                   |               | A list of tuples (Title, URL) for additional menu items to appear at the beginning of the main menu.                                                           |
+| `RIGHT_SIDEBAR`                                                                               |               | HTML content to put as-is in the right sidebar.                                                                                                                |
+| [`SITESUBTITLE`](http://docs.getpelican.com/en/stable/settings.html#SITESUBTITLE)             |               | A subtitle to appear in the header.                                                                                                                            |
+| `SITE_THUMBNAIL_TEXT`                                                                         |               | Text displayed behind site's thumbnail.                                                                                                                        |
+| `SITE_THUMBNAIL`                                                                              |               | Site's thumbnail URL as displayed in the header. Should be a square image of at least 80x80 pixels.                                                            |
+| [`SOCIAL_WIDGET_NAME`](http://docs.getpelican.com/en/stable/settings.html#SOCIAL_WIDGET_NAME) | `"Social"`    | Allows override of the name of the “social” widget.                                                                                                            |
+| [`SOCIAL`](http://docs.getpelican.com/en/stable/settings.html#SOCIAL)                         |               | A list of tuples (Title, URL) to appear in the first columns of the footer.                                                                                    |
+| `STORK_SEARCH`                                                                                | `False`       | Activate [Stork](https://stork-search.net) static search engine. Requires the [official Pelican's `search` plugin](https://github.com/pelican-plugins/search). |
 
 Most of these [parameters are similar to `notmyidea`'s
 ](https://docs.getpelican.com/en/latest/settings.html#themes) (Pelican's default
 theme). For usage example, please have a look into [my own `pelicanconf.py`
 ](https://github.com/kdeldycke/kevin-deldycke-blog/blob/main/pelicanconf.py).
 
 The theme is also sensible to this list of [standard Pelican parameters
@@ -372,35 +330,18 @@
 
 ```markdown
 ![Image title](/folder/image.png){: .noZoom}
 ```
 
 ### Why is the search not working?
 
-The [`tipue-search`](https://github.com/pelican-plugins/tipue-search) needs to
-be installed then have an additional template file registered in your
-`pelicanconf.py`.
-
-There are two alternatives:
-
-- update the `TEMPLATE_PAGES` variable:
-
-  ```python
-  TEMPLATE_PAGES = {
-      (…)
-      "search.html": "search.html",
-   }
-  ```
-
-- or `DIRECT_TEMPLATES`:
-  ([example](https://github.com/kdeldycke/kevin-deldycke-blog/commit/cd4bf8d1f4c55d835d7bfe1d7233cffe48e67a8a)):
-
-  ```python
-  DIRECT_TEMPLATES = [(…), "search"]
-  ```
+The [official Pelican's `search` plugin](https://github.com/pelican-plugins/search) needs to
+be installed.
+
+TODO: Activate search field automaticcaly if the plugin is present.
 
 ## License
 
 This software is licensed under the [GNU General Public License v2 or later
 (GPLv2+)](https://github.com/kdeldycke/plumage/blob/main/LICENSE).
 
 Copyright (C) 2012-2020 [Kevin Deldycke](https://kevin.deldycke.com) and
@@ -408,21 +349,14 @@
 
 ## Third-party assets
 
 The theme embed copies of some external softwares, scripts, libraries and
 artworks:
 
 ```text
-Tipue Search v7.1
-Copyright (c) 2019 Tipue
-Distributed under a MIT license
-Source: https://web.archive.org/web/20200703134724/https://www.tipue.com/search/tipuesearch.zip
-```
-
-```text
 jQuery MGlass v1.1
 Copyright (c) 2012 Younès El Biache
 Distributed under a MIT license
 Source: https://github.com/younes0/jQuery-MGlass
 ```
 
 ```text
@@ -446,8 +380,7 @@
 Source: https://fontawesome.com/icons/feather-alt?style=solid
 ```
 
 ```text
 Macro shot of White Feather
 Source: https://unsplash.com/photos/Sw7f58YJbc0
 ```
-
```

#### html2text {}

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1 Name: plumage Version: 3.0.0 Summary: Clean and tidy
-theme for Pelican. Home-page: https://github.com/kdeldycke/plumage License:
-GPL-2.0-or-later Keywords: pelican,pelican-theme,tipue-
-search,masonry,theme,bootstrap,jquery,font-awesome Author: Kevin Deldycke
-Author-email: kevin@deldycke.com Requires-Python: >=3.11,<4.0 Classifier:
-Development Status :: 5 - Production/Stable Classifier: Environment :: Plugins
-Classifier: Environment :: Web Environment Classifier: Framework :: Pelican ::
-Themes Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Information Technology Classifier: License :: OSI Approved :: GNU
-General Public License v2 or later (GPLv2+) Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: JavaScript Classifier:
-Programming Language :: Other Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Internet :: WWW/HTTP Classifier: Topic :: Text Processing :: Markup :: HTML
-Classifier: Typing :: Typed Requires-Dist: Markdown (>=3.4.1,<4.0.0) Requires-
-Dist: closure (>=20191111,<20191112) Requires-Dist: cssmin (>=0.2.0,<0.3.0)
-Requires-Dist: libsass (>=0.22.0,<0.23.0) Requires-Dist: pelican
-(>=4.8.0,<5.0.0) Requires-Dist: pelican-webassets (>=2.0.0,<3.0.0) Requires-
-Dist: pygments (>=2.14.0,<3.0.0) Requires-Dist: pymdown-extensions
-(>=9.9.2,<10.0.0) Requires-Dist: pynpm (>=0.1.2,<0.2.0) Requires-Dist: pyquery
-(>=2.0.0,<3.0.0) Project-URL: Changelog, https://github.com/kdeldycke/plumage/
-blob/main/changelog.md#changelog Project-URL: Documentation, https://
-github.com/kdeldycke/plumage#settings Project-URL: Funding, https://github.com/
-sponsors/kdeldycke Project-URL: Issues, https://github.com/kdeldycke/plumage/
-issues Project-URL: Repository, https://github.com/kdeldycke/plumage
-Description-Content-Type: text/markdown
                           [Plumage,_a_Pelican_theme]
 Plumage is a clean and tidy theme for [Pelican](https://getpelican.com), a
 static site generator. I initially created this theme for [my blog](https://
 kevin.deldycke.com), but it is now generic enough to be used by anyone. ##
 Features - Standard Pelican views: | ![Plumage article view](https://
 raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/article.jpeg) | !
 [Plumage categories view](https://raw.githubusercontent.com/kdeldycke/plumage/
@@ -62,45 +36,44 @@
 code.html)) | Videos showcase ([source](https://github.com/kdeldycke/kevin-
 deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/
 videos.html)) | Themes showcase ([source](https://github.com/kdeldycke/kevin-
 deldycke-blog/blob/f778998376fa5c68f1a02129884b89592b641777/content/templates/
 themes.html)) | - Based on [Bootstrap v4](https://getbootstrap.com). - [Code
 syntax highlighting](#code-syntax-highlighting) with [30+ styles](https://
 github.com/pygments/pygments/tree/master/pygments/styles). - Site-wide static
-search via [Tipue-search](https://web.archive.org/web/20200703134724/https://
-tipue.com/search/). - Bare YouTube links in articles gets rendered as embedded
-videos: ![Plumage YouTube link](https://raw.githubusercontent.com/kdeldycke/
-plumage/main/screenshots/youtube-link.jpeg) - Direct link to edit articles on
-GitHub: ![Plumage GitHub edit link](https://raw.githubusercontent.com/
-kdeldycke/plumage/main/screenshots/github-edit-link.jpeg) - Magnifying glass
-overlays on images and zoom: ![Plumage image magnifying glass](https://
-raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/magnifying-
-glass.jpeg) ![Plumage image zoom](https://raw.githubusercontent.com/kdeldycke/
-plumage/main/screenshots/zoom.jpeg) - External assets (Bootstrap, Jquery,
-etc...) uses [CDNjs ](https://cdnjs.com/about). - Disqus integration: ![Plumage
-disqus comments](https://raw.githubusercontent.com/kdeldycke/plumage/main/
-screenshots/disqus.jpeg) ## Plugins Plumage has built-in support for the
-following plugins and extensions: | Plugin name | Type | Status | Notes | | :--
--------------------------------------------------------------------------------
------------------------------- | :----------------- | :------- | :-------------
--------------------------------------------------------------------------------
----------------- | | [`pelican-image-process`](https://github.com/pelican-
-plugins/image-process) | Pelican plugin | Optional | Embed a hack to [fix
-parsing of external images](https://github.com/pelican-plugins/image-process/
-issues/33). | | [`pelican-neighbors`](https://github.com/pelican-plugins/
-neighbors) | Pelican plugin | Optional | | | [`pelican-related-posts`](https://
-github.com/pelican-plugins/related-posts) | Pelican plugin | Optional | | |
-[`pelican-similar-posts`](https://github.com/pelican-plugins/similar-posts) |
-Pelican plugin | Optional | | | [`pelican-tipue-search`](https://github.com/
-pelican-plugins/tipue-search) | Pelican plugin | Optional | | | [`pelican-
-webassets`](https://github.com/pelican-plugins/webassets) | Pelican plugin |
-Required | | | [`markdown.extensions.admonition`](https://python-
-markdown.github.io/extensions/admonition/) | Markdown extension | Optional |
-Re-style admonitions into [alerts](https://getbootstrap.com/docs/4.5/
-components/alerts/). | | [`markdown.extensions.codehilite`](https://python-
+search via [Stork](https://stork-search.net). - Bare YouTube links in articles
+gets rendered as embedded videos: ![Plumage YouTube link](https://
+raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/youtube-link.jpeg)
+- Direct link to edit articles on GitHub: ![Plumage GitHub edit link](https://
+raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/github-edit-
+link.jpeg) - Magnifying glass overlays on images and zoom: ![Plumage image
+magnifying glass](https://raw.githubusercontent.com/kdeldycke/plumage/main/
+screenshots/magnifying-glass.jpeg) ![Plumage image zoom](https://
+raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/zoom.jpeg) -
+External assets (Bootstrap, Jquery, etc...) uses [CDNjs ](https://cdnjs.com/
+about). - Disqus integration: ![Plumage disqus comments](https://
+raw.githubusercontent.com/kdeldycke/plumage/main/screenshots/disqus.jpeg) ##
+Plugins Plumage has built-in support for the following plugins and extensions:
+| Plugin name | Type | Status | Notes | | :------------------------------------
+--------------------------------------------------------------------------- | :
+----------------- | :------- | :-----------------------------------------------
+------------------------------------------------------------- | | [`pelican-
+image-process`](https://github.com/pelican-plugins/image-process) | Pelican
+plugin | Optional | Embed a hack to [fix parsing of external images](https://
+github.com/pelican-plugins/image-process/issues/33). | | [`pelican-neighbors`]
+(https://github.com/pelican-plugins/neighbors) | Pelican plugin | Optional | |
+| [`pelican-related-posts`](https://github.com/pelican-plugins/related-posts) |
+Pelican plugin | Optional | | | [`pelican-similar-posts`](https://github.com/
+pelican-plugins/similar-posts) | Pelican plugin | Optional | | | [`pelican-
+search`](https://github.com/pelican-plugins/search) | Pelican plugin | Optional
+| | | [`pelican-webassets`](https://github.com/pelican-plugins/webassets) |
+Pelican plugin | Required | | | [`markdown.extensions.admonition`](https://
+python-markdown.github.io/extensions/admonition/) | Markdown extension |
+Optional | Re-style admonitions into [alerts](https://getbootstrap.com/docs/
+4.5/components/alerts/). | | [`markdown.extensions.codehilite`](https://python-
 markdown.github.io/extensions/code_hilite/) | Markdown extension | Optional |
 Style highlighted code with Pygment style. | | [`markdown.extensions.toc`]
 (https://python-markdown.github.io/extensions/toc/#usage) | Markdown extension
 | Optional | Adds permalink anchors to article's subtitles. | |
 [`pymdownx.emoji`](https://facelessuser.github.io/pymdown-extensions/
 extensions/emoji/#default-emoji-generators) | Markdown extension | Optional |
 Style `emojione` set for proper integration into text. | |
@@ -131,31 +104,30 @@
 up to date, audited 96 packages in 984ms found 0 vulnerabilities -> postcss CLI
 found at (â¦)/plumage/node_modules/.bin/postcss (â¦) ``` ## Settings Plumage
 can be customized by adding these optionnal parameters to your `pelicanconf.py`
 file: | Setting name | Default value | Description | | :-----------------------
 --------------------------------------------------------------------- | :------
 ------ | :---------------------------------------------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------------------------------------------
-- | | `ARTICLE_EDIT_LINK` | | Generate an edit link besides each article. Can
-use `%(slug)s` to include dynamic article's slug in the link. | | `CODE_STYLE`
-| `"monokai"` | Pygments' style ID. Choose one from `poetry run pygmentize -
-L styles`. | | `COPYRIGHT` | | Additional copyright statement to add in the
-third column of the footer. | | `DISCLAIMER` | | Overide the disclaimer notice
-that gets displayed at the fourth column of the footer. | | [`DISQUS_SITENAME`]
-(http://docs.getpelican.com/en/stable/settings.html#DISQUS_SITENAME) | |
-Pelican can handle Disqus comments. Specify the Disqus sitename identifier
-here. | | `FAVICON_LINKS` | `True` | Fetch link's icons from [Google's favicons
-webservice](https://www.google.com/s2/favicons). | | [`GOOGLE_ANALYTICS`](http:
-//docs.getpelican.com/en/stable/settings.html#GOOGLE_ANALYTICS) | | Set to `UA-
-XXXXXX-Y` Property's tracking ID to activate Google Analytics. | |
-`LEFT_SIDEBAR` | | HTML content to put as-is in the left sidebar. | |
-[`LINKS_WIDGET_NAME`](http://docs.getpelican.com/en/stable/
-settings.html#LINKS_WIDGET_NAME) | `"Links"` | Allows override of the name of
-the links widget. | | [`LINKS`](http://docs.getpelican.com/en/stable/
+--------- | | `ARTICLE_EDIT_LINK` | | Generate an edit link besides each
+article. Can use `%(slug)s` to include dynamic article's slug in the link. | |
+`CODE_STYLE` | `"monokai"` | Pygments' style ID. Choose one from `poetry run
+pygmentize -L styles`. | | `COPYRIGHT` | | Additional copyright statement to
+add in the third column of the footer. | | `DISCLAIMER` | | Overide the
+disclaimer notice that gets displayed at the fourth column of the footer. | |
+[`DISQUS_SITENAME`](http://docs.getpelican.com/en/stable/
+settings.html#DISQUS_SITENAME) | | Pelican can handle Disqus comments. Specify
+the Disqus sitename identifier here. | | `FAVICON_LINKS` | `True` | Fetch
+link's icons from [Google's favicons webservice](https://www.google.com/s2/
+favicons). | | [`GOOGLE_ANALYTICS`](http://docs.getpelican.com/en/stable/
+settings.html#GOOGLE_ANALYTICS) | | Set to `UA-XXXXXX-Y` Property's tracking ID
+to activate Google Analytics. | | `LEFT_SIDEBAR` | | HTML content to put as-is
+in the left sidebar. | | [`LINKS_WIDGET_NAME`](http://docs.getpelican.com/en/
+stable/settings.html#LINKS_WIDGET_NAME) | `"Links"` | Allows override of the
+name of the links widget. | | [`LINKS`](http://docs.getpelican.com/en/stable/
 settings.html#LINKS) | | A list of tuples (Title, URL) for links to appear in
 the second column of the footer. | | [`MANUAL_LINKS`](http://
 docs.getpelican.com/en/stable/settings.html#MANUAL_LINKS) | | When enabling
 this, you must pass the links (in LINKS & SOCIAL settins) not as tuples
 anymore, but as list, where every entry is formatted as you like | |
 [`MENUITEMS`](http://docs.getpelican.com/en/stable/settings.html#MENUITEMS) | |
 A list of tuples (Title, URL) for additional menu items to appear at the
@@ -164,25 +136,24 @@
 stable/settings.html#SITESUBTITLE) | | A subtitle to appear in the header. | |
 `SITE_THUMBNAIL_TEXT` | | Text displayed behind site's thumbnail. | |
 `SITE_THUMBNAIL` | | Site's thumbnail URL as displayed in the header. Should be
 a square image of at least 80x80 pixels. | | [`SOCIAL_WIDGET_NAME`](http://
 docs.getpelican.com/en/stable/settings.html#SOCIAL_WIDGET_NAME) | `"Social"` |
 Allows override of the name of the âsocialâ widget. | | [`SOCIAL`](http://
 docs.getpelican.com/en/stable/settings.html#SOCIAL) | | A list of tuples
-(Title, URL) to appear in the first columns of the footer. | | `TIPUE_SEARCH` |
-`False` | Activate [Tipue Search](https://web.archive.org/web/20200703134724/
-https://tipue.com/search/) (javascript static search engine) into the site.
-Requires the [`tipue_search`](https://github.com/pelican-plugins/tipue-search)
-plugin. | Most of these [parameters are similar to `notmyidea`'s ](https://
-docs.getpelican.com/en/latest/settings.html#themes) (Pelican's default theme).
-For usage example, please have a look into [my own `pelicanconf.py` ](https://
-github.com/kdeldycke/kevin-deldycke-blog/blob/main/pelicanconf.py). The theme
-is also sensible to this list of [standard Pelican parameters ](https://
-docs.getpelican.com/en/latest/settings.html): - `ARCHIVES_SAVE_AS` - `AUTHOR` -
-`AUTHOR_SAVE_AS` - `AUTHORS_SAVE_AS` - `CATEGORIES_SAVE_AS` -
+(Title, URL) to appear in the first columns of the footer. | | `STORK_SEARCH` |
+`False` | Activate [Stork](https://stork-search.net) static search engine.
+Requires the [official Pelican's `search` plugin](https://github.com/pelican-
+plugins/search). | Most of these [parameters are similar to `notmyidea`'s ]
+(https://docs.getpelican.com/en/latest/settings.html#themes) (Pelican's default
+theme). For usage example, please have a look into [my own `pelicanconf.py` ]
+(https://github.com/kdeldycke/kevin-deldycke-blog/blob/main/pelicanconf.py).
+The theme is also sensible to this list of [standard Pelican parameters ]
+(https://docs.getpelican.com/en/latest/settings.html): - `ARCHIVES_SAVE_AS` -
+`AUTHOR` - `AUTHOR_SAVE_AS` - `AUTHORS_SAVE_AS` - `CATEGORIES_SAVE_AS` -
 `CATEGORY_FEED_ATOM` - `CATEGORY_FEED_RSS` - `DEFAULT_LANG` -
 `DEFAULT_PAGINATION` - `DISPLAY_PAGES_ON_MENU` - `DISPLAY_CATEGORIES_ON_MENU` -
 `FEED_ALL_ATOM` - `FEED_ALL_RSS` - `FEED_ATOM` - `FEED_DOMAIN` - `FEED_RSS` -
 `PAGINATION_PATTERNS` - `SITENAME` - `SITEURL` - `TAG_FEED_ATOM` -
 `TAG_FEED_RSS` - `TAGS_SAVE_AS` ## Code Syntax Highlighting There is two
 alternatives, all relying on [Pygments syntax highlighter](https://
 pygments.org), sharing most features, with some differences: | Feature |
@@ -227,33 +198,26 @@
 Extensions' Highlight rendering](https://raw.githubusercontent.com/kdeldycke/
 plumage/main/screenshots/highlight-rendering.jpeg) ## FAQ ### How can I disable
 the zoom on images? All images of an article are zoomable by default. You can
 deactivate the magnifying glass per-image by adding a `noZoom` CSS class. So
 instead of the following Markdown code: ```markdown ![Image title](/folder/
 image.png) ``` You have to use the following template to deactivate the zoom of
 an image: ```markdown ![Image title](/folder/image.png){: .noZoom} ``` ### Why
-is the search not working? The [`tipue-search`](https://github.com/pelican-
-plugins/tipue-search) needs to be installed then have an additional template
-file registered in your `pelicanconf.py`. There are two alternatives: - update
-the `TEMPLATE_PAGES` variable: ```python TEMPLATE_PAGES = { (â¦)
-"search.html": "search.html", } ``` - or `DIRECT_TEMPLATES`: ([example](https:/
-/github.com/kdeldycke/kevin-deldycke-blog/commit/
-cd4bf8d1f4c55d835d7bfe1d7233cffe48e67a8a)): ```python DIRECT_TEMPLATES = [
-(â¦), "search"] ``` ## License This software is licensed under the [GNU
-General Public License v2 or later (GPLv2+)](https://github.com/kdeldycke/
-plumage/blob/main/LICENSE). Copyright (C) 2012-2020 [Kevin Deldycke](https://
-kevin.deldycke.com) and [contributors](https://github.com/kdeldycke/plumage/
-graphs/contributors). ## Third-party assets The theme embed copies of some
-external softwares, scripts, libraries and artworks: ```text Tipue Search v7.1
-Copyright (c) 2019 Tipue Distributed under a MIT license Source: https://
-web.archive.org/web/20200703134724/https://www.tipue.com/search/tipuesearch.zip
-``` ```text jQuery MGlass v1.1 Copyright (c) 2012 YounÃ¨s El Biache Distributed
-under a MIT license Source: https://github.com/younes0/jQuery-MGlass ```
-```text Fabric (Plaid) Copyright (c) 2012 James Basoo Distributed under a
-Creative Commons Attribution-ShareAlike 3.0 Unported license Source: https://
-subtlepatterns.com/fabric-plaid/ ``` ```text Cream paper Copyright (c) 2012
-Devin Holmes Distributed under a Creative Commons Attribution-ShareAlike 3.0
-Unported license Source: https://subtlepatterns.com/cream-paper/ ``` ```text
-Feather-alt icon v5.1.0 Copyright (c) 2020 Font Awesome project Distributed
-under a Creative Commons Attribution 4.0 International license Source: https://
+is the search not working? The [official Pelican's `search` plugin](https://
+github.com/pelican-plugins/search) needs to be installed. TODO: Activate search
+field automaticcaly if the plugin is present. ## License This software is
+licensed under the [GNU General Public License v2 or later (GPLv2+)](https://
+github.com/kdeldycke/plumage/blob/main/LICENSE). Copyright (C) 2012-2020 [Kevin
+Deldycke](https://kevin.deldycke.com) and [contributors](https://github.com/
+kdeldycke/plumage/graphs/contributors). ## Third-party assets The theme embed
+copies of some external softwares, scripts, libraries and artworks: ```text
+jQuery MGlass v1.1 Copyright (c) 2012 YounÃ¨s El Biache Distributed under a MIT
+license Source: https://github.com/younes0/jQuery-MGlass ``` ```text Fabric
+(Plaid) Copyright (c) 2012 James Basoo Distributed under a Creative Commons
+Attribution-ShareAlike 3.0 Unported license Source: https://subtlepatterns.com/
+fabric-plaid/ ``` ```text Cream paper Copyright (c) 2012 Devin Holmes
+Distributed under a Creative Commons Attribution-ShareAlike 3.0 Unported
+license Source: https://subtlepatterns.com/cream-paper/ ``` ```text Feather-alt
+icon v5.1.0 Copyright (c) 2020 Font Awesome project Distributed under a
+Creative Commons Attribution 4.0 International license Source: https://
 fontawesome.com/icons/feather-alt?style=solid ``` ```text Macro shot of White
 Feather Source: https://unsplash.com/photos/Sw7f58YJbc0 ```
```

