# Comparing `tmp/markdown-it-py-2.2.0.tar.gz` & `tmp/markdown-it-py-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-it-py-2.2.0.tar", last modified: Wed Feb 22 05:54:29 2023, max compression
+gzip compressed data, was "markdown-it-py-3.0.0.tar", last modified: Sat Jun  3 06:41:09 2023, max compression
```

## Comparing `markdown-it-py-2.2.0.tar` & `markdown-it-py-3.0.0.tar`

### file list

```diff
@@ -1,82 +1,89 @@
--rw-r--r--   0        0        0      598 2023-02-22 05:54:25.754665 markdown-it-py-2.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1170 2023-02-22 05:54:25.754665 markdown-it-py-2.2.0/.github/workflows/benchmark.yml
--rw-r--r--   0        0        0     3491 2023-02-22 05:54:25.754665 markdown-it-py-2.2.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1930 2023-02-22 05:54:25.754665 markdown-it-py-2.2.0/.gitignore
--rw-r--r--   0        0        0      893 2023-02-22 05:54:25.754665 markdown-it-py-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      213 2023-02-22 05:54:25.754665 markdown-it-py-2.2.0/.readthedocs.yml
--rw-r--r--   0        0        0    11980 2023-02-22 05:54:25.754665 markdown-it-py-2.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-22 05:54:25.754665 markdown-it-py-2.2.0/LICENSE
--rw-r--r--   0        0        0     1073 2023-02-22 05:54:25.754665 markdown-it-py-2.2.0/LICENSE.markdown-it
--rw-r--r--   0        0        0     4314 2023-02-22 05:54:25.754665 markdown-it-py-2.2.0/README.md
--rw-r--r--   0        0        0      582 2023-02-22 05:54:25.754665 markdown-it-py-2.2.0/SECURITY.md
--rw-r--r--   0        0        0      162 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/codecov.yml
--rw-r--r--   0        0        0      113 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/__init__.py
--rw-r--r--   0        0        0      248 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/_compat.py
--rw-r--r--   0        0        0     2317 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/_punycode.py
--rw-r--r--   0        0        0        0 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/cli/__init__.py
--rw-r--r--   0        0        0     2901 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/cli/parse.py
--rw-r--r--   0        0        0        0 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/common/__init__.py
--rw-r--r--   0        0        0      156 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/common/entities.py
--rw-r--r--   0        0        0      932 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/common/html_blocks.py
--rw-r--r--   0        0        0      929 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/common/html_re.py
--rw-r--r--   0        0        0     2631 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/common/normalize_url.py
--rw-r--r--   0        0        0    10894 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/common/utils.py
--rw-r--r--   0        0        0      253 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/helpers/__init__.py
--rw-r--r--   0        0        0     1953 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/helpers/parse_link_destination.py
--rw-r--r--   0        0        0     1070 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/helpers/parse_link_label.py
--rw-r--r--   0        0        0     1410 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/helpers/parse_link_title.py
--rw-r--r--   0        0        0    12228 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/main.py
--rw-r--r--   0        0        0     3662 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/parser_block.py
--rw-r--r--   0        0        0      835 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/parser_core.py
--rw-r--r--   0        0        0     4130 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/parser_inline.py
--rw-r--r--   0        0        0     2516 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/port.yaml
--rw-r--r--   0        0        0      898 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/presets/__init__.py
--rw-r--r--   0        0        0     2809 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/presets/commonmark.py
--rw-r--r--   0        0        0     1765 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/presets/default.py
--rw-r--r--   0        0        0     2006 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/presets/zero.py
--rw-r--r--   0        0        0       26 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/py.typed
--rw-r--r--   0        0        0    10041 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/renderer.py
--rw-r--r--   0        0        0     8376 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/ruler.py
--rw-r--r--   0        0        0      553 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_block/__init__.py
--rw-r--r--   0        0        0     9057 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_block/blockquote.py
--rw-r--r--   0        0        0      886 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_block/code.py
--rw-r--r--   0        0        0     2704 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_block/fence.py
--rw-r--r--   0        0        0     1879 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_block/heading.py
--rw-r--r--   0        0        0     1309 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_block/hr.py
--rw-r--r--   0        0        0     2808 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_block/html_block.py
--rw-r--r--   0        0        0     2798 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_block/lheading.py
--rw-r--r--   0        0        0     9944 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_block/list.py
--rw-r--r--   0        0        0     1851 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_block/paragraph.py
--rw-r--r--   0        0        0     6323 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_block/reference.py
--rw-r--r--   0        0        0     7226 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_block/state_block.py
--rw-r--r--   0        0        0     7226 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_block/table.py
--rw-r--r--   0        0        0      344 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_core/__init__.py
--rw-r--r--   0        0        0      413 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_core/block.py
--rw-r--r--   0        0        0      325 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_core/inline.py
--rw-r--r--   0        0        0     4833 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_core/linkify.py
--rw-r--r--   0        0        0      402 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_core/normalize.py
--rw-r--r--   0        0        0     3560 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_core/replacements.py
--rw-r--r--   0        0        0     7251 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_core/smartquotes.py
--rw-r--r--   0        0        0      584 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_core/state_core.py
--rw-r--r--   0        0        0      649 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_inline/__init__.py
--rw-r--r--   0        0        0     2131 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_inline/autolink.py
--rw-r--r--   0        0        0     2112 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_inline/backticks.py
--rw-r--r--   0        0        0     4062 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_inline/balance_pairs.py
--rw-r--r--   0        0        0     2948 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_inline/emphasis.py
--rw-r--r--   0        0        0     1653 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_inline/entity.py
--rw-r--r--   0        0        0     1116 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_inline/escape.py
--rw-r--r--   0        0        0     1019 2023-02-22 05:54:25.758665 markdown-it-py-2.2.0/markdown_it/rules_inline/html_inline.py
--rw-r--r--   0        0        0     4260 2023-02-22 05:54:25.762665 markdown-it-py-2.2.0/markdown_it/rules_inline/image.py
--rw-r--r--   0        0        0     4362 2023-02-22 05:54:25.762665 markdown-it-py-2.2.0/markdown_it/rules_inline/link.py
--rw-r--r--   0        0        0     1176 2023-02-22 05:54:25.762665 markdown-it-py-2.2.0/markdown_it/rules_inline/newline.py
--rw-r--r--   0        0        0     5388 2023-02-22 05:54:25.762665 markdown-it-py-2.2.0/markdown_it/rules_inline/state_inline.py
--rw-r--r--   0        0        0     3390 2023-02-22 05:54:25.762665 markdown-it-py-2.2.0/markdown_it/rules_inline/strikethrough.py
--rw-r--r--   0        0        0     1427 2023-02-22 05:54:25.762665 markdown-it-py-2.2.0/markdown_it/rules_inline/text.py
--rw-r--r--   0        0        0     1491 2023-02-22 05:54:25.762665 markdown-it-py-2.2.0/markdown_it/rules_inline/text_collapse.py
--rw-r--r--   0        0        0     6374 2023-02-22 05:54:25.762665 markdown-it-py-2.2.0/markdown_it/token.py
--rw-r--r--   0        0        0    11052 2023-02-22 05:54:25.762665 markdown-it-py-2.2.0/markdown_it/tree.py
--rw-r--r--   0        0        0     3262 2023-02-22 05:54:25.762665 markdown-it-py-2.2.0/markdown_it/utils.py
--rw-r--r--   0        0        0      440 2023-02-22 05:54:25.762665 markdown-it-py-2.2.0/profiler.py
--rw-r--r--   0        0        0     2497 2023-02-22 05:54:25.762665 markdown-it-py-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     1859 2023-02-22 05:54:25.766665 markdown-it-py-2.2.0/tox.ini
--rw-r--r--   0        0        0     6812 1970-01-01 00:00:00.000000 markdown-it-py-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1669 2023-06-02 22:15:29.978911 markdown-it-py-3.0.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      232 2023-06-02 22:08:01.058235 markdown-it-py-3.0.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1152 2023-06-02 22:05:56.704103 markdown-it-py-3.0.0/.github/ISSUE_TEMPLATE/enhancement.yml
+-rw-r--r--   0        0        0      598 2023-02-22 05:16:06.034604 markdown-it-py-3.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1170 2023-04-27 14:35:15.079594 markdown-it-py-3.0.0/.github/workflows/benchmark.yml
+-rw-r--r--   0        0        0     1176 2023-04-25 17:36:14.764882 markdown-it-py-3.0.0/.github/workflows/fuzz.yml
+-rw-r--r--   0        0        0     3530 2023-05-31 19:00:21.173759 markdown-it-py-3.0.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1930 2020-08-17 12:06:42.809720 markdown-it-py-3.0.0/.gitignore
+-rw-r--r--   0        0        0      980 2023-05-31 19:22:19.943410 markdown-it-py-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      197 2023-06-02 21:29:23.440918 markdown-it-py-3.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0    17137 2023-06-02 23:05:58.331225 markdown-it-py-3.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2020-08-17 18:24:49.078116 markdown-it-py-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1073 2020-08-17 12:07:58.080481 markdown-it-py-3.0.0/LICENSE.markdown-it
+-rw-r--r--   0        0        0     4445 2023-06-02 23:10:28.020847 markdown-it-py-3.0.0/README.md
+-rw-r--r--   0        0        0      582 2023-02-22 05:30:46.917610 markdown-it-py-3.0.0/SECURITY.md
+-rw-r--r--   0        0        0      162 2020-08-22 03:25:55.440118 markdown-it-py-3.0.0/codecov.yml
+-rw-r--r--   0        0        0      113 2023-06-02 22:19:25.394489 markdown-it-py-3.0.0/markdown_it/__init__.py
+-rw-r--r--   0        0        0      246 2023-04-27 14:52:36.751985 markdown-it-py-3.0.0/markdown_it/_compat.py
+-rw-r--r--   0        0        0     2364 2023-05-31 19:00:21.175286 markdown-it-py-3.0.0/markdown_it/_punycode.py
+-rw-r--r--   0        0        0        0 2020-08-17 12:07:58.093418 markdown-it-py-3.0.0/markdown_it/cli/__init__.py
+-rw-r--r--   0        0        0     2901 2023-04-27 15:03:46.217035 markdown-it-py-3.0.0/markdown_it/cli/parse.py
+-rw-r--r--   0        0        0        0 2020-08-17 12:07:58.096467 markdown-it-py-3.0.0/markdown_it/common/__init__.py
+-rw-r--r--   0        0        0      156 2021-12-03 08:14:21.023945 markdown-it-py-3.0.0/markdown_it/common/entities.py
+-rw-r--r--   0        0        0      932 2022-04-14 21:00:54.421274 markdown-it-py-3.0.0/markdown_it/common/html_blocks.py
+-rw-r--r--   0        0        0      929 2021-03-10 11:01:59.861261 markdown-it-py-3.0.0/markdown_it/common/html_re.py
+-rw-r--r--   0        0        0     2568 2023-05-31 19:27:46.192426 markdown-it-py-3.0.0/markdown_it/common/normalize_url.py
+-rw-r--r--   0        0        0    10728 2023-06-02 17:28:48.285828 markdown-it-py-3.0.0/markdown_it/common/utils.py
+-rw-r--r--   0        0        0      253 2023-05-31 23:14:23.068155 markdown-it-py-3.0.0/markdown_it/helpers/__init__.py
+-rw-r--r--   0        0        0     1977 2023-06-01 00:50:08.944519 markdown-it-py-3.0.0/markdown_it/helpers/parse_link_destination.py
+-rw-r--r--   0        0        0     1036 2023-06-01 00:50:08.945861 markdown-it-py-3.0.0/markdown_it/helpers/parse_link_label.py
+-rw-r--r--   0        0        0     1425 2023-05-31 19:00:21.176852 markdown-it-py-3.0.0/markdown_it/helpers/parse_link_title.py
+-rw-r--r--   0        0        0    12772 2023-06-02 06:58:15.457300 markdown-it-py-3.0.0/markdown_it/main.py
+-rw-r--r--   0        0        0     3911 2023-06-02 21:17:30.732849 markdown-it-py-3.0.0/markdown_it/parser_block.py
+-rw-r--r--   0        0        0     1010 2023-06-02 19:55:17.742607 markdown-it-py-3.0.0/markdown_it/parser_core.py
+-rw-r--r--   0        0        0     4997 2023-06-02 20:27:50.962828 markdown-it-py-3.0.0/markdown_it/parser_inline.py
+-rw-r--r--   0        0        0     2446 2023-06-02 19:00:25.345600 markdown-it-py-3.0.0/markdown_it/port.yaml
+-rw-r--r--   0        0        0      970 2023-06-02 17:25:36.105394 markdown-it-py-3.0.0/markdown_it/presets/__init__.py
+-rw-r--r--   0        0        0     2868 2023-06-02 13:12:19.159771 markdown-it-py-3.0.0/markdown_it/presets/commonmark.py
+-rw-r--r--   0        0        0     1810 2023-05-31 19:00:21.180165 markdown-it-py-3.0.0/markdown_it/presets/default.py
+-rw-r--r--   0        0        0     2112 2023-06-02 13:12:19.160283 markdown-it-py-3.0.0/markdown_it/presets/zero.py
+-rw-r--r--   0        0        0       26 2020-12-14 18:24:47.829455 markdown-it-py-3.0.0/markdown_it/py.typed
+-rw-r--r--   0        0        0     9970 2023-05-31 19:36:46.126969 markdown-it-py-3.0.0/markdown_it/renderer.py
+-rw-r--r--   0        0        0     9199 2023-06-02 20:15:33.490455 markdown-it-py-3.0.0/markdown_it/ruler.py
+-rw-r--r--   0        0        0      553 2022-04-14 22:41:09.549196 markdown-it-py-3.0.0/markdown_it/rules_block/__init__.py
+-rw-r--r--   0        0        0     8887 2023-06-01 00:50:08.949225 markdown-it-py-3.0.0/markdown_it/rules_block/blockquote.py
+-rw-r--r--   0        0        0      859 2023-05-31 19:00:21.236320 markdown-it-py-3.0.0/markdown_it/rules_block/code.py
+-rw-r--r--   0        0        0     2537 2023-06-01 00:50:08.949869 markdown-it-py-3.0.0/markdown_it/rules_block/fence.py
+-rw-r--r--   0        0        0     1746 2023-06-01 00:50:08.950996 markdown-it-py-3.0.0/markdown_it/rules_block/heading.py
+-rw-r--r--   0        0        0     1226 2023-06-01 00:50:08.951769 markdown-it-py-3.0.0/markdown_it/rules_block/hr.py
+-rw-r--r--   0        0        0     2721 2023-06-01 00:50:08.953519 markdown-it-py-3.0.0/markdown_it/rules_block/html_block.py
+-rw-r--r--   0        0        0     2625 2023-06-02 20:04:26.119568 markdown-it-py-3.0.0/markdown_it/rules_block/lheading.py
+-rw-r--r--   0        0        0     9668 2023-06-02 20:33:30.137665 markdown-it-py-3.0.0/markdown_it/rules_block/list.py
+-rw-r--r--   0        0        0     1818 2023-06-02 20:04:54.352720 markdown-it-py-3.0.0/markdown_it/rules_block/paragraph.py
+-rw-r--r--   0        0        0     6168 2023-06-01 00:50:08.956070 markdown-it-py-3.0.0/markdown_it/rules_block/reference.py
+-rw-r--r--   0        0        0     8422 2023-06-01 02:32:31.330762 markdown-it-py-3.0.0/markdown_it/rules_block/state_block.py
+-rw-r--r--   0        0        0     6987 2023-06-01 00:50:08.958057 markdown-it-py-3.0.0/markdown_it/rules_block/table.py
+-rw-r--r--   0        0        0      394 2023-06-02 13:12:19.160858 markdown-it-py-3.0.0/markdown_it/rules_core/__init__.py
+-rw-r--r--   0        0        0      372 2023-06-01 00:50:08.959650 markdown-it-py-3.0.0/markdown_it/rules_core/block.py
+-rw-r--r--   0        0        0      325 2021-01-01 15:48:35.788855 markdown-it-py-3.0.0/markdown_it/rules_core/inline.py
+-rw-r--r--   0        0        0     5141 2023-06-02 17:28:46.667352 markdown-it-py-3.0.0/markdown_it/rules_core/linkify.py
+-rw-r--r--   0        0        0      402 2023-02-22 05:16:06.052672 markdown-it-py-3.0.0/markdown_it/rules_core/normalize.py
+-rw-r--r--   0        0        0     3470 2023-06-02 18:49:53.812439 markdown-it-py-3.0.0/markdown_it/rules_core/replacements.py
+-rw-r--r--   0        0        0     7443 2023-06-01 00:50:08.960494 markdown-it-py-3.0.0/markdown_it/rules_core/smartquotes.py
+-rw-r--r--   0        0        0      570 2023-05-31 19:00:21.187860 markdown-it-py-3.0.0/markdown_it/rules_core/state_core.py
+-rw-r--r--   0        0        0     1172 2023-06-02 13:13:21.942233 markdown-it-py-3.0.0/markdown_it/rules_core/text_join.py
+-rw-r--r--   0        0        0      696 2023-06-02 15:16:22.057270 markdown-it-py-3.0.0/markdown_it/rules_inline/__init__.py
+-rw-r--r--   0        0        0     2079 2023-06-01 00:50:08.961029 markdown-it-py-3.0.0/markdown_it/rules_inline/autolink.py
+-rw-r--r--   0        0        0     2037 2023-06-01 00:50:08.961696 markdown-it-py-3.0.0/markdown_it/rules_inline/backticks.py
+-rw-r--r--   0        0        0     4851 2023-06-02 11:22:00.115133 markdown-it-py-3.0.0/markdown_it/rules_inline/balance_pairs.py
+-rw-r--r--   0        0        0     3123 2023-06-02 11:25:09.940585 markdown-it-py-3.0.0/markdown_it/rules_inline/emphasis.py
+-rw-r--r--   0        0        0     1651 2023-06-02 18:23:41.998479 markdown-it-py-3.0.0/markdown_it/rules_inline/entity.py
+-rw-r--r--   0        0        0     1658 2023-06-02 13:12:19.162066 markdown-it-py-3.0.0/markdown_it/rules_inline/escape.py
+-rw-r--r--   0        0        0     1493 2023-06-02 13:12:19.162339 markdown-it-py-3.0.0/markdown_it/rules_inline/fragments_join.py
+-rw-r--r--   0        0        0     1130 2023-06-02 17:28:46.675039 markdown-it-py-3.0.0/markdown_it/rules_inline/html_inline.py
+-rw-r--r--   0        0        0     4135 2023-06-01 00:50:08.964606 markdown-it-py-3.0.0/markdown_it/rules_inline/image.py
+-rw-r--r--   0        0        0     4318 2023-06-02 14:01:04.743633 markdown-it-py-3.0.0/markdown_it/rules_inline/link.py
+-rw-r--r--   0        0        0     1704 2023-06-02 17:29:01.959030 markdown-it-py-3.0.0/markdown_it/rules_inline/linkify.py
+-rw-r--r--   0        0        0     1296 2023-06-02 11:55:45.815624 markdown-it-py-3.0.0/markdown_it/rules_inline/newline.py
+-rw-r--r--   0        0        0     5101 2023-06-02 13:59:20.243655 markdown-it-py-3.0.0/markdown_it/rules_inline/state_inline.py
+-rw-r--r--   0        0        0     3214 2023-06-02 11:22:00.116453 markdown-it-py-3.0.0/markdown_it/rules_inline/strikethrough.py
+-rw-r--r--   0        0        0      901 2023-06-01 00:50:08.968573 markdown-it-py-3.0.0/markdown_it/rules_inline/text.py
+-rw-r--r--   0        0        0     6439 2023-05-31 19:34:57.357400 markdown-it-py-3.0.0/markdown_it/token.py
+-rw-r--r--   0        0        0    11421 2023-06-02 19:13:39.784557 markdown-it-py-3.0.0/markdown_it/tree.py
+-rw-r--r--   0        0        0     5365 2023-05-31 19:00:21.192268 markdown-it-py-3.0.0/markdown_it/utils.py
+-rw-r--r--   0        0        0     2684 2023-06-03 06:36:09.363796 markdown-it-py-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1161 2023-06-02 02:07:01.373232 markdown-it-py-3.0.0/scripts/build_fuzzers.py
+-rw-r--r--   0        0        0      447 2023-06-01 00:50:08.969303 markdown-it-py-3.0.0/scripts/profiler.py
+-rw-r--r--   0        0        0     2119 2023-06-01 00:57:07.396250 markdown-it-py-3.0.0/tox.ini
+-rw-r--r--   0        0        0     6940 1970-01-01 00:00:00.000000 markdown-it-py-3.0.0/PKG-INFO
```

### Comparing `markdown-it-py-2.2.0/.github/dependabot.yml` & `markdown-it-py-3.0.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `markdown-it-py-2.2.0/.github/workflows/benchmark.yml` & `markdown-it-py-3.0.0/.github/workflows/benchmark.yml`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     branches: [master]
 
 jobs:
   benchmark-packages:
 
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Set up Python 3.8
       uses: actions/setup-python@v4
       with:
         python-version: 3.8
 
     - name: install pandoc
```

### Comparing `markdown-it-py-2.2.0/.github/workflows/tests.yml` & `markdown-it-py-3.0.0/.github/workflows/tests.yml`

 * *Files 12% similar despite different names*

```diff
@@ -15,58 +15,59 @@
 jobs:
 
   pre-commit:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python 3.8
       uses: actions/setup-python@v4
       with:
         python-version: '3.8'
     - uses: pre-commit/action@v3.0.0
 
   tests:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['pypy-3.7', '3.7', '3.8', '3.9', '3.10']
+        python-version: ['pypy-3.8', '3.8', '3.9', '3.10', '3.11']
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install .[testing,linkify]
     - name: Run pytest
       run: |
         pytest tests/ --cov=markdown_it --cov-report=xml --cov-report=term-missing
     - name: Upload to Codecov
-      if: matrix.python-version == '3.7' && github.repository == 'executablebooks/markdown-it-py'
+      if: matrix.python-version == '3.8' && github.repository == 'executablebooks/markdown-it-py'
       uses: codecov/codecov-action@v3
       with:
-        name: markdown-it-py-pytests-py3.7
+        name: markdown-it-py-pytests
         flags: pytests
         file: ./coverage.xml
         fail_ci_if_error: true
+        token: ${{ secrets.CODECOV_TOKEN }}
 
   test-plugins:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ['3.8']
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install markdown-it-py
       run: |
         python -m pip install --upgrade pip
@@ -78,15 +79,15 @@
     - name: Run pytest for unit tests of mdit-py-plugins
       run: cd mdit-py-plugins; pytest
 
   benchmark:
 
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Set up Python 3.8
       uses: actions/setup-python@v4
       with:
         python-version: '3.8'
 
     - name: Install tox
@@ -108,15 +109,15 @@
 
     name: Publish to PyPi
     needs: [pre-commit, tests]
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
     runs-on: ubuntu-latest
     steps:
     - name: Checkout source
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
     - name: Set up Python 3.8
       uses: actions/setup-python@v4
       with:
         python-version: '3.8'
     - name: install flit
       run: |
         pip install flit~=3.4
```

### Comparing `markdown-it-py-2.2.0/.gitignore` & `markdown-it-py-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `markdown-it-py-2.2.0/LICENSE` & `markdown-it-py-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown-it-py-2.2.0/LICENSE.markdown-it` & `markdown-it-py-3.0.0/LICENSE.markdown-it`

 * *Files identical despite different names*

### Comparing `markdown-it-py-2.2.0/README.md` & `markdown-it-py-3.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 > Markdown parser done right.
 
 - Follows the __[CommonMark spec](http://spec.commonmark.org/)__ for baseline parsing
 - Configurable syntax: you can add new rules and even replace existing ones.
 - Pluggable: Adds syntax extensions to extend the parser (see the [plugin list][md-plugins]).
 - High speed (see our [benchmarking tests][md-performance])
 - [Safe by default][md-security]
+- Member of [Google's Assured Open Source Software](https://cloud.google.com/assured-open-source-software/docs/supported-packages)
 
 This is a Python port of [markdown-it], and some of its associated plugins.
 For more details see: <https://markdown-it-py.readthedocs.io>.
 
 For details on [markdown-it] itself, see:
 
 - The __[Live demo](https://markdown-it.github.io)__
```

### Comparing `markdown-it-py-2.2.0/SECURITY.md` & `markdown-it-py-3.0.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `markdown-it-py-2.2.0/markdown_it/_punycode.py` & `markdown-it-py-3.0.0/markdown_it/_punycode.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,28 +18,29 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 import codecs
 import re
+from typing import Callable
 
 REGEX_SEPARATORS = re.compile(r"[\x2E\u3002\uFF0E\uFF61]")
 REGEX_NON_ASCII = re.compile(r"[^\0-\x7E]")
 
 
 def encode(uni: str) -> str:
     return codecs.encode(uni, encoding="punycode").decode()
 
 
 def decode(ascii: str) -> str:
-    return codecs.decode(ascii, encoding="punycode")  # type: ignore[call-overload]
+    return codecs.decode(ascii, encoding="punycode")  # type: ignore
 
 
-def map_domain(string, fn):
+def map_domain(string: str, fn: Callable[[str], str]) -> str:
     parts = string.split("@")
     result = ""
     if len(parts) > 1:
         # In email addresses, only the domain name should be punycoded. Leave
         # the local part (i.e. everything up to `@`) intact.
         result = parts[0] + "@"
         string = parts[1]
```

### Comparing `markdown-it-py-2.2.0/markdown_it/cli/parse.py` & `markdown-it-py-3.0.0/markdown_it/cli/parse.py`

 * *Files identical despite different names*

### Comparing `markdown-it-py-2.2.0/markdown_it/common/html_blocks.py` & `markdown-it-py-3.0.0/markdown_it/common/html_blocks.py`

 * *Files identical despite different names*

### Comparing `markdown-it-py-2.2.0/markdown_it/common/html_re.py` & `markdown-it-py-3.0.0/markdown_it/common/html_re.py`

 * *Files identical despite different names*

### Comparing `markdown-it-py-2.2.0/markdown_it/common/normalize_url.py` & `markdown-it-py-3.0.0/markdown_it/common/normalize_url.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from collections.abc import Callable
+from contextlib import suppress
 import re
 from urllib.parse import quote, unquote, urlparse, urlunparse  # noqa: F401
 
 import mdurl
 
 from .. import _punycode
 
@@ -17,62 +18,60 @@
     ::
 
         [label]:   destination   'title'
                 ^^^^^^^^^^^
     """
     parsed = mdurl.parse(url, slashes_denote_host=True)
 
-    if parsed.hostname:
-        # Encode hostnames in urls like:
-        # `http://host/`, `https://host/`, `mailto:user@host`, `//host/`
-        #
-        # We don't encode unknown schemas, because it's likely that we encode
-        # something we shouldn't (e.g. `skype:name` treated as `skype:host`)
-        #
-        if not parsed.protocol or parsed.protocol in RECODE_HOSTNAME_FOR:
-            try:
-                parsed = parsed._replace(hostname=_punycode.to_ascii(parsed.hostname))
-            except Exception:
-                pass
+    # Encode hostnames in urls like:
+    # `http://host/`, `https://host/`, `mailto:user@host`, `//host/`
+    #
+    # We don't encode unknown schemas, because it's likely that we encode
+    # something we shouldn't (e.g. `skype:name` treated as `skype:host`)
+    #
+    if parsed.hostname and (
+        not parsed.protocol or parsed.protocol in RECODE_HOSTNAME_FOR
+    ):
+        with suppress(Exception):
+            parsed = parsed._replace(hostname=_punycode.to_ascii(parsed.hostname))
 
     return mdurl.encode(mdurl.format(parsed))
 
 
 def normalizeLinkText(url: str) -> str:
     """Normalize autolink content
 
     ::
 
         <destination>
          ~~~~~~~~~~~
     """
     parsed = mdurl.parse(url, slashes_denote_host=True)
 
-    if parsed.hostname:
-        # Encode hostnames in urls like:
-        # `http://host/`, `https://host/`, `mailto:user@host`, `//host/`
-        #
-        # We don't encode unknown schemas, because it's likely that we encode
-        # something we shouldn't (e.g. `skype:name` treated as `skype:host`)
-        #
-        if not parsed.protocol or parsed.protocol in RECODE_HOSTNAME_FOR:
-            try:
-                parsed = parsed._replace(hostname=_punycode.to_unicode(parsed.hostname))
-            except Exception:
-                pass
+    # Encode hostnames in urls like:
+    # `http://host/`, `https://host/`, `mailto:user@host`, `//host/`
+    #
+    # We don't encode unknown schemas, because it's likely that we encode
+    # something we shouldn't (e.g. `skype:name` treated as `skype:host`)
+    #
+    if parsed.hostname and (
+        not parsed.protocol or parsed.protocol in RECODE_HOSTNAME_FOR
+    ):
+        with suppress(Exception):
+            parsed = parsed._replace(hostname=_punycode.to_unicode(parsed.hostname))
 
     # add '%' to exclude list because of https://github.com/markdown-it/markdown-it/issues/720
     return mdurl.decode(mdurl.format(parsed), mdurl.DECODE_DEFAULT_CHARS + "%")
 
 
 BAD_PROTO_RE = re.compile(r"^(vbscript|javascript|file|data):")
 GOOD_DATA_RE = re.compile(r"^data:image\/(gif|png|jpeg|webp);")
 
 
-def validateLink(url: str, validator: Callable | None = None) -> bool:
+def validateLink(url: str, validator: Callable[[str], bool] | None = None) -> bool:
     """Validate URL link is allowed in output.
 
     This validator can prohibit more than really needed to prevent XSS.
     It's a tradeoff to keep code simple and to be secure by default.
 
     Note: url should be normalized at this point, and existing entities decoded.
     """
```

### Comparing `markdown-it-py-2.2.0/markdown_it/common/utils.py` & `markdown-it-py-3.0.0/markdown_it/common/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,60 @@
 """Utilities for parsing source text
 """
-import html
+from __future__ import annotations
+
 import re
-from typing import Any
+from typing import Match, TypeVar
 
 from .entities import entities
 
 
-def charCodeAt(src: str, pos: int) -> Any:
+def charCodeAt(src: str, pos: int) -> int | None:
     """
     Returns the Unicode value of the character at the specified location.
 
     @param - index The zero-based index of the desired character.
     If there is no character at the specified index, NaN is returned.
 
     This was added for compatibility with python
     """
     try:
         return ord(src[pos])
     except IndexError:
         return None
 
 
-# Merge objects
-#
-def assign(obj):
-    """Merge objects /*from1, from2, from3, ...*/)"""
-    raise NotImplementedError
-    # sources = Array.prototype.slice.call(arguments, 1)
+def charStrAt(src: str, pos: int) -> str | None:
+    """
+    Returns the Unicode value of the character at the specified location.
 
-    # sources.forEach(function (source) {
-    #   if (!source) { return; }
+    @param - index The zero-based index of the desired character.
+    If there is no character at the specified index, NaN is returned.
 
-    #   if (typeof source !== 'object') {
-    #     throw new TypeError(source + 'must be object')
-    #   }
+    This was added for compatibility with python
+    """
+    try:
+        return src[pos]
+    except IndexError:
+        return None
 
-    #   Object.keys(source).forEach(function (key) {
-    #     obj[key] = source[key]
-    #   })
-    # })
 
-    # return obj
+_ItemTV = TypeVar("_ItemTV")
 
 
-def arrayReplaceAt(src: list, pos: int, newElements: list) -> list:
+def arrayReplaceAt(
+    src: list[_ItemTV], pos: int, newElements: list[_ItemTV]
+) -> list[_ItemTV]:
     """
     Remove element from array and put another array at those position.
     Useful for some operations with tokens
     """
     return src[:pos] + newElements + src[pos + 1 :]
 
 
-######################################################################
-
-
 def isValidEntityCode(c: int) -> bool:
     # broken sequence
     if c >= 0xD800 and c <= 0xDFFF:
         return False
     # never used
     if c >= 0xFDD0 and c <= 0xFDEF:
         return False
@@ -85,59 +81,45 @@
     Note, in the original Javascript two string characters were required,
     for codepoints larger than `0xFFFF`.
     But Python 3 can represent any unicode codepoint in one character.
     """
     return chr(c)
 
 
-UNESCAPE_MD_RE = re.compile(r'\\([!"#$%&\'()*+,\-.\/:;<=>?@[\\\]^_`{|}~])')
+# UNESCAPE_MD_RE = re.compile(r'\\([!"#$%&\'()*+,\-.\/:;<=>?@[\\\]^_`{|}~])')
 # ENTITY_RE_g       = re.compile(r'&([a-z#][a-z0-9]{1,31})', re.IGNORECASE)
 UNESCAPE_ALL_RE = re.compile(
     r'\\([!"#$%&\'()*+,\-.\/:;<=>?@[\\\]^_`{|}~])' + "|" + r"&([a-z#][a-z0-9]{1,31});",
     re.IGNORECASE,
 )
-DIGITAL_ENTITY_TEST_RE = re.compile(r"^#((?:x[a-f0-9]{1,8}|[0-9]{1,8}))", re.IGNORECASE)
+DIGITAL_ENTITY_BASE10_RE = re.compile(r"#([0-9]{1,8})")
+DIGITAL_ENTITY_BASE16_RE = re.compile(r"#x([a-f0-9]{1,8})", re.IGNORECASE)
 
 
 def replaceEntityPattern(match: str, name: str) -> str:
-    """Convert HTML entity patterns
-
-    ::
-
-        https://www.google.com -> https%3A//www.google.com
-
+    """Convert HTML entity patterns,
+    see https://spec.commonmark.org/0.30/#entity-references
     """
-    code = 0
-
     if name in entities:
         return entities[name]
 
-    if ord(name[0]) == 0x23 and DIGITAL_ENTITY_TEST_RE.search(name):
-        code = int(name[2:], 16) if name[1].lower() == "x" else int(name[1:], 10)
-        if isValidEntityCode(code):
-            return fromCodePoint(code)
-
-    return match
-
+    code: None | int = None
+    if pat := DIGITAL_ENTITY_BASE10_RE.fullmatch(name):
+        code = int(pat.group(1), 10)
+    elif pat := DIGITAL_ENTITY_BASE16_RE.fullmatch(name):
+        code = int(pat.group(1), 16)
 
-# def replaceEntities(string):
-#   if (string.indexOf('&') < 0):
-#       return string
-#   return string.replace(ENTITY_RE, replaceEntityPattern)
+    if code is not None and isValidEntityCode(code):
+        return fromCodePoint(code)
 
-
-def unescapeMd(string: str) -> str:
-    raise NotImplementedError
-    # if "\\" in string:
-    #     return string
-    # return string.replace(UNESCAPE_MD_RE, "$1")
+    return match
 
 
 def unescapeAll(string: str) -> str:
-    def replacer_func(match):
+    def replacer_func(match: Match[str]) -> str:
         escaped = match.group(1)
         if escaped:
             return escaped
         entity = match.group(2)
         return replaceEntityPattern(match.group(), entity)
 
     if "\\" not in string and "&" not in string:
@@ -150,38 +132,22 @@
 
 
 def stripEscape(string: str) -> str:
     """Strip escape \\ characters"""
     return ESCAPE_CHAR.sub(r"\1", string)
 
 
-# //////////////////////////////////////////////////////////////////////////////
-
-# TODO This section changed quite a lot, should re-check
-
-# UNESCAPE_HTML_RE = re.compile(r"\\&(?=(amp\;|lt\;|gt\;|quot\;))")
-# ESCAPE_AND_HTML = re.compile(r"&(?!(amp\;|lt\;|gt\;|quot\;))")
-# HTML_ESCAPE_REPLACE_RE = re.compile(r'[&<>"]')
-
-
-# def escapeHtml(string: str):
-
-#     if HTML_ESCAPE_REPLACE_RE.search(string):
-
-#         string = UNESCAPE_HTML_RE.sub("&", string)
-#         string = ESCAPE_AND_HTML.sub("&amp;", string)
-#         for k, v in {"<": "&lt;", ">": "&gt;", '"': "&quot;"}.items():
-#             string = string.replace(k, v)
-
-#     return string
-
-
 def escapeHtml(raw: str) -> str:
-    # return html.escape(html.unescape(raw)).replace("&#x27;", "'")
-    return html.escape(raw).replace("&#x27;", "'")
+    """Replace special characters "&", "<", ">" and '"' to HTML-safe sequences."""
+    # like html.escape, but without escaping single quotes
+    raw = raw.replace("&", "&amp;")  # Must be done first!
+    raw = raw.replace("<", "&lt;")
+    raw = raw.replace(">", "&gt;")
+    raw = raw.replace('"', "&quot;")
+    return raw
 
 
 # //////////////////////////////////////////////////////////////////////////////
 
 REGEXP_ESCAPE_RE = re.compile(r"[.?*+^$[\]\\(){}|-]")
 
 
@@ -189,25 +155,31 @@
     string = REGEXP_ESCAPE_RE.sub("\\$&", string)
     return string
 
 
 # //////////////////////////////////////////////////////////////////////////////
 
 
-def isSpace(code: object) -> bool:
-    return code in {0x09, 0x20}
+def isSpace(code: int | None) -> bool:
+    """Check if character code is a whitespace."""
+    return code in (0x09, 0x20)
+
+
+def isStrSpace(ch: str | None) -> bool:
+    """Check if character is a whitespace."""
+    return ch in ("\t", " ")
 
 
 MD_WHITESPACE = {
     0x09,  # \t
     0x0A,  # \n
     0x0B,  # \v
     0x0C,  # \f
     0x0D,  # \r
-    0x20,
+    0x20,  # space
     0xA0,
     0x1680,
     0x202F,
     0x205F,
     0x3000,
 }
 
@@ -224,14 +196,15 @@
 UNICODE_PUNCT_RE = re.compile(
     r"[!-#%-\*,-\/:;\?@\[-\]_\{\}\xA1\xA7\xAB\xB6\xB7\xBB\xBF\u037E\u0387\u055A-\u055F\u0589\u058A\u05BE\u05C0\u05C3\u05C6\u05F3\u05F4\u0609\u060A\u060C\u060D\u061B\u061E\u061F\u066A-\u066D\u06D4\u0700-\u070D\u07F7-\u07F9\u0830-\u083E\u085E\u0964\u0965\u0970\u09FD\u0A76\u0AF0\u0C84\u0DF4\u0E4F\u0E5A\u0E5B\u0F04-\u0F12\u0F14\u0F3A-\u0F3D\u0F85\u0FD0-\u0FD4\u0FD9\u0FDA\u104A-\u104F\u10FB\u1360-\u1368\u1400\u166D\u166E\u169B\u169C\u16EB-\u16ED\u1735\u1736\u17D4-\u17D6\u17D8-\u17DA\u1800-\u180A\u1944\u1945\u1A1E\u1A1F\u1AA0-\u1AA6\u1AA8-\u1AAD\u1B5A-\u1B60\u1BFC-\u1BFF\u1C3B-\u1C3F\u1C7E\u1C7F\u1CC0-\u1CC7\u1CD3\u2010-\u2027\u2030-\u2043\u2045-\u2051\u2053-\u205E\u207D\u207E\u208D\u208E\u2308-\u230B\u2329\u232A\u2768-\u2775\u27C5\u27C6\u27E6-\u27EF\u2983-\u2998\u29D8-\u29DB\u29FC\u29FD\u2CF9-\u2CFC\u2CFE\u2CFF\u2D70\u2E00-\u2E2E\u2E30-\u2E4E\u3001-\u3003\u3008-\u3011\u3014-\u301F\u3030\u303D\u30A0\u30FB\uA4FE\uA4FF\uA60D-\uA60F\uA673\uA67E\uA6F2-\uA6F7\uA874-\uA877\uA8CE\uA8CF\uA8F8-\uA8FA\uA8FC\uA92E\uA92F\uA95F\uA9C1-\uA9CD\uA9DE\uA9DF\uAA5C-\uAA5F\uAADE\uAADF\uAAF0\uAAF1\uABEB\uFD3E\uFD3F\uFE10-\uFE19\uFE30-\uFE52\uFE54-\uFE61\uFE63\uFE68\uFE6A\uFE6B\uFF01-\uFF03\uFF05-\uFF0A\uFF0C-\uFF0F\uFF1A\uFF1B\uFF1F\uFF20\uFF3B-\uFF3D\uFF3F\uFF5B\uFF5D\uFF5F-\uFF65]|\uD800[\uDD00-\uDD02\uDF9F\uDFD0]|\uD801\uDD6F|\uD802[\uDC57\uDD1F\uDD3F\uDE50-\uDE58\uDE7F\uDEF0-\uDEF6\uDF39-\uDF3F\uDF99-\uDF9C]|\uD803[\uDF55-\uDF59]|\uD804[\uDC47-\uDC4D\uDCBB\uDCBC\uDCBE-\uDCC1\uDD40-\uDD43\uDD74\uDD75\uDDC5-\uDDC8\uDDCD\uDDDB\uDDDD-\uDDDF\uDE38-\uDE3D\uDEA9]|\uD805[\uDC4B-\uDC4F\uDC5B\uDC5D\uDCC6\uDDC1-\uDDD7\uDE41-\uDE43\uDE60-\uDE6C\uDF3C-\uDF3E]|\uD806[\uDC3B\uDE3F-\uDE46\uDE9A-\uDE9C\uDE9E-\uDEA2]|\uD807[\uDC41-\uDC45\uDC70\uDC71\uDEF7\uDEF8]|\uD809[\uDC70-\uDC74]|\uD81A[\uDE6E\uDE6F\uDEF5\uDF37-\uDF3B\uDF44]|\uD81B[\uDE97-\uDE9A]|\uD82F\uDC9F|\uD836[\uDE87-\uDE8B]|\uD83A[\uDD5E\uDD5F]"  # noqa: E501
 )
 
 
 # Currently without astral characters support.
 def isPunctChar(ch: str) -> bool:
+    """Check if character is a punctuation character."""
     return UNICODE_PUNCT_RE.search(ch) is not None
 
 
 MD_ASCII_PUNCT = {
     0x21,  # /* ! */
     0x22,  # /* " */
     0x23,  # /* # */
@@ -327,7 +300,19 @@
     # is a different step that is not required here.
     #
     # Final result should be uppercased, because it's later stored in an object
     # (this avoid a conflict with Object.prototype members,
     # most notably, `__proto__`)
     #
     return string.lower().upper()
+
+
+LINK_OPEN_RE = re.compile(r"^<a[>\s]", flags=re.IGNORECASE)
+LINK_CLOSE_RE = re.compile(r"^</a\s*>", flags=re.IGNORECASE)
+
+
+def isLinkOpen(string: str) -> bool:
+    return bool(LINK_OPEN_RE.search(string))
+
+
+def isLinkClose(string: str) -> bool:
+    return bool(LINK_CLOSE_RE.search(string))
```

### Comparing `markdown-it-py-2.2.0/markdown_it/helpers/parse_link_destination.py` & `markdown-it-py-3.0.0/markdown_it/helpers/parse_link_destination.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..common.utils import charCodeAt, unescapeAll
 
 
 class _Result:
     __slots__ = ("ok", "pos", "lines", "str")
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.ok = False
         self.pos = 0
         self.lines = 0
         self.str = ""
 
 
 def parseLinkDestination(string: str, pos: int, maximum: int) -> _Result:
@@ -45,15 +45,15 @@
 
     # this should be ... } else { ... branch
 
     level = 0
     while pos < maximum:
         code = charCodeAt(string, pos)
 
-        if code == 0x20:
+        if code is None or code == 0x20:
             break
 
         # ascii control characters
         if code < 0x20 or code == 0x7F:
             break
 
         if code == 0x5C and pos + 1 < maximum:
```

### Comparing `markdown-it-py-2.2.0/markdown_it/helpers/parse_link_label.py` & `markdown-it-py-3.0.0/markdown_it/helpers/parse_link_label.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,24 +13,24 @@
     oldPos = state.pos
     found = False
 
     state.pos = start + 1
     level = 1
 
     while state.pos < state.posMax:
-        marker = state.srcCharCode[state.pos]
-        if marker == 0x5D:  # /* ] */)
+        marker = state.src[state.pos]
+        if marker == "]":
             level -= 1
             if level == 0:
                 found = True
                 break
 
         prevPos = state.pos
         state.md.inline.skipToken(state)
-        if marker == 0x5B:  # /* [ */)
+        if marker == "[":
             if prevPos == state.pos - 1:
                 # increase level if we find text `[`,
                 # which is not a part of any token
                 level += 1
             elif disableNested:
                 state.pos = oldPos
                 return -1
```

### Comparing `markdown-it-py-2.2.0/markdown_it/helpers/parse_link_title.py` & `markdown-it-py-3.0.0/markdown_it/helpers/parse_link_title.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 """
 from ..common.utils import charCodeAt, unescapeAll
 
 
 class _Result:
     __slots__ = ("ok", "pos", "lines", "str")
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.ok = False
         self.pos = 0
         self.lines = 0
         self.str = ""
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.str
 
 
 def parseLinkTitle(string: str, pos: int, maximum: int) -> _Result:
     lines = 0
     start = pos
     result = _Result()
```

### Comparing `markdown-it-py-2.2.0/markdown_it/main.py` & `markdown-it-py-3.0.0/markdown_it/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 from __future__ import annotations
 
 from collections.abc import Callable, Generator, Iterable, Mapping, MutableMapping
 from contextlib import contextmanager
-from typing import Any
+from typing import Any, Literal, overload
 
-from . import helpers, presets  # noqa F401
-from .common import normalize_url, utils  # noqa F401
-from .parser_block import ParserBlock  # noqa F401
-from .parser_core import ParserCore  # noqa F401
-from .parser_inline import ParserInline  # noqa F401
+from . import helpers, presets
+from .common import normalize_url, utils
+from .parser_block import ParserBlock
+from .parser_core import ParserCore
+from .parser_inline import ParserInline
 from .renderer import RendererHTML, RendererProtocol
 from .rules_core.state_core import StateCore
 from .token import Token
-from .utils import OptionsDict
+from .utils import EnvType, OptionsDict, OptionsType, PresetType
 
 try:
     import linkify_it
 except ModuleNotFoundError:
     linkify_it = None
 
 
-_PRESETS = {
+_PRESETS: dict[str, PresetType] = {
     "default": presets.default.make(),
     "js-default": presets.js_default.make(),
     "zero": presets.zero.make(),
     "commonmark": presets.commonmark.make(),
     "gfm-like": presets.gfm_like.make(),
 }
 
 
 class MarkdownIt:
     def __init__(
         self,
-        config: str | Mapping = "commonmark",
-        options_update: Mapping | None = None,
+        config: str | PresetType = "commonmark",
+        options_update: Mapping[str, Any] | None = None,
         *,
         renderer_cls: Callable[[MarkdownIt], RendererProtocol] = RendererHTML,
     ):
         """Main parser class
 
         :param config: name of configuration to load or a pre-defined dictionary
         :param options_update: dictionary that will be merged into ``config["options"]``
         :param renderer_cls: the class to load as the renderer:
             ``self.renderer = renderer_cls(self)
         """
         # add modules
         self.utils = utils
-        self.helpers: Any = helpers
+        self.helpers = helpers
 
         # initialise classes
         self.inline = ParserInline()
         self.block = ParserBlock()
         self.core = ParserCore()
         self.renderer = renderer_cls(self)
         self.linkify = linkify_it.LinkifyIt() if linkify_it else None
@@ -63,34 +63,54 @@
                 "\n(Perhaps you intended this to be the renderer_cls?)"
             )
         self.configure(config, options_update=options_update)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__module__}.{self.__class__.__name__}()"
 
+    @overload
+    def __getitem__(self, name: Literal["inline"]) -> ParserInline:
+        ...
+
+    @overload
+    def __getitem__(self, name: Literal["block"]) -> ParserBlock:
+        ...
+
+    @overload
+    def __getitem__(self, name: Literal["core"]) -> ParserCore:
+        ...
+
+    @overload
+    def __getitem__(self, name: Literal["renderer"]) -> RendererProtocol:
+        ...
+
+    @overload
+    def __getitem__(self, name: str) -> Any:
+        ...
+
     def __getitem__(self, name: str) -> Any:
         return {
             "inline": self.inline,
             "block": self.block,
             "core": self.core,
             "renderer": self.renderer,
         }[name]
 
-    def set(self, options: MutableMapping) -> None:
+    def set(self, options: OptionsType) -> None:
         """Set parser options (in the same format as in constructor).
         Probably, you will never need it, but you can change options after constructor call.
 
         __Note:__ To achieve the best possible performance, don't modify a
         `markdown-it` instance options on the fly. If you need multiple configurations
         it's best to create multiple instances and initialize each with separate config.
         """
         self.options = OptionsDict(options)
 
     def configure(
-        self, presets: str | Mapping, options_update: Mapping | None = None
+        self, presets: str | PresetType, options_update: Mapping[str, Any] | None = None
     ) -> MarkdownIt:
         """Batch load of all options and component settings.
         This is an internal method, and you probably will not need it.
         But if you will - see available presets and data structure
         [here](https://github.com/markdown-it/markdown-it/tree/master/lib/presets)
 
         We strongly recommend to use presets instead of direct config loads.
@@ -104,17 +124,17 @@
             config = presets
 
         if not config:
             raise ValueError("Wrong `markdown-it` config, can't be empty")
 
         options = config.get("options", {}) or {}
         if options_update:
-            options = {**options, **options_update}
+            options = {**options, **options_update}  # type: ignore
 
-        self.set(options)
+        self.set(options)  # type: ignore
 
         if "components" in config:
             for name, component in config["components"].items():
                 rules = component.get("rules", None)
                 if rules:
                     self[name].ruler.enableOnly(rules)
                 rules2 = component.get("rules2", None)
@@ -202,38 +222,42 @@
         chain_rules = self.get_active_rules()
         yield
         for chain, rules in chain_rules.items():
             if chain != "inline2":
                 self[chain].ruler.enableOnly(rules)
         self.inline.ruler2.enableOnly(chain_rules["inline2"])
 
-    def add_render_rule(self, name: str, function: Callable, fmt: str = "html") -> None:
+    def add_render_rule(
+        self, name: str, function: Callable[..., Any], fmt: str = "html"
+    ) -> None:
         """Add a rule for rendering a particular Token type.
 
         Only applied when ``renderer.__output__ == fmt``
         """
         if self.renderer.__output__ == fmt:
             self.renderer.rules[name] = function.__get__(self.renderer)  # type: ignore
 
-    def use(self, plugin: Callable, *params, **options) -> MarkdownIt:
+    def use(
+        self, plugin: Callable[..., None], *params: Any, **options: Any
+    ) -> MarkdownIt:
         """Load specified plugin with given params into current parser instance. (chainable)
 
         It's just a sugar to call `plugin(md, params)` with curring.
 
         Example::
 
             def func(tokens, idx):
                 tokens[idx].content = tokens[idx].content.replace('foo', 'bar')
             md = MarkdownIt().use(plugin, 'foo_replace', 'text', func)
 
         """
         plugin(self, *params, **options)
         return self
 
-    def parse(self, src: str, env: MutableMapping | None = None) -> list[Token]:
+    def parse(self, src: str, env: EnvType | None = None) -> list[Token]:
         """Parse the source string to a token stream
 
         :param src: source string
         :param env: environment sandbox
 
         Parse input string and return list of block tokens (special token type
         "inline" will contain list of inline tokens).
@@ -248,29 +272,29 @@
             raise TypeError(f"Input data should be a MutableMapping, not {type(env)}")
         if not isinstance(src, str):
             raise TypeError(f"Input data should be a string, not {type(src)}")
         state = StateCore(src, self, env)
         self.core.process(state)
         return state.tokens
 
-    def render(self, src: str, env: MutableMapping | None = None) -> Any:
+    def render(self, src: str, env: EnvType | None = None) -> Any:
         """Render markdown string into html. It does all magic for you :).
 
         :param src: source string
         :param env: environment sandbox
         :returns: The output of the loaded renderer
 
         `env` can be used to inject additional metadata (`{}` by default).
         But you will not need it with high probability. See also comment
         in [[MarkdownIt.parse]].
         """
         env = {} if env is None else env
         return self.renderer.render(self.parse(src, env), self.options, env)
 
-    def parseInline(self, src: str, env: MutableMapping | None = None) -> list[Token]:
+    def parseInline(self, src: str, env: EnvType | None = None) -> list[Token]:
         """The same as [[MarkdownIt.parse]] but skip all block rules.
 
         :param src: source string
         :param env: environment sandbox
 
         It returns the
         block tokens list with the single `inline` element, containing parsed inline
@@ -282,15 +306,15 @@
         if not isinstance(src, str):
             raise TypeError(f"Input data should be a string, not {type(src)}")
         state = StateCore(src, self, env)
         state.inlineMode = True
         self.core.process(state)
         return state.tokens
 
-    def renderInline(self, src: str, env: MutableMapping | None = None) -> Any:
+    def renderInline(self, src: str, env: EnvType | None = None) -> Any:
         """Similar to [[MarkdownIt.render]] but for single paragraph content.
 
         :param src: source string
         :param env: environment sandbox
 
         Similar to [[MarkdownIt.render]] but for single paragraph content. Result
         will NOT be wrapped into `<p>` tags.
```

### Comparing `markdown-it-py-2.2.0/markdown_it/parser_block.py` & `markdown-it-py-3.0.0/markdown_it/parser_block.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 """Block-level tokenizer."""
 from __future__ import annotations
 
 import logging
+from typing import TYPE_CHECKING, Callable
 
 from . import rules_block
 from .ruler import Ruler
 from .rules_block.state_block import StateBlock
 from .token import Token
+from .utils import EnvType
+
+if TYPE_CHECKING:
+    from markdown_it import MarkdownIt
 
 LOGGER = logging.getLogger(__name__)
 
 
-_rules: list[tuple] = [
+RuleFuncBlockType = Callable[[StateBlock, int, int, bool], bool]
+"""(state: StateBlock, startLine: int, endLine: int, silent: bool) -> matched: bool)
+
+`silent` disables token generation, useful for lookahead.
+"""
+
+_rules: list[tuple[str, RuleFuncBlockType, list[str]]] = [
     # First 2 params - rule name & source. Secondary array - list of rules,
     # which can be terminated by this one.
     ("table", rules_block.table, ["paragraph", "reference"]),
-    ("code", rules_block.code),
+    ("code", rules_block.code, []),
     ("fence", rules_block.fence, ["paragraph", "reference", "blockquote", "list"]),
     (
         "blockquote",
         rules_block.blockquote,
         ["paragraph", "reference", "blockquote", "list"],
     ),
     ("hr", rules_block.hr, ["paragraph", "reference", "blockquote", "list"]),
     ("list", rules_block.list_block, ["paragraph", "reference", "blockquote"]),
-    ("reference", rules_block.reference),
+    ("reference", rules_block.reference, []),
     ("html_block", rules_block.html_block, ["paragraph", "reference", "blockquote"]),
     ("heading", rules_block.heading, ["paragraph", "reference", "blockquote"]),
-    ("lheading", rules_block.lheading),
-    ("paragraph", rules_block.paragraph),
+    ("lheading", rules_block.lheading, []),
+    ("paragraph", rules_block.paragraph, []),
 ]
 
 
 class ParserBlock:
     """
     ParserBlock#ruler -> Ruler
 
     [[Ruler]] instance. Keep configuration of block rules.
     """
 
-    def __init__(self):
-        self.ruler = Ruler()
-        for data in _rules:
-            name = data[0]
-            rule = data[1]
-            self.ruler.push(name, rule, {"alt": data[2] if len(data) > 2 else []})
-
-    def tokenize(
-        self, state: StateBlock, startLine: int, endLine: int, silent: bool = False
-    ) -> None:
+    def __init__(self) -> None:
+        self.ruler = Ruler[RuleFuncBlockType]()
+        for name, rule, alt in _rules:
+            self.ruler.push(name, rule, {"alt": alt})
+
+    def tokenize(self, state: StateBlock, startLine: int, endLine: int) -> None:
         """Generate tokens for input range."""
         rules = self.ruler.getRules("")
         line = startLine
         maxNesting = state.md.options.maxNesting
         hasEmptyLines = False
 
         while line < endLine:
@@ -90,20 +97,15 @@
 
             if line < endLine and state.isEmpty(line):
                 hasEmptyLines = True
                 line += 1
                 state.line = line
 
     def parse(
-        self,
-        src: str,
-        md,
-        env,
-        outTokens: list[Token],
-        ords: tuple[int, ...] | None = None,
+        self, src: str, md: MarkdownIt, env: EnvType, outTokens: list[Token]
     ) -> list[Token] | None:
         """Process input string and push block tokens into `outTokens`."""
         if not src:
             return None
-        state = StateBlock(src, md, env, outTokens, ords)
+        state = StateBlock(src, md, env, outTokens)
         self.tokenize(state, state.line, state.lineMax)
         return state.tokens
```

### Comparing `markdown-it-py-2.2.0/markdown_it/parser_inline.py` & `markdown-it-py-3.0.0/markdown_it/parser_inline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,67 @@
 """Tokenizes paragraph content.
 """
 from __future__ import annotations
 
+from typing import TYPE_CHECKING, Callable
+
 from . import rules_inline
-from .ruler import RuleFunc, Ruler
+from .ruler import Ruler
 from .rules_inline.state_inline import StateInline
 from .token import Token
+from .utils import EnvType
+
+if TYPE_CHECKING:
+    from markdown_it import MarkdownIt
+
 
 # Parser rules
-_rules: list[tuple[str, RuleFunc]] = [
+RuleFuncInlineType = Callable[[StateInline, bool], bool]
+"""(state: StateInline, silent: bool) -> matched: bool)
+
+`silent` disables token generation, useful for lookahead.
+"""
+_rules: list[tuple[str, RuleFuncInlineType]] = [
     ("text", rules_inline.text),
+    ("linkify", rules_inline.linkify),
     ("newline", rules_inline.newline),
     ("escape", rules_inline.escape),
     ("backticks", rules_inline.backtick),
     ("strikethrough", rules_inline.strikethrough.tokenize),
     ("emphasis", rules_inline.emphasis.tokenize),
     ("link", rules_inline.link),
     ("image", rules_inline.image),
     ("autolink", rules_inline.autolink),
     ("html_inline", rules_inline.html_inline),
     ("entity", rules_inline.entity),
 ]
 
-_rules2: list[tuple[str, RuleFunc]] = [
+# Note `rule2` ruleset was created specifically for emphasis/strikethrough
+# post-processing and may be changed in the future.
+#
+# Don't use this for anything except pairs (plugins working with `balance_pairs`).
+#
+RuleFuncInline2Type = Callable[[StateInline], None]
+_rules2: list[tuple[str, RuleFuncInline2Type]] = [
     ("balance_pairs", rules_inline.link_pairs),
     ("strikethrough", rules_inline.strikethrough.postProcess),
     ("emphasis", rules_inline.emphasis.postProcess),
-    ("text_collapse", rules_inline.text_collapse),
+    # rules for pairs separate '**' into its own text tokens, which may be left unused,
+    # rule below merges unused segments back with the rest of the text
+    ("fragments_join", rules_inline.fragments_join),
 ]
 
 
 class ParserInline:
-    def __init__(self):
-        self.ruler = Ruler()
+    def __init__(self) -> None:
+        self.ruler = Ruler[RuleFuncInlineType]()
         for name, rule in _rules:
             self.ruler.push(name, rule)
         # Second ruler used for post-processing (e.g. in emphasis-like rules)
-        self.ruler2 = Ruler()
+        self.ruler2 = Ruler[RuleFuncInline2Type]()
         for name, rule2 in _rules2:
             self.ruler2.push(name, rule2)
 
     def skipToken(self, state: StateInline) -> None:
         """Skip single token by running all rules in validation mode;
         returns `True` if any rule reported success
         """
@@ -110,15 +131,17 @@
 
             state.pending += state.src[state.pos]
             state.pos += 1
 
         if state.pending:
             state.pushPending()
 
-    def parse(self, src: str, md, env, tokens: list[Token]) -> list[Token]:
+    def parse(
+        self, src: str, md: MarkdownIt, env: EnvType, tokens: list[Token]
+    ) -> list[Token]:
         """Process input string and push inline tokens into `tokens`"""
         state = StateInline(src, md, env, tokens)
         self.tokenize(state)
         rules2 = self.ruler2.getRules("")
         for rule in rules2:
             rule(state)
         return state.tokens
```

### Comparing `markdown-it-py-2.2.0/markdown_it/port.yaml` & `markdown-it-py-3.0.0/markdown_it/port.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 - package: markdown-it/markdown-it
-  version: 12.2.0
-  commit: 6e2de08a0b03d3d0dcc524b89710ce05f83a0283
-  date: Aug 2, 2021
+  version: 13.0.1
+  commit: e843acc9edad115cbf8cf85e676443f01658be08
+  date: May 3, 2022
   notes:
     - Rename variables that use python built-in names, e.g.
       - `max` -> `maximum`
       - `len` -> `length`
       - `str` -> `string`
     - |
       Convert JS `for` loops to `while` loops
@@ -19,16 +19,15 @@
       `Token.attrs` is a dictionary, instead of a list of lists.
       Upstream the list format is only used to guarantee order: https://github.com/markdown-it/markdown-it/issues/142,
       but in Python 3.7+ order of dictionaries is guaranteed.
       One should anyhow use the `attrGet`, `attrSet`, `attrPush` and `attrJoin` methods
       to manipulate `Token.attrs`, which have an identical signature to those upstream.
     - Use python version of `charCodeAt`
     - |
-      Reduce use of charCodeAt() by storing char codes in a srcCharCodes attribute for state
-      objects and sharing those whenever possible
+      Use `str` units instead of `int`s to represent Unicode codepoints.
       This provides a significant performance boost
     - |
       In markdown_it/rules_block/reference.py,
       record line range in state.env["references"] and add state.env["duplicate_refs"]
       This is to allow renderers to report on issues regarding references
     - |
       The `MarkdownIt.__init__` signature is slightly different for updating options,
```

### Comparing `markdown-it-py-2.2.0/markdown_it/presets/commonmark.py` & `markdown-it-py-3.0.0/markdown_it/presets/commonmark.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 This differs to presets.default,
 primarily in that it allows HTML and does not enable components:
 
 - block: table
 - inline: strikethrough
 """
+from ..utils import PresetType
 
 
-def make():
+def make() -> PresetType:
     return {
         "options": {
             "maxNesting": 20,  # Internal protection, recursion limit
             "html": True,  # Enable HTML tags in source,
             # this is just a shorthand for .enable(["html_inline", "html_block"])
             # used by the linkify rule:
             "linkify": False,  # autoconvert URL-like texts to links
@@ -35,15 +36,15 @@
             # If result starts with <pre... internal wrapper is skipped.
             #
             # function (/*str, lang, attrs*/) { return ''; }
             #
             "highlight": None,
         },
         "components": {
-            "core": {"rules": ["normalize", "block", "inline"]},
+            "core": {"rules": ["normalize", "block", "inline", "text_join"]},
             "block": {
                 "rules": [
                     "blockquote",
                     "code",
                     "fence",
                     "heading",
                     "hr",
@@ -63,11 +64,11 @@
                     "escape",
                     "html_inline",
                     "image",
                     "link",
                     "newline",
                     "text",
                 ],
-                "rules2": ["balance_pairs", "emphasis", "text_collapse"],
+                "rules2": ["balance_pairs", "emphasis", "fragments_join"],
             },
         },
     }
```

### Comparing `markdown-it-py-2.2.0/markdown_it/presets/default.py` & `markdown-it-py-3.0.0/markdown_it/presets/default.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """markdown-it default options."""
+from ..utils import PresetType
 
 
-def make():
+def make() -> PresetType:
     return {
         "options": {
             "maxNesting": 100,  # Internal protection, recursion limit
             "html": False,  # Enable HTML tags in source
             # this is just a shorthand for .disable(["html_inline", "html_block"])
             # used by the linkify rule:
             "linkify": False,  # autoconvert URL-like texts to links
```

### Comparing `markdown-it-py-2.2.0/markdown_it/presets/zero.py` & `markdown-it-py-3.0.0/markdown_it/presets/zero.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 "Zero" preset, with nothing enabled. Useful for manual configuring of simple
 modes. For example, to parse bold/italic only.
 """
+from ..utils import PresetType
 
 
-def make():
+def make() -> PresetType:
     return {
         "options": {
             "maxNesting": 20,  # Internal protection, recursion limit
             "html": False,  # Enable HTML tags in source
             # this is just a shorthand for .disable(["html_inline", "html_block"])
             # used by the linkify rule:
             "linkify": False,  # autoconvert URL-like texts to links
@@ -28,12 +29,15 @@
             # Highlighter function. Should return escaped HTML,
             # or '' if the source string is not changed and should be escaped externally.
             # If result starts with <pre... internal wrapper is skipped.
             # function (/*str, lang, attrs*/) { return ''; }
             "highlight": None,
         },
         "components": {
-            "core": {"rules": ["normalize", "block", "inline"]},
+            "core": {"rules": ["normalize", "block", "inline", "text_join"]},
             "block": {"rules": ["paragraph"]},
-            "inline": {"rules": ["text"], "rules2": ["balance_pairs", "text_collapse"]},
+            "inline": {
+                "rules": ["text"],
+                "rules2": ["balance_pairs", "fragments_join"],
+            },
         },
     }
```

### Comparing `markdown-it-py-2.2.0/markdown_it/renderer.py` & `markdown-it-py-3.0.0/markdown_it/renderer.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,33 +3,28 @@
 
 Generates HTML from parsed token stream. Each instance has independent
 copy of rules. Those can be rewritten with ease. Also, you can add new
 rules if you create plugin and adds new token types.
 """
 from __future__ import annotations
 
-from collections.abc import MutableMapping, Sequence
+from collections.abc import Sequence
 import inspect
-from typing import Any, ClassVar
+from typing import Any, ClassVar, Protocol
 
 from .common.utils import escapeHtml, unescapeAll
 from .token import Token
-from .utils import OptionsDict
-
-try:
-    from typing import Protocol
-except ImportError:  # Python <3.8 doesn't have `Protocol` in the stdlib
-    from typing_extensions import Protocol  # type: ignore
+from .utils import EnvType, OptionsDict
 
 
 class RendererProtocol(Protocol):
     __output__: ClassVar[str]
 
     def render(
-        self, tokens: Sequence[Token], options: OptionsDict, env: MutableMapping
+        self, tokens: Sequence[Token], options: OptionsDict, env: EnvType
     ) -> Any:
         ...
 
 
 class RendererHTML(RendererProtocol):
     """Contains render rules for tokens. Can be updated and extended.
 
@@ -58,23 +53,23 @@
 
     See https://github.com/markdown-it/markdown-it/blob/master/lib/renderer.js
     for more details and examples.
     """
 
     __output__ = "html"
 
-    def __init__(self, parser=None):
+    def __init__(self, parser: Any = None):
         self.rules = {
             k: v
             for k, v in inspect.getmembers(self, predicate=inspect.ismethod)
             if not (k.startswith("render") or k.startswith("_"))
         }
 
     def render(
-        self, tokens: Sequence[Token], options: OptionsDict, env: MutableMapping
+        self, tokens: Sequence[Token], options: OptionsDict, env: EnvType
     ) -> str:
         """Takes token stream and generates HTML.
 
         :param tokens: list on block tokens to render
         :param options: params of parser instance
         :param env: additional data from parsed input
 
@@ -89,15 +84,15 @@
                 result += self.rules[token.type](tokens, i, options, env)
             else:
                 result += self.renderToken(tokens, i, options, env)
 
         return result
 
     def renderInline(
-        self, tokens: Sequence[Token], options: OptionsDict, env: MutableMapping
+        self, tokens: Sequence[Token], options: OptionsDict, env: EnvType
     ) -> str:
         """The same as ``render``, but for single token of `inline` type.
 
         :param tokens: list on block tokens to render
         :param options: params of parser instance
         :param env: additional data from parsed input (references, for example)
         """
@@ -112,15 +107,15 @@
         return result
 
     def renderToken(
         self,
         tokens: Sequence[Token],
         idx: int,
         options: OptionsDict,
-        env: MutableMapping,
+        env: EnvType,
     ) -> str:
         """Default token renderer.
 
         Can be overridden by custom function
 
         :param idx: token index to render
         :param options: params of parser instance
@@ -153,27 +148,26 @@
         if token.nesting == 0 and options["xhtmlOut"]:
             result += " /"
 
         # Check if we need to add a newline after this tag
         if token.block:
             needLf = True
 
-            if token.nesting == 1:
-                if idx + 1 < len(tokens):
-                    nextToken = tokens[idx + 1]
-
-                    if nextToken.type == "inline" or nextToken.hidden:
-                        # Block-level tag containing an inline tag.
-                        #
-                        needLf = False
-
-                    elif nextToken.nesting == -1 and nextToken.tag == token.tag:
-                        # Opening tag + closing tag of the same type. E.g. `<li></li>`.
-                        #
-                        needLf = False
+            if token.nesting == 1 and (idx + 1 < len(tokens)):
+                nextToken = tokens[idx + 1]
+
+                if nextToken.type == "inline" or nextToken.hidden:  # noqa: SIM114
+                    # Block-level tag containing an inline tag.
+                    #
+                    needLf = False
+
+                elif nextToken.nesting == -1 and nextToken.tag == token.tag:
+                    # Opening tag + closing tag of the same type. E.g. `<li></li>`.
+                    #
+                    needLf = False
 
         result += ">\n" if needLf else ">"
 
         return result
 
     @staticmethod
     def renderAttrs(token: Token) -> str:
@@ -185,15 +179,15 @@
 
         return result
 
     def renderInlineAsText(
         self,
         tokens: Sequence[Token] | None,
         options: OptionsDict,
-        env: MutableMapping,
+        env: EnvType,
     ) -> str:
         """Special kludge for image `alt` attributes to conform CommonMark spec.
 
         Don't try to use it! Spec requires to show `alt` content with stripped markup,
         instead of simple escaping.
 
         :param tokens: list on block tokens to render
@@ -211,30 +205,32 @@
             elif token.type == "softbreak":
                 result += "\n"
 
         return result
 
     ###################################################
 
-    def code_inline(self, tokens: Sequence[Token], idx: int, options, env) -> str:
+    def code_inline(
+        self, tokens: Sequence[Token], idx: int, options: OptionsDict, env: EnvType
+    ) -> str:
         token = tokens[idx]
         return (
             "<code"
             + self.renderAttrs(token)
             + ">"
             + escapeHtml(tokens[idx].content)
             + "</code>"
         )
 
     def code_block(
         self,
         tokens: Sequence[Token],
         idx: int,
         options: OptionsDict,
-        env: MutableMapping,
+        env: EnvType,
     ) -> str:
         token = tokens[idx]
 
         return (
             "<pre"
             + self.renderAttrs(token)
             + "><code>"
@@ -243,15 +239,15 @@
         )
 
     def fence(
         self,
         tokens: Sequence[Token],
         idx: int,
         options: OptionsDict,
-        env: MutableMapping,
+        env: EnvType,
     ) -> str:
         token = tokens[idx]
         info = unescapeAll(token.info).strip() if token.info else ""
         langName = ""
         langAttrs = ""
 
         if info:
@@ -295,40 +291,46 @@
         )
 
     def image(
         self,
         tokens: Sequence[Token],
         idx: int,
         options: OptionsDict,
-        env: MutableMapping,
+        env: EnvType,
     ) -> str:
         token = tokens[idx]
 
         # "alt" attr MUST be set, even if empty. Because it's mandatory and
         # should be placed on proper position for tests.
         if token.children:
             token.attrSet("alt", self.renderInlineAsText(token.children, options, env))
         else:
             token.attrSet("alt", "")
 
         return self.renderToken(tokens, idx, options, env)
 
     def hardbreak(
-        self, tokens: Sequence[Token], idx: int, options: OptionsDict, *args
+        self, tokens: Sequence[Token], idx: int, options: OptionsDict, env: EnvType
     ) -> str:
         return "<br />\n" if options.xhtmlOut else "<br>\n"
 
     def softbreak(
-        self, tokens: Sequence[Token], idx: int, options: OptionsDict, *args
+        self, tokens: Sequence[Token], idx: int, options: OptionsDict, env: EnvType
     ) -> str:
         return (
             ("<br />\n" if options.xhtmlOut else "<br>\n") if options.breaks else "\n"
         )
 
-    def text(self, tokens: Sequence[Token], idx: int, *args) -> str:
+    def text(
+        self, tokens: Sequence[Token], idx: int, options: OptionsDict, env: EnvType
+    ) -> str:
         return escapeHtml(tokens[idx].content)
 
-    def html_block(self, tokens: Sequence[Token], idx: int, *args) -> str:
+    def html_block(
+        self, tokens: Sequence[Token], idx: int, options: OptionsDict, env: EnvType
+    ) -> str:
         return tokens[idx].content
 
-    def html_inline(self, tokens: Sequence[Token], idx: int, *args) -> str:
+    def html_inline(
+        self, tokens: Sequence[Token], idx: int, options: OptionsDict, env: EnvType
+    ) -> str:
         return tokens[idx].content
```

### Comparing `markdown-it-py-2.2.0/markdown_it/ruler.py` & `markdown-it-py-3.0.0/markdown_it/ruler.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,65 +13,78 @@
 
 You will not need use this class directly until write plugins. For simple
 rules control use [[MarkdownIt.disable]], [[MarkdownIt.enable]] and
 [[MarkdownIt.use]].
 """
 from __future__ import annotations
 
-from collections.abc import Callable, Iterable, MutableMapping
+from collections.abc import Iterable
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Generic, TypedDict, TypeVar
+import warnings
 
 from markdown_it._compat import DATACLASS_KWARGS
 
+from .utils import EnvType
+
 if TYPE_CHECKING:
     from markdown_it import MarkdownIt
 
 
 class StateBase:
-    srcCharCode: tuple[int, ...]
-
-    def __init__(self, src: str, md: MarkdownIt, env: MutableMapping):
+    def __init__(self, src: str, md: MarkdownIt, env: EnvType):
         self.src = src
         self.env = env
         self.md = md
 
     @property
     def src(self) -> str:
         return self._src
 
     @src.setter
     def src(self, value: str) -> None:
         self._src = value
-        self.srcCharCode = tuple(ord(c) for c in self.src)
+        self._srcCharCode: tuple[int, ...] | None = None
+
+    @property
+    def srcCharCode(self) -> tuple[int, ...]:
+        warnings.warn(
+            "StateBase.srcCharCode is deprecated. Use StateBase.src instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        if self._srcCharCode is None:
+            self._srcCharCode = tuple(ord(c) for c in self._src)
+        return self._srcCharCode
+
+
+class RuleOptionsType(TypedDict, total=False):
+    alt: list[str]
 
 
-# The first positional arg is always a subtype of `StateBase`. Other
-# arguments may or may not exist, based on the rule's type (block,
-# core, inline). Return type is either `None` or `bool` based on the
-# rule's type.
-RuleFunc = Callable
+RuleFuncTv = TypeVar("RuleFuncTv")
+"""A rule function, whose signature is dependent on the state type."""
 
 
 @dataclass(**DATACLASS_KWARGS)
-class Rule:
+class Rule(Generic[RuleFuncTv]):
     name: str
     enabled: bool
-    fn: RuleFunc = field(repr=False)
+    fn: RuleFuncTv = field(repr=False)
     alt: list[str]
 
 
-class Ruler:
-    def __init__(self):
+class Ruler(Generic[RuleFuncTv]):
+    def __init__(self) -> None:
         # List of added rules.
-        self.__rules__: list[Rule] = []
+        self.__rules__: list[Rule[RuleFuncTv]] = []
         # Cached rule chains.
         # First level - chain name, '' for default.
         # Second level - diginal anchor for fast filtering by charcodes.
-        self.__cache__: dict[str, list[RuleFunc]] | None = None
+        self.__cache__: dict[str, list[RuleFuncTv]] | None = None
 
     def __find__(self, name: str) -> int:
         """Find rule index by name"""
         for i, rule in enumerate(self.__rules__):
             if rule.name == name:
                 return i
         return -1
@@ -91,15 +104,17 @@
             for rule in self.__rules__:
                 if not rule.enabled:
                     continue
                 if chain and (chain not in rule.alt):
                     continue
                 self.__cache__[chain].append(rule.fn)
 
-    def at(self, ruleName: str, fn: RuleFunc, options=None):
+    def at(
+        self, ruleName: str, fn: RuleFuncTv, options: RuleOptionsType | None = None
+    ) -> None:
         """Replace rule by name with new function & options.
 
         :param ruleName: rule name to replace.
         :param fn: new rule function.
         :param options: new rule options (not mandatory).
         :raises: KeyError if name not found
         """
@@ -107,96 +122,120 @@
         options = options or {}
         if index == -1:
             raise KeyError(f"Parser rule not found: {ruleName}")
         self.__rules__[index].fn = fn
         self.__rules__[index].alt = options.get("alt", [])
         self.__cache__ = None
 
-    def before(self, beforeName: str, ruleName: str, fn: RuleFunc, options=None):
+    def before(
+        self,
+        beforeName: str,
+        ruleName: str,
+        fn: RuleFuncTv,
+        options: RuleOptionsType | None = None,
+    ) -> None:
         """Add new rule to chain before one with given name.
 
         :param beforeName: new rule will be added before this one.
         :param ruleName: new rule will be added before this one.
         :param fn: new rule function.
         :param options: new rule options (not mandatory).
         :raises: KeyError if name not found
         """
         index = self.__find__(beforeName)
         options = options or {}
         if index == -1:
             raise KeyError(f"Parser rule not found: {beforeName}")
-        self.__rules__.insert(index, Rule(ruleName, True, fn, options.get("alt", [])))
+        self.__rules__.insert(
+            index, Rule[RuleFuncTv](ruleName, True, fn, options.get("alt", []))
+        )
         self.__cache__ = None
 
-    def after(self, afterName: str, ruleName: str, fn: RuleFunc, options=None):
+    def after(
+        self,
+        afterName: str,
+        ruleName: str,
+        fn: RuleFuncTv,
+        options: RuleOptionsType | None = None,
+    ) -> None:
         """Add new rule to chain after one with given name.
 
         :param afterName: new rule will be added after this one.
         :param ruleName: new rule will be added after this one.
         :param fn: new rule function.
         :param options: new rule options (not mandatory).
         :raises: KeyError if name not found
         """
         index = self.__find__(afterName)
         options = options or {}
         if index == -1:
             raise KeyError(f"Parser rule not found: {afterName}")
         self.__rules__.insert(
-            index + 1, Rule(ruleName, True, fn, options.get("alt", []))
+            index + 1, Rule[RuleFuncTv](ruleName, True, fn, options.get("alt", []))
         )
         self.__cache__ = None
 
-    def push(self, ruleName: str, fn: RuleFunc, options=None):
+    def push(
+        self, ruleName: str, fn: RuleFuncTv, options: RuleOptionsType | None = None
+    ) -> None:
         """Push new rule to the end of chain.
 
         :param ruleName: new rule will be added to the end of chain.
         :param fn: new rule function.
         :param options: new rule options (not mandatory).
 
         """
-        self.__rules__.append(Rule(ruleName, True, fn, (options or {}).get("alt", [])))
+        self.__rules__.append(
+            Rule[RuleFuncTv](ruleName, True, fn, (options or {}).get("alt", []))
+        )
         self.__cache__ = None
 
-    def enable(self, names: str | Iterable[str], ignoreInvalid: bool = False):
+    def enable(
+        self, names: str | Iterable[str], ignoreInvalid: bool = False
+    ) -> list[str]:
         """Enable rules with given names.
 
         :param names: name or list of rule names to enable.
         :param ignoreInvalid: ignore errors when rule not found
         :raises: KeyError if name not found and not ignoreInvalid
         :return: list of found rule names
         """
         if isinstance(names, str):
             names = [names]
-        result = []
+        result: list[str] = []
         for name in names:
             idx = self.__find__(name)
             if (idx < 0) and ignoreInvalid:
                 continue
             if (idx < 0) and not ignoreInvalid:
                 raise KeyError(f"Rules manager: invalid rule name {name}")
             self.__rules__[idx].enabled = True
             result.append(name)
         self.__cache__ = None
         return result
 
-    def enableOnly(self, names: str | Iterable[str], ignoreInvalid: bool = False):
+    def enableOnly(
+        self, names: str | Iterable[str], ignoreInvalid: bool = False
+    ) -> list[str]:
         """Enable rules with given names, and disable everything else.
 
         :param names: name or list of rule names to enable.
         :param ignoreInvalid: ignore errors when rule not found
         :raises: KeyError if name not found and not ignoreInvalid
         :return: list of found rule names
         """
         if isinstance(names, str):
             names = [names]
         for rule in self.__rules__:
             rule.enabled = False
-        self.enable(names, ignoreInvalid)
+        return self.enable(names, ignoreInvalid)
 
-    def disable(self, names: str | Iterable[str], ignoreInvalid: bool = False):
+    def disable(
+        self, names: str | Iterable[str], ignoreInvalid: bool = False
+    ) -> list[str]:
         """Disable rules with given names.
 
         :param names: name or list of rule names to enable.
         :param ignoreInvalid: ignore errors when rule not found
         :raises: KeyError if name not found and not ignoreInvalid
         :return: list of found rule names
         """
@@ -210,15 +249,15 @@
             if (idx < 0) and not ignoreInvalid:
                 raise KeyError(f"Rules manager: invalid rule name {name}")
             self.__rules__[idx].enabled = False
             result.append(name)
         self.__cache__ = None
         return result
 
-    def getRules(self, chainName: str) -> list[RuleFunc]:
+    def getRules(self, chainName: str = "") -> list[RuleFuncTv]:
         """Return array of active functions (rules) for given chain name.
         It analyzes rules configuration, compiles caches if not exists and returns result.
 
         Default chain name is `''` (empty string). It can't be skipped.
         That's done intentionally, to keep signature monomorphic for high speed.
 
         """
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_block/__init__.py` & `markdown-it-py-3.0.0/markdown_it/rules_block/__init__.py`

 * *Files identical despite different names*

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_block/blockquote.py` & `markdown-it-py-3.0.0/markdown_it/rules_block/blockquote.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 # Block quotes
 from __future__ import annotations
 
 import logging
 
-from ..common.utils import isSpace
+from ..common.utils import isStrSpace
 from .state_block import StateBlock
 
 LOGGER = logging.getLogger(__name__)
 
 
-def blockquote(state: StateBlock, startLine: int, endLine: int, silent: bool):
+def blockquote(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
     LOGGER.debug(
         "entering blockquote: %s, %s, %s, %s", state, startLine, endLine, silent
     )
 
     oldLineMax = state.lineMax
     pos = state.bMarks[startLine] + state.tShift[startLine]
     max = state.eMarks[startLine]
 
-    # if it's indented more than 3 spaces, it should be a code block
-    if (state.sCount[startLine] - state.blkIndent) >= 4:
+    if state.is_code_block(startLine):
         return False
 
     # check the block quote marker
-    if state.srcCharCode[pos] != 0x3E:  # /* > */
+    try:
+        if state.src[pos] != ">":
+            return False
+    except IndexError:
         return False
     pos += 1
 
     # we know that it's going to be a valid blockquote,
     # so no point trying to find the end of it in silent mode
     if silent:
         return True
 
     # set offset past spaces and ">"
     initial = offset = state.sCount[startLine] + 1
 
     try:
-        second_char_code: int | None = state.srcCharCode[pos]
+        second_char: str | None = state.src[pos]
     except IndexError:
-        second_char_code = None
+        second_char = None
 
     # skip one optional space after '>'
-    if second_char_code == 0x20:  # /* space */
+    if second_char == " ":
         # ' >   test '
         #     ^ -- position start of line here:
         pos += 1
         initial += 1
         offset += 1
         adjustTab = False
         spaceAfterMarker = True
-    elif second_char_code == 0x09:  # /* tab */
+    elif second_char == "\t":
         spaceAfterMarker = True
 
         if (state.bsCount[startLine] + offset) % 4 == 3:
             # '  >\t  test '
             #       ^ -- position start of line here (tab has width==1)
             pos += 1
             initial += 1
@@ -68,18 +70,18 @@
     else:
         spaceAfterMarker = False
 
     oldBMarks = [state.bMarks[startLine]]
     state.bMarks[startLine] = pos
 
     while pos < max:
-        ch = state.srcCharCode[pos]
+        ch = state.src[pos]
 
-        if isSpace(ch):
-            if ch == 0x09:  # / tab /
+        if isStrSpace(ch):
+            if ch == "\t":
                 offset += (
                     4
                     - (offset + state.bsCount[startLine] + (1 if adjustTab else 0)) % 4
                 )
             else:
                 offset += 1
 
@@ -141,37 +143,37 @@
         pos = state.bMarks[nextLine] + state.tShift[nextLine]
         max = state.eMarks[nextLine]
 
         if pos >= max:
             # Case 1: line is not inside the blockquote, and this line is empty.
             break
 
-        evaluatesTrue = state.srcCharCode[pos] == 0x3E and not isOutdented  # /* > */
+        evaluatesTrue = state.src[pos] == ">" and not isOutdented
         pos += 1
         if evaluatesTrue:
             # This line is inside the blockquote.
 
             # set offset past spaces and ">"
             initial = offset = state.sCount[nextLine] + 1
 
             try:
-                next_char: int | None = state.srcCharCode[pos]
+                next_char: str | None = state.src[pos]
             except IndexError:
                 next_char = None
 
             # skip one optional space after '>'
-            if next_char == 0x20:  # /* space */
+            if next_char == " ":
                 # ' >   test '
                 #     ^ -- position start of line here:
                 pos += 1
                 initial += 1
                 offset += 1
                 adjustTab = False
                 spaceAfterMarker = True
-            elif next_char == 0x09:  # /* tab */
+            elif next_char == "\t":
                 spaceAfterMarker = True
 
                 if (state.bsCount[nextLine] + offset) % 4 == 3:
                     # '  >\t  test '
                     #       ^ -- position start of line here (tab has width==1)
                     pos += 1
                     initial += 1
@@ -186,18 +188,18 @@
             else:
                 spaceAfterMarker = False
 
             oldBMarks.append(state.bMarks[nextLine])
             state.bMarks[nextLine] = pos
 
             while pos < max:
-                ch = state.srcCharCode[pos]
+                ch = state.src[pos]
 
-                if isSpace(ch):
-                    if ch == 0x09:
+                if isStrSpace(ch):
+                    if ch == "\t":
                         offset += (
                             4
                             - (
                                 offset
                                 + state.bsCount[nextLine]
                                 + (1 if adjustTab else 0)
                             )
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_block/code.py` & `markdown-it-py-3.0.0/markdown_it/rules_block/code.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 import logging
 
 from .state_block import StateBlock
 
 LOGGER = logging.getLogger(__name__)
 
 
-def code(state: StateBlock, startLine: int, endLine: int, silent: bool = False):
+def code(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
     LOGGER.debug("entering code: %s, %s, %s, %s", state, startLine, endLine, silent)
 
-    if state.sCount[startLine] - state.blkIndent < 4:
+    if not state.is_code_block(startLine):
         return False
 
     last = nextLine = startLine + 1
 
     while nextLine < endLine:
         if state.isEmpty(nextLine):
             nextLine += 1
             continue
 
-        if state.sCount[nextLine] - state.blkIndent >= 4:
+        if state.is_code_block(nextLine):
             nextLine += 1
             last = nextLine
             continue
 
         break
 
     state.line = last
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_block/fence.py` & `markdown-it-py-3.0.0/markdown_it/rules_block/fence.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,50 +2,46 @@
 import logging
 
 from .state_block import StateBlock
 
 LOGGER = logging.getLogger(__name__)
 
 
-def fence(state: StateBlock, startLine: int, endLine: int, silent: bool):
+def fence(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
     LOGGER.debug("entering fence: %s, %s, %s, %s", state, startLine, endLine, silent)
 
     haveEndMarker = False
     pos = state.bMarks[startLine] + state.tShift[startLine]
     maximum = state.eMarks[startLine]
 
-    # if it's indented more than 3 spaces, it should be a code block
-    if state.sCount[startLine] - state.blkIndent >= 4:
+    if state.is_code_block(startLine):
         return False
 
     if pos + 3 > maximum:
         return False
 
-    marker = state.srcCharCode[pos]
+    marker = state.src[pos]
 
-    # /* ~ */  /* ` */
-    if marker != 0x7E and marker != 0x60:
+    if marker not in ("~", "`"):
         return False
 
     # scan marker length
     mem = pos
-    pos = state.skipChars(pos, marker)
+    pos = state.skipCharsStr(pos, marker)
 
     length = pos - mem
 
     if length < 3:
         return False
 
     markup = state.src[mem:pos]
     params = state.src[pos:maximum]
 
-    # /* ` */
-    if marker == 0x60:
-        if chr(marker) in params:
-            return False
+    if marker == "`" and marker in params:
+        return False
 
     # Since start is found, we can report success here in validation mode
     if silent:
         return True
 
     # search end of block
     nextLine = startLine
@@ -62,22 +58,24 @@
 
         if pos < maximum and state.sCount[nextLine] < state.blkIndent:
             # non-empty line with negative indent should stop the list:
             # - ```
             #  test
             break
 
-        if state.srcCharCode[pos] != marker:
-            continue
+        try:
+            if state.src[pos] != marker:
+                continue
+        except IndexError:
+            break
 
-        if state.sCount[nextLine] - state.blkIndent >= 4:
-            # closing fence should be indented less than 4 spaces
+        if state.is_code_block(nextLine):
             continue
 
-        pos = state.skipChars(pos, marker)
+        pos = state.skipCharsStr(pos, marker)
 
         # closing code fence must be at least as long as the opening one
         if pos - mem < length:
             continue
 
         # make sure tail has spaces only
         pos = state.skipSpaces(pos)
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_block/heading.py` & `markdown-it-py-3.0.0/markdown_it/rules_block/heading.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,58 @@
 """ Atex heading (#, ##, ...) """
 from __future__ import annotations
 
 import logging
 
-from ..common.utils import isSpace
+from ..common.utils import isStrSpace
 from .state_block import StateBlock
 
 LOGGER = logging.getLogger(__name__)
 
 
-def heading(state: StateBlock, startLine: int, endLine: int, silent: bool):
+def heading(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
     LOGGER.debug("entering heading: %s, %s, %s, %s", state, startLine, endLine, silent)
 
     pos = state.bMarks[startLine] + state.tShift[startLine]
     maximum = state.eMarks[startLine]
 
-    # if it's indented more than 3 spaces, it should be a code block
-    if state.sCount[startLine] - state.blkIndent >= 4:
+    if state.is_code_block(startLine):
         return False
 
-    ch: int | None = state.srcCharCode[pos]
+    ch: str | None = state.src[pos]
 
-    # /* # */
-    if ch != 0x23 or pos >= maximum:
+    if ch != "#" or pos >= maximum:
         return False
 
     # count heading level
     level = 1
     pos += 1
     try:
-        ch = state.srcCharCode[pos]
+        ch = state.src[pos]
     except IndexError:
         ch = None
-    # /* # */
-    while ch == 0x23 and pos < maximum and level <= 6:
+    while ch == "#" and pos < maximum and level <= 6:
         level += 1
         pos += 1
         try:
-            ch = state.srcCharCode[pos]
+            ch = state.src[pos]
         except IndexError:
             ch = None
 
-    if level > 6 or (pos < maximum and not isSpace(ch)):
+    if level > 6 or (pos < maximum and not isStrSpace(ch)):
         return False
 
     if silent:
         return True
 
     # Let's cut tails like '    ###  ' from the end of string
 
     maximum = state.skipSpacesBack(maximum, pos)
-    tmp = state.skipCharsBack(maximum, 0x23, pos)  # #
-    if tmp > pos and isSpace(state.srcCharCode[tmp - 1]):
+    tmp = state.skipCharsStrBack(maximum, "#", pos)
+    if tmp > pos and isStrSpace(state.src[tmp - 1]):
         maximum = tmp
 
     state.line = startLine + 1
 
     token = state.push("heading_open", "h" + str(level), 1)
     token.markup = "########"[:level]
     token.map = [startLine, state.line]
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_block/hr.py` & `markdown-it-py-3.0.0/markdown_it/rules_block/hr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 """Horizontal rule
 
 At least 3 of these characters on a line * - _
 """
 import logging
 
-from ..common.utils import isSpace
+from ..common.utils import isStrSpace
 from .state_block import StateBlock
 
 LOGGER = logging.getLogger(__name__)
 
 
-def hr(state: StateBlock, startLine: int, endLine: int, silent: bool):
+def hr(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
     LOGGER.debug("entering hr: %s, %s, %s, %s", state, startLine, endLine, silent)
 
     pos = state.bMarks[startLine] + state.tShift[startLine]
     maximum = state.eMarks[startLine]
 
-    # if it's indented more than 3 spaces, it should be a code block
-    if state.sCount[startLine] - state.blkIndent >= 4:
+    if state.is_code_block(startLine):
         return False
 
-    marker = state.srcCharCode[pos]
+    try:
+        marker = state.src[pos]
+    except IndexError:
+        return False
     pos += 1
 
-    # Check hr marker: /* * */ /* - */ /* _ */
-    if marker != 0x2A and marker != 0x2D and marker != 0x5F:
+    # Check hr marker
+    if marker not in ("*", "-", "_"):
         return False
 
     # markers can be mixed with spaces, but there should be at least 3 of them
 
     cnt = 1
     while pos < maximum:
-        ch = state.srcCharCode[pos]
+        ch = state.src[pos]
         pos += 1
-        if ch != marker and not isSpace(ch):
+        if ch != marker and not isStrSpace(ch):
             return False
         if ch == marker:
             cnt += 1
 
     if cnt < 3:
         return False
 
     if silent:
         return True
 
     state.line = startLine + 1
 
     token = state.push("hr", "hr", 0)
     token.map = [startLine, state.line]
-    token.markup = chr(marker) * (cnt + 1)
+    token.markup = marker * (cnt + 1)
 
     return True
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_block/html_block.py` & `markdown-it-py-3.0.0/markdown_it/rules_block/html_block.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..common.html_re import HTML_OPEN_CLOSE_TAG_STR
 from .state_block import StateBlock
 
 LOGGER = logging.getLogger(__name__)
 
 # An array of opening and corresponding closing sequences for html tags,
 # last argument defines whether it can terminate a paragraph or not
-HTML_SEQUENCES: list[tuple[re.Pattern, re.Pattern, bool]] = [
+HTML_SEQUENCES: list[tuple[re.Pattern[str], re.Pattern[str], bool]] = [
     (
         re.compile(r"^<(script|pre|style|textarea)(?=(\s|>|$))", re.IGNORECASE),
         re.compile(r"<\/(script|pre|style|textarea)>", re.IGNORECASE),
         True,
     ),
     (re.compile(r"^<!--"), re.compile(r"-->"), True),
     (re.compile(r"^<\?"), re.compile(r"\?>"), True),
@@ -27,29 +27,28 @@
         re.compile(r"^$"),
         True,
     ),
     (re.compile(HTML_OPEN_CLOSE_TAG_STR + "\\s*$"), re.compile(r"^$"), False),
 ]
 
 
-def html_block(state: StateBlock, startLine: int, endLine: int, silent: bool):
+def html_block(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
     LOGGER.debug(
         "entering html_block: %s, %s, %s, %s", state, startLine, endLine, silent
     )
     pos = state.bMarks[startLine] + state.tShift[startLine]
     maximum = state.eMarks[startLine]
 
-    # if it's indented more than 3 spaces, it should be a code block
-    if state.sCount[startLine] - state.blkIndent >= 4:
+    if state.is_code_block(startLine):
         return False
 
     if not state.md.options.get("html", None):
         return False
 
-    if state.srcCharCode[pos] != 0x3C:  # /* < */
+    if state.src[pos] != "<":
         return False
 
     lineText = state.src[pos:maximum]
 
     html_seq = None
     for HTML_SEQUENCE in HTML_SEQUENCES:
         if HTML_SEQUENCE[0].search(lineText):
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_block/lheading.py` & `markdown-it-py-3.0.0/markdown_it/rules_block/lheading.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # lheading (---, ==)
 import logging
 
-from ..ruler import Ruler
 from .state_block import StateBlock
 
 LOGGER = logging.getLogger(__name__)
 
 
-def lheading(state: StateBlock, startLine: int, endLine: int, silent: bool):
+def lheading(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
     LOGGER.debug("entering lheading: %s, %s, %s, %s", state, startLine, endLine, silent)
 
     level = None
     nextLine = startLine + 1
-    ruler: Ruler = state.md.block.ruler
+    ruler = state.md.block.ruler
     terminatorRules = ruler.getRules("paragraph")
 
-    # if it's indented more than 3 spaces, it should be a code block
-    if state.sCount[startLine] - state.blkIndent >= 4:
+    if state.is_code_block(startLine):
         return False
 
     oldParentType = state.parentType
     state.parentType = "paragraph"  # use paragraph to match terminatorRules
 
     # jump line-by-line until empty one or EOF
     while nextLine < endLine and not state.isEmpty(nextLine):
@@ -32,24 +30,23 @@
 
         # Check for underline in setext header
         if state.sCount[nextLine] >= state.blkIndent:
             pos = state.bMarks[nextLine] + state.tShift[nextLine]
             maximum = state.eMarks[nextLine]
 
             if pos < maximum:
-                marker = state.srcCharCode[pos]
+                marker = state.src[pos]
 
-                # /* - */  /* = */
-                if marker == 0x2D or marker == 0x3D:
-                    pos = state.skipChars(pos, marker)
+                if marker in ("-", "="):
+                    pos = state.skipCharsStr(pos, marker)
                     pos = state.skipSpaces(pos)
 
                     # /* = */
                     if pos >= maximum:
-                        level = 1 if marker == 0x3D else 2
+                        level = 1 if marker == "=" else 2
                         break
 
         # quirk for blockquotes, this line should already be checked by that rule
         if state.sCount[nextLine] < 0:
             nextLine += 1
             continue
 
@@ -69,21 +66,21 @@
         return False
 
     content = state.getLines(startLine, nextLine, state.blkIndent, False).strip()
 
     state.line = nextLine + 1
 
     token = state.push("heading_open", "h" + str(level), 1)
-    token.markup = chr(marker)
+    token.markup = marker
     token.map = [startLine, state.line]
 
     token = state.push("inline", "", 0)
     token.content = content
     token.map = [startLine, state.line - 1]
     token.children = []
 
     token = state.push("heading_close", "h" + str(level), -1)
-    token.markup = chr(marker)
+    token.markup = marker
 
     state.parentType = oldParentType
 
     return True
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_block/list.py` & `markdown-it-py-3.0.0/markdown_it/rules_block/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,110 +1,114 @@
 # Lists
 import logging
 
-from ..common.utils import isSpace
+from ..common.utils import isStrSpace
 from .state_block import StateBlock
 
 LOGGER = logging.getLogger(__name__)
 
 
 # Search `[-+*][\n ]`, returns next pos after marker on success
 # or -1 on fail.
-def skipBulletListMarker(state: StateBlock, startLine: int):
+def skipBulletListMarker(state: StateBlock, startLine: int) -> int:
     pos = state.bMarks[startLine] + state.tShift[startLine]
     maximum = state.eMarks[startLine]
 
-    marker = state.srcCharCode[pos]
+    try:
+        marker = state.src[pos]
+    except IndexError:
+        return -1
     pos += 1
-    # Check bullet /* * */ /* - */ /* + */
-    if marker != 0x2A and marker != 0x2D and marker != 0x2B:
+
+    if marker not in ("*", "-", "+"):
         return -1
 
     if pos < maximum:
-        ch = state.srcCharCode[pos]
+        ch = state.src[pos]
 
-        if not isSpace(ch):
+        if not isStrSpace(ch):
             # " -test " - is not a list item
             return -1
 
     return pos
 
 
 # Search `\d+[.)][\n ]`, returns next pos after marker on success
 # or -1 on fail.
-def skipOrderedListMarker(state: StateBlock, startLine: int):
+def skipOrderedListMarker(state: StateBlock, startLine: int) -> int:
     start = state.bMarks[startLine] + state.tShift[startLine]
     pos = start
     maximum = state.eMarks[startLine]
 
     # List marker should have at least 2 chars (digit + dot)
     if pos + 1 >= maximum:
         return -1
 
-    ch = state.srcCharCode[pos]
+    ch = state.src[pos]
     pos += 1
 
+    ch_ord = ord(ch)
     # /* 0 */  /* 9 */
-    if ch < 0x30 or ch > 0x39:
+    if ch_ord < 0x30 or ch_ord > 0x39:
         return -1
 
     while True:
         # EOL -> fail
         if pos >= maximum:
             return -1
 
-        ch = state.srcCharCode[pos]
+        ch = state.src[pos]
         pos += 1
 
         # /* 0 */  /* 9 */
-        if ch >= 0x30 and ch <= 0x39:
+        ch_ord = ord(ch)
+        if ch_ord >= 0x30 and ch_ord <= 0x39:
             # List marker should have no more than 9 digits
             # (prevents integer overflow in browsers)
             if pos - start >= 10:
                 return -1
 
             continue
 
-        # found valid marker: /* ) */ /* . */
-        if ch == 0x29 or ch == 0x2E:
+        # found valid marker
+        if ch in (")", "."):
             break
 
         return -1
 
     if pos < maximum:
-        ch = state.srcCharCode[pos]
+        ch = state.src[pos]
 
-        if not isSpace(ch):
+        if not isStrSpace(ch):
             # " 1.test " - is not a list item
             return -1
 
     return pos
 
 
-def markTightParagraphs(state: StateBlock, idx: int):
+def markTightParagraphs(state: StateBlock, idx: int) -> None:
     level = state.level + 2
 
     i = idx + 2
     length = len(state.tokens) - 2
     while i < length:
         if state.tokens[i].level == level and state.tokens[i].type == "paragraph_open":
             state.tokens[i + 2].hidden = True
             state.tokens[i].hidden = True
             i += 2
         i += 1
 
 
-def list_block(state: StateBlock, startLine: int, endLine: int, silent: bool):
+def list_block(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
     LOGGER.debug("entering list: %s, %s, %s, %s", state, startLine, endLine, silent)
 
     isTerminatingParagraph = False
     tight = True
 
-    # if it's indented more than 3 spaces, it should be a code block
-    if state.sCount[startLine] - state.blkIndent >= 4:
+    if state.is_code_block(startLine):
         return False
 
     # Special case:
     #  - item 1
     #   - item 2
     #    - item 3
     #     - item 4
@@ -114,22 +118,25 @@
         and state.sCount[startLine] - state.listIndent >= 4
         and state.sCount[startLine] < state.blkIndent
     ):
         return False
 
     # limit conditions when list can interrupt
     # a paragraph (validation mode only)
-    if silent and state.parentType == "paragraph":
-        # Next list item should still terminate previous list item
-        #
-        # This code can fail if plugins use blkIndent as well as lists,
-        # but I hope the spec gets fixed long before that happens.
-        #
-        if state.tShift[startLine] >= state.blkIndent:
-            isTerminatingParagraph = True
+    # Next list item should still terminate previous list item
+    #
+    # This code can fail if plugins use blkIndent as well as lists,
+    # but I hope the spec gets fixed long before that happens.
+    #
+    if (
+        silent
+        and state.parentType == "paragraph"
+        and state.sCount[startLine] >= state.blkIndent
+    ):
+        isTerminatingParagraph = True
 
     # Detect list type and position after marker
     posAfterMarker = skipOrderedListMarker(state, startLine)
     if posAfterMarker >= 0:
         isOrdered = True
         start = state.bMarks[startLine] + state.tShift[startLine]
         markerValue = int(state.src[start : posAfterMarker - 1])
@@ -143,20 +150,22 @@
         if posAfterMarker >= 0:
             isOrdered = False
         else:
             return False
 
     # If we're starting a new unordered list right after
     # a paragraph, first line should not be empty.
-    if isTerminatingParagraph:
-        if state.skipSpaces(posAfterMarker) >= state.eMarks[startLine]:
-            return False
+    if (
+        isTerminatingParagraph
+        and state.skipSpaces(posAfterMarker) >= state.eMarks[startLine]
+    ):
+        return False
 
     # We should terminate list on style change. Remember first one to compare.
-    markerCharCode = state.srcCharCode[posAfterMarker - 1]
+    markerChar = state.src[posAfterMarker - 1]
 
     # For validation mode we can terminate immediately
     if silent:
         return True
 
     # Start list
     listTokIdx = len(state.tokens)
@@ -166,15 +175,15 @@
         if markerValue != 1:
             token.attrs = {"start": markerValue}
 
     else:
         token = state.push("bullet_list_open", "ul", 1)
 
     token.map = listLines = [startLine, 0]
-    token.markup = chr(markerCharCode)
+    token.markup = markerChar
 
     #
     # Iterate list items
     #
 
     nextLine = startLine
     prevEmptyEnd = False
@@ -190,45 +199,42 @@
         initial = offset = (
             state.sCount[nextLine]
             + posAfterMarker
             - (state.bMarks[startLine] + state.tShift[startLine])
         )
 
         while pos < maximum:
-            ch = state.srcCharCode[pos]
+            ch = state.src[pos]
 
-            if ch == 0x09:  # \t
+            if ch == "\t":
                 offset += 4 - (offset + state.bsCount[nextLine]) % 4
-            elif ch == 0x20:  # \s
+            elif ch == " ":
                 offset += 1
             else:
                 break
 
             pos += 1
 
         contentStart = pos
 
-        if contentStart >= maximum:
-            # trimming space in "-    \n  3" case, indent is 1 here
-            indentAfterMarker = 1
-        else:
-            indentAfterMarker = offset - initial
+        # trimming space in "-    \n  3" case, indent is 1 here
+        indentAfterMarker = 1 if contentStart >= maximum else offset - initial
 
         # If we have more than 4 spaces, the indent is 1
         # (the rest is just indented code block)
         if indentAfterMarker > 4:
             indentAfterMarker = 1
 
         # "  -  test"
         #  ^^^^^ - calculating total length of this thing
         indent = initial + indentAfterMarker
 
         # Run subparser & write tokens
         token = state.push("list_item_open", "li", 1)
-        token.markup = chr(markerCharCode)
+        token.markup = markerChar
         token.map = itemLines = [startLine, 0]
         if isOrdered:
             token.info = state.src[start : posAfterMarker - 1]
 
         # change current state, then restore it after parser subcall
         oldTight = state.tight
         oldTShift = state.tShift[startLine]
@@ -272,15 +278,15 @@
         state.blkIndent = state.listIndent
         state.listIndent = oldListIndent
         state.tShift[startLine] = oldTShift
         state.sCount[startLine] = oldSCount
         state.tight = oldTight
 
         token = state.push("list_item_close", "li", -1)
-        token.markup = chr(markerCharCode)
+        token.markup = markerChar
 
         nextLine = startLine = state.line
         itemLines[1] = nextLine
 
         if nextLine >= endLine:
             break
 
@@ -288,16 +294,15 @@
 
         #
         # Try to check if list is terminated or continued.
         #
         if state.sCount[nextLine] < state.blkIndent:
             break
 
-        # if it's indented more than 3 spaces, it should be a code block
-        if state.sCount[startLine] - state.blkIndent >= 4:
+        if state.is_code_block(startLine):
             break
 
         # fail if terminating block found
         terminate = False
         for terminatorRule in terminatorRules:
             if terminatorRule(state, nextLine, endLine, True):
                 terminate = True
@@ -313,24 +318,24 @@
                 break
             start = state.bMarks[nextLine] + state.tShift[nextLine]
         else:
             posAfterMarker = skipBulletListMarker(state, nextLine)
             if posAfterMarker < 0:
                 break
 
-        if markerCharCode != state.srcCharCode[posAfterMarker - 1]:
+        if markerChar != state.src[posAfterMarker - 1]:
             break
 
     # Finalize list
     if isOrdered:
         token = state.push("ordered_list_close", "ol", -1)
     else:
         token = state.push("bullet_list_close", "ul", -1)
 
-    token.markup = chr(markerCharCode)
+    token.markup = markerChar
 
     listLines[1] = nextLine
     state.line = nextLine
 
     state.parentType = oldParentType
 
     # mark paragraphs tight if needed
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_block/paragraph.py` & `markdown-it-py-3.0.0/markdown_it/rules_block/paragraph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Paragraph."""
 import logging
 
-from ..ruler import Ruler
 from .state_block import StateBlock
 
 LOGGER = logging.getLogger(__name__)
 
 
-def paragraph(state: StateBlock, startLine: int, endLine: int, silent: bool = False):
+def paragraph(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
     LOGGER.debug(
         "entering paragraph: %s, %s, %s, %s", state, startLine, endLine, silent
     )
 
     nextLine = startLine + 1
-    ruler: Ruler = state.md.block.ruler
+    ruler = state.md.block.ruler
     terminatorRules = ruler.getRules("paragraph")
     endLine = state.lineMax
 
     oldParentType = state.parentType
     state.parentType = "paragraph"
 
     # jump line-by-line until empty one or EOF
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_block/reference.py` & `markdown-it-py-3.0.0/markdown_it/rules_block/reference.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,39 +2,38 @@
 
 from ..common.utils import charCodeAt, isSpace, normalizeReference
 from .state_block import StateBlock
 
 LOGGER = logging.getLogger(__name__)
 
 
-def reference(state: StateBlock, startLine, _endLine, silent):
+def reference(state: StateBlock, startLine: int, _endLine: int, silent: bool) -> bool:
     LOGGER.debug(
         "entering reference: %s, %s, %s, %s", state, startLine, _endLine, silent
     )
 
     lines = 0
     pos = state.bMarks[startLine] + state.tShift[startLine]
     maximum = state.eMarks[startLine]
     nextLine = startLine + 1
 
-    # if it's indented more than 3 spaces, it should be a code block
-    if state.sCount[startLine] - state.blkIndent >= 4:
+    if state.is_code_block(startLine):
         return False
 
-    if state.srcCharCode[pos] != 0x5B:  # /* [ */
+    if state.src[pos] != "[":
         return False
 
     # Simple check to quickly interrupt scan on [link](url) at the start of line.
     # Can be useful on practice: https:#github.com/markdown-it/markdown-it/issues/54
     while pos < maximum:
         # /* ] */  /* \ */  /* : */
-        if state.srcCharCode[pos] == 0x5D and state.srcCharCode[pos - 1] != 0x5C:
+        if state.src[pos] == "]" and state.src[pos - 1] != "\\":
             if pos + 1 == maximum:
                 return False
-            if state.srcCharCode[pos + 1] != 0x3A:
+            if state.src[pos + 1] != ":":
                 return False
             break
         pos += 1
 
     endLine = state.lineMax
 
     # jump line-by-line until empty one or EOF
@@ -150,26 +149,25 @@
     # skip trailing spaces until the rest of the line
     while pos < maximum:
         ch = charCodeAt(string, pos)
         if not isSpace(ch):
             break
         pos += 1
 
-    if pos < maximum and charCodeAt(string, pos) != 0x0A:
-        if title:
-            # garbage at the end of the line after title,
-            # but it could still be a valid reference if we roll back
-            title = ""
-            pos = destEndPos
-            lines = destEndLineNo
-            while pos < maximum:
-                ch = charCodeAt(string, pos)
-                if not isSpace(ch):
-                    break
-                pos += 1
+    if pos < maximum and charCodeAt(string, pos) != 0x0A and title:
+        # garbage at the end of the line after title,
+        # but it could still be a valid reference if we roll back
+        title = ""
+        pos = destEndPos
+        lines = destEndLineNo
+        while pos < maximum:
+            ch = charCodeAt(string, pos)
+            if not isSpace(ch):
+                break
+            pos += 1
 
     if pos < maximum and charCodeAt(string, pos) != 0x0A:
         # garbage at the end of the line
         return False
 
     label = normalizeReference(string[1:labelEnd])
     if not label:
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_block/state_block.py` & `markdown-it-py-3.0.0/markdown_it/rules_block/state_block.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,54 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal
 
-from ..common.utils import isSpace
+from ..common.utils import isStrSpace
 from ..ruler import StateBase
 from ..token import Token
+from ..utils import EnvType
 
 if TYPE_CHECKING:
     from markdown_it.main import MarkdownIt
 
 
 class StateBlock(StateBase):
     def __init__(
-        self,
-        src: str,
-        md: MarkdownIt,
-        env,
-        tokens: list[Token],
-        srcCharCode: tuple[int, ...] | None = None,
-    ):
-        if srcCharCode is not None:
-            self._src = src
-            self.srcCharCode = srcCharCode
-        else:
-            self.src = src
+        self, src: str, md: MarkdownIt, env: EnvType, tokens: list[Token]
+    ) -> None:
+        self.src = src
 
         # link to parser instance
         self.md = md
 
         self.env = env
 
         #
         # Internal state variables
         #
 
         self.tokens = tokens
 
-        self.bMarks = []  # line begin offsets for fast jumps
-        self.eMarks = []  # line end offsets for fast jumps
+        self.bMarks: list[int] = []  # line begin offsets for fast jumps
+        self.eMarks: list[int] = []  # line end offsets for fast jumps
         # offsets of the first non-space characters (tabs not expanded)
-        self.tShift = []
-        self.sCount = []  # indents for each line (tabs expanded)
+        self.tShift: list[int] = []
+        self.sCount: list[int] = []  # indents for each line (tabs expanded)
 
         # An amount of virtual spaces (tabs expanded) between beginning
         # of each line (bMarks) and real beginning of that line.
         #
         # It exists only as a hack because blockquotes override bMarks
         # losing information in the process.
         #
         # It's used only when expanding tabs, you can think about it as
         # an initial tab length, e.g. bsCount=21 applied to string `\t123`
         # means first tab should be expanded to 4-21%4 === 3 spaces.
         #
-        self.bsCount = []
+        self.bsCount: list[int] = []
 
         # block parser variables
         self.blkIndent = 0  # required block content indent (for example, if we are
         # inside a list, it would be positioned after list marker)
         self.line = 0  # line index in src
         self.lineMax = 0  # lines count
         self.tight = False  # loose/tight mode for lists
@@ -75,29 +67,29 @@
         # Create caches
         # Generate markers.
         indent_found = False
 
         start = pos = indent = offset = 0
         length = len(self.src)
 
-        for pos, character in enumerate(self.srcCharCode):
+        for pos, character in enumerate(self.src):
             if not indent_found:
-                if isSpace(character):
+                if isStrSpace(character):
                     indent += 1
 
-                    if character == 0x09:
+                    if character == "\t":
                         offset += 4 - offset % 4
                     else:
                         offset += 1
                     continue
                 else:
                     indent_found = True
 
-            if character == 0x0A or pos == length - 1:
-                if character != 0x0A:
+            if character == "\n" or pos == length - 1:
+                if character != "\n":
                     pos += 1
                 self.bMarks.append(start)
                 self.eMarks.append(pos)
                 self.tShift.append(indent)
                 self.sCount.append(offset)
                 self.bsCount.append(0)
 
@@ -111,21 +103,24 @@
         self.eMarks.append(length)
         self.tShift.append(0)
         self.sCount.append(0)
         self.bsCount.append(0)
 
         self.lineMax = len(self.bMarks) - 1  # don't count last fake line
 
-    def __repr__(self):
+        # pre-check if code blocks are enabled, to speed up is_code_block method
+        self._code_enabled = "code" in self.md["block"].ruler.get_active_rules()
+
+    def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}"
             f"(line={self.line},level={self.level},tokens={len(self.tokens)})"
         )
 
-    def push(self, ttype: str, tag: str, nesting: int) -> Token:
+    def push(self, ttype: str, tag: str, nesting: Literal[-1, 0, 1]) -> Token:
         """Push new token to "stream"."""
         token = Token(ttype, tag, nesting)
         token.block = True
         if nesting < 0:
             self.level -= 1  # closing tag
         token.level = self.level
         if nesting > 0:
@@ -148,69 +143,100 @@
             except IndexError:
                 pass
             from_pos += 1
         return from_pos
 
     def skipSpaces(self, pos: int) -> int:
         """Skip spaces from given position."""
-        while pos < len(self.src):
-            if not isSpace(self.srcCharCode[pos]):
+        while True:
+            try:
+                current = self.src[pos]
+            except IndexError:
+                break
+            if not isStrSpace(current):
                 break
             pos += 1
         return pos
 
     def skipSpacesBack(self, pos: int, minimum: int) -> int:
         """Skip spaces from given position in reverse."""
         if pos <= minimum:
             return pos
         while pos > minimum:
             pos -= 1
-            if not isSpace(self.srcCharCode[pos]):
+            if not isStrSpace(self.src[pos]):
                 return pos + 1
         return pos
 
     def skipChars(self, pos: int, code: int) -> int:
-        """Skip char codes from given position."""
-        while pos < len(self.src):
-            if self.srcCharCode[pos] != code:
+        """Skip character code from given position."""
+        while True:
+            try:
+                current = self.srcCharCode[pos]
+            except IndexError:
+                break
+            if current != code:
+                break
+            pos += 1
+        return pos
+
+    def skipCharsStr(self, pos: int, ch: str) -> int:
+        """Skip character string from given position."""
+        while True:
+            try:
+                current = self.src[pos]
+            except IndexError:
+                break
+            if current != ch:
                 break
             pos += 1
         return pos
 
     def skipCharsBack(self, pos: int, code: int, minimum: int) -> int:
-        """Skip char codes reverse from given position - 1."""
+        """Skip character code reverse from given position - 1."""
         if pos <= minimum:
             return pos
         while pos > minimum:
             pos -= 1
             if code != self.srcCharCode[pos]:
                 return pos + 1
         return pos
 
+    def skipCharsStrBack(self, pos: int, ch: str, minimum: int) -> int:
+        """Skip character string reverse from given position - 1."""
+        if pos <= minimum:
+            return pos
+        while pos > minimum:
+            pos -= 1
+            if ch != self.src[pos]:
+                return pos + 1
+        return pos
+
     def getLines(self, begin: int, end: int, indent: int, keepLastLF: bool) -> str:
         """Cut lines range from source."""
         line = begin
         if begin >= end:
             return ""
 
         queue = [""] * (end - begin)
 
         i = 1
         while line < end:
             lineIndent = 0
             lineStart = first = self.bMarks[line]
-            if line + 1 < end or keepLastLF:
-                last = self.eMarks[line] + 1
-            else:
-                last = self.eMarks[line]
+            last = (
+                self.eMarks[line] + 1
+                if line + 1 < end or keepLastLF
+                else self.eMarks[line]
+            )
 
             while (first < last) and (lineIndent < indent):
-                ch = self.srcCharCode[first]
-                if isSpace(ch):
-                    if ch == 0x09:
+                ch = self.src[first]
+                if isStrSpace(ch):
+                    if ch == "\t":
                         lineIndent += 4 - (lineIndent + self.bsCount[line]) % 4
                     else:
                         lineIndent += 1
                 elif first - lineStart < self.tShift[line]:
                     lineIndent += 1
                 else:
                     break
@@ -223,7 +249,13 @@
             else:
                 queue[i - 1] = self.src[first:last]
 
             line += 1
             i += 1
 
         return "".join(queue)
+
+    def is_code_block(self, line: int) -> bool:
+        """Check if line is a code block,
+        i.e. the code block rule is enabled and text is indented by more than 3 spaces.
+        """
+        return self._code_enabled and (self.sCount[line] - self.blkIndent) >= 4
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_block/table.py` & `markdown-it-py-3.0.0/markdown_it/rules_block/table.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,102 +1,101 @@
 # GFM table, https://github.github.com/gfm/#tables-extension-
+from __future__ import annotations
+
 import re
 
-from ..common.utils import charCodeAt, isSpace
+from ..common.utils import charStrAt, isStrSpace
 from .state_block import StateBlock
 
 headerLineRe = re.compile(r"^:?-+:?$")
 enclosingPipesRe = re.compile(r"^\||\|$")
 
 
-def getLine(state: StateBlock, line: int):
+def getLine(state: StateBlock, line: int) -> str:
     pos = state.bMarks[line] + state.tShift[line]
     maximum = state.eMarks[line]
 
     # return state.src.substr(pos, max - pos)
     return state.src[pos:maximum]
 
 
-def escapedSplit(string):
-    result = []
+def escapedSplit(string: str) -> list[str]:
+    result: list[str] = []
     pos = 0
     max = len(string)
     isEscaped = False
     lastPos = 0
     current = ""
-    ch = charCodeAt(string, pos)
+    ch = charStrAt(string, pos)
 
     while pos < max:
-        if ch == 0x7C:  # /* | */
+        if ch == "|":
             if not isEscaped:
                 # pipe separating cells, '|'
                 result.append(current + string[lastPos:pos])
                 current = ""
                 lastPos = pos + 1
             else:
                 # escaped pipe, '\|'
                 current += string[lastPos : pos - 1]
                 lastPos = pos
 
-        isEscaped = ch == 0x5C  # /* \ */
+        isEscaped = ch == "\\"
         pos += 1
 
-        ch = charCodeAt(string, pos)
+        ch = charStrAt(string, pos)
 
     result.append(current + string[lastPos:])
 
     return result
 
 
-def table(state: StateBlock, startLine: int, endLine: int, silent: bool):
+def table(state: StateBlock, startLine: int, endLine: int, silent: bool) -> bool:
     tbodyLines = None
 
     # should have at least two lines
     if startLine + 2 > endLine:
         return False
 
     nextLine = startLine + 1
 
     if state.sCount[nextLine] < state.blkIndent:
         return False
 
-    # if it's indented more than 3 spaces, it should be a code block
-    if state.sCount[nextLine] - state.blkIndent >= 4:
+    if state.is_code_block(nextLine):
         return False
 
     # first character of the second line should be '|', '-', ':',
     # and no other characters are allowed but spaces;
     # basically, this is the equivalent of /^[-:|][-:|\s]*$/ regexp
 
     pos = state.bMarks[nextLine] + state.tShift[nextLine]
     if pos >= state.eMarks[nextLine]:
         return False
-    first_ch = state.srcCharCode[pos]
+    first_ch = state.src[pos]
     pos += 1
-    if first_ch not in {0x7C, 0x2D, 0x3A}:  # not in {"|", "-", ":"}
+    if first_ch not in ("|", "-", ":"):
         return False
 
     if pos >= state.eMarks[nextLine]:
         return False
-    second_ch = state.srcCharCode[pos]
+    second_ch = state.src[pos]
     pos += 1
-    # not in {"|", "-", ":"} and not space
-    if second_ch not in {0x7C, 0x2D, 0x3A} and not isSpace(second_ch):
+    if second_ch not in ("|", "-", ":") and not isStrSpace(second_ch):
         return False
 
     # if first character is '-', then second character must not be a space
     # (due to parsing ambiguity with list)
-    if first_ch == 0x2D and isSpace(second_ch):
+    if first_ch == "-" and isStrSpace(second_ch):
         return False
 
     while pos < state.eMarks[nextLine]:
-        ch = state.srcCharCode[pos]
+        ch = state.src[pos]
 
-        # /* | */  /* - */ /* : */
-        if ch not in {0x7C, 0x2D, 0x3A} and not isSpace(ch):
+        if ch not in ("|", "-", ":") and not isStrSpace(ch):
             return False
 
         pos += 1
 
     lineText = getLine(state, startLine + 1)
 
     columns = lineText.split("|")
@@ -109,26 +108,25 @@
             if i == 0 or i == len(columns) - 1:
                 continue
             else:
                 return False
 
         if not headerLineRe.search(t):
             return False
-        if charCodeAt(t, len(t) - 1) == 0x3A:  # /* : */
-            # /* : */
-            aligns.append("center" if charCodeAt(t, 0) == 0x3A else "right")
-        elif charCodeAt(t, 0) == 0x3A:  # /* : */
+        if charStrAt(t, len(t) - 1) == ":":
+            aligns.append("center" if charStrAt(t, 0) == ":" else "right")
+        elif charStrAt(t, 0) == ":":
             aligns.append("left")
         else:
             aligns.append("")
 
     lineText = getLine(state, startLine).strip()
     if "|" not in lineText:
         return False
-    if state.sCount[startLine] - state.blkIndent >= 4:
+    if state.is_code_block(startLine):
         return False
     columns = escapedSplit(lineText)
     if columns and columns[0] == "":
         columns.pop(0)
     if columns and columns[-1] == "":
         columns.pop()
 
@@ -186,15 +184,15 @@
                 break
 
         if terminate:
             break
         lineText = getLine(state, nextLine).strip()
         if not lineText:
             break
-        if state.sCount[nextLine] - state.blkIndent >= 4:
+        if state.is_code_block(nextLine):
             break
         columns = escapedSplit(lineText)
         if columns and columns[0] == "":
             columns.pop(0)
         if columns and columns[-1] == "":
             columns.pop()
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_core/linkify.py` & `markdown-it-py-3.0.0/markdown_it/rules_core/linkify.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,36 @@
+from __future__ import annotations
+
 import re
+from typing import Protocol
 
-from ..common.utils import arrayReplaceAt
+from ..common.utils import arrayReplaceAt, isLinkClose, isLinkOpen
 from ..token import Token
 from .state_core import StateCore
 
-LINK_OPEN_RE = re.compile(r"^<a[>\s]", flags=re.IGNORECASE)
-LINK_CLOSE_RE = re.compile(r"^</a\s*>", flags=re.IGNORECASE)
-
 HTTP_RE = re.compile(r"^http://")
 MAILTO_RE = re.compile(r"^mailto:")
 TEST_MAILTO_RE = re.compile(r"^mailto:", flags=re.IGNORECASE)
 
 
-def isLinkOpen(string: str) -> bool:
-    return bool(LINK_OPEN_RE.search(string))
-
-
-def isLinkClose(string: str) -> bool:
-    return bool(LINK_CLOSE_RE.search(string))
-
-
 def linkify(state: StateCore) -> None:
-    blockTokens = state.tokens
-
+    """Rule for identifying plain-text links."""
     if not state.md.options.linkify:
         return
 
     if not state.md.linkify:
         raise ModuleNotFoundError("Linkify enabled but not installed.")
 
-    for j in range(len(blockTokens)):
-        if blockTokens[j].type != "inline" or not state.md.linkify.pretest(
-            blockTokens[j].content
+    for inline_token in state.tokens:
+        if inline_token.type != "inline" or not state.md.linkify.pretest(
+            inline_token.content
         ):
             continue
 
-        tokens = blockTokens[j].children
+        tokens = inline_token.children
 
         htmlLinkLevel = 0
 
         # We scan from the end, to keep position when new tags added.
         # Use reversed logic in links start/end match
         assert tokens is not None
         i = len(tokens)
@@ -67,46 +58,55 @@
             if htmlLinkLevel > 0:
                 continue
 
             if currentToken.type == "text" and state.md.linkify.test(
                 currentToken.content
             ):
                 text = currentToken.content
-                links = state.md.linkify.match(text)
+                links: list[_LinkType] = state.md.linkify.match(text) or []
 
                 # Now split string to nodes
                 nodes = []
                 level = currentToken.level
                 lastPos = 0
 
-                for ln in range(len(links)):
-                    url = links[ln].url
+                # forbid escape sequence at the start of the string,
+                # this avoids http\://example.com/ from being linkified as
+                # http:<a href="//example.com/">//example.com/</a>
+                if (
+                    links
+                    and links[0].index == 0
+                    and i > 0
+                    and tokens[i - 1].type == "text_special"
+                ):
+                    links = links[1:]
+
+                for link in links:
+                    url = link.url
                     fullUrl = state.md.normalizeLink(url)
                     if not state.md.validateLink(fullUrl):
                         continue
 
-                    urlText = links[ln].text
+                    urlText = link.text
 
                     # Linkifier might send raw hostnames like "example.com", where url
                     # starts with domain name. So we prepend http:// in those cases,
                     # and remove it afterwards.
-                    if not links[ln].schema:
+                    if not link.schema:
                         urlText = HTTP_RE.sub(
                             "", state.md.normalizeLinkText("http://" + urlText)
                         )
-                    elif links[ln].schema == "mailto:" and TEST_MAILTO_RE.search(
-                        urlText
-                    ):
+                    elif link.schema == "mailto:" and TEST_MAILTO_RE.search(urlText):
                         urlText = MAILTO_RE.sub(
                             "", state.md.normalizeLinkText("mailto:" + urlText)
                         )
                     else:
                         urlText = state.md.normalizeLinkText(urlText)
 
-                    pos = links[ln].index
+                    pos = link.index
 
                     if pos > lastPos:
                         token = Token("text", "", 0)
                         token.content = text[lastPos:pos]
                         token.level = level
                         nodes.append(token)
 
@@ -126,16 +126,24 @@
                     token = Token("link_close", "a", -1)
                     level -= 1
                     token.level = level
                     token.markup = "linkify"
                     token.info = "auto"
                     nodes.append(token)
 
-                    lastPos = links[ln].last_index
+                    lastPos = link.last_index
 
                 if lastPos < len(text):
                     token = Token("text", "", 0)
                     token.content = text[lastPos:]
                     token.level = level
                     nodes.append(token)
 
-                blockTokens[j].children = tokens = arrayReplaceAt(tokens, i, nodes)
+                inline_token.children = tokens = arrayReplaceAt(tokens, i, nodes)
+
+
+class _LinkType(Protocol):
+    url: str
+    text: str
+    index: int
+    last_index: int
+    schema: str | None
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_core/replacements.py` & `markdown-it-py-3.0.0/markdown_it/rules_core/replacements.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Simple typographic replacements
 
 * ``(c)``, ``(C)`` → ©
 * ``(tm)``, ``(TM)`` → ™
 * ``(r)``, ``(R)`` → ®
-* ``(p)``, ``(P)`` → §
 * ``+-`` → ±
 * ``...`` → …
 * ``?....`` → ?..
 * ``!....`` → !..
 * ``????????`` → ???
 * ``!!!!!`` → !!!
 * ``,,,`` → ,
@@ -22,23 +21,23 @@
 from ..token import Token
 from .state_core import StateCore
 
 LOGGER = logging.getLogger(__name__)
 
 # TODO:
 # - fractionals 1/2, 1/4, 3/4 -> ½, ¼, ¾
-# - miltiplication 2 x 4 -> 2 × 4
+# - multiplication 2 x 4 -> 2 × 4
 
 RARE_RE = re.compile(r"\+-|\.\.|\?\?\?\?|!!!!|,,|--")
 
 # Workaround for phantomjs - need regex without /g flag,
 # or root check will fail every second time
-# SCOPED_ABBR_TEST_RE = r"\((c|tm|r|p)\)"
+# SCOPED_ABBR_TEST_RE = r"\((c|tm|r)\)"
 
-SCOPED_ABBR_RE = re.compile(r"\((c|tm|r|p)\)", flags=re.IGNORECASE)
+SCOPED_ABBR_RE = re.compile(r"\((c|tm|r)\)", flags=re.IGNORECASE)
 
 PLUS_MINUS_RE = re.compile(r"\+-")
 
 ELLIPSIS_RE = re.compile(r"\.{2,}")
 
 ELLIPSIS_QUESTION_EXCLAMATION_RE = re.compile(r"([?!])…")
 
@@ -49,18 +48,18 @@
 EM_DASH_RE = re.compile(r"(^|[^-])---(?=[^-]|$)", flags=re.MULTILINE)
 
 EN_DASH_RE = re.compile(r"(^|\s)--(?=\s|$)", flags=re.MULTILINE)
 
 EN_DASH_INDENT_RE = re.compile(r"(^|[^-\s])--(?=[^-\s]|$)", flags=re.MULTILINE)
 
 
-SCOPED_ABBR = {"c": "©", "r": "®", "p": "§", "tm": "™"}
+SCOPED_ABBR = {"c": "©", "r": "®", "tm": "™"}
 
 
-def replaceFn(match: re.Match[str]):
+def replaceFn(match: re.Match[str]) -> str:
     return SCOPED_ABBR[match.group(1).lower()]
 
 
 def replace_scoped(inlineTokens: list[Token]) -> None:
     inside_autolink = 0
 
     for token in inlineTokens:
@@ -74,37 +73,38 @@
             inside_autolink += 1
 
 
 def replace_rare(inlineTokens: list[Token]) -> None:
     inside_autolink = 0
 
     for token in inlineTokens:
-        if token.type == "text" and not inside_autolink:
-            if RARE_RE.search(token.content):
-                # +- -> ±
-                token.content = PLUS_MINUS_RE.sub("±", token.content)
-
-                # .., ..., ....... -> …
-                token.content = ELLIPSIS_RE.sub("…", token.content)
-
-                # but ?..... & !..... -> ?.. & !..
-                token.content = ELLIPSIS_QUESTION_EXCLAMATION_RE.sub(
-                    "\\1..", token.content
-                )
-                token.content = QUESTION_EXCLAMATION_RE.sub("\\1\\1\\1", token.content)
-
-                # ,,  ,,,  ,,,, -> ,
-                token.content = COMMA_RE.sub(",", token.content)
-
-                # em-dash
-                token.content = EM_DASH_RE.sub("\\1\u2014", token.content)
-
-                # en-dash
-                token.content = EN_DASH_RE.sub("\\1\u2013", token.content)
-                token.content = EN_DASH_INDENT_RE.sub("\\1\u2013", token.content)
+        if (
+            token.type == "text"
+            and (not inside_autolink)
+            and RARE_RE.search(token.content)
+        ):
+            # +- -> ±
+            token.content = PLUS_MINUS_RE.sub("±", token.content)
+
+            # .., ..., ....... -> …
+            token.content = ELLIPSIS_RE.sub("…", token.content)
+
+            # but ?..... & !..... -> ?.. & !..
+            token.content = ELLIPSIS_QUESTION_EXCLAMATION_RE.sub("\\1..", token.content)
+            token.content = QUESTION_EXCLAMATION_RE.sub("\\1\\1\\1", token.content)
+
+            # ,,  ,,,  ,,,, -> ,
+            token.content = COMMA_RE.sub(",", token.content)
+
+            # em-dash
+            token.content = EM_DASH_RE.sub("\\1\u2014", token.content)
+
+            # en-dash
+            token.content = EN_DASH_RE.sub("\\1\u2013", token.content)
+            token.content = EN_DASH_INDENT_RE.sub("\\1\u2013", token.content)
 
         if token.type == "link_open" and token.info == "auto":
             inside_autolink -= 1
 
         if token.type == "link_close" and token.info == "auto":
             inside_autolink += 1
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_core/smartquotes.py` & `markdown-it-py-3.0.0/markdown_it/rules_core/smartquotes.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,15 @@
     assert index >= 0
     return string[:index] + ch + string[index + 1 :]
 
 
 def process_inlines(tokens: list[Token], state: StateCore) -> None:
     stack: list[dict[str, Any]] = []
 
-    for i in range(len(tokens)):
-        token = tokens[i]
-
+    for i, token in enumerate(tokens):
         thisLevel = token.level
 
         j = 0
         for j in range(len(stack))[::-1]:
             if stack[j]["level"] <= thisLevel:
                 break
         else:
@@ -56,33 +54,32 @@
 
             canOpen = canClose = True
             pos = t.start(0) + lastIndex + 1
             isSingle = t.group(0) == "'"
 
             # Find previous character,
             # default to space if it's the beginning of the line
-            lastChar = 0x20
+            lastChar: None | int = 0x20
 
             if t.start(0) + lastIndex - 1 >= 0:
                 lastChar = charCodeAt(text, t.start(0) + lastIndex - 1)
             else:
                 for j in range(i)[::-1]:
-                    # lastChar defaults to 0x20
                     if tokens[j].type == "softbreak" or tokens[j].type == "hardbreak":
                         break
                     # should skip all tokens except 'text', 'html_inline' or 'code_inline'
                     if not tokens[j].content:
                         continue
 
                     lastChar = charCodeAt(tokens[j].content, len(tokens[j].content) - 1)
                     break
 
             # Find next character,
             # default to space if it's the end of the line
-            nextChar = 0x20
+            nextChar: None | int = 0x20
 
             if pos < maximum:
                 nextChar = charCodeAt(text, pos)
             else:
                 for j in range(i + 1, len(tokens)):
                     # nextChar defaults to 0x20
                     if tokens[j].type == "softbreak" or tokens[j].type == "hardbreak":
@@ -90,34 +87,38 @@
                     # should skip all tokens except 'text', 'html_inline' or 'code_inline'
                     if not tokens[j].content:
                         continue
 
                     nextChar = charCodeAt(tokens[j].content, 0)
                     break
 
-            isLastPunctChar = isMdAsciiPunct(lastChar) or isPunctChar(chr(lastChar))
-            isNextPunctChar = isMdAsciiPunct(nextChar) or isPunctChar(chr(nextChar))
+            isLastPunctChar = lastChar is not None and (
+                isMdAsciiPunct(lastChar) or isPunctChar(chr(lastChar))
+            )
+            isNextPunctChar = nextChar is not None and (
+                isMdAsciiPunct(nextChar) or isPunctChar(chr(nextChar))
+            )
 
-            isLastWhiteSpace = isWhiteSpace(lastChar)
-            isNextWhiteSpace = isWhiteSpace(nextChar)
+            isLastWhiteSpace = lastChar is not None and isWhiteSpace(lastChar)
+            isNextWhiteSpace = nextChar is not None and isWhiteSpace(nextChar)
 
-            if isNextWhiteSpace:
+            if isNextWhiteSpace:  # noqa: SIM114
+                canOpen = False
+            elif isNextPunctChar and not (isLastWhiteSpace or isLastPunctChar):
                 canOpen = False
-            elif isNextPunctChar:
-                if not (isLastWhiteSpace or isLastPunctChar):
-                    canOpen = False
 
-            if isLastWhiteSpace:
+            if isLastWhiteSpace:  # noqa: SIM114
+                canClose = False
+            elif isLastPunctChar and not (isNextWhiteSpace or isNextPunctChar):
                 canClose = False
-            elif isLastPunctChar:
-                if not (isNextWhiteSpace or isNextPunctChar):
-                    canClose = False
 
-            if nextChar == 0x22 and t.group(0) == '"':  # 0x22: "
-                if lastChar >= 0x30 and lastChar <= 0x39:  # 0x30: 0, 0x39: 9
+            if nextChar == 0x22 and t.group(0) == '"':  # 0x22: "  # noqa: SIM102
+                if (
+                    lastChar is not None and lastChar >= 0x30 and lastChar <= 0x39
+                ):  # 0x30: 0, 0x39: 9
                     # special case: 1"" - count first quote as an inch
                     canClose = canOpen = False
 
             if canOpen and canClose:
                 # Replace quotes in the middle of punctuation sequence, but not
                 # in the middle of the words, i.e.:
                 #
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_core/state_core.py` & `markdown-it-py-3.0.0/markdown_it/rules_core/state_core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
-from collections.abc import MutableMapping
 from typing import TYPE_CHECKING
 
 from ..ruler import StateBase
 from ..token import Token
+from ..utils import EnvType
 
 if TYPE_CHECKING:
     from markdown_it import MarkdownIt
 
 
 class StateCore(StateBase):
     def __init__(
         self,
         src: str,
         md: MarkdownIt,
-        env: MutableMapping,
+        env: EnvType,
         tokens: list[Token] | None = None,
-    ):
+    ) -> None:
         self.src = src
         self.md = md  # link to parser instance
         self.env = env
         self.tokens: list[Token] = tokens or []
         self.inlineMode = False
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_inline/__init__.py` & `markdown-it-py-3.0.0/markdown_it/rules_inline/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __all__ = (
     "StateInline",
     "text",
-    "text_collapse",
+    "fragments_join",
     "link_pairs",
+    "linkify",
     "escape",
     "newline",
     "backtick",
     "emphasis",
     "image",
     "link",
     "autolink",
@@ -16,14 +17,15 @@
 )
 from . import emphasis, strikethrough
 from .autolink import autolink
 from .backticks import backtick
 from .balance_pairs import link_pairs
 from .entity import entity
 from .escape import escape
+from .fragments_join import fragments_join
 from .html_inline import html_inline
 from .image import image
 from .link import link
+from .linkify import linkify
 from .newline import newline
 from .state_inline import StateInline
 from .text import text
-from .text_collapse import text_collapse
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_inline/autolink.py` & `markdown-it-py-3.0.0/markdown_it/rules_inline/autolink.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 )
 AUTOLINK_RE = re.compile(r"^([a-zA-Z][a-zA-Z0-9+.\-]{1,31}):([^<>\x00-\x20]*)$")
 
 
 def autolink(state: StateInline, silent: bool) -> bool:
     pos = state.pos
 
-    if state.srcCharCode[pos] != 0x3C:  # /* < */
+    if state.src[pos] != "<":
         return False
 
     start = state.pos
     maximum = state.posMax
 
     while True:
         pos += 1
         if pos >= maximum:
             return False
 
-        ch = state.srcCharCode[pos]
+        ch = state.src[pos]
 
-        if ch == 0x3C:  # /* < */
+        if ch == "<":
             return False
-        if ch == 0x3E:  # /* > */
+        if ch == ">":
             break
 
     url = state.src[start + 1 : pos]
 
     if AUTOLINK_RE.search(url) is not None:
         fullUrl = state.md.normalizeLink(url)
         if not state.md.validateLink(fullUrl):
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_inline/backticks.py` & `markdown-it-py-3.0.0/markdown_it/rules_inline/backticks.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,26 +4,24 @@
 from .state_inline import StateInline
 
 regex = re.compile("^ (.+) $")
 
 
 def backtick(state: StateInline, silent: bool) -> bool:
     pos = state.pos
-    ch = state.srcCharCode[pos]
 
-    # /* ` */
-    if ch != 0x60:
+    if state.src[pos] != "`":
         return False
 
     start = pos
     pos += 1
     maximum = state.posMax
 
     # scan marker length
-    while pos < maximum and (state.srcCharCode[pos] == 0x60):  # /* ` */
+    while pos < maximum and (state.src[pos] == "`"):
         pos += 1
 
     marker = state.src[start:pos]
     openerLength = len(marker)
 
     if state.backticksScanned and state.backticks.get(openerLength, 0) <= start:
         if not silent:
@@ -38,15 +36,15 @@
         try:
             matchStart = state.src.index("`", matchEnd)
         except ValueError:
             break
         matchEnd = matchStart + 1
 
         # scan marker length
-        while matchEnd < maximum and (state.srcCharCode[matchEnd] == 0x60):  # /* ` */
+        while matchEnd < maximum and (state.src[matchEnd] == "`"):
             matchEnd += 1
 
         closerLength = matchEnd - matchStart
 
         if closerLength == openerLength:
             # Found matching closer length.
             if not silent:
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_inline/balance_pairs.py` & `markdown-it-py-3.0.0/markdown_it/rules_inline/balance_pairs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,42 @@
-# For each opening emphasis-like marker find a matching closing one
-#
-from .state_inline import StateInline
+"""Balance paired characters (*, _, etc) in inline tokens."""
+from __future__ import annotations
 
+from .state_inline import Delimiter, StateInline
+
+
+def processDelimiters(state: StateInline, delimiters: list[Delimiter]) -> None:
+    """For each opening emphasis-like marker find a matching closing one."""
+    if not delimiters:
+        return
 
-def processDelimiters(state: StateInline, delimiters, *args):
     openersBottom = {}
     maximum = len(delimiters)
 
+    # headerIdx is the first delimiter of the current (where closer is) delimiter run
+    headerIdx = 0
+    lastTokenIdx = -2  # needs any value lower than -1
+    jumps: list[int] = []
     closerIdx = 0
     while closerIdx < maximum:
         closer = delimiters[closerIdx]
 
+        jumps.append(0)
+
+        # markers belong to same delimiter run if:
+        #  - they have adjacent tokens
+        #  - AND markers are the same
+        #
+        if (
+            delimiters[headerIdx].marker != closer.marker
+            or lastTokenIdx != closer.token - 1
+        ):
+            headerIdx = closerIdx
+        lastTokenIdx = closer.token
+
         # Length is only used for emphasis-specific "rule of 3",
         # if it's not defined (in strikethrough or 3rd party plugins),
         # we can default it to 0 to disable those checks.
         #
         closer.length = closer.length or 0
 
         if not closer.close:
@@ -28,64 +50,67 @@
         if closer.marker not in openersBottom:
             openersBottom[closer.marker] = [-1, -1, -1, -1, -1, -1]
 
         minOpenerIdx = openersBottom[closer.marker][
             (3 if closer.open else 0) + (closer.length % 3)
         ]
 
-        openerIdx = closerIdx - closer.jump - 1
-
-        # avoid crash if `closer.jump` is pointing outside of the array,
-        # e.g. for strikethrough
-        if openerIdx < -1:
-            openerIdx = -1
+        openerIdx = headerIdx - jumps[headerIdx] - 1
 
         newMinOpenerIdx = openerIdx
 
         while openerIdx > minOpenerIdx:
             opener = delimiters[openerIdx]
 
             if opener.marker != closer.marker:
-                openerIdx -= opener.jump + 1
+                openerIdx -= jumps[openerIdx] + 1
                 continue
 
             if opener.open and opener.end < 0:
                 isOddMatch = False
 
                 # from spec:
                 #
                 # If one of the delimiters can both open and close emphasis, then the
                 # sum of the lengths of the delimiter runs containing the opening and
                 # closing delimiters must not be a multiple of 3 unless both lengths
                 # are multiples of 3.
                 #
-                if opener.close or closer.open:
-                    if (opener.length + closer.length) % 3 == 0:
-                        if opener.length % 3 != 0 or closer.length % 3 != 0:
-                            isOddMatch = True
+                if (
+                    (opener.close or closer.open)
+                    and ((opener.length + closer.length) % 3 == 0)
+                    and (opener.length % 3 != 0 or closer.length % 3 != 0)
+                ):
+                    isOddMatch = True
 
                 if not isOddMatch:
                     # If previous delimiter cannot be an opener, we can safely skip
                     # the entire sequence in future checks. This is required to make
                     # sure algorithm has linear complexity (see *_*_*_*_*_... case).
                     #
                     if openerIdx > 0 and not delimiters[openerIdx - 1].open:
-                        lastJump = delimiters[openerIdx - 1].jump + 1
+                        lastJump = jumps[openerIdx - 1] + 1
                     else:
                         lastJump = 0
 
-                    closer.jump = closerIdx - openerIdx + lastJump
+                    jumps[closerIdx] = closerIdx - openerIdx + lastJump
+                    jumps[openerIdx] = lastJump
+
                     closer.open = False
                     opener.end = closerIdx
-                    opener.jump = lastJump
                     opener.close = False
                     newMinOpenerIdx = -1
+
+                    # treat next token as start of run,
+                    # it optimizes skips in **<...>**a**<...>** pathological case
+                    lastTokenIdx = -2
+
                     break
 
-            openerIdx -= opener.jump + 1
+            openerIdx -= jumps[openerIdx] + 1
 
         if newMinOpenerIdx != -1:
             # If match for this delimiter run failed, we want to set lower bound for
             # future lookups. This is required to make sure algorithm has linear
             # complexity.
             #
             # See details here:
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_inline/emphasis.py` & `markdown-it-py-3.0.0/markdown_it/rules_inline/emphasis.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 # Process *this* and _that_
 #
+from __future__ import annotations
 
 from .state_inline import Delimiter, StateInline
 
 
-def tokenize(state: StateInline, silent: bool):
+def tokenize(state: StateInline, silent: bool) -> bool:
     """Insert each marker as a separate text token, and add it to delimiter list"""
     start = state.pos
-    marker = state.srcCharCode[start]
+    marker = state.src[start]
 
     if silent:
         return False
 
-    # /* _ */  /* * */
-    if marker != 0x5F and marker != 0x2A:
+    if marker not in ("_", "*"):
         return False
 
-    scanned = state.scanDelims(state.pos, marker == 0x2A)
+    scanned = state.scanDelims(state.pos, marker == "*")
 
-    for i in range(scanned.length):
+    for _ in range(scanned.length):
         token = state.push("text", "", 0)
-        token.content = chr(marker)
+        token.content = marker
         state.delimiters.append(
             Delimiter(
-                marker=marker,
+                marker=ord(marker),
                 length=scanned.length,
-                jump=i,
                 token=len(state.tokens) - 1,
                 end=-1,
                 open=scanned.can_open,
                 close=scanned.can_close,
             )
         )
 
     state.pos += scanned.length
 
     return True
 
 
-def _postProcess(state, delimiters):
+def _postProcess(state: StateInline, delimiters: list[Delimiter]) -> None:
     i = len(delimiters) - 1
     while i >= 0:
         startDelim = delimiters[i]
 
         # /* _ */  /* * */
         if startDelim.marker != 0x5F and startDelim.marker != 0x2A:
             i -= 1
@@ -59,17 +58,19 @@
         # merge those into one strong delimiter.
         #
         # `<em><em>whatever</em></em>` -> `<strong>whatever</strong>`
         #
         isStrong = (
             i > 0
             and delimiters[i - 1].end == startDelim.end + 1
+            # check that first two markers match and adjacent
+            and delimiters[i - 1].marker == startDelim.marker
             and delimiters[i - 1].token == startDelim.token - 1
+            # check that last two markers are adjacent (we can safely assume they match)
             and delimiters[startDelim.end + 1].token == endDelim.token + 1
-            and delimiters[i - 1].marker == startDelim.marker
         )
 
         ch = chr(startDelim.marker)
 
         token = state.tokens[startDelim.token]
         token.type = "strong_open" if isStrong else "em_open"
         token.tag = "strong" if isStrong else "em"
@@ -88,14 +89,14 @@
             state.tokens[delimiters[i - 1].token].content = ""
             state.tokens[delimiters[startDelim.end + 1].token].content = ""
             i -= 1
 
         i -= 1
 
 
-def postProcess(state: StateInline):
+def postProcess(state: StateInline) -> None:
     """Walk through delimiter list and replace text tokens with tags."""
     _postProcess(state, state.delimiters)
 
     for token in state.tokens_meta:
         if token and "delimiters" in token:
             _postProcess(state, token["delimiters"])
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_inline/entity.py` & `markdown-it-py-3.0.0/markdown_it/rules_inline/entity.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,49 +5,49 @@
 from ..common.utils import fromCodePoint, isValidEntityCode
 from .state_inline import StateInline
 
 DIGITAL_RE = re.compile(r"^&#((?:x[a-f0-9]{1,6}|[0-9]{1,7}));", re.IGNORECASE)
 NAMED_RE = re.compile(r"^&([a-z][a-z0-9]{1,31});", re.IGNORECASE)
 
 
-def entity(state: StateInline, silent: bool):
+def entity(state: StateInline, silent: bool) -> bool:
     pos = state.pos
     maximum = state.posMax
 
-    if state.srcCharCode[pos] != 0x26:  # /* & */
+    if state.src[pos] != "&":
         return False
 
-    if (pos + 1) < maximum:
-        ch = state.srcCharCode[pos + 1]
+    if pos + 1 >= maximum:
+        return False
+
+    if state.src[pos + 1] == "#":
+        if match := DIGITAL_RE.search(state.src[pos:]):
+            if not silent:
+                match1 = match.group(1)
+                code = (
+                    int(match1[1:], 16) if match1[0].lower() == "x" else int(match1, 10)
+                )
+
+                token = state.push("text_special", "", 0)
+                token.content = (
+                    fromCodePoint(code)
+                    if isValidEntityCode(code)
+                    else fromCodePoint(0xFFFD)
+                )
+                token.markup = match.group(0)
+                token.info = "entity"
+
+            state.pos += len(match.group(0))
+            return True
+
+    else:
+        if (match := NAMED_RE.search(state.src[pos:])) and match.group(1) in entities:
+            if not silent:
+                token = state.push("text_special", "", 0)
+                token.content = entities[match.group(1)]
+                token.markup = match.group(0)
+                token.info = "entity"
+
+            state.pos += len(match.group(0))
+            return True
 
-        if ch == 0x23:  # /* # */
-            match = DIGITAL_RE.search(state.src[pos:])
-            if match:
-                if not silent:
-                    match1 = match.group(1)
-                    code = (
-                        int(match1[1:], 16)
-                        if match1[0].lower() == "x"
-                        else int(match1, 10)
-                    )
-                    state.pending += (
-                        fromCodePoint(code)
-                        if isValidEntityCode(code)
-                        else fromCodePoint(0xFFFD)
-                    )
-
-                state.pos += len(match.group(0))
-                return True
-
-        else:
-            match = NAMED_RE.search(state.src[pos:])
-            if match:
-                if match.group(1) in entities:
-                    if not silent:
-                        state.pending += entities[match.group(1)]
-                    state.pos += len(match.group(0))
-                    return True
-
-    if not silent:
-        state.pending += "&"
-    state.pos += 1
-    return True
+    return False
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_inline/image.py` & `markdown-it-py-3.0.0/markdown_it/rules_inline/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 # Process ![image](<src> "title")
 from __future__ import annotations
 
-from ..common.utils import isSpace, normalizeReference
+from ..common.utils import isStrSpace, normalizeReference
 from ..token import Token
 from .state_inline import StateInline
 
 
-def image(state: StateInline, silent: bool):
+def image(state: StateInline, silent: bool) -> bool:
     label = None
     href = ""
     oldPos = state.pos
     max = state.posMax
 
-    # /* ! */
-    if state.srcCharCode[state.pos] != 0x21:
+    if state.src[state.pos] != "!":
         return False
-    # /* [ */
-    if state.pos + 1 < state.posMax and state.srcCharCode[state.pos + 1] != 0x5B:
+
+    if state.pos + 1 < state.posMax and state.src[state.pos + 1] != "[":
         return False
 
     labelStart = state.pos + 2
     labelEnd = state.md.helpers.parseLinkLabel(state, state.pos + 1, False)
 
     # parser failed to find ']', so it's not a valid link
     if labelEnd < 0:
         return False
 
     pos = labelEnd + 1
-    # /* ( */
-    if pos < max and state.srcCharCode[pos] == 0x28:
+
+    if pos < max and state.src[pos] == "(":
         #
         # Inline link
         #
 
         # [link](  <href>  "title"  )
         #        ^^ skipping these spaces
         pos += 1
         while pos < max:
-            code = state.srcCharCode[pos]
-            if not isSpace(code) and code != 0x0A:
+            ch = state.src[pos]
+            if not isStrSpace(ch) and ch != "\n":
                 break
             pos += 1
 
         if pos >= max:
             return False
 
         # [link](  <href>  "title"  )
@@ -56,52 +55,51 @@
             else:
                 href = ""
 
         # [link](  <href>  "title"  )
         #                ^^ skipping these spaces
         start = pos
         while pos < max:
-            code = state.srcCharCode[pos]
-            if not isSpace(code) and code != 0x0A:
+            ch = state.src[pos]
+            if not isStrSpace(ch) and ch != "\n":
                 break
             pos += 1
 
         # [link](  <href>  "title"  )
         #                  ^^^^^^^ parsing link title
         res = state.md.helpers.parseLinkTitle(state.src, pos, state.posMax)
         if pos < max and start != pos and res.ok:
             title = res.str
             pos = res.pos
 
             # [link](  <href>  "title"  )
             #                         ^^ skipping these spaces
             while pos < max:
-                code = state.srcCharCode[pos]
-                if not isSpace(code) and code != 0x0A:
+                ch = state.src[pos]
+                if not isStrSpace(ch) and ch != "\n":
                     break
                 pos += 1
         else:
             title = ""
 
-        # /* ) */
-        if pos >= max or state.srcCharCode[pos] != 0x29:
+        if pos >= max or state.src[pos] != ")":
             state.pos = oldPos
             return False
 
         pos += 1
 
     else:
         #
         # Link reference
         #
         if "references" not in state.env:
             return False
 
         # /* [ */
-        if pos < max and state.srcCharCode[pos] == 0x5B:
+        if pos < max and state.src[pos] == "[":
             start = pos + 1
             pos = state.md.helpers.parseLinkLabel(state, pos)
             if pos >= 0:
                 label = state.src[start:pos]
                 pos += 1
             else:
                 pos = labelEnd + 1
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_inline/link.py` & `markdown-it-py-3.0.0/markdown_it/rules_inline/link.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # Process [link](<to> "stuff")
 
-from ..common.utils import isSpace, normalizeReference
+from ..common.utils import isStrSpace, normalizeReference
 from .state_inline import StateInline
 
 
-def link(state: StateInline, silent: bool):
+def link(state: StateInline, silent: bool) -> bool:
     href = ""
     title = ""
     label = None
     oldPos = state.pos
     maximum = state.posMax
     start = state.pos
     parseReference = True
 
-    if state.srcCharCode[state.pos] != 0x5B:  # /* [ */
+    if state.src[state.pos] != "[":
         return False
 
     labelStart = state.pos + 1
     labelEnd = state.md.helpers.parseLinkLabel(state, state.pos, True)
 
     # parser failed to find ']', so it's not a valid link
     if labelEnd < 0:
         return False
 
     pos = labelEnd + 1
 
-    if pos < maximum and state.srcCharCode[pos] == 0x28:  # /* ( */
+    if pos < maximum and state.src[pos] == "(":
         #
         # Inline link
         #
 
         # might have found a valid shortcut link, disable reference parsing
         parseReference = False
 
         # [link](  <href>  "title"  )
         #        ^^ skipping these spaces
         pos += 1
         while pos < maximum:
-            code = state.srcCharCode[pos]
-            if not isSpace(code) and code != 0x0A:
+            ch = state.src[pos]
+            if not isStrSpace(ch) and ch != "\n":
                 break
             pos += 1
 
         if pos >= maximum:
             return False
 
         # [link](  <href>  "title"  )
@@ -56,48 +56,48 @@
             else:
                 href = ""
 
             # [link](  <href>  "title"  )
             #                ^^ skipping these spaces
             start = pos
             while pos < maximum:
-                code = state.srcCharCode[pos]
-                if not isSpace(code) and code != 0x0A:
+                ch = state.src[pos]
+                if not isStrSpace(ch) and ch != "\n":
                     break
                 pos += 1
 
             # [link](  <href>  "title"  )
             #                  ^^^^^^^ parsing link title
             res = state.md.helpers.parseLinkTitle(state.src, pos, state.posMax)
             if pos < maximum and start != pos and res.ok:
                 title = res.str
                 pos = res.pos
 
                 # [link](  <href>  "title"  )
                 #                         ^^ skipping these spaces
                 while pos < maximum:
-                    code = state.srcCharCode[pos]
-                    if not isSpace(code) and code != 0x0A:
+                    ch = state.src[pos]
+                    if not isStrSpace(ch) and ch != "\n":
                         break
                     pos += 1
 
-        if pos >= maximum or state.srcCharCode[pos] != 0x29:  # /* ) */
+        if pos >= maximum or state.src[pos] != ")":
             # parsing a valid shortcut link failed, fallback to reference
             parseReference = True
 
         pos += 1
 
     if parseReference:
         #
         # Link reference
         #
         if "references" not in state.env:
             return False
 
-        if pos < maximum and state.srcCharCode[pos] == 0x5B:  # /* [ */
+        if pos < maximum and state.src[pos] == "[":
             start = pos + 1
             pos = state.md.helpers.parseLinkLabel(state, pos)
             if pos >= 0:
                 label = state.src[start:pos]
                 pos += 1
             else:
                 pos = labelEnd + 1
@@ -136,14 +136,16 @@
         if title:
             token.attrSet("title", title)
 
         # note, this is not part of markdown-it JS, but is useful for renderers
         if label and state.md.options.get("store_labels", False):
             token.meta["label"] = label
 
+        state.linkLevel += 1
         state.md.inline.tokenize(state)
+        state.linkLevel -= 1
 
         token = state.push("link_close", "a", -1)
 
     state.pos = pos
     state.posMax = maximum
     return True
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_inline/newline.py` & `markdown-it-py-3.0.0/markdown_it/rules_inline/newline.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# Proceess '\n'
-import re
-
-from ..common.utils import charCodeAt, isSpace
+"""Proceess '\n'."""
+from ..common.utils import charStrAt, isStrSpace
 from .state_inline import StateInline
 
-endSpace = re.compile(r" +$")
-
 
-def newline(state: StateInline, silent: bool):
+def newline(state: StateInline, silent: bool) -> bool:
     pos = state.pos
 
-    # /* \n */
-    if state.srcCharCode[pos] != 0x0A:
+    if state.src[pos] != "\n":
         return False
 
     pmax = len(state.pending) - 1
     maximum = state.posMax
 
     # '  \n' -> hardbreak
     # Lookup in pending chars is bad practice! Don't copy to other rules!
     # Pending string is stored in concat mode, indexed lookups will cause
     # conversion to flat mode.
     if not silent:
-        if pmax >= 0 and charCodeAt(state.pending, pmax) == 0x20:
-            if pmax >= 1 and charCodeAt(state.pending, pmax - 1) == 0x20:
-                state.pending = endSpace.sub("", state.pending)
+        if pmax >= 0 and charStrAt(state.pending, pmax) == " ":
+            if pmax >= 1 and charStrAt(state.pending, pmax - 1) == " ":
+                # Find whitespaces tail of pending chars.
+                ws = pmax - 1
+                while ws >= 1 and charStrAt(state.pending, ws - 1) == " ":
+                    ws -= 1
+                state.pending = state.pending[:ws]
+
                 state.push("hardbreak", "br", 0)
             else:
                 state.pending = state.pending[:-1]
                 state.push("softbreak", "br", 0)
 
         else:
             state.push("softbreak", "br", 0)
 
     pos += 1
 
     # skip heading spaces for next line
-    while pos < maximum and isSpace(state.srcCharCode[pos]):
+    while pos < maximum and isStrSpace(state.src[pos]):
         pos += 1
 
     state.pos = pos
     return True
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_inline/state_inline.py` & `markdown-it-py-3.0.0/markdown_it/rules_inline/state_inline.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 from __future__ import annotations
 
 from collections import namedtuple
-from collections.abc import MutableMapping
 from dataclasses import dataclass
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Literal
 
 from .._compat import DATACLASS_KWARGS
 from ..common.utils import isMdAsciiPunct, isPunctChar, isWhiteSpace
 from ..ruler import StateBase
 from ..token import Token
+from ..utils import EnvType
 
 if TYPE_CHECKING:
     from markdown_it import MarkdownIt
 
 
 @dataclass(**DATACLASS_KWARGS)
 class Delimiter:
     # Char code of the starting marker (number).
     marker: int
 
     # Total length of these series of delimiters.
     length: int
 
-    # An amount of characters before this one that's equivalent to
-    # current one. In plain English: if this delimiter does not open
-    # an emphasis, neither do previous `jump` characters.
-    #
-    # Used to skip sequences like "*****" in one step, for 1st asterisk
-    # value will be 0, for 2nd it's 1 and so on.
-    jump: int
-
     # A position of the token this delimiter corresponds to.
     token: int
 
     # If this delimiter is matched as a valid opener, `end` will be
     # equal to its position, otherwise it's `-1`.
     end: int
 
@@ -46,21 +38,21 @@
 
 
 Scanned = namedtuple("Scanned", ["can_open", "can_close", "length"])
 
 
 class StateInline(StateBase):
     def __init__(
-        self, src: str, md: MarkdownIt, env: MutableMapping, outTokens: list[Token]
-    ):
+        self, src: str, md: MarkdownIt, env: EnvType, outTokens: list[Token]
+    ) -> None:
         self.src = src
         self.env = env
         self.md = md
         self.tokens = outTokens
-        self.tokens_meta: list[dict | None] = [None] * len(outTokens)
+        self.tokens_meta: list[dict[str, Any] | None] = [None] * len(outTokens)
 
         self.pos = 0
         self.posMax = len(self.src)
         self.level = 0
         self.pending = ""
         self.pendingLevel = 0
 
@@ -74,29 +66,33 @@
         # Stack of delimiter lists for upper level tags
         self._prev_delimiters: list[list[Delimiter]] = []
 
         # backticklength => last seen position
         self.backticks: dict[int, int] = {}
         self.backticksScanned = False
 
-    def __repr__(self):
+        # Counter used to disable inline linkify-it execution
+        # inside <a> and markdown links
+        self.linkLevel = 0
+
+    def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}"
             f"(pos=[{self.pos} of {self.posMax}], token={len(self.tokens)})"
         )
 
-    def pushPending(self):
+    def pushPending(self) -> Token:
         token = Token("text", "", 0)
         token.content = self.pending
         token.level = self.pendingLevel
         self.tokens.append(token)
         self.pending = ""
         return token
 
-    def push(self, ttype, tag, nesting):
+    def push(self, ttype: str, tag: str, nesting: Literal[-1, 0, 1]) -> Token:
         """Push new token to "stream".
         If pending text exists - flush it as text token
         """
         if self.pending:
             self.pushPending()
 
         token = Token(ttype, tag, nesting)
@@ -117,57 +113,52 @@
             token_meta = {"delimiters": self.delimiters}
 
         self.pendingLevel = self.level
         self.tokens.append(token)
         self.tokens_meta.append(token_meta)
         return token
 
-    def scanDelims(self, start, canSplitWord):
+    def scanDelims(self, start: int, canSplitWord: bool) -> Scanned:
         """
         Scan a sequence of emphasis-like markers, and determine whether
         it can start an emphasis sequence or end an emphasis sequence.
 
          - start - position to scan from (it should point at a valid marker);
          - canSplitWord - determine if these markers can be found inside a word
 
         """
         pos = start
-        left_flanking = True
-        right_flanking = True
         maximum = self.posMax
-        marker = self.srcCharCode[start]
+        marker = self.src[start]
 
         # treat beginning of the line as a whitespace
-        lastChar = self.srcCharCode[start - 1] if start > 0 else 0x20
+        lastChar = self.src[start - 1] if start > 0 else " "
 
-        while pos < maximum and self.srcCharCode[pos] == marker:
+        while pos < maximum and self.src[pos] == marker:
             pos += 1
 
         count = pos - start
 
         # treat end of the line as a whitespace
-        nextChar = self.srcCharCode[pos] if pos < maximum else 0x20
+        nextChar = self.src[pos] if pos < maximum else " "
 
-        isLastPunctChar = isMdAsciiPunct(lastChar) or isPunctChar(chr(lastChar))
-        isNextPunctChar = isMdAsciiPunct(nextChar) or isPunctChar(chr(nextChar))
+        isLastPunctChar = isMdAsciiPunct(ord(lastChar)) or isPunctChar(lastChar)
+        isNextPunctChar = isMdAsciiPunct(ord(nextChar)) or isPunctChar(nextChar)
 
-        isLastWhiteSpace = isWhiteSpace(lastChar)
-        isNextWhiteSpace = isWhiteSpace(nextChar)
+        isLastWhiteSpace = isWhiteSpace(ord(lastChar))
+        isNextWhiteSpace = isWhiteSpace(ord(nextChar))
 
-        if isNextWhiteSpace:
-            left_flanking = False
-        elif isNextPunctChar:
-            if not (isLastWhiteSpace or isLastPunctChar):
-                left_flanking = False
-
-        if isLastWhiteSpace:
-            right_flanking = False
-        elif isLastPunctChar:
-            if not (isNextWhiteSpace or isNextPunctChar):
-                right_flanking = False
+        left_flanking = not (
+            isNextWhiteSpace
+            or (isNextPunctChar and not (isLastWhiteSpace or isLastPunctChar))
+        )
+        right_flanking = not (
+            isLastWhiteSpace
+            or (isLastPunctChar and not (isNextWhiteSpace or isNextPunctChar))
+        )
 
         if not canSplitWord:
             can_open = left_flanking and ((not right_flanking) or isLastPunctChar)
             can_close = right_flanking and ((not left_flanking) or isNextPunctChar)
         else:
             can_open = left_flanking
             can_close = right_flanking
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_inline/strikethrough.py` & `markdown-it-py-3.0.0/markdown_it/rules_inline/strikethrough.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # ~~strike through~~
 from __future__ import annotations
 
 from .state_inline import Delimiter, StateInline
 
 
-def tokenize(state: StateInline, silent: bool):
+def tokenize(state: StateInline, silent: bool) -> bool:
     """Insert each marker as a separate text token, and add it to delimiter list"""
     start = state.pos
-    marker = state.srcCharCode[start]
+    ch = state.src[start]
 
     if silent:
         return False
 
-    if marker != 0x7E:  # /* ~ */
+    if ch != "~":
         return False
 
     scanned = state.scanDelims(state.pos, True)
     length = scanned.length
-    ch = chr(marker)
 
     if length < 2:
         return False
 
     if length % 2:
         token = state.push("text", "", 0)
         token.content = ch
@@ -29,34 +28,31 @@
 
     i = 0
     while i < length:
         token = state.push("text", "", 0)
         token.content = ch + ch
         state.delimiters.append(
             Delimiter(
-                **{
-                    "marker": marker,
-                    "length": 0,  # disable "rule of 3" length checks meant for emphasis
-                    "jump": i // 2,  # for `~~` 1 marker = 2 characters
-                    "token": len(state.tokens) - 1,
-                    "end": -1,
-                    "open": scanned.can_open,
-                    "close": scanned.can_close,
-                }
+                marker=ord(ch),
+                length=0,  # disable "rule of 3" length checks meant for emphasis
+                token=len(state.tokens) - 1,
+                end=-1,
+                open=scanned.can_open,
+                close=scanned.can_close,
             )
         )
 
         i += 2
 
     state.pos += scanned.length
 
     return True
 
 
-def _postProcess(state: StateInline, delimiters: list[Delimiter]):
+def _postProcess(state: StateInline, delimiters: list[Delimiter]) -> None:
     loneMarkers = []
     maximum = len(delimiters)
 
     i = 0
     while i < maximum:
         startDelim = delimiters[i]
 
@@ -109,15 +105,15 @@
 
         if i != j:
             token = state.tokens[j]
             state.tokens[j] = state.tokens[i]
             state.tokens[i] = token
 
 
-def postProcess(state: StateInline):
+def postProcess(state: StateInline) -> None:
     """Walk through delimiter list and replace text tokens with tags."""
     tokens_meta = state.tokens_meta
     maximum = len(state.tokens_meta)
     _postProcess(state, state.delimiters)
 
     curr = 0
     while curr < maximum:
```

### Comparing `markdown-it-py-2.2.0/markdown_it/rules_inline/text_collapse.py` & `markdown-it-py-3.0.0/markdown_it/rules_inline/fragments_join.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .state_inline import StateInline
 
 
-def text_collapse(state: StateInline, *args):
+def fragments_join(state: StateInline) -> None:
     """
     Clean up tokens after emphasis and strikethrough postprocessing:
     merge adjacent text nodes into one and re-calculate all token levels
 
     This is necessary because initially emphasis delimiter markers (``*, _, ~``)
     are treated as their own separate text tokens. Then emphasis rule either
     leaves them as text (needed to merge with adjacent text) or turns them
```

### Comparing `markdown-it-py-2.2.0/markdown_it/token.py` & `markdown-it-py-3.0.0/markdown_it/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from collections.abc import Callable, MutableMapping
 import dataclasses as dc
-from typing import Any
+from typing import Any, Literal
 import warnings
 
 from markdown_it._compat import DATACLASS_KWARGS
 
 
 def convert_attrs(value: Any) -> Any:
     """Convert Token.attrs set as ``None`` or ``[[key, value], ...]`` to a dict.
@@ -24,15 +24,15 @@
 class Token:
     type: str
     """Type of the token (string, e.g. "paragraph_open")"""
 
     tag: str
     """HTML tag name, e.g. 'p'"""
 
-    nesting: int
+    nesting: Literal[-1, 0, 1]
     """Level change (number in {-1, 0, 1} set), where:
     -  `1` means the tag is opening
     -  `0` means the tag is self-closing
     - `-1` means the tag is closing
     """
 
     attrs: dict[str, str | int | float] = dc.field(default_factory=dict)
@@ -59,32 +59,32 @@
     info: str = ""
     """Additional information:
     - Info string for "fence" tokens
     - The value "auto" for autolink "link_open" and "link_close" tokens
     - The string value of the item marker for ordered-list "list_item_open" tokens
     """
 
-    meta: dict = dc.field(default_factory=dict)
+    meta: dict[Any, Any] = dc.field(default_factory=dict)
     """A place for plugins to store any arbitrary data"""
 
     block: bool = False
     """True for block-level tokens, false for inline tokens.
     Used in renderer to calculate line breaks
     """
 
     hidden: bool = False
     """If true, ignore this element when rendering.
     Used for tight lists to hide paragraphs.
     """
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.attrs = convert_attrs(self.attrs)
 
     def attrIndex(self, name: str) -> int:
-        warnings.warn(
+        warnings.warn(  # noqa: B028
             "Token.attrIndex should not be used, since Token.attrs is a dictionary",
             UserWarning,
         )
         if name not in self.attrs:
             return -1
         return list(self.attrs.keys()).index(name)
 
@@ -125,15 +125,15 @@
         return dc.replace(self, **changes)
 
     def as_dict(
         self,
         *,
         children: bool = True,
         as_upstream: bool = True,
-        meta_serializer: Callable[[dict], Any] | None = None,
+        meta_serializer: Callable[[dict[Any, Any]], Any] | None = None,
         filter: Callable[[str, Any], bool] | None = None,
         dict_factory: Callable[..., MutableMapping[str, Any]] = dict,
     ) -> MutableMapping[str, Any]:
         """Return the token as a dictionary.
 
         :param children: Also convert children to dicts
         :param as_upstream: Ensure the output dictionary is equal to that created by markdown-it
```

### Comparing `markdown-it-py-2.2.0/markdown_it/tree.py` & `markdown-it-py-3.0.0/markdown_it/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from __future__ import annotations
 
 from collections.abc import Generator, Sequence
 import textwrap
 from typing import Any, NamedTuple, TypeVar, overload
 
 from .token import Token
-from .utils import _removesuffix
 
 
 class _NesterTokens(NamedTuple):
     opening: Token
     closing: Token
 
 
@@ -47,15 +46,15 @@
         self.nester_tokens: _NesterTokens | None = None
 
         # Root node does not have self.parent
         self._parent: Any = None
 
         # Empty list unless a non-empty container, or unnested token that has
         # children (i.e. inline or img)
-        self._children: list = []
+        self._children: list[Any] = []
 
         if create_root:
             self._set_children_from_tokens(tokens)
             return
 
         if not tokens:
             raise ValueError(
@@ -115,15 +114,15 @@
 
     @children.setter
     def children(self: _NodeType, value: list[_NodeType]) -> None:
         self._children = value
 
     @property
     def parent(self: _NodeType) -> _NodeType | None:
-        return self._parent
+        return self._parent  # type: ignore
 
     @parent.setter
     def parent(self: _NodeType, value: _NodeType | None) -> None:
         self._parent = value
 
     @property
     def is_root(self) -> bool:
@@ -226,15 +225,20 @@
     ) -> str:
         """Create an XML style string of the tree."""
         prefix = " " * _current
         text = prefix + f"<{self.type}"
         if not self.is_root and self.attrs:
             text += " " + " ".join(f"{k}={v!r}" for k, v in self.attrs.items())
         text += ">"
-        if show_text and not self.is_root and self.type == "text" and self.content:
+        if (
+            show_text
+            and not self.is_root
+            and self.type in ("text", "text_special")
+            and self.content
+        ):
             text += "\n" + textwrap.indent(self.content, prefix + " " * indent)
         for child in self.children:
             text += "\n" + child.pretty(
                 indent=indent, show_text=show_text, _current=_current + indent
             )
         return text
 
@@ -310,21 +314,32 @@
 
     @property
     def info(self) -> str:
         """fence infostring"""
         return self._attribute_token().info
 
     @property
-    def meta(self) -> dict:
+    def meta(self) -> dict[Any, Any]:
         """A place for plugins to store an arbitrary data."""
         return self._attribute_token().meta
 
     @property
     def block(self) -> bool:
         """True for block-level tokens, false for inline tokens."""
         return self._attribute_token().block
 
     @property
     def hidden(self) -> bool:
         """If it's true, ignore this element when rendering.
         Used for tight lists to hide paragraphs."""
         return self._attribute_token().hidden
+
+
+def _removesuffix(string: str, suffix: str) -> str:
+    """Remove a suffix from a string.
+
+    Replace this with str.removesuffix() from stdlib when minimum Python
+    version is 3.9.
+    """
+    if suffix and string.endswith(suffix):
+        return string[: -len(suffix)]
+    return string
```

### Comparing `markdown-it-py-2.2.0/pyproject.toml` & `markdown-it-py-3.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 authors = [{name = "Chris Sewell", email = "chrisj_sewell@hotmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: Markup",
 ]
 keywords = ["markdown", "lexer", "parser", "commonmark", "markdown-it"]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "mdurl~=0.1",
-    "typing_extensions>=3.7.4;python_version<'3.8'",
 ]
 
 [project.urls]
 Homepage = "https://github.com/executablebooks/markdown-it-py"
 Documentation = "https://markdown-it-py.readthedocs.io"
 
 [project.optional-dependencies]
@@ -42,21 +41,22 @@
     "mistletoe~=1.0",
     "mistune~=2.0",
     "panflute~=2.3",
 ]
 linkify = ["linkify-it-py>=1,<3"]
 plugins = ["mdit-py-plugins"]
 rtd = [
-    "attrs",
+    "mdit-py-plugins",
     "myst-parser",
     "pyyaml",
     "sphinx",
     "sphinx-copybutton",
     "sphinx-design",
     "sphinx_book_theme",
+    "jupyter_sphinx",
 ]
 testing = [
     "coverage",
     "pytest",
     "pytest-cov",
     "pytest-regressions",
 ]
@@ -80,21 +80,29 @@
     "benchmarking/"
 ]
 
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
 
+[tool.ruff]
+line-length = 100
+extend-select = ["B0", "C4", "ICN", "ISC", "N", "RUF", "SIM"]
+extend-ignore = ["ISC003", "N802", "N803", "N806", "N816", "RUF003"]
+
 [tool.mypy]
 show_error_codes = true
 warn_unused_ignores = true
 warn_redundant_casts = true
-no_implicit_optional = true
-strict_equality = true
-implicit_reexport = false
+strict = true
+
+[[tool.mypy.overrides]]
+module = ["tests.*"]
+disallow_untyped_calls = false
+disallow_untyped_defs = false
 
 [[tool.mypy.overrides]]
 module = ["tests.test_plugins.*", "markdown.*"]
 ignore_errors = true
 
 [[tool.mypy.overrides]]
 module = ["markdown.*"]
```

### Comparing `markdown-it-py-2.2.0/tox.ini` & `markdown-it-py-3.0.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # To use tox, see https://tox.readthedocs.io
 # Simply pip or conda install tox
 # If you use conda, you may also want to install tox-conda
 # then run `tox` or `tox -- {pytest args}`
 # run in parallel using `tox -p`
 [tox]
-envlist = py37
+envlist = py38
 
 [testenv]
 usedevelop = true
 
-[testenv:py{37,38,39,310}]
+[testenv:py{38,39,310,311}]
 extras =
     linkify
     testing
 commands = pytest {posargs:tests/}
 
-[testenv:py{37,38,39,310}-plugins]
+[testenv:py{38,39,310,311}-plugins]
 extras = testing
 changedir = {envtmpdir}
 allowlist_externals =
     git
     pip
 commands_pre =
     git clone https://github.com/executablebooks/mdit-py-plugins.git
     pip install --no-deps -e mdit-py-plugins
 commands =
     pytest {posargs}
 
-[testenv:py{37,38,39}-bench-core]
+[testenv:py{38,39,310,311}-bench-core]
 extras = benchmarking
 commands = pytest benchmarking/bench_core.py {posargs}
 
-[testenv:py{37,38}-bench-packages]
+[testenv:py{38,39,310,311}-bench-packages]
 extras = benchmarking,compare
 commands = pytest benchmarking/bench_packages.py {posargs}
 
 [testenv:docs-{update,clean}]
 extras = linkify,plugins,rtd
 whitelist_externals =
     echo
@@ -51,15 +51,18 @@
 description = run profiler (use e.g. `firefox .tox/prof/output.svg` to open)
 extras = profiling
 allowlist_externals =
     mkdir
     dot
 commands =
     mkdir -p "{toxworkdir}/prof"
-    python -m cProfile -o "{toxworkdir}/prof/output.pstats" profiler.py
+    python -m cProfile -o "{toxworkdir}/prof/output.pstats" scripts/profiler.py
     gprof2dot -f pstats -o "{toxworkdir}/prof/output.dot" "{toxworkdir}/prof/output.pstats"
     dot -Tsvg -o "{toxworkdir}/prof/output.svg" "{toxworkdir}/prof/output.dot"
     python -c 'import pathlib; print("profiler svg output under file://\{0\}".format(pathlib.Path(r"{toxworkdir}") / "prof" / "output.svg"))'
 
-[flake8]
-max-line-length = 100
-extend-ignore = E203
+[testenv:fuzz]
+description = run fuzzer on testcase file
+; See: https://google.github.io/oss-fuzz/
+deps = atheris
+commands_pre = python scripts/build_fuzzers.py {envdir}/oss-fuzz
+commands = python {envdir}/oss-fuzz/infra/helper.py reproduce markdown-it-py fuzz_markdown {posargs:testcase}
```

### Comparing `markdown-it-py-2.2.0/PKG-INFO` & `markdown-it-py-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: markdown-it-py
-Version: 2.2.0
+Version: 3.0.0
 Summary: Python port of markdown-it. Markdown parsing, done right!
 Keywords: markdown,lexer,parser,commonmark,markdown-it
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Requires-Dist: mdurl~=0.1
-Requires-Dist: typing_extensions>=3.7.4;python_version<'3.8'
 Requires-Dist: psutil ; extra == "benchmarking"
 Requires-Dist: pytest ; extra == "benchmarking"
 Requires-Dist: pytest-benchmark ; extra == "benchmarking"
 Requires-Dist: pre-commit~=3.0 ; extra == "code_style"
 Requires-Dist: commonmark~=0.9 ; extra == "compare"
 Requires-Dist: markdown~=3.4 ; extra == "compare"
 Requires-Dist: mistletoe~=1.0 ; extra == "compare"
 Requires-Dist: mistune~=2.0 ; extra == "compare"
 Requires-Dist: panflute~=2.3 ; extra == "compare"
 Requires-Dist: linkify-it-py>=1,<3 ; extra == "linkify"
 Requires-Dist: mdit-py-plugins ; extra == "plugins"
 Requires-Dist: gprof2dot ; extra == "profiling"
-Requires-Dist: attrs ; extra == "rtd"
+Requires-Dist: mdit-py-plugins ; extra == "rtd"
 Requires-Dist: myst-parser ; extra == "rtd"
 Requires-Dist: pyyaml ; extra == "rtd"
 Requires-Dist: sphinx ; extra == "rtd"
 Requires-Dist: sphinx-copybutton ; extra == "rtd"
 Requires-Dist: sphinx-design ; extra == "rtd"
 Requires-Dist: sphinx_book_theme ; extra == "rtd"
+Requires-Dist: jupyter_sphinx ; extra == "rtd"
 Requires-Dist: coverage ; extra == "testing"
 Requires-Dist: pytest ; extra == "testing"
 Requires-Dist: pytest-cov ; extra == "testing"
 Requires-Dist: pytest-regressions ; extra == "testing"
 Project-URL: Documentation, https://markdown-it-py.readthedocs.io
 Project-URL: Homepage, https://github.com/executablebooks/markdown-it-py
 Provides-Extra: benchmarking
@@ -66,14 +66,15 @@
 > Markdown parser done right.
 
 - Follows the __[CommonMark spec](http://spec.commonmark.org/)__ for baseline parsing
 - Configurable syntax: you can add new rules and even replace existing ones.
 - Pluggable: Adds syntax extensions to extend the parser (see the [plugin list][md-plugins]).
 - High speed (see our [benchmarking tests][md-performance])
 - [Safe by default][md-security]
+- Member of [Google's Assured Open Source Software](https://cloud.google.com/assured-open-source-software/docs/supported-packages)
 
 This is a Python port of [markdown-it], and some of its associated plugins.
 For more details see: <https://markdown-it-py.readthedocs.io>.
 
 For details on [markdown-it] itself, see:
 
 - The __[Live demo](https://markdown-it.github.io)__
```

