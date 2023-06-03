# Comparing `tmp/m-abac-test-1.0.4.tar.gz` & `tmp/m-abac-test-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abac-test-1.0.4.tar", last modified: Wed May 24 07:58:47 2023, max compression
+gzip compressed data, was "m-abac-test-1.0.5.tar", last modified: Sat Jun  3 02:38:06 2023, max compression
```

## Comparing `m-abac-test-1.0.4.tar` & `m-abac-test-1.0.5.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.335215 m-abac-test-1.0.4/
--rw-r--r--   0 root         (0) root         (0)     1746 2023-05-24 07:58:47.331215 m-abac-test-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.279214 m-abac-test-1.0.4/m_abac_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1746 2023-05-24 07:58:46.000000 m-abac-test-1.0.4/m_abac_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3725 2023-05-24 07:58:47.000000 m-abac-test-1.0.4/m_abac_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:58:46.000000 m-abac-test-1.0.4/m_abac_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-24 07:58:46.000000 m-abac-test-1.0.4/m_abac_test.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-24 07:58:46.000000 m-abac-test-1.0.4/m_abac_test.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.269213 m-abac-test-1.0.4/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.269213 m-abac-test-1.0.4/mobio/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.282214 m-abac-test-1.0.4/mobio/libs/abac/
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.284214 m-abac-test-1.0.4/mobio/libs/abac/adapter/
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/adapter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/adapter/adapter.py
--rw-r--r--   0 root         (0) root         (0)    15511 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/adapter/elasticsearch_adapter.py
--rw-r--r--   0 root         (0) root         (0)     7837 2023-05-24 07:57:21.000000 m-abac-test-1.0.4/mobio/libs/abac/call_api.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-05-24 07:57:21.000000 m-abac-test-1.0.4/mobio/libs/abac/config.py
--rw-r--r--   0 root         (0) root         (0)    13319 2023-05-24 07:57:21.000000 m-abac-test-1.0.4/mobio/libs/abac/pdp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.287214 m-abac-test-1.0.4/mobio/libs/abac/policy/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.288214 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.290214 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/boolean/
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/boolean/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/boolean/base.py
--rw-r--r--   0 root         (0) root         (0)     1107 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/boolean/check_bool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.296214 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/
--rw-r--r--   0 root         (0) root         (0)      323 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/__init__.py
--rw-r--r--   0 root         (0) root         (0)      629 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/all_in.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/all_not_in.py
--rw-r--r--   0 root         (0) root         (0)      638 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/any_in.py
--rw-r--r--   0 root         (0) root         (0)      664 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/any_not_in.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/base.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_empty.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_in.py
--rw-r--r--   0 root         (0) root         (0)      774 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
--rw-r--r--   0 root         (0) root         (0)      728 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_in.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.302214 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/
--rw-r--r--   0 root         (0) root         (0)      243 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2524 2023-05-19 09:33:30.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/base.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_eq.py
--rw-r--r--   0 root         (0) root         (0)     1367 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gt.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gte.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lt.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lte.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.309214 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/base.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_eq.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_gt.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_gte.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_lt.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_lte.py
--rw-r--r--   0 root         (0) root         (0)      978 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.314214 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/base.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.319214 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/base.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/eq.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/gt.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/gte.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/lt.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/lte.py
--rw-r--r--   0 root         (0) root         (0)      869 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.322215 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/__init__.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/base.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/exists.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/not_exists.py
--rw-r--r--   0 root         (0) root         (0)     2126 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:58:47.330215 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/
--rw-r--r--   0 root         (0) root         (0)      401 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/base.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/contains.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/equals.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_contains.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1214 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_equals.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/regex_match.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     6037 2023-05-19 09:33:30.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/policy.py
--rw-r--r--   0 root         (0) root         (0)     5139 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/mobio/libs/abac/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     3631 2023-05-19 09:33:30.000000 m-abac-test-1.0.4/mobio/libs/abac/result_access.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-15 08:15:49.000000 m-abac-test-1.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 07:58:47.335215 m-abac-test-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9779 2023-05-24 07:58:45.000000 m-abac-test-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.057211 m-abac-test-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-06-03 02:38:06.056211 m-abac-test-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.006209 m-abac-test-1.0.5/m_abac_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-06-03 02:38:05.000000 m-abac-test-1.0.5/m_abac_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3725 2023-06-03 02:38:05.000000 m-abac-test-1.0.5/m_abac_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 02:38:05.000000 m-abac-test-1.0.5/m_abac_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-03 02:38:05.000000 m-abac-test-1.0.5/m_abac_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-03 02:38:05.000000 m-abac-test-1.0.5/m_abac_test.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:05.996209 m-abac-test-1.0.5/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:05.997209 m-abac-test-1.0.5/mobio/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.010209 m-abac-test-1.0.5/mobio/libs/abac/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.011209 m-abac-test-1.0.5/mobio/libs/abac/adapter/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/adapter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/adapter/adapter.py
+-rw-r--r--   0 root         (0) root         (0)    15511 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/adapter/elasticsearch_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     7883 2023-06-03 02:36:04.000000 m-abac-test-1.0.5/mobio/libs/abac/call_api.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-05-24 07:57:21.000000 m-abac-test-1.0.5/mobio/libs/abac/config.py
+-rw-r--r--   0 root         (0) root         (0)    13656 2023-06-03 02:36:04.000000 m-abac-test-1.0.5/mobio/libs/abac/pdp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.015210 m-abac-test-1.0.5/mobio/libs/abac/policy/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.016209 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.018210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/boolean/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/boolean/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/boolean/base.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/boolean/check_bool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.026210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      629 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/all_in.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/all_not_in.py
+-rw-r--r--   0 root         (0) root         (0)      638 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/any_in.py
+-rw-r--r--   0 root         (0) root         (0)      664 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/any_not_in.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/base.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_empty.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_in.py
+-rw-r--r--   0 root         (0) root         (0)      774 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
+-rw-r--r--   0 root         (0) root         (0)      728 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_in.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.031210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-05-19 09:33:30.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/base.py
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_eq.py
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gt.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gte.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lt.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lte.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.037210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/base.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_eq.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_gt.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_gte.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_lt.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_lte.py
+-rw-r--r--   0 root         (0) root         (0)      978 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.040210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/base.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.045210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/base.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/eq.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/gt.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/gte.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/lt.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/lte.py
+-rw-r--r--   0 root         (0) root         (0)      869 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.048210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/base.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/exists.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/not_exists.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.055210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/base.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/contains.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/equals.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_contains.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_equals.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/regex_match.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-05-19 09:33:30.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/policy.py
+-rw-r--r--   0 root         (0) root         (0)     5139 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4976 2023-06-03 02:36:04.000000 m-abac-test-1.0.5/mobio/libs/abac/result_access.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 02:38:06.057211 m-abac-test-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9779 2023-06-03 02:38:05.000000 m-abac-test-1.0.5/setup.py
```

### Comparing `m-abac-test-1.0.4/PKG-INFO` & `m-abac-test-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-test
-Version: 1.0.4
+Version: 1.0.5
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: ### ABAC Engine
```

### Comparing `m-abac-test-1.0.4/README.md` & `m-abac-test-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/m_abac_test.egg-info/PKG-INFO` & `m-abac-test-1.0.5/m_abac_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-test
-Version: 1.0.4
+Version: 1.0.5
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: ### ABAC Engine
```

### Comparing `m-abac-test-1.0.4/m_abac_test.egg-info/SOURCES.txt` & `m-abac-test-1.0.5/m_abac_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/adapter/elasticsearch_adapter.py` & `m-abac-test-1.0.5/mobio/libs/abac/adapter/elasticsearch_adapter.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/call_api.py` & `m-abac-test-1.0.5/mobio/libs/abac/call_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,16 +61,17 @@
             # print("admin_get_json_action: {}".format(data))
             return data
         except Exception as er:
             err_msg = "admin_get_json_action err: {}".format(er)
             print(err_msg)
             return {}
 
+    # TODO: thay expiration cho production 15p
     @staticmethod
-    @lru_cache_redis.add(expiration=900)
+    @lru_cache_redis.add(expiration=60)
     def admin_get_list_statement(merchant_id, account_id, resource, action, service):
         """
         :param merchant_id:
         :param account_id:
         :param resource:
         :param action:
         :return: [{
```

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/config.py` & `m-abac-test-1.0.5/mobio/libs/abac/config.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/pdp.py` & `m-abac-test-1.0.5/mobio/libs/abac/pdp.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from .call_api import CallAPI
 from .policy import PolicySchema, AccessType
 from .policy.utils import Utils
 from .result_access import ResultAccess
 from .config import RedisClient
 
+
 class PolicyDecisionPoint(object):
     """
         Policy decision point
     """
 
     class AccountType:
         SYSTEM = "system"
@@ -74,15 +75,17 @@
             self.resource: data_before if data_before else {}
         })
         self.data_after = data_after if data_after else {}
         self.data_before = data_before if data_before else {}
         self.access_level = ""
         self.service = ""
 
-    def check_merchant_use_abac(self, merchant_id):
+    # TODO: bo su dung ham nay tren production
+    @classmethod
+    def check_merchant_use_abac(cls, merchant_id):
         use_abac = False
         data_cache = RedisClient().get_value(RedisClient.KeyCache.MERCHANT_USE_ABAC)
         if data_cache:
             data_merchant = str(data_cache.decode("utf-8")).split(";")
             if merchant_id in data_merchant:
                 use_abac = True
         return use_abac
@@ -127,20 +130,23 @@
                 if statement_check_allow:
                     self.result_access.set_allow_access(self.check_list_statement_is_allow(statement_check_allow))
                 else:
                     self.result_access.set_allow_access(False)
             else:
                 self.result_access.set_allow_access(False)
         except Exception as err:
-            print("Exception: {}".format(err))
+            msg_err = "is_allowed err: {}".format(err)
+            print(msg_err)
+            self.result_access.add_log_error(msg_err)
             self.result_access.set_allow_access(False)
 
         return self.result_access
 
-    def get_info_environment(self, environment):
+    @classmethod
+    def get_info_environment(cls, environment):
         if not environment:
             environment = Utils.get_info_from_header_request()
             if environment:
                 if environment.get("env:user_agent"):
                     environment.update(Utils.parse_user_agent(environment.get("env:user_agent")))
         environment = environment if environment else {}
         environment.update({"env:current_time": Utils.get_date_utcnow()})
@@ -237,15 +243,17 @@
                         if statement.get("check_field") and statement.get("fields"):
                             if not Utils.field_in_body_request(statement.get("fields"), self.data_after):
                                 continue
                     self.result_access.add_log_deny(statement)
                     result_deny = True
                     break
         except Exception as err:
-            print("check_list_statement_is_deny err: {}".format(err))
+            msg_err = "check_list_statement_is_deny err: {}".format(err)
+            print(msg_err)
+            self.result_access.add_log_error(msg_err)
             result_deny = False
         return result_deny
 
     def check_list_statement_is_allow(self, list_statement: list):
         result_allow = False
         try:
             for statement in list_statement:
@@ -276,10 +284,12 @@
                             list_field_data_after = list(self.data_after.keys())
                             if not set(list_field_data_after).issubset(statement.get("fields")):
                                 result_allow = False
                                 continue
                         break
 
         except Exception as err:
-            print("check_list_statement_is_allow err: {}".format(err))
+            msg_err = "check_list_statement_is_allow err: {}".format(err)
+            print(msg_err)
+            self.result_access.add_log_error(msg_err)
             result_allow = False
         return result_allow
```

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/base.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/boolean/base.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/boolean/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/boolean/check_bool.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/boolean/check_bool.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/all_in.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/all_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/all_not_in.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/all_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/any_in.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/any_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/any_not_in.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/any_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/base.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_empty.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_in.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_empty.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/collection/is_not_in.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/base.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_eq.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gt.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_gte.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lt.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_lte.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/date_time/date_neq.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/base.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_eq.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_gt.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_gte.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_lt.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_lte.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/day/day_neq.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/base.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/base.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/eq.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/gt.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/gte.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/lt.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/lte.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/numeric/neq.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/base.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/exists.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/others/not_exists.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/not_exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/schema.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/schema.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/base.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/contains.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/ends_with.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/equals.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_contains.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_ends_with.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_equals.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/not_starts_with.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/regex_match.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/regex_match.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/conditions/string/starts_with.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/exceptions.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/exceptions.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/policy.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/policy.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/policy/utils.py` & `m-abac-test-1.0.5/mobio/libs/abac/policy/utils.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.4/mobio/libs/abac/result_access.py` & `m-abac-test-1.0.5/mobio/libs/abac/result_access.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,37 @@
 class ResultAccess:
     def __init__(self):
         self.allow_access = False
         self.display_config = []
         self.filter_config = []
         self.log_statement_deny = []
         self.log_statement_allow = []
+        self.log_error = []
 
     def get_allow_access(self):
         if self.allow_access:
             print("statement_allow: {}".format(self.log_statement_allow))
         else:
             print("statement_deny: {}".format(self.log_statement_deny))
-
+        print("log_error: {}".format(self.log_error))
         return self.allow_access
 
     def set_allow_access(self, value: bool):
         self.allow_access = value
 
     def get_filter_config(self):
         """
-
         filter: [{'effect': 'allow', 'condition': [{'operator': 'StringEquals', 'field': 'deal:block',
         'values': ['KHDN'], 'qualifier': 'ForAnyValue', 'if_exists': False, 'ignore_case': False},
         {'operator': 'StringStartsWith', 'field': 'deal:scope_code', 'values': ['MB##HN'],
         'qualifier': 'ForAnyValue', 'if_exists': False, 'ignore_case': False}]}]
         :return:
         """
         # print(self.filter_config)
-        dict_field = {}
-        dict_exists = {}
-        list_filter_config = []
-        index_statement = 0
-        for statement in self.filter_config:
-            item_condition = []
-            index_condition = 0
-            effect = statement.get("effect")
-            for condition in statement.get("condition"):
-                operator = condition.get("operator")
-                field = condition.get("field")
-                qualifier = condition.get("qualifier")
-                key_filter = self.build_key_filter_config(effect, operator, field, qualifier)
-                if key_filter not in dict_field:
-                    dict_field[key_filter] = [index_statement, index_condition]
-                    item_condition.append(condition)
-                else:
-                    dict_exists[key_filter] = condition
-                index_condition += 1
-            if item_condition:
-                list_filter_config.append({
-                    'effect': effect,
-                    'condition': item_condition
-                })
-            index_statement += 1
-        for k, v in dict_exists.items():
-            if k in dict_field:
-                list_filter_config[dict_field.get(k)[0]].get("condition")[dict_field.get(k)[1]].get("values").extend(v.get("values"))
-
-        return list_filter_config
+        return self.filter_config
 
     def add_filter_config(self, value):
         self.filter_config.append(value)
 
     def get_display_config(self):
         return self.display_config
 
@@ -76,14 +47,15 @@
         items = key_filter.split("#")
         return {
             "effect": items[0],
             "operator": items[1],
             "field": items[2],
             "qualifier": items[3],
         }
+
     @classmethod
     def convert_data_save_log(cls, value):
         return {
             'merchant_id': value.get('merchant_id'),
             'policy_code': value.get('policy_code'),
             'statement_id': value.get('statement_id'),
             'effect': value.get('effect'),
@@ -92,7 +64,61 @@
         }
 
     def add_log_deny(self, value):
         self.log_statement_deny.append(self.convert_data_save_log(value))
 
     def add_log_allow(self, value):
         self.log_statement_allow.append(self.convert_data_save_log(value))
+
+    def add_log_error(self, value):
+        self.log_error.append(value)
+
+    def get_log(self):
+        return {
+            "error": self.log_error,
+            "statement_allow": self.log_statement_allow,
+            "statement_deny": self.log_statement_deny,
+        }
+
+    # gom các condition cùng key ở các statement lại thành 1 condition,
+    # nhưng logic chạy list statement thay đổi thành statement or với nhau, các condition trong statement and,
+    # như vậy gom sẽ thành sai logic, kể cả gom trong 1 statement cũng là sai logic,
+    # ví dụ user nào xem dữ liệu theo mã cấp user đó hoặc 2 mã cấp khác, policy sẽ tạo 2 statment để thỏa mãn logic trên
+    def group_condition_key(self):
+        """
+        filter: [{'effect': 'allow', 'condition': [{'operator': 'StringEquals', 'field': 'deal:block',
+        'values': ['KHDN'], 'qualifier': 'ForAnyValue', 'if_exists': False, 'ignore_case': False},
+        {'operator': 'StringStartsWith', 'field': 'deal:scope_code', 'values': ['MB##HN'],
+        'qualifier': 'ForAnyValue', 'if_exists': False, 'ignore_case': False}]}]
+        :return:
+        """
+        # print(self.filter_config)
+        dict_field = {}
+        dict_exists = {}
+        list_filter_config = []
+        index_statement = 0
+        for statement in self.filter_config:
+            item_condition = []
+            index_condition = 0
+            effect = statement.get("effect")
+            for condition in statement.get("condition"):
+                operator = condition.get("operator")
+                field = condition.get("field")
+                qualifier = condition.get("qualifier")
+                key_filter = self.build_key_filter_config(effect, operator, field, qualifier)
+                if key_filter not in dict_field:
+                    dict_field[key_filter] = [index_statement, index_condition]
+                    item_condition.append(condition)
+                else:
+                    dict_exists[key_filter] = condition
+                index_condition += 1
+            if item_condition:
+                list_filter_config.append({
+                    'effect': effect,
+                    'condition': item_condition
+                })
+            index_statement += 1
+        for k, v in dict_exists.items():
+            if k in dict_field:
+                list_filter_config[dict_field.get(k)[0]].get("condition")[dict_field.get(k)[1]].get("values").extend(
+                    v.get("values"))
+        return list_filter_config
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `m-abac-test-1.0.4/setup.py` & `m-abac-test-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         ]
         # with open(Requirements.requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
-version_dev='1.0.4'
+version_dev='1.0.5'
 version_prod='1.0.0'
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
@@ -70,15 +70,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.4',  # Required
+    version='1.0.5',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

