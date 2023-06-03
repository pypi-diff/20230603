# Comparing `tmp/aind_metadata_service-0.4.7.tar.gz` & `tmp/aind_metadata_service-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_service-0.4.7.tar", last modified: Fri Jun  2 18:49:08 2023, max compression
+gzip compressed data, was "aind_metadata_service-0.4.8.tar", last modified: Sat Jun  3 00:35:56 2023, max compression
```

## Comparing `aind_metadata_service-0.4.7.tar` & `aind_metadata_service-0.4.8.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.905799 aind_metadata_service-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.889798 aind_metadata_service-0.4.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.893799 aind_metadata_service-0.4.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.893799 aind_metadata_service-0.4.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-02 18:49:08.905799 aind_metadata_service-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.893799 aind_metadata_service-0.4.7/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.893799 aind_metadata_service-0.4.7/doc_template/source/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/doc_template/source/aind_metadata_service.labtracks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/doc_template/source/aind_metadata_service.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/doc_template/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 18:49:08.905799 aind_metadata_service-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.889798 aind_metadata_service-0.4.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.893799 aind_metadata_service-0.4.7/src/aind_metadata_service/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.893799 aind_metadata_service-0.4.7/src/aind_metadata_service/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13629 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/labtracks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/labtracks/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.897799 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.897799 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66243 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.897799 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113149 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    57053 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/procedures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.893799 aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-02 18:49:08.000000 aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-02 18:49:08.000000 aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:49:08.000000 aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-02 18:49:08.000000 aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 18:49:08.000000 aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.897799 aind_metadata_service-0.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.897799 aind_metadata_service-0.4.7/tests/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/labtracks/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/labtracks/test_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/labtracks/test_response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.889798 aind_metadata_service-0.4.7/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.897799 aind_metadata_service-0.4.7/tests/resources/json_responses/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/json_responses/combined.json
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/json_responses/mapped_las_procedure.json
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/json_responses/mapped_sp_procedure.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.889798 aind_metadata_service-0.4.7/tests/resources/sharepoint/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.889798 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.901799 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item19.json
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.901799 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item19.json
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.889798 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.901799 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item18.json
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.905799 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item18.json
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.905799 aind_metadata_service-0.4.7/tests/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.905799 aind_metadata_service-0.4.7/tests/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/nsb2019/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/nsb2019/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:49:08.905799 aind_metadata_service-0.4.7/tests/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/nsb2023/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/nsb2023/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/sharepoint/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-06-02 18:48:48.000000 aind_metadata_service-0.4.7/tests/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.042134 aind_metadata_service-0.4.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/doc_template/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/doc_template/source/aind_metadata_service.labtracks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/doc_template/source/aind_metadata_service.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/doc_template/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.042134 aind_metadata_service-0.4.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/src/aind_metadata_service/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-03 00:35:37.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/src/aind_metadata_service/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13629 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/labtracks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/labtracks/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66243 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.050134 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113301 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57053 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.046134 aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-03 00:35:56.000000 aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-03 00:35:56.000000 aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 00:35:56.000000 aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-03 00:35:56.000000 aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 00:35:56.000000 aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.050134 aind_metadata_service-0.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.050134 aind_metadata_service-0.4.8/tests/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/labtracks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/labtracks/test_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/labtracks/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.042134 aind_metadata_service-0.4.8/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.050134 aind_metadata_service-0.4.8/tests/resources/json_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/json_responses/combined.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/json_responses/mapped_las_procedure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/json_responses/mapped_sp_procedure.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.042134 aind_metadata_service-0.4.8/tests/resources/sharepoint/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.042134 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.050134 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item19.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.050134 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item19.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.042134 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item18.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item18.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/tests/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/tests/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/nsb2019/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/nsb2019/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 00:35:56.054134 aind_metadata_service-0.4.8/tests/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/nsb2023/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/nsb2023/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/sharepoint/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-06-03 00:35:36.000000 aind_metadata_service-0.4.8/tests/test_response_handler.py
```

### Comparing `aind_metadata_service-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_service-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_service-0.4.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_service-0.4.8/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/.github/workflows/ci.yml` & `aind_metadata_service-0.4.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/.github/workflows/publish.yml` & `aind_metadata_service-0.4.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/.gitignore` & `aind_metadata_service-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/Dockerfile` & `aind_metadata_service-0.4.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/LICENSE` & `aind_metadata_service-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/PKG-INFO` & `aind_metadata_service-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_metadata_service
-Version: 0.4.7
+Version: 0.4.8
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.7/README.md` & `aind_metadata_service-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/doc_template/Makefile` & `aind_metadata_service-0.4.8/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/doc_template/make.bat` & `aind_metadata_service-0.4.8/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/doc_template/source/aind_metadata_service.labtracks.rst` & `aind_metadata_service-0.4.8/doc_template/source/aind_metadata_service.labtracks.rst`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/doc_template/source/conf.py` & `aind_metadata_service-0.4.8/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/pyproject.toml` & `aind_metadata_service-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/src/aind_metadata_service/client.py` & `aind_metadata_service-0.4.8/src/aind_metadata_service/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/src/aind_metadata_service/labtracks/client.py` & `aind_metadata_service-0.4.8/src/aind_metadata_service/labtracks/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/src/aind_metadata_service/labtracks/query_builder.py` & `aind_metadata_service-0.4.8/src/aind_metadata_service/labtracks/query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/src/aind_metadata_service/response_handler.py` & `aind_metadata_service-0.4.8/src/aind_metadata_service/response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/src/aind_metadata_service/server.py` & `aind_metadata_service-0.4.8/src/aind_metadata_service/server.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/client.py` & `aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/mapping.py` & `aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/models.py` & `aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2019/procedures.py` & `aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2019/procedures.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/mapping.py` & `aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -2266,14 +2266,15 @@
         if during == During.FOLLOW_UP:
             if inj_type == InjectionType.NANOJECT:
                 instrument_id = self.aind_nanoject_number_inj2
             elif inj_type == InjectionType.IONTOPHORESIS:
                 instrument_id = self.aind_ionto_number_inj2
             else:
                 instrument_id = None
+            # backend fields titled "1st injection" correlate with followup procedures
             return SurgeryDuringInfo(
                 anaesthetic_duration_in_minutes=(
                     self.aind_first_injection_iso_durat
                 ),
                 anaesthetic_level=self.aind_round1_inj_isolevel,
                 start_date=self.aind_date1st_injection,
                 workstation_id=self.aind_work_station1st_injection,
@@ -2285,19 +2286,20 @@
         elif during == During.INITIAL:
             if inj_type == InjectionType.NANOJECT:
                 instrument_id = self.aind_nanoject_number_inj10
             elif inj_type == InjectionType.IONTOPHORESIS:
                 instrument_id = self.aind_ionto_number_inj1
             else:
                 instrument_id = None
+            # backend fields titled "HP" correlate with initial procedures
             return SurgeryDuringInfo(
                 anaesthetic_duration_in_minutes=self.aind_iso_on,
                 anaesthetic_level=self.aind_hp_iso_level,
                 start_date=self.aind_date_of_surgery,
-                workstation_id=self.aind_work_station1st_injection,
+                workstation_id=self.aind_hp_work_station,
                 recovery_time=self.aind_hp_recovery,
                 weight_prior=self.aind_weight_before_surger,
                 weight_post=self.aind_weight_after_surgery,
                 instrument_id=instrument_id,
             )
         else:
             return SurgeryDuringInfo()
```

### Comparing `aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/models.py` & `aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/src/aind_metadata_service/sharepoint/nsb2023/procedures.py` & `aind_metadata_service-0.4.8/src/aind_metadata_service/sharepoint/nsb2023/procedures.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/PKG-INFO` & `aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-service
-Version: 0.4.7
+Version: 0.4.8
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.7/src/aind_metadata_service.egg-info/SOURCES.txt` & `aind_metadata_service-0.4.8/src/aind_metadata_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/labtracks/test_client.py` & `aind_metadata_service-0.4.8/tests/labtracks/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/labtracks/test_query_builder.py` & `aind_metadata_service-0.4.8/tests/labtracks/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/labtracks/test_response_handler.py` & `aind_metadata_service-0.4.8/tests/labtracks/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/json_responses/combined.json` & `aind_metadata_service-0.4.8/tests/resources/json_responses/combined.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/json_responses/mapped_las_procedure.json` & `aind_metadata_service-0.4.8/tests/resources/json_responses/mapped_las_procedure.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/json_responses/mapped_sp_procedure.json` & `aind_metadata_service-0.4.8/tests/resources/json_responses/mapped_sp_procedure.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item1.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item12.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item12.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item19.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item19.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item2.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item3.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item4.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item5.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item6.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2019/raw/list_item7.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2019/raw/list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692307%*

 * *Differences: {'0': "{'workstation_id': 'SWS 4'}"}*

```diff
@@ -26,10 +26,10 @@
         "notes": null,
         "procedure_type": "Craniotomy",
         "protective_material": null,
         "recovery_time": 25.0,
         "recovery_time_unit": "minute",
         "start_date": "2022-01-03",
         "weight_unit": "gram",
-        "workstation_id": null
+        "workstation_id": "SWS 4"
     }
 ]
```

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99609375%*

 * *Differences: {'1': "{'workstation_id': 'SWS 4'}"}*

```diff
@@ -54,15 +54,15 @@
         "notes": null,
         "procedure_type": "Nanoject injection",
         "recovery_time": 25.0,
         "recovery_time_unit": "minute",
         "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": null
+        "workstation_id": "SWS 4"
     },
     {
         "alternating_current": null,
         "anaesthesia": {
             "duration": 120.0,
             "duration_unit": "minute",
             "level": 2.5,
@@ -88,15 +88,15 @@
         "injection_hemisphere": null,
         "injection_materials": null,
         "injection_volume": null,
         "injection_volume_unit": "nanoliter",
         "instrument_id": null,
         "notes": null,
         "procedure_type": "Nanoject injection",
-        "recovery_time": 30,
+        "recovery_time": 30.0,
         "recovery_time_unit": "minute",
         "start_date": null,
         "targeted_structure": null,
         "weight_unit": "gram",
         "workstation_id": null
     },
     {
```

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9928875448028676%*

 * *Differences: {'1': "{'workstation_id': 'SWS 4'}",*

 * * '3': "{'workstation_id': 'SWS 4'}",*

 * * '5': "{'workstation_id': 'SWS 4'}",*

 * * '7': "{'workstation_id': 'SWS 4'}"}*

```diff
@@ -54,15 +54,15 @@
         "notes": null,
         "procedure_type": "Nanoject injection",
         "recovery_time": 25.0,
         "recovery_time_unit": "minute",
         "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": null
+        "workstation_id": "SWS 4"
     },
     {
         "anaesthesia": {
             "duration": 90.0,
             "duration_unit": "minute",
             "level": 2.0,
             "type": "isoflurane"
@@ -124,15 +124,15 @@
         "notes": null,
         "procedure_type": "Iontophoresis injection",
         "recovery_time": 25.0,
         "recovery_time_unit": "minute",
         "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": null
+        "workstation_id": "SWS 4"
     },
     {
         "anaesthesia": {
             "duration": 90.0,
             "duration_unit": "minute",
             "level": 2.0,
             "type": "isoflurane"
@@ -194,15 +194,15 @@
         "notes": null,
         "procedure_type": "Iontophoresis injection",
         "recovery_time": 25.0,
         "recovery_time_unit": "minute",
         "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": null
+        "workstation_id": "SWS 4"
     },
     {
         "anaesthesia": {
             "duration": 90.0,
             "duration_unit": "minute",
             "level": 2.0,
             "type": "isoflurane"
@@ -264,15 +264,15 @@
         "notes": null,
         "procedure_type": "Iontophoresis injection",
         "recovery_time": 25.0,
         "recovery_time_unit": "minute",
         "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": null
+        "workstation_id": "SWS 4"
     },
     {
         "anaesthesia": {
             "duration": 90.0,
             "duration_unit": "minute",
             "level": 2.0,
             "type": "isoflurane"
```

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9928875448028676%*

 * *Differences: {'1': "{'workstation_id': 'SWS 3'}",*

 * * '3': "{'workstation_id': 'SWS 3'}",*

 * * '5': "{'workstation_id': 'SWS 3'}",*

 * * '7': "{'workstation_id': 'SWS 3'}"}*

```diff
@@ -54,15 +54,15 @@
         "notes": null,
         "procedure_type": "Nanoject injection",
         "recovery_time": 25.0,
         "recovery_time_unit": "minute",
         "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": null
+        "workstation_id": "SWS 3"
     },
     {
         "anaesthesia": {
             "duration": 90.0,
             "duration_unit": "minute",
             "level": 2.0,
             "type": "isoflurane"
@@ -124,15 +124,15 @@
         "notes": null,
         "procedure_type": "Iontophoresis injection",
         "recovery_time": 25.0,
         "recovery_time_unit": "minute",
         "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": null
+        "workstation_id": "SWS 3"
     },
     {
         "anaesthesia": {
             "duration": 90.0,
             "duration_unit": "minute",
             "level": 2.0,
             "type": "isoflurane"
@@ -194,15 +194,15 @@
         "notes": null,
         "procedure_type": "Iontophoresis injection",
         "recovery_time": 25.0,
         "recovery_time_unit": "minute",
         "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": null
+        "workstation_id": "SWS 3"
     },
     {
         "anaesthesia": {
             "duration": 90.0,
             "duration_unit": "minute",
             "level": 2.0,
             "type": "isoflurane"
@@ -264,15 +264,15 @@
         "notes": null,
         "procedure_type": "Iontophoresis injection",
         "recovery_time": 25.0,
         "recovery_time_unit": "minute",
         "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": null
+        "workstation_id": "SWS 3"
     },
     {
         "anaesthesia": {
             "duration": 90.0,
             "duration_unit": "minute",
             "level": 2.0,
             "type": "isoflurane"
```

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6005988467177983%*

 * *Differences: {'0': "{'start_date': '2022-01-03', 'end_date': '2022-01-03', 'animal_weight_prior': 25.2, "*

 * *      "'animal_weight_post': 28.2, 'anaesthesia': {'duration': 90.0, 'level': 2.0}, "*

 * *      "'recovery_time': 25.0, 'workstation_id': 'SWS 4', 'procedure_type': 'Iontophoresis "*

 * *      "injection', 'injection_current_unit': 'microamps', delete: ['injection_volume', "*

 * *      "'injection_volume_unit']}",*

 * * '1': "{'start_date': '2022-01-03', 'end_date': '2022-01-03', 'animal_weight_prior': 25.2, "*

 * *      "'animal_weight_po […]*

```diff
@@ -1,114 +1,113 @@
 [
     {
+        "alternating_current": null,
         "anaesthesia": {
             "duration": 90.0,
             "duration_unit": "minute",
             "level": 2.0,
             "type": "isoflurane"
         },
         "animal_weight_post": 28.2,
         "animal_weight_prior": 25.2,
-        "end_date": "2022-01-03",
-        "experimenter_full_name": "NSB-187",
-        "headframe_material": null,
-        "headframe_part_number": null,
-        "headframe_type": "AI Straight bar",
-        "iacuc_protocol": "2103",
-        "notes": null,
-        "procedure_type": "Headframe",
-        "start_date": "2022-01-03",
-        "weight_unit": "gram",
-        "well_part_number": null,
-        "well_type": "No Well"
-    },
-    {
-        "alternating_current": null,
-        "anaesthesia": {
-            "duration": null,
-            "duration_unit": "minute",
-            "level": null,
-            "type": "isoflurane"
-        },
-        "animal_weight_post": null,
-        "animal_weight_prior": null,
         "bregma_to_lambda_distance": null,
         "bregma_to_lambda_unit": "millimeter",
-        "end_date": null,
+        "end_date": "2022-01-03",
         "experimenter_full_name": "NSB-187",
         "iacuc_protocol": "2103",
         "injection_angle": null,
         "injection_angle_unit": "degree",
         "injection_coordinate_ap": null,
         "injection_coordinate_depth": null,
         "injection_coordinate_ml": null,
         "injection_coordinate_reference": "Bregma",
         "injection_coordinate_unit": "millimeter",
         "injection_current": null,
+        "injection_current_unit": "microamps",
         "injection_duration": null,
         "injection_duration_unit": "minute",
         "injection_hemisphere": "Left",
         "injection_materials": null,
-        "injection_volume": null,
-        "injection_volume_unit": "nanoliter",
         "instrument_id": null,
         "notes": null,
-        "procedure_type": "Nanoject injection",
-        "recovery_time": null,
+        "procedure_type": "Iontophoresis injection",
+        "recovery_time": 25.0,
         "recovery_time_unit": "minute",
-        "start_date": null,
+        "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": null
+        "workstation_id": "SWS 4"
     },
     {
         "anaesthesia": {
-            "duration": null,
+            "duration": 90.0,
             "duration_unit": "minute",
-            "level": null,
+            "level": 2.0,
             "type": "isoflurane"
         },
-        "animal_weight_post": null,
-        "animal_weight_prior": null,
-        "end_date": null,
+        "animal_weight_post": 28.2,
+        "animal_weight_prior": 25.2,
+        "end_date": "2022-01-03",
         "experimenter_full_name": "NSB-187",
         "iacuc_protocol": "2103",
         "notes": null,
         "probes": {
             "angle": null,
             "angle_unit": "degree",
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
-            "name": "Probe A",
+            "name": "Probe B",
             "notes": null,
             "stereotactic_coordinate_ap": null,
             "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
-        "start_date": null,
+        "start_date": "2022-01-03",
         "weight_unit": "gram"
     },
     {
-        "alternating_current": null,
         "anaesthesia": {
             "duration": 90.0,
             "duration_unit": "minute",
             "level": 2.0,
             "type": "isoflurane"
         },
         "animal_weight_post": 28.2,
         "animal_weight_prior": 25.2,
+        "end_date": "2022-01-03",
+        "experimenter_full_name": "NSB-187",
+        "headframe_material": null,
+        "headframe_part_number": null,
+        "headframe_type": "AI Straight bar",
+        "iacuc_protocol": "2103",
+        "notes": null,
+        "procedure_type": "Headframe",
+        "start_date": "2022-01-03",
+        "weight_unit": "gram",
+        "well_part_number": null,
+        "well_type": "No Well"
+    },
+    {
+        "alternating_current": null,
+        "anaesthesia": {
+            "duration": null,
+            "duration_unit": "minute",
+            "level": null,
+            "type": "isoflurane"
+        },
+        "animal_weight_post": null,
+        "animal_weight_prior": null,
         "bregma_to_lambda_distance": null,
         "bregma_to_lambda_unit": "millimeter",
-        "end_date": "2022-01-03",
+        "end_date": null,
         "experimenter_full_name": "NSB-187",
         "iacuc_protocol": "2103",
         "injection_angle": null,
         "injection_angle_unit": "degree",
         "injection_coordinate_ap": null,
         "injection_coordinate_depth": null,
         "injection_coordinate_ml": null,
@@ -119,52 +118,59 @@
         "injection_duration": null,
         "injection_duration_unit": "minute",
         "injection_hemisphere": "Left",
         "injection_materials": null,
         "instrument_id": null,
         "notes": null,
         "procedure_type": "Iontophoresis injection",
-        "recovery_time": 25.0,
+        "recovery_time": null,
         "recovery_time_unit": "minute",
-        "start_date": "2022-01-03",
+        "start_date": null,
         "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": null
+        "workstation_id": "SWS 4"
     },
     {
+        "alternating_current": null,
         "anaesthesia": {
-            "duration": 90.0,
+            "duration": null,
             "duration_unit": "minute",
-            "level": 2.0,
+            "level": null,
             "type": "isoflurane"
         },
-        "animal_weight_post": 28.2,
-        "animal_weight_prior": 25.2,
-        "end_date": "2022-01-03",
+        "animal_weight_post": null,
+        "animal_weight_prior": null,
+        "bregma_to_lambda_distance": null,
+        "bregma_to_lambda_unit": "millimeter",
+        "end_date": null,
         "experimenter_full_name": "NSB-187",
         "iacuc_protocol": "2103",
+        "injection_angle": null,
+        "injection_angle_unit": "degree",
+        "injection_coordinate_ap": null,
+        "injection_coordinate_depth": null,
+        "injection_coordinate_ml": null,
+        "injection_coordinate_reference": "Bregma",
+        "injection_coordinate_unit": "millimeter",
+        "injection_current": null,
+        "injection_duration": null,
+        "injection_duration_unit": "minute",
+        "injection_hemisphere": "Left",
+        "injection_materials": null,
+        "injection_volume": null,
+        "injection_volume_unit": "nanoliter",
+        "instrument_id": null,
         "notes": null,
-        "probes": {
-            "angle": null,
-            "angle_unit": "degree",
-            "bregma_to_lambda_distance": null,
-            "bregma_to_lambda_unit": "millimeter",
-            "core_diameter_unit": "\u03bcm",
-            "ferrule_material": null,
-            "name": "Probe B",
-            "notes": null,
-            "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": null,
-            "stereotactic_coordinate_ml": null,
-            "stereotactic_coordinate_reference": "Bregma",
-            "stereotactic_coordinate_unit": "millimeter"
-        },
-        "procedure_type": "Fiber implant",
-        "start_date": "2022-01-03",
-        "weight_unit": "gram"
+        "procedure_type": "Nanoject injection",
+        "recovery_time": null,
+        "recovery_time_unit": "minute",
+        "start_date": null,
+        "targeted_structure": null,
+        "weight_unit": "gram",
+        "workstation_id": null
     },
     {
         "alternating_current": null,
         "anaesthesia": {
             "duration": null,
             "duration_unit": "minute",
             "level": null,
@@ -184,15 +190,15 @@
         "injection_coordinate_ml": null,
         "injection_coordinate_reference": "Bregma",
         "injection_coordinate_unit": "millimeter",
         "injection_current": null,
         "injection_current_unit": "microamps",
         "injection_duration": null,
         "injection_duration_unit": "minute",
-        "injection_hemisphere": "Left",
+        "injection_hemisphere": "Right",
         "injection_materials": null,
         "instrument_id": null,
         "notes": null,
         "procedure_type": "Iontophoresis injection",
         "recovery_time": null,
         "recovery_time_unit": "minute",
         "start_date": null,
@@ -216,63 +222,57 @@
         "probes": {
             "angle": null,
             "angle_unit": "degree",
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
-            "name": "Probe C",
+            "name": "Probe A",
             "notes": null,
             "stereotactic_coordinate_ap": null,
             "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": null,
         "weight_unit": "gram"
     },
     {
-        "alternating_current": null,
         "anaesthesia": {
             "duration": null,
             "duration_unit": "minute",
             "level": null,
             "type": "isoflurane"
         },
         "animal_weight_post": null,
         "animal_weight_prior": null,
-        "bregma_to_lambda_distance": null,
-        "bregma_to_lambda_unit": "millimeter",
         "end_date": null,
         "experimenter_full_name": "NSB-187",
         "iacuc_protocol": "2103",
-        "injection_angle": null,
-        "injection_angle_unit": "degree",
-        "injection_coordinate_ap": null,
-        "injection_coordinate_depth": null,
-        "injection_coordinate_ml": null,
-        "injection_coordinate_reference": "Bregma",
-        "injection_coordinate_unit": "millimeter",
-        "injection_current": null,
-        "injection_current_unit": "microamps",
-        "injection_duration": null,
-        "injection_duration_unit": "minute",
-        "injection_hemisphere": "Right",
-        "injection_materials": null,
-        "instrument_id": null,
         "notes": null,
-        "procedure_type": "Iontophoresis injection",
-        "recovery_time": null,
-        "recovery_time_unit": "minute",
+        "probes": {
+            "angle": null,
+            "angle_unit": "degree",
+            "bregma_to_lambda_distance": null,
+            "bregma_to_lambda_unit": "millimeter",
+            "core_diameter_unit": "\u03bcm",
+            "ferrule_material": null,
+            "name": "Probe C",
+            "notes": null,
+            "stereotactic_coordinate_ap": null,
+            "stereotactic_coordinate_dv": null,
+            "stereotactic_coordinate_ml": null,
+            "stereotactic_coordinate_reference": "Bregma",
+            "stereotactic_coordinate_unit": "millimeter"
+        },
+        "procedure_type": "Fiber implant",
         "start_date": null,
-        "targeted_structure": null,
-        "weight_unit": "gram",
-        "workstation_id": null
+        "weight_unit": "gram"
     },
     {
         "anaesthesia": {
             "duration": null,
             "duration_unit": "minute",
             "level": null,
             "type": "isoflurane"
```

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982078853046595%*

 * *Differences: {'3': "{'workstation_id': 'SWS 4'}"}*

```diff
@@ -124,15 +124,15 @@
         "notes": null,
         "procedure_type": "Iontophoresis injection",
         "recovery_time": 25.0,
         "recovery_time_unit": "minute",
         "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": null
+        "workstation_id": "SWS 4"
     },
     {
         "anaesthesia": {
             "duration": 90.0,
             "duration_unit": "minute",
             "level": 2.0,
             "type": "isoflurane"
```

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9838709677419355%*

 * *Differences: {'0': "{'workstation_id': 'SWS 4'}"}*

```diff
@@ -31,10 +31,10 @@
         "notes": null,
         "procedure_type": "Iontophoresis injection",
         "recovery_time": null,
         "recovery_time_unit": "minute",
         "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
-        "workstation_id": null
+        "workstation_id": "SWS 4"
     }
 ]
```

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item10.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item11.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item13.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item13.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item14.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item14.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965753424657534%*

 * *Differences: {"'WorkStation1stInjection'": "'SWS 4'"}*

```diff
@@ -135,14 +135,14 @@
     "Title": "657849Visual Ctx 2P",
     "Virus_x0020_A_x002f_P": "-.85",
     "Virus_x0020_D_x002f_V": "-3.1",
     "Virus_x0020_Hemisphere": "Left",
     "Virus_x0020_M_x002f_L": "-5.2",
     "Weight_x0020_after_x0020_Surgery": "28.2",
     "Weight_x0020_before_x0020_Surger": "25.2",
-    "WorkStation1stInjection": "Select...",
+    "WorkStation1stInjection": "SWS 4",
     "inj1volperdepth": "600 nl",
     "inj2volperdepth": null,
     "inj3volperdepth": null,
     "retSetting0": "Off",
     "retSetting1": "Off"
 }
```

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item15.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item15.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965753424657534%*

 * *Differences: {"'HpWorkStation'": "'SWS 3'"}*

```diff
@@ -61,15 +61,15 @@
     "HPIsoLevel": "2",
     "HPRecovery": "25",
     "HPSurgeonComments": "Went very well",
     "Headpost": "Motor Ctx",
     "HeadpostType": "Scientifica (CAM)",
     "Headpost_x0020_Perform_x0020_Dur": "Initial Surgery",
     "Hemisphere2ndInj": "Left",
-    "HpWorkStation": "SWS 4",
+    "HpWorkStation": "SWS 3",
     "IACUC_x0020_Protocol_x0020__x002": "2103",
     "ID": 190,
     "Id": 190,
     "ImplantIDCoverslipType": "5mm stacked coverslip",
     "Inj1AlternatingTime": null,
     "Inj1Angle_v2": "0",
     "Inj1Current": null,
```

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item16.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item16.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965753424657534%*

 * *Differences: {"'WorkStation1stInjection'": "'SWS 4'"}*

```diff
@@ -135,14 +135,14 @@
     "Title": "657849Visual Ctx 2P",
     "Virus_x0020_A_x002f_P": "-.85",
     "Virus_x0020_D_x002f_V": "-3.1",
     "Virus_x0020_Hemisphere": "Left",
     "Virus_x0020_M_x002f_L": "-5.2",
     "Weight_x0020_after_x0020_Surgery": "28.2",
     "Weight_x0020_before_x0020_Surger": "25.2",
-    "WorkStation1stInjection": "Select...",
+    "WorkStation1stInjection": "SWS 4",
     "inj1volperdepth": "600 nl",
     "inj2volperdepth": null,
     "inj3volperdepth": null,
     "retSetting0": "Off",
     "retSetting1": "Off"
 }
```

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item17.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item17.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item18.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item18.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item8.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/resources/sharepoint/nsb2023/raw/list_item9.json` & `aind_metadata_service-0.4.8/tests/resources/sharepoint/nsb2023/raw/list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/sharepoint/nsb2019/test_mapping.py` & `aind_metadata_service-0.4.8/tests/sharepoint/nsb2019/test_mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/sharepoint/nsb2019/test_models.py` & `aind_metadata_service-0.4.8/tests/sharepoint/nsb2019/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/sharepoint/nsb2023/test_mapping.py` & `aind_metadata_service-0.4.8/tests/sharepoint/nsb2023/test_mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/sharepoint/nsb2023/test_models.py` & `aind_metadata_service-0.4.8/tests/sharepoint/nsb2023/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/sharepoint/test_client.py` & `aind_metadata_service-0.4.8/tests/sharepoint/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/test_client.py` & `aind_metadata_service-0.4.8/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.7/tests/test_response_handler.py` & `aind_metadata_service-0.4.8/tests/test_response_handler.py`

 * *Files identical despite different names*

