# Comparing `tmp/click-reviewers-tools-0.78.tar.gz` & `tmp/click-reviewers-tools-0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click-reviewers-tools-0.78.tar", last modified: Thu Apr  6 13:27:58 2023, max compression
+gzip compressed data, was "click-reviewers-tools-0.79.tar", last modified: Sat Jun  3 02:27:40 2023, max compression
```

## Comparing `click-reviewers-tools-0.78.tar` & `click-reviewers-tools-0.79.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:27:58.744434 click-reviewers-tools-0.78/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-06 13:27:58.744434 click-reviewers-tools-0.78/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2089 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:27:58.723433 click-reviewers-tools-0.78/bin/
--rwxrwxrwx   0 root         (0) root         (0)      913 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-check-bin-path
--rwxrwxrwx   0 root         (0) root         (0)      931 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-check-content-hub
--rwxrwxrwx   0 root         (0) root         (0)      894 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-check-desktop
--rwxrwxrwx   0 root         (0) root         (0)      920 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-check-framework
--rwxrwxrwx   0 root         (0) root         (0)      938 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-check-functional
--rwxrwxrwx   0 root         (0) root         (0)      885 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-check-lint
--rwxrwxrwx   0 root         (0) root         (0)      949 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-check-online-accounts
--rwxrwxrwx   0 root         (0) root         (0)      931 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-check-push-helper
--rwxrwxrwx   0 root         (0) root         (0)      896 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-check-scope
--rwxrwxrwx   0 root         (0) root         (0)      909 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-check-security
--rwxrwxrwx   0 root         (0) root         (0)      914 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-check-skeleton
--rwxrwxrwx   0 root         (0) root         (0)      908 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-check-systemd
--rwxrwxrwx   0 root         (0) root         (0)      949 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-check-url-dispatcher
--rwxrwxrwx   0 root         (0) root         (0)     6760 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-review
--rwxrwxrwx   0 root         (0) root         (0)     1282 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-run-checks
--rwxrwxrwx   0 root         (0) root         (0)     6884 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/click-show-files
--rwxrwxrwx   0 root         (0) root         (0)      288 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/detect-package
--rwxrwxrwx   0 root         (0) root         (0)     1546 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/empty-click
--rwxrwxrwx   0 root         (0) root         (0)     2113 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/repack-click
--rwxrwxrwx   0 root         (0) root         (0)      332 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/bin/unpack-package
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:27:58.725433 click-reviewers-tools-0.78/click_reviewers_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-06 13:27:58.000000 click-reviewers-tools-0.78/click_reviewers_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2159 2023-04-06 13:27:58.000000 click-reviewers-tools-0.78/click_reviewers_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 13:27:58.000000 click-reviewers-tools-0.78/click_reviewers_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-06 13:27:58.000000 click-reviewers-tools-0.78/click_reviewers_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-06 13:27:58.000000 click-reviewers-tools-0.78/click_reviewers_tools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:27:58.734434 click-reviewers-tools-0.78/clickreviews/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14827 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/apparmor.py
--rw-rw-rw-   0 root         (0) root         (0)    21755 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/common.py
--rw-rw-rw-   0 root         (0) root         (0)     7743 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_bin_path.py
--rw-rw-rw-   0 root         (0) root         (0)    21600 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_common.py
--rw-rw-rw-   0 root         (0) root         (0)     4841 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_content_hub.py
--rw-rw-rw-   0 root         (0) root         (0)    36327 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_desktop.py
--rw-rw-rw-   0 root         (0) root         (0)    10104 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_framework.py
--rw-rw-rw-   0 root         (0) root         (0)    17291 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_functional.py
--rw-rw-rw-   0 root         (0) root         (0)     3594 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_language_packs.py
--rw-rw-rw-   0 root         (0) root         (0)    49990 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_lint.py
--rw-rw-rw-   0 root         (0) root         (0)    15922 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_online_accounts.py
--rw-rw-rw-   0 root         (0) root         (0)     5596 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_push_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7237 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_scope.py
--rw-rw-rw-   0 root         (0) root         (0)    62507 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_security.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_skeleton.py
--rw-rw-rw-   0 root         (0) root         (0)    26054 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_systemd.py
--rw-rw-rw-   0 root         (0) root         (0)    43114 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     6662 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/cr_url_dispatcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:27:58.734434 click-reviewers-tools-0.78/clickreviews/data/
--rw-rw-rw-   0 root         (0) root         (0)     2870 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/data/icon.png
--rw-rw-rw-   0 root         (0) root         (0)     5429 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/frameworks.py
--rw-rw-rw-   0 root         (0) root         (0)     2442 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     6931 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/overrides.py
--rw-rw-rw-   0 root         (0) root         (0)     3435 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/remote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:27:58.742434 click-reviewers-tools-0.78/clickreviews/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4850 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_aaa_example_cr_skeleton.py
--rw-rw-rw-   0 root         (0) root         (0)     6934 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_cr_bin_path.py
--rw-rw-rw-   0 root         (0) root         (0)     5766 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_cr_common.py
--rw-rw-rw-   0 root         (0) root         (0)     7203 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_cr_content_hub.py
--rw-rw-rw-   0 root         (0) root         (0)    44349 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_cr_desktop.py
--rw-rw-rw-   0 root         (0) root         (0)     8757 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_cr_framework.py
--rw-rw-rw-   0 root         (0) root         (0)    83423 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_cr_lint.py
--rw-rw-rw-   0 root         (0) root         (0)    27032 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_cr_online_accounts.py
--rw-rw-rw-   0 root         (0) root         (0)     8157 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_cr_push_helper.py
--rw-rw-rw-   0 root         (0) root         (0)    10592 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_cr_scope.py
--rw-rw-rw-   0 root         (0) root         (0)   113985 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_cr_security.py
--rw-rw-rw-   0 root         (0) root         (0)    39587 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_cr_systemd.py
--rw-rw-rw-   0 root         (0) root         (0)    11869 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_cr_url_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/test_remote.py
--rw-rw-rw-   0 root         (0) root         (0)     9488 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/clickreviews/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 13:27:58.744434 click-reviewers-tools-0.78/debian/
--rw-rw-rw-   0 root         (0) root         (0)    43595 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/debian/changelog
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/debian/compat
--rw-rw-rw-   0 root         (0) root         (0)     1094 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/debian/control
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/debian/copyright
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/debian/docs
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/debian/links
--rwxrwxrwx   0 root         (0) root         (0)     1503 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/debian/rules
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-06 13:27:58.745435 click-reviewers-tools-0.78/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      755 2023-04-06 13:27:57.000000 click-reviewers-tools-0.78/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:27:40.947424 click-reviewers-tools-0.79/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-03 02:27:40.947424 click-reviewers-tools-0.79/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2089 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:27:40.936424 click-reviewers-tools-0.79/bin/
+-rwxrwxrwx   0 root         (0) root         (0)      913 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-check-bin-path
+-rwxrwxrwx   0 root         (0) root         (0)      931 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-check-content-hub
+-rwxrwxrwx   0 root         (0) root         (0)      894 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-check-desktop
+-rwxrwxrwx   0 root         (0) root         (0)      920 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-check-framework
+-rwxrwxrwx   0 root         (0) root         (0)      938 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-check-functional
+-rwxrwxrwx   0 root         (0) root         (0)      885 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-check-lint
+-rwxrwxrwx   0 root         (0) root         (0)      949 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-check-online-accounts
+-rwxrwxrwx   0 root         (0) root         (0)      931 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-check-push-helper
+-rwxrwxrwx   0 root         (0) root         (0)      896 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-check-scope
+-rwxrwxrwx   0 root         (0) root         (0)      909 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-check-security
+-rwxrwxrwx   0 root         (0) root         (0)      914 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-check-skeleton
+-rwxrwxrwx   0 root         (0) root         (0)      908 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-check-systemd
+-rwxrwxrwx   0 root         (0) root         (0)      949 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-check-url-dispatcher
+-rwxrwxrwx   0 root         (0) root         (0)     6760 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-review
+-rwxrwxrwx   0 root         (0) root         (0)     1282 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-run-checks
+-rwxrwxrwx   0 root         (0) root         (0)     6884 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/click-show-files
+-rwxrwxrwx   0 root         (0) root         (0)      288 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/detect-package
+-rwxrwxrwx   0 root         (0) root         (0)     1546 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/empty-click
+-rwxrwxrwx   0 root         (0) root         (0)     2113 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/repack-click
+-rwxrwxrwx   0 root         (0) root         (0)      332 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/bin/unpack-package
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:27:40.937424 click-reviewers-tools-0.79/click_reviewers_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/click_reviewers_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/click_reviewers_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/click_reviewers_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/click_reviewers_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/click_reviewers_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:27:40.942424 click-reviewers-tools-0.79/clickreviews/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14827 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/apparmor.py
+-rw-rw-rw-   0 root         (0) root         (0)    21795 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     7743 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_bin_path.py
+-rw-rw-rw-   0 root         (0) root         (0)    21600 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     4841 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_content_hub.py
+-rw-rw-rw-   0 root         (0) root         (0)    36327 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_desktop.py
+-rw-rw-rw-   0 root         (0) root         (0)    10104 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_framework.py
+-rw-rw-rw-   0 root         (0) root         (0)    17291 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_functional.py
+-rw-rw-rw-   0 root         (0) root         (0)     3594 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_language_packs.py
+-rw-rw-rw-   0 root         (0) root         (0)    49990 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_lint.py
+-rw-rw-rw-   0 root         (0) root         (0)    15922 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_online_accounts.py
+-rw-rw-rw-   0 root         (0) root         (0)     5596 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_push_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7237 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_scope.py
+-rw-rw-rw-   0 root         (0) root         (0)    62507 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_skeleton.py
+-rw-rw-rw-   0 root         (0) root         (0)    26054 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_systemd.py
+-rw-rw-rw-   0 root         (0) root         (0)    43114 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     6662 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/cr_url_dispatcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:27:40.942424 click-reviewers-tools-0.79/clickreviews/data/
+-rw-rw-rw-   0 root         (0) root         (0)     2870 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/data/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     5429 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/frameworks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2442 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     6931 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/overrides.py
+-rw-rw-rw-   0 root         (0) root         (0)     3435 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/remote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:27:40.945424 click-reviewers-tools-0.79/clickreviews/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_aaa_example_cr_skeleton.py
+-rw-rw-rw-   0 root         (0) root         (0)     6934 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_cr_bin_path.py
+-rw-rw-rw-   0 root         (0) root         (0)     5766 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_cr_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     7203 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_cr_content_hub.py
+-rw-rw-rw-   0 root         (0) root         (0)    44349 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_cr_desktop.py
+-rw-rw-rw-   0 root         (0) root         (0)     8757 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_cr_framework.py
+-rw-rw-rw-   0 root         (0) root         (0)    83423 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_cr_lint.py
+-rw-rw-rw-   0 root         (0) root         (0)    27032 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_cr_online_accounts.py
+-rw-rw-rw-   0 root         (0) root         (0)     8157 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_cr_push_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)    10592 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_cr_scope.py
+-rw-rw-rw-   0 root         (0) root         (0)   113985 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_cr_security.py
+-rw-rw-rw-   0 root         (0) root         (0)    39587 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_cr_systemd.py
+-rw-rw-rw-   0 root         (0) root         (0)    11869 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_cr_url_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/test_remote.py
+-rw-rw-rw-   0 root         (0) root         (0)     9488 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/clickreviews/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:27:40.947424 click-reviewers-tools-0.79/debian/
+-rw-rw-rw-   0 root         (0) root         (0)    43795 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/debian/changelog
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/debian/control
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/debian/copyright
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/debian/docs
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/debian/links
+-rwxrwxrwx   0 root         (0) root         (0)     1503 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/debian/rules
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-03 02:27:40.947424 click-reviewers-tools-0.79/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      755 2023-06-03 02:27:40.000000 click-reviewers-tools-0.79/setup.py
```

### Comparing `click-reviewers-tools-0.78/COPYING` & `click-reviewers-tools-0.79/COPYING`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/README.md` & `click-reviewers-tools-0.79/README.md`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-check-bin-path` & `click-reviewers-tools-0.79/bin/click-check-bin-path`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-check-content-hub` & `click-reviewers-tools-0.79/bin/click-check-content-hub`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-check-desktop` & `click-reviewers-tools-0.79/bin/click-check-desktop`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-check-framework` & `click-reviewers-tools-0.79/bin/click-check-framework`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-check-functional` & `click-reviewers-tools-0.79/bin/click-check-functional`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-check-lint` & `click-reviewers-tools-0.79/bin/click-check-lint`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-check-online-accounts` & `click-reviewers-tools-0.79/bin/click-check-online-accounts`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-check-push-helper` & `click-reviewers-tools-0.79/bin/click-check-push-helper`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-check-scope` & `click-reviewers-tools-0.79/bin/click-check-scope`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-check-security` & `click-reviewers-tools-0.79/bin/click-check-security`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-check-skeleton` & `click-reviewers-tools-0.79/bin/click-check-skeleton`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-check-systemd` & `click-reviewers-tools-0.79/bin/click-check-systemd`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-check-url-dispatcher` & `click-reviewers-tools-0.79/bin/click-check-url-dispatcher`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-review` & `click-reviewers-tools-0.79/bin/click-review`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-run-checks` & `click-reviewers-tools-0.79/bin/click-run-checks`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/click-show-files` & `click-reviewers-tools-0.79/bin/click-show-files`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/empty-click` & `click-reviewers-tools-0.79/bin/empty-click`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/bin/repack-click` & `click-reviewers-tools-0.79/bin/repack-click`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/click_reviewers_tools.egg-info/SOURCES.txt` & `click-reviewers-tools-0.79/click_reviewers_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/apparmor.py` & `click-reviewers-tools-0.79/clickreviews/apparmor.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/common.py` & `click-reviewers-tools-0.79/clickreviews/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     magic_binary_file_descriptions = [
         'application/x-executable; charset=binary',
         'application/x-sharedlib; charset=binary',
         'application/x-object; charset=binary',
         'application/x-executable',
         'application/x-sharedlib',
         'application/x-object',
+        'application/x-pie-executable',
     ]
 
     def __init__(self, fn, review_type, overrides=None):
         self.pkg_filename = fn
         self._check_package_exists()
 
         self.review_type = review_type
```

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_bin_path.py` & `click-reviewers-tools-0.79/clickreviews/cr_bin_path.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_common.py` & `click-reviewers-tools-0.79/clickreviews/cr_common.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_content_hub.py` & `click-reviewers-tools-0.79/clickreviews/cr_content_hub.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_desktop.py` & `click-reviewers-tools-0.79/clickreviews/cr_desktop.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_framework.py` & `click-reviewers-tools-0.79/clickreviews/cr_framework.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_functional.py` & `click-reviewers-tools-0.79/clickreviews/cr_functional.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_language_packs.py` & `click-reviewers-tools-0.79/clickreviews/cr_language_packs.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_lint.py` & `click-reviewers-tools-0.79/clickreviews/cr_lint.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_online_accounts.py` & `click-reviewers-tools-0.79/clickreviews/cr_online_accounts.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_push_helper.py` & `click-reviewers-tools-0.79/clickreviews/cr_push_helper.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_scope.py` & `click-reviewers-tools-0.79/clickreviews/cr_scope.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_security.py` & `click-reviewers-tools-0.79/clickreviews/cr_security.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_skeleton.py` & `click-reviewers-tools-0.79/clickreviews/cr_skeleton.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_systemd.py` & `click-reviewers-tools-0.79/clickreviews/cr_systemd.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_tests.py` & `click-reviewers-tools-0.79/clickreviews/cr_tests.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/cr_url_dispatcher.py` & `click-reviewers-tools-0.79/clickreviews/cr_url_dispatcher.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/data/icon.png` & `click-reviewers-tools-0.79/clickreviews/data/icon.png`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/frameworks.py` & `click-reviewers-tools-0.79/clickreviews/frameworks.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/modules.py` & `click-reviewers-tools-0.79/clickreviews/modules.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/overrides.py` & `click-reviewers-tools-0.79/clickreviews/overrides.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/remote.py` & `click-reviewers-tools-0.79/clickreviews/remote.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_aaa_example_cr_skeleton.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_aaa_example_cr_skeleton.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_cr_bin_path.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_cr_bin_path.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_cr_common.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_cr_common.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_cr_content_hub.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_cr_content_hub.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_cr_desktop.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_cr_desktop.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_cr_framework.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_cr_framework.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_cr_lint.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_cr_lint.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_cr_online_accounts.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_cr_online_accounts.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_cr_push_helper.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_cr_push_helper.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_cr_scope.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_cr_scope.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_cr_security.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_cr_security.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_cr_systemd.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_cr_systemd.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_cr_url_dispatcher.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_cr_url_dispatcher.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_modules.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/test_remote.py` & `click-reviewers-tools-0.79/clickreviews/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/clickreviews/tests/utils.py` & `click-reviewers-tools-0.79/clickreviews/tests/utils.py`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/debian/changelog` & `click-reviewers-tools-0.79/debian/changelog`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+click-reviewers-tools (0.79) unstable; urgency=medium
+
+  * Added application/x-pie-executable to the binary detection
+
+ -- Clickable <bhdouglass+clickable@gmail.com>  Fri, 02 Jul 2023 10:24:00 -0500
+
 click-reviewers-tools (0.78) unstable; urgency=medium
 
   * Python scripts are now allowed in desktop file Execs
 
  -- Clickable <bhdouglass+clickable@gmail.com>  Thu, 06 Apr 2023 09:23:00 -0500
 
 click-reviewers-tools (0.77) unstable; urgency=medium
```

### Comparing `click-reviewers-tools-0.78/debian/control` & `click-reviewers-tools-0.79/debian/control`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/debian/copyright` & `click-reviewers-tools-0.79/debian/copyright`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/debian/rules` & `click-reviewers-tools-0.79/debian/rules`

 * *Files identical despite different names*

### Comparing `click-reviewers-tools-0.78/setup.py` & `click-reviewers-tools-0.79/setup.py`

 * *Files identical despite different names*

