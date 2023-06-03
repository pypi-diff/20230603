# Comparing `tmp/argos-nac-0.1.2.tar.gz` & `tmp/argos-nac-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argos-nac-0.1.2.tar", last modified: Fri Jun  2 19:36:32 2023, max compression
+gzip compressed data, was "argos-nac-0.1.3.tar", last modified: Sat Jun  3 09:38:36 2023, max compression
```

## Comparing `argos-nac-0.1.2.tar` & `argos-nac-0.1.3.tar`

### file list

```diff
@@ -1,689 +1,689 @@
--rw-r--r--   0        0        0       10 2023-03-21 16:37:52.480936 argos-nac-0.1.2/graphql_schema/.gitignore
--rw-r--r--   0        0        0      311 2023-04-06 09:35:21.416520 argos-nac-0.1.2/graphql_schema/__init__.py
--rw-r--r--   0        0        0     1158 2023-03-21 16:37:09.958974 argos-nac-0.1.2/graphql_schema/gen_schema.py
--rw-r--r--   0        0        0  2602951 2023-03-20 15:36:54.363420 argos-nac-0.1.2/graphql_schema/schema.py
--rw-r--r--   0        0        0     1440 2023-03-20 13:23:43.292829 argos-nac-0.1.2/graphql_schema/schema_query.gql
--rw-r--r--   0        0        0       36 2023-05-10 23:04:17.246649 argos-nac-0.1.2/nac/.mypy_cache/.gitignore
--rw-r--r--   0        0        0        2 2023-05-12 06:43:07.044719 argos-nac-0.1.2/nac/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180391 2023-05-10 23:04:17.062153 argos-nac-0.1.2/nac/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1601 2023-05-10 23:04:17.063151 argos-nac-0.1.2/nac/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    58135 2023-05-10 23:04:17.054152 argos-nac-0.1.2/nac/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1694 2023-05-10 23:04:17.055653 argos-nac-0.1.2/nac/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18250 2023-05-10 23:04:17.049652 argos-nac-0.1.2/nac/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1620 2023-05-10 23:04:17.051151 argos-nac-0.1.2/nac/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     7234 2023-05-10 23:04:17.046155 argos-nac-0.1.2/nac/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1619 2023-05-10 23:04:17.047655 argos-nac-0.1.2/nac/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    23884 2023-05-10 23:04:17.174654 argos-nac-0.1.2/nac/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1655 2023-05-10 23:04:17.176653 argos-nac-0.1.2/nac/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    89078 2023-05-10 23:04:17.043152 argos-nac-0.1.2/nac/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1724 2023-05-10 23:04:17.044155 argos-nac-0.1.2/nac/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    62849 2023-05-10 23:04:17.036155 argos-nac-0.1.2/nac/.mypy_cache/3.11/_winapi.data.json
--rw-r--r--   0        0        0     1680 2023-05-10 23:04:17.038153 argos-nac-0.1.2/nac/.mypy_cache/3.11/_winapi.meta.json
--rw-r--r--   0        0        0    23359 2023-05-10 23:04:17.031650 argos-nac-0.1.2/nac/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1608 2023-05-10 23:04:17.033154 argos-nac-0.1.2/nac/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60699 2023-05-10 23:04:17.028653 argos-nac-0.1.2/nac/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1663 2023-05-10 23:04:17.030152 argos-nac-0.1.2/nac/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0  1130864 2023-05-10 23:04:17.142151 argos-nac-0.1.2/nac/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1755 2023-05-10 23:04:17.143150 argos-nac-0.1.2/nac/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   124034 2023-05-10 23:04:17.024152 argos-nac-0.1.2/nac/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1705 2023-05-10 23:04:17.025154 argos-nac-0.1.2/nac/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   408012 2023-05-10 23:04:17.018152 argos-nac-0.1.2/nac/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1682 2023-05-10 23:04:17.019652 argos-nac-0.1.2/nac/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3755 2023-05-10 23:04:17.003651 argos-nac-0.1.2/nac/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1593 2023-05-10 23:04:17.005152 argos-nac-0.1.2/nac/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   109227 2023-05-10 23:04:17.001152 argos-nac-0.1.2/nac/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1654 2023-05-10 23:04:17.002157 argos-nac-0.1.2/nac/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0   136839 2023-05-10 23:04:16.995650 argos-nac-0.1.2/nac/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1701 2023-05-10 23:04:16.997152 argos-nac-0.1.2/nac/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    57768 2023-05-10 23:04:16.988915 argos-nac-0.1.2/nac/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1659 2023-05-10 23:04:16.990152 argos-nac-0.1.2/nac/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0     7462 2023-05-10 23:04:16.985151 argos-nac-0.1.2/nac/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1645 2023-05-10 23:04:16.986152 argos-nac-0.1.2/nac/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12224 2023-05-10 23:04:16.982154 argos-nac-0.1.2/nac/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1590 2023-05-10 23:04:16.983652 argos-nac-0.1.2/nac/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7273 2023-05-10 23:04:16.979151 argos-nac-0.1.2/nac/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1622 2023-05-10 23:04:16.980654 argos-nac-0.1.2/nac/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25097 2023-05-10 23:04:16.976152 argos-nac-0.1.2/nac/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1594 2023-05-10 23:04:16.977152 argos-nac-0.1.2/nac/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9178 2023-05-10 23:04:16.973152 argos-nac-0.1.2/nac/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1607 2023-05-10 23:04:16.974652 argos-nac-0.1.2/nac/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79294 2023-05-10 23:04:16.970652 argos-nac-0.1.2/nac/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1710 2023-05-10 23:04:16.971651 argos-nac-0.1.2/nac/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30881 2023-05-10 23:04:16.965152 argos-nac-0.1.2/nac/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1671 2023-05-10 23:04:16.966651 argos-nac-0.1.2/nac/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0    90146 2023-05-10 23:04:16.960655 argos-nac-0.1.2/nac/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1634 2023-05-10 23:04:16.962154 argos-nac-0.1.2/nac/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    22411 2023-05-10 23:04:16.955651 argos-nac-0.1.2/nac/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1634 2023-05-10 23:04:16.956655 argos-nac-0.1.2/nac/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     6149 2023-05-10 23:04:16.952653 argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1622 2023-05-10 23:04:16.953654 argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70603 2023-05-10 23:04:16.946152 argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1768 2023-05-10 23:04:16.947152 argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64595 2023-05-10 23:04:16.941153 argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1757 2023-05-10 23:04:16.942653 argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91144 2023-05-10 23:04:16.936651 argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1767 2023-05-10 23:04:16.938152 argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11960 2023-05-10 23:04:16.930652 argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1611 2023-05-10 23:04:16.932152 argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    85360 2023-05-10 23:04:16.927651 argos-nac-0.1.2/nac/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1707 2023-05-10 23:04:16.928654 argos-nac-0.1.2/nac/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   144294 2023-05-10 23:04:17.226153 argos-nac-0.1.2/nac/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1721 2023-05-10 23:04:17.227652 argos-nac-0.1.2/nac/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0    23330 2023-05-10 23:04:16.922653 argos-nac-0.1.2/nac/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1662 2023-05-10 23:04:16.924155 argos-nac-0.1.2/nac/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    14103 2023-05-10 23:04:16.919151 argos-nac-0.1.2/nac/.mypy_cache/3.11/ntpath.data.json
--rw-r--r--   0        0        0     1650 2023-05-10 23:04:16.920653 argos-nac-0.1.2/nac/.mypy_cache/3.11/ntpath.meta.json
--rw-r--r--   0        0        0   237007 2023-05-10 23:04:16.915651 argos-nac-0.1.2/nac/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1760 2023-05-10 23:04:16.916652 argos-nac-0.1.2/nac/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4920 2023-05-10 23:04:16.906151 argos-nac-0.1.2/nac/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1579 2023-05-10 23:04:16.907653 argos-nac-0.1.2/nac/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0    85743 2023-05-10 23:04:16.903653 argos-nac-0.1.2/nac/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1716 2023-05-10 23:04:16.904654 argos-nac-0.1.2/nac/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    44416 2023-05-10 23:04:16.898152 argos-nac-0.1.2/nac/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1664 2023-05-10 23:04:16.899652 argos-nac-0.1.2/nac/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75220 2023-05-10 23:04:16.895151 argos-nac-0.1.2/nac/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1661 2023-05-10 23:04:16.896153 argos-nac-0.1.2/nac/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167568 2023-05-10 23:04:16.890152 argos-nac-0.1.2/nac/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1735 2023-05-10 23:04:16.891651 argos-nac-0.1.2/nac/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14396 2023-05-10 23:04:16.882652 argos-nac-0.1.2/nac/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1606 2023-05-10 23:04:16.883651 argos-nac-0.1.2/nac/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28503 2023-05-10 23:04:16.879651 argos-nac-0.1.2/nac/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1618 2023-05-10 23:04:16.880651 argos-nac-0.1.2/nac/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49764 2023-05-10 23:04:16.876154 argos-nac-0.1.2/nac/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1661 2023-05-10 23:04:16.877652 argos-nac-0.1.2/nac/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0    27771 2023-05-10 23:04:17.157652 argos-nac-0.1.2/nac/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1646 2023-05-10 23:04:17.159151 argos-nac-0.1.2/nac/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0   167824 2023-05-10 23:04:16.872153 argos-nac-0.1.2/nac/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1726 2023-05-10 23:04:16.873153 argos-nac-0.1.2/nac/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   159493 2023-05-10 23:04:16.864652 argos-nac-0.1.2/nac/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1694 2023-05-10 23:04:16.866152 argos-nac-0.1.2/nac/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    64738 2023-05-10 23:04:17.179651 argos-nac-0.1.2/nac/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1658 2023-05-10 23:04:17.181153 argos-nac-0.1.2/nac/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    38027 2023-05-10 23:04:17.151151 argos-nac-0.1.2/nac/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1599 2023-05-10 23:04:17.153154 argos-nac-0.1.2/nac/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   239655 2023-05-10 23:04:16.857152 argos-nac-0.1.2/nac/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1672 2023-05-10 23:04:16.858652 argos-nac-0.1.2/nac/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432425 2023-05-10 23:04:16.847651 argos-nac-0.1.2/nac/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1723 2023-05-10 23:04:16.848651 argos-nac-0.1.2/nac/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57889 2023-05-10 23:04:16.832150 argos-nac-0.1.2/nac/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1679 2023-05-10 23:04:16.833651 argos-nac-0.1.2/nac/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0     1400 2023-05-10 23:04:17.182651 argos-nac-0.1.2/nac/.mypy_cache/3.11/work/__init__.data.json
--rw-r--r--   0        0        0     1452 2023-05-10 23:04:17.184152 argos-nac-0.1.2/nac/.mypy_cache/3.11/work/__init__.meta.json
--rw-r--r--   0        0        0     1698 2023-05-10 23:04:17.193651 argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.data.json
--rw-r--r--   0        0        0     1528 2023-05-10 23:04:17.194653 argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.meta.json
--rw-r--r--   0        0        0    49114 2023-05-10 23:04:17.238651 argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/model.data.json
--rw-r--r--   0        0        0     1656 2023-05-10 23:04:17.240153 argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/model.meta.json
--rw-r--r--   0        0        0     1395 2023-05-10 23:04:17.190652 argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos/controller.data.json
--rw-r--r--   0        0        0     1445 2023-05-10 23:04:17.191652 argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos/controller.meta.json
--rw-r--r--   0        0        0     1317 2023-05-10 23:04:17.188154 argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos.data.json
--rw-r--r--   0        0        0     1422 2023-05-11 08:05:37.470673 argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos.meta.json
--rw-r--r--   0        0        0     1274 2023-05-10 23:04:17.185653 argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects.data.json
--rw-r--r--   0        0        0     1409 2023-05-10 23:04:17.187153 argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects.meta.json
--rw-r--r--   0        0        0      193 2023-05-10 23:04:17.250652 argos-nac-0.1.2/nac/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        0 2023-05-30 06:35:53.597209 argos-nac-0.1.2/nac/__init__.py
--rw-r--r--   0        0        0      353 2023-05-30 08:20:54.895213 argos-nac-0.1.2/nac/__main__.py
--rw-r--r--   0        0        0       22 2023-06-02 19:36:03.141898 argos-nac-0.1.2/nac/__version__.py
--rw-r--r--   0        0        0       74 2023-05-26 06:59:58.793027 argos-nac-0.1.2/nac/cisco/__init__.py
--rw-r--r--   0        0        0     3571 2023-05-30 13:13:31.234054 argos-nac-0.1.2/nac/cisco/controller.py
--rw-r--r--   0        0        0     2650 2023-05-30 13:13:31.235056 argos-nac-0.1.2/nac/cisco/nornir_util.py
--rw-r--r--   0        0        0       75 2023-05-26 06:59:58.797861 argos-nac-0.1.2/nac/cisco/protocols/__init__.py
--rw-r--r--   0        0        0     5728 2023-05-30 13:13:31.236055 argos-nac-0.1.2/nac/cisco/protocols/bgp.py
--rw-r--r--   0        0        0     1880 2023-05-30 13:13:31.236055 argos-nac-0.1.2/nac/cisco/protocols/ldp.py
--rw-r--r--   0        0        0     2337 2023-05-30 13:13:31.237055 argos-nac-0.1.2/nac/cisco/protocols/vrf.py
--rw-r--r--   0        0        0       98 2023-05-30 13:13:31.238055 argos-nac-0.1.2/nac/constants.py
--rw-r--r--   0        0        0     6977 2023-06-02 19:35:22.133757 argos-nac-0.1.2/nac/main.py
--rw-r--r--   0        0        0     5182 2023-05-30 13:13:31.242743 argos-nac-0.1.2/nac/model.py
--rw-r--r--   0        0        0     2188 2023-05-30 13:13:31.243293 argos-nac-0.1.2/nac/queries/main.gql
--rw-r--r--   0        0        0       36 2023-05-28 09:22:24.169770 argos-nac-0.1.2/nac/util/.mypy_cache/.gitignore
--rw-r--r--   0        0        0        2 2023-05-29 09:23:35.916730 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180382 2023-05-28 09:22:23.971852 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1645 2023-05-28 09:22:23.972852 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    58126 2023-05-28 09:22:23.963749 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1685 2023-05-28 09:22:23.965862 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18241 2023-05-28 09:22:23.958748 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1611 2023-05-28 09:22:23.960749 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     7225 2023-05-28 09:22:23.955882 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1610 2023-05-28 09:22:23.957753 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    23875 2023-05-28 09:22:24.086799 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1646 2023-05-28 09:22:24.088770 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    89069 2023-05-28 09:22:23.954330 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1715 2023-05-28 09:22:23.955330 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    62840 2023-05-28 09:22:23.948350 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_winapi.data.json
--rw-r--r--   0        0        0     1671 2023-05-28 09:22:23.950332 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_winapi.meta.json
--rw-r--r--   0        0        0    23350 2023-05-28 09:22:23.944352 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1599 2023-05-28 09:22:23.945351 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60690 2023-05-28 09:22:23.941348 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1654 2023-05-28 09:22:23.942349 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0  1130855 2023-05-28 09:22:24.049760 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1736 2023-05-28 09:22:24.051759 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   124025 2023-05-28 09:22:23.937349 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1696 2023-05-28 09:22:23.938351 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   408003 2023-05-28 09:22:23.930336 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1726 2023-05-28 09:22:23.932340 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3746 2023-05-28 09:22:23.916029 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1584 2023-05-28 09:22:23.917028 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   109218 2023-05-28 09:22:23.912028 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1645 2023-05-28 09:22:23.914029 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0   136830 2023-05-28 09:22:23.907027 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1692 2023-05-28 09:22:23.908031 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    57759 2023-05-28 09:22:23.899009 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1650 2023-05-28 09:22:23.901007 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0     7453 2023-05-28 09:22:23.894746 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1636 2023-05-28 09:22:23.896013 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12215 2023-05-28 09:22:23.892746 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1581 2023-05-28 09:22:23.893747 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7264 2023-05-28 09:22:23.889750 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1613 2023-05-28 09:22:23.890748 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25088 2023-05-28 09:22:23.887656 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1585 2023-05-28 09:22:23.888749 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9169 2023-05-28 09:22:23.883658 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1598 2023-05-28 09:22:23.884658 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79285 2023-05-28 09:22:23.880656 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1701 2023-05-28 09:22:23.881657 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30872 2023-05-28 09:22:23.876657 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1662 2023-05-28 09:22:23.877659 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0    90137 2023-05-28 09:22:23.872659 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1625 2023-05-28 09:22:23.873656 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    22402 2023-05-28 09:22:23.867657 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1625 2023-05-28 09:22:23.868657 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     6140 2023-05-28 09:22:23.863779 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1613 2023-05-28 09:22:23.865743 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70594 2023-05-28 09:22:23.861779 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1759 2023-05-28 09:22:23.862779 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64586 2023-05-28 09:22:23.856745 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1748 2023-05-28 09:22:23.858780 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91135 2023-05-28 09:22:23.851745 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1758 2023-05-28 09:22:23.852744 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11951 2023-05-28 09:22:23.845728 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1602 2023-05-28 09:22:23.846728 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    85351 2023-05-28 09:22:23.842728 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1698 2023-05-28 09:22:23.843728 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   144400 2023-05-28 09:22:24.138780 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1712 2023-05-28 09:22:24.139777 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0    23321 2023-05-28 09:22:23.837728 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1653 2023-05-28 09:22:23.838727 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    14094 2023-05-28 09:22:23.834730 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/ntpath.data.json
--rw-r--r--   0        0        0     1641 2023-05-28 09:22:23.836727 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/ntpath.meta.json
--rw-r--r--   0        0        0   236998 2023-05-28 09:22:23.831728 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1751 2023-05-28 09:22:23.832730 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4911 2023-05-28 09:22:23.821749 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1570 2023-05-28 09:22:23.822749 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0    85758 2023-05-28 09:22:23.818753 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1707 2023-05-28 09:22:23.819750 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    44407 2023-05-28 09:22:23.813750 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1655 2023-05-28 09:22:23.814749 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75211 2023-05-28 09:22:23.810750 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1652 2023-05-28 09:22:23.811751 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167559 2023-05-28 09:22:23.805751 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1726 2023-05-28 09:22:23.806749 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14387 2023-05-28 09:22:23.798751 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1597 2023-05-28 09:22:23.799750 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28494 2023-05-28 09:22:23.795754 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1609 2023-05-28 09:22:23.797717 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49755 2023-05-28 09:22:23.792746 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1652 2023-05-28 09:22:23.793747 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0    27762 2023-05-28 09:22:24.068900 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1637 2023-05-28 09:22:24.069897 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0   167815 2023-05-28 09:22:23.789745 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1717 2023-05-28 09:22:23.790746 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   165686 2023-05-28 09:22:23.782597 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1685 2023-05-28 09:22:23.783595 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    64729 2023-05-28 09:22:24.090772 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1649 2023-05-28 09:22:24.092773 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    38018 2023-05-28 09:22:24.060158 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1590 2023-05-28 09:22:24.063161 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   239646 2023-05-28 09:22:23.775599 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1663 2023-05-28 09:22:23.776596 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432248 2023-05-28 09:22:23.765854 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1714 2023-05-28 09:22:23.766848 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57859 2023-05-28 09:22:23.749761 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1670 2023-05-28 09:22:23.750757 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0     1400 2023-05-28 09:22:24.093772 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/__init__.data.json
--rw-r--r--   0        0        0     1452 2023-05-28 09:22:24.094771 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/__init__.meta.json
--rw-r--r--   0        0        0     1698 2023-05-28 09:22:24.103771 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.data.json
--rw-r--r--   0        0        0     1528 2023-05-28 09:22:24.104771 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.meta.json
--rw-r--r--   0        0        0     5955 2023-05-28 09:22:24.162781 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util/netbox_api.data.json
--rw-r--r--   0        0        0     1609 2023-05-28 09:22:24.163782 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util/netbox_api.meta.json
--rw-r--r--   0        0        0     1460 2023-05-28 09:22:24.106782 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util.data.json
--rw-r--r--   0        0        0     1465 2023-05-29 09:23:32.839349 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util.meta.json
--rw-r--r--   0        0        0     1395 2023-05-28 09:22:24.101775 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller.data.json
--rw-r--r--   0        0        0     1445 2023-05-28 09:22:24.102772 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller.meta.json
--rw-r--r--   0        0        0     1317 2023-05-28 09:22:24.098772 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos.data.json
--rw-r--r--   0        0        0     1422 2023-05-28 09:22:24.099773 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos.meta.json
--rw-r--r--   0        0        0     1274 2023-05-28 09:22:24.095772 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects.data.json
--rw-r--r--   0        0        0     1409 2023-05-28 09:22:24.096775 argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects.meta.json
--rw-r--r--   0        0        0      193 2023-05-28 09:22:24.173767 argos-nac-0.1.2/nac/util/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        0 2023-05-31 13:41:33.410344 argos-nac-0.1.2/nac/util/__init__.py
--rw-r--r--   0        0        0     3792 2023-05-30 13:13:31.244367 argos-nac-0.1.2/nac/util/common.py
--rw-r--r--   0        0        0     2738 2023-05-30 13:13:31.244892 argos-nac-0.1.2/nac/util/graphql_util.py
--rw-r--r--   0        0        0      369 2023-05-26 06:59:58.806115 argos-nac-0.1.2/nac/util/jinja_util.py
--rw-r--r--   0        0        0     2092 2023-05-30 13:23:09.225378 argos-nac-0.1.2/nac/util/netbox_api.py
--rw-r--r--   0        0        0     1335 2023-06-02 12:42:26.372725 argos-nac-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      170 2023-05-31 13:41:33.812536 argos-nac-0.1.2/README.md
--rw-r--r--   0        0        0       36 2023-05-26 09:05:50.098560 argos-nac-0.1.2/tests/.mypy_cache/.gitignore
--rw-r--r--   0        0        0        2 2023-05-26 10:05:55.185213 argos-nac-0.1.2/tests/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7835 2023-05-26 09:05:47.068757 argos-nac-0.1.2/tests/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1575 2023-05-26 09:05:47.069756 argos-nac-0.1.2/tests/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180382 2023-05-26 09:05:46.903810 argos-nac-0.1.2/tests/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1592 2023-05-26 09:05:46.904813 argos-nac-0.1.2/tests/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    43208 2023-05-26 09:05:46.992186 argos-nac-0.1.2/tests/.mypy_cache/3.11/_bisect.data.json
--rw-r--r--   0        0        0     1594 2023-05-26 09:05:46.993185 argos-nac-0.1.2/tests/.mypy_cache/3.11/_bisect.meta.json
--rw-r--r--   0        0        0    58126 2023-05-26 09:05:46.895812 argos-nac-0.1.2/tests/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1685 2023-05-26 09:05:46.897807 argos-nac-0.1.2/tests/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18241 2023-05-26 09:05:46.889812 argos-nac-0.1.2/tests/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1611 2023-05-26 09:05:46.891808 argos-nac-0.1.2/tests/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     7225 2023-05-26 09:05:46.886289 argos-nac-0.1.2/tests/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1610 2023-05-26 09:05:46.887288 argos-nac-0.1.2/tests/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171945 2023-05-26 09:05:47.596194 argos-nac-0.1.2/tests/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1649 2023-05-26 09:05:47.597193 argos-nac-0.1.2/tests/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0   113943 2023-05-26 09:05:46.957662 argos-nac-0.1.2/tests/.mypy_cache/3.11/_operator.data.json
--rw-r--r--   0        0        0     1622 2023-05-26 09:05:46.959665 argos-nac-0.1.2/tests/.mypy_cache/3.11/_operator.meta.json
--rw-r--r--   0        0        0     2096 2023-05-26 09:05:47.861430 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/__init__.data.json
--rw-r--r--   0        0        0     1553 2023-05-26 09:05:47.862420 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/__init__.meta.json
--rw-r--r--   0        0        0     5668 2023-05-26 09:05:47.856892 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_argcomplete.data.json
--rw-r--r--   0        0        0     1705 2023-05-26 09:05:47.858894 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_argcomplete.meta.json
--rw-r--r--   0        0        0     2851 2023-05-26 09:05:49.954398 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_code/__init__.data.json
--rw-r--r--   0        0        0     1595 2023-05-26 09:05:49.956397 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_code/__init__.meta.json
--rw-r--r--   0        0        0   201366 2023-05-26 09:05:49.952399 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_code/code.data.json
--rw-r--r--   0        0        0     1984 2023-05-26 09:05:49.953398 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_code/code.meta.json
--rw-r--r--   0        0        0    18070 2023-05-26 09:05:48.152361 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_code/source.data.json
--rw-r--r--   0        0        0     1780 2023-05-26 09:05:48.153361 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_code/source.meta.json
--rw-r--r--   0        0        0     2173 2023-05-26 09:05:49.927884 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/__init__.data.json
--rw-r--r--   0        0        0     1572 2023-05-26 09:05:49.928884 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/__init__.meta.json
--rw-r--r--   0        0        0    12069 2023-05-26 09:05:47.665769 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/saferepr.data.json
--rw-r--r--   0        0        0     1594 2023-05-26 09:05:47.666768 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json
--rw-r--r--   0        0        0    15783 2023-05-26 09:05:49.916368 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json
--rw-r--r--   0        0        0     1893 2023-05-26 09:05:49.917369 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json
--rw-r--r--   0        0        0     2946 2023-05-26 09:05:47.638735 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json
--rw-r--r--   0        0        0     1582 2023-05-26 09:05:47.640735 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json
--rw-r--r--   0        0        0     2657 2023-05-26 09:05:47.222503 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_version.data.json
--rw-r--r--   0        0        0     1539 2023-05-26 09:05:47.223504 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_version.meta.json
--rw-r--r--   0        0        0    12240 2023-05-26 09:05:50.068039 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/__init__.data.json
--rw-r--r--   0        0        0     1896 2023-05-26 09:05:50.069038 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json
--rw-r--r--   0        0        0    58200 2023-05-26 09:05:50.036508 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json
--rw-r--r--   0        0        0     2318 2023-05-26 09:05:50.037510 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json
--rw-r--r--   0        0        0     5807 2023-05-26 09:05:49.984915 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/truncate.data.json
--rw-r--r--   0        0        0     1674 2023-05-26 09:05:49.985914 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json
--rw-r--r--   0        0        0    22273 2023-05-26 09:05:49.972914 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/util.data.json
--rw-r--r--   0        0        0     1970 2023-05-26 09:05:49.973912 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/util.meta.json
--rw-r--r--   0        0        0    49255 2023-05-26 09:05:50.064039 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/cacheprovider.data.json
--rw-r--r--   0        0        0     2354 2023-05-26 09:05:50.066039 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/cacheprovider.meta.json
--rw-r--r--   0        0        0   122253 2023-05-26 09:05:50.024052 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/capture.data.json
--rw-r--r--   0        0        0     1962 2023-05-26 09:05:50.025052 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/capture.meta.json
--rw-r--r--   0        0        0    30716 2023-05-26 09:05:49.912924 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/compat.data.json
--rw-r--r--   0        0        0     1886 2023-05-26 09:05:49.914368 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/compat.meta.json
--rw-r--r--   0        0        0   106084 2023-05-26 09:05:49.962915 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/__init__.data.json
--rw-r--r--   0        0        0     2763 2023-05-26 09:05:49.964912 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/__init__.meta.json
--rw-r--r--   0        0        0    38719 2023-05-26 09:05:49.938398 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/argparsing.data.json
--rw-r--r--   0        0        0     2004 2023-05-26 09:05:49.939397 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/argparsing.meta.json
--rw-r--r--   0        0        0     4457 2023-05-26 09:05:49.981912 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/compat.data.json
--rw-r--r--   0        0        0     1690 2023-05-26 09:05:49.982913 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/compat.meta.json
--rw-r--r--   0        0        0     3004 2023-05-26 09:05:49.918367 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/exceptions.data.json
--rw-r--r--   0        0        0     1579 2023-05-26 09:05:49.920369 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/exceptions.meta.json
--rw-r--r--   0        0        0     9287 2023-05-26 09:05:49.944400 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/findpaths.data.json
--rw-r--r--   0        0        0     1828 2023-05-26 09:05:49.945400 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/findpaths.meta.json
--rw-r--r--   0        0        0    30461 2023-05-26 09:05:50.018051 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/debugging.data.json
--rw-r--r--   0        0        0     2135 2023-05-26 09:05:50.019053 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/debugging.meta.json
--rw-r--r--   0        0        0     7724 2023-05-26 09:05:49.925883 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/deprecated.data.json
--rw-r--r--   0        0        0     1606 2023-05-26 09:05:49.926883 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/deprecated.meta.json
--rw-r--r--   0        0        0    49561 2023-05-26 09:05:50.059039 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/doctest.data.json
--rw-r--r--   0        0        0     2251 2023-05-26 09:05:50.060038 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/doctest.meta.json
--rw-r--r--   0        0        0   173647 2023-05-26 09:05:49.995430 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/fixtures.data.json
--rw-r--r--   0        0        0     2322 2023-05-26 09:05:49.996429 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/fixtures.meta.json
--rw-r--r--   0        0        0     3113 2023-05-26 09:05:48.037452 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/freeze_support.data.json
--rw-r--r--   0        0        0     1662 2023-05-26 09:05:48.039451 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/freeze_support.meta.json
--rw-r--r--   0        0        0     8846 2023-05-26 09:05:50.082039 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/helpconfig.data.json
--rw-r--r--   0        0        0     1782 2023-05-26 09:05:50.083038 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/helpconfig.meta.json
--rw-r--r--   0        0        0    56857 2023-05-26 09:05:49.931884 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/hookspec.data.json
--rw-r--r--   0        0        0     2058 2023-05-26 09:05:49.932883 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/hookspec.meta.json
--rw-r--r--   0        0        0    68092 2023-05-26 09:05:50.073040 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/legacypath.data.json
--rw-r--r--   0        0        0     2000 2023-05-26 09:05:50.074038 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/legacypath.meta.json
--rw-r--r--   0        0        0    73622 2023-05-26 09:05:50.055038 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/logging.data.json
--rw-r--r--   0        0        0     2194 2023-05-26 09:05:50.056038 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/logging.meta.json
--rw-r--r--   0        0        0    50797 2023-05-26 09:05:50.031055 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/main.data.json
--rw-r--r--   0        0        0     2264 2023-05-26 09:05:50.033510 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/main.meta.json
--rw-r--r--   0        0        0    34788 2023-05-26 09:05:49.979914 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/mark/__init__.data.json
--rw-r--r--   0        0        0     1988 2023-05-26 09:05:49.980912 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/mark/__init__.meta.json
--rw-r--r--   0        0        0    36117 2023-05-26 09:05:47.923512 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/mark/expression.data.json
--rw-r--r--   0        0        0     1720 2023-05-26 09:05:47.925041 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/mark/expression.meta.json
--rw-r--r--   0        0        0   126266 2023-05-26 09:05:49.969912 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/mark/structures.data.json
--rw-r--r--   0        0        0     2001 2023-05-26 09:05:49.970912 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/mark/structures.meta.json
--rw-r--r--   0        0        0    24902 2023-05-26 09:05:50.015055 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/monkeypatch.data.json
--rw-r--r--   0        0        0     1832 2023-05-26 09:05:50.016051 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/monkeypatch.meta.json
--rw-r--r--   0        0        0    55874 2023-05-26 09:05:49.975915 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/nodes.data.json
--rw-r--r--   0        0        0     2028 2023-05-26 09:05:49.976912 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/nodes.meta.json
--rw-r--r--   0        0        0    29287 2023-05-26 09:05:49.935401 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/outcomes.data.json
--rw-r--r--   0        0        0     1877 2023-05-26 09:05:49.936401 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/outcomes.meta.json
--rw-r--r--   0        0        0    32236 2023-05-26 09:05:49.941401 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/pathlib.data.json
--rw-r--r--   0        0        0     2075 2023-05-26 09:05:49.942397 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/pathlib.meta.json
--rw-r--r--   0        0        0   128647 2023-05-26 09:05:50.050042 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/pytester.data.json
--rw-r--r--   0        0        0     2554 2023-05-26 09:05:50.051038 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/pytester.meta.json
--rw-r--r--   0        0        0     4466 2023-05-26 09:05:49.998429 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/pytester_assertions.data.json
--rw-r--r--   0        0        0     1584 2023-05-26 09:05:50.000430 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json
--rw-r--r--   0        0        0   130991 2023-05-26 09:05:50.043041 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/python.data.json
--rw-r--r--   0        0        0     2438 2023-05-26 09:05:50.044039 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/python.meta.json
--rw-r--r--   0        0        0    49533 2023-05-26 09:05:49.958911 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/python_api.data.json
--rw-r--r--   0        0        0     1932 2023-05-26 09:05:49.959912 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/python_api.meta.json
--rw-r--r--   0        0        0    29608 2023-05-26 09:05:50.012054 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/recwarn.data.json
--rw-r--r--   0        0        0     1807 2023-05-26 09:05:50.013053 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/recwarn.meta.json
--rw-r--r--   0        0        0    47879 2023-05-26 09:05:49.987916 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/reports.data.json
--rw-r--r--   0        0        0     1931 2023-05-26 09:05:49.989430 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/reports.meta.json
--rw-r--r--   0        0        0    49890 2023-05-26 09:05:50.007429 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/runner.data.json
--rw-r--r--   0        0        0     2162 2023-05-26 09:05:50.009053 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/runner.meta.json
--rw-r--r--   0        0        0    11134 2023-05-26 09:05:49.909925 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/scope.data.json
--rw-r--r--   0        0        0     1614 2023-05-26 09:05:49.910924 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/scope.meta.json
--rw-r--r--   0        0        0    13846 2023-05-26 09:05:47.519041 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/stash.data.json
--rw-r--r--   0        0        0     1533 2023-05-26 09:05:47.520037 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/stash.meta.json
--rw-r--r--   0        0        0    98667 2023-05-26 09:05:50.004428 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/terminal.data.json
--rw-r--r--   0        0        0     2407 2023-05-26 09:05:50.005427 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/terminal.meta.json
--rw-r--r--   0        0        0     1934 2023-05-26 09:05:47.685284 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/timing.data.json
--rw-r--r--   0        0        0     1546 2023-05-26 09:05:47.686286 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/timing.meta.json
--rw-r--r--   0        0        0    23725 2023-05-26 09:05:50.027052 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/tmpdir.data.json
--rw-r--r--   0        0        0     1899 2023-05-26 09:05:50.029054 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/tmpdir.meta.json
--rw-r--r--   0        0        0    33752 2023-05-26 09:05:49.922369 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/warning_types.data.json
--rw-r--r--   0        0        0     1663 2023-05-26 09:05:49.924368 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/warning_types.meta.json
--rw-r--r--   0        0        0    12293 2023-05-26 09:05:50.079040 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/warnings.data.json
--rw-r--r--   0        0        0     1904 2023-05-26 09:05:50.080039 argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/warnings.meta.json
--rw-r--r--   0        0        0    24870 2023-05-26 09:05:46.985187 argos-nac-0.1.2/tests/.mypy_cache/3.11/_stat.data.json
--rw-r--r--   0        0        0     1594 2023-05-26 09:05:46.986187 argos-nac-0.1.2/tests/.mypy_cache/3.11/_stat.meta.json
--rw-r--r--   0        0        0    23875 2023-05-26 09:05:47.057756 argos-nac-0.1.2/tests/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1646 2023-05-26 09:05:47.060756 argos-nac-0.1.2/tests/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0     8141 2023-05-26 09:05:46.976189 argos-nac-0.1.2/tests/.mypy_cache/3.11/_tracemalloc.data.json
--rw-r--r--   0        0        0     1623 2023-05-26 09:05:46.977188 argos-nac-0.1.2/tests/.mypy_cache/3.11/_tracemalloc.meta.json
--rw-r--r--   0        0        0    89069 2023-05-26 09:05:46.883288 argos-nac-0.1.2/tests/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1715 2023-05-26 09:05:46.884288 argos-nac-0.1.2/tests/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    13092 2023-05-26 09:05:47.218990 argos-nac-0.1.2/tests/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1549 2023-05-26 09:05:47.220505 argos-nac-0.1.2/tests/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    27323 2023-05-26 09:05:47.021238 argos-nac-0.1.2/tests/.mypy_cache/3.11/_weakref.data.json
--rw-r--r--   0        0        0     1633 2023-05-26 09:05:47.022239 argos-nac-0.1.2/tests/.mypy_cache/3.11/_weakref.meta.json
--rw-r--r--   0        0        0    50443 2023-05-26 09:05:47.013238 argos-nac-0.1.2/tests/.mypy_cache/3.11/_weakrefset.data.json
--rw-r--r--   0        0        0     1639 2023-05-26 09:05:47.015237 argos-nac-0.1.2/tests/.mypy_cache/3.11/_weakrefset.meta.json
--rw-r--r--   0        0        0    62840 2023-05-26 09:05:46.877289 argos-nac-0.1.2/tests/.mypy_cache/3.11/_winapi.data.json
--rw-r--r--   0        0        0     1671 2023-05-26 09:05:46.878289 argos-nac-0.1.2/tests/.mypy_cache/3.11/_winapi.meta.json
--rw-r--r--   0        0        0    23350 2023-05-26 09:05:46.872290 argos-nac-0.1.2/tests/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1599 2023-05-26 09:05:46.874288 argos-nac-0.1.2/tests/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0   149848 2023-05-26 09:05:47.511409 argos-nac-0.1.2/tests/.mypy_cache/3.11/argparse.data.json
--rw-r--r--   0        0        0     1631 2023-05-26 09:05:47.513407 argos-nac-0.1.2/tests/.mypy_cache/3.11/argparse.meta.json
--rw-r--r--   0        0        0    60690 2023-05-26 09:05:46.868289 argos-nac-0.1.2/tests/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1654 2023-05-26 09:05:46.870288 argos-nac-0.1.2/tests/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137634 2023-05-26 09:05:47.214988 argos-nac-0.1.2/tests/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1685 2023-05-26 09:05:47.215990 argos-nac-0.1.2/tests/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0     8141 2023-05-26 09:05:47.149841 argos-nac-0.1.2/tests/.mypy_cache/3.11/atexit.data.json
--rw-r--r--   0        0        0     1588 2023-05-26 09:05:47.151841 argos-nac-0.1.2/tests/.mypy_cache/3.11/atexit.meta.json
--rw-r--r--   0        0        0   203398 2023-05-26 09:05:47.828367 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/__init__.data.json
--rw-r--r--   0        0        0     1750 2023-05-26 09:05:47.829891 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/__init__.meta.json
--rw-r--r--   0        0        0     3923 2023-05-26 09:05:47.132796 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/_cmp.data.json
--rw-r--r--   0        0        0     1525 2023-05-26 09:05:47.134796 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/_cmp.meta.json
--rw-r--r--   0        0        0     3032 2023-05-26 09:05:47.128798 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/_typing_compat.data.json
--rw-r--r--   0        0        0     1545 2023-05-26 09:05:47.130796 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/_typing_compat.meta.json
--rw-r--r--   0        0        0     7021 2023-05-26 09:05:47.125271 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/_version_info.data.json
--rw-r--r--   0        0        0     1544 2023-05-26 09:05:47.126797 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/_version_info.meta.json
--rw-r--r--   0        0        0     8304 2023-05-26 09:05:47.841893 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/converters.data.json
--rw-r--r--   0        0        0     1548 2023-05-26 09:05:47.842892 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/converters.meta.json
--rw-r--r--   0        0        0    10254 2023-05-26 09:05:47.137314 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/exceptions.data.json
--rw-r--r--   0        0        0     1537 2023-05-26 09:05:47.139313 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/exceptions.meta.json
--rw-r--r--   0        0        0     3555 2023-05-26 09:05:47.838891 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/filters.data.json
--rw-r--r--   0        0        0     1542 2023-05-26 09:05:47.839890 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/filters.meta.json
--rw-r--r--   0        0        0     7687 2023-05-26 09:05:47.835891 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/setters.data.json
--rw-r--r--   0        0        0     1542 2023-05-26 09:05:47.837892 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/setters.meta.json
--rw-r--r--   0        0        0    41655 2023-05-26 09:05:47.831893 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/validators.data.json
--rw-r--r--   0        0        0     1578 2023-05-26 09:05:47.833893 argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/validators.meta.json
--rw-r--r--   0        0        0    50473 2023-05-26 09:05:47.401295 argos-nac-0.1.2/tests/.mypy_cache/3.11/bdb.data.json
--rw-r--r--   0        0        0     1622 2023-05-26 09:05:47.402299 argos-nac-0.1.2/tests/.mypy_cache/3.11/bdb.meta.json
--rw-r--r--   0        0        0    11215 2023-05-26 09:05:47.645732 argos-nac-0.1.2/tests/.mypy_cache/3.11/bisect.data.json
--rw-r--r--   0        0        0     1573 2023-05-26 09:05:47.646732 argos-nac-0.1.2/tests/.mypy_cache/3.11/bisect.meta.json
--rw-r--r--   0        0        0  1130855 2023-05-26 09:05:46.936329 argos-nac-0.1.2/tests/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1736 2023-05-26 09:05:46.938330 argos-nac-0.1.2/tests/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0    20278 2023-05-26 09:05:47.074181 argos-nac-0.1.2/tests/.mypy_cache/3.11/cmd.data.json
--rw-r--r--   0        0        0     1583 2023-05-26 09:05:47.076181 argos-nac-0.1.2/tests/.mypy_cache/3.11/cmd.meta.json
--rw-r--r--   0        0        0   124025 2023-05-26 09:05:46.863291 argos-nac-0.1.2/tests/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1696 2023-05-26 09:05:46.865290 argos-nac-0.1.2/tests/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   408003 2023-05-26 09:05:46.858288 argos-nac-0.1.2/tests/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1673 2023-05-26 09:05:46.859289 argos-nac-0.1.2/tests/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3746 2023-05-26 09:05:46.845245 argos-nac-0.1.2/tests/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1584 2023-05-26 09:05:46.846246 argos-nac-0.1.2/tests/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   109218 2023-05-26 09:05:46.842247 argos-nac-0.1.2/tests/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1645 2023-05-26 09:05:46.843246 argos-nac-0.1.2/tests/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0     5423 2023-05-26 09:05:47.415776 argos-nac-0.1.2/tests/.mypy_cache/3.11/copy.data.json
--rw-r--r--   0        0        0     1538 2023-05-26 09:05:47.416779 argos-nac-0.1.2/tests/.mypy_cache/3.11/copy.meta.json
--rw-r--r--   0        0        0   136830 2023-05-26 09:05:46.836249 argos-nac-0.1.2/tests/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1692 2023-05-26 09:05:46.837247 argos-nac-0.1.2/tests/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0    57759 2023-05-26 09:05:46.829101 argos-nac-0.1.2/tests/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1650 2023-05-26 09:05:46.831100 argos-nac-0.1.2/tests/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142222 2023-05-26 09:05:47.633737 argos-nac-0.1.2/tests/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1610 2023-05-26 09:05:47.634732 argos-nac-0.1.2/tests/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4925 2023-05-26 09:05:47.904994 argos-nac-0.1.2/tests/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1560 2023-05-26 09:05:47.906993 argos-nac-0.1.2/tests/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    58305 2023-05-26 09:05:47.160366 argos-nac-0.1.2/tests/.mypy_cache/3.11/difflib.data.json
--rw-r--r--   0        0        0     1607 2023-05-26 09:05:47.161365 argos-nac-0.1.2/tests/.mypy_cache/3.11/difflib.meta.json
--rw-r--r--   0        0        0    62920 2023-05-26 09:05:47.609710 argos-nac-0.1.2/tests/.mypy_cache/3.11/dis.data.json
--rw-r--r--   0        0        0     1637 2023-05-26 09:05:47.612710 argos-nac-0.1.2/tests/.mypy_cache/3.11/dis.meta.json
--rw-r--r--   0        0        0    69848 2023-05-26 09:05:48.111837 argos-nac-0.1.2/tests/.mypy_cache/3.11/doctest.data.json
--rw-r--r--   0        0        0     1679 2023-05-26 09:05:48.112837 argos-nac-0.1.2/tests/.mypy_cache/3.11/doctest.meta.json
--rw-r--r--   0        0        0     7453 2023-05-26 09:05:46.825578 argos-nac-0.1.2/tests/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1636 2023-05-26 09:05:46.827104 argos-nac-0.1.2/tests/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12215 2023-05-26 09:05:46.822578 argos-nac-0.1.2/tests/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1581 2023-05-26 09:05:46.823578 argos-nac-0.1.2/tests/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7264 2023-05-26 09:05:46.818580 argos-nac-0.1.2/tests/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1613 2023-05-26 09:05:46.820578 argos-nac-0.1.2/tests/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25088 2023-05-26 09:05:46.815580 argos-nac-0.1.2/tests/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1585 2023-05-26 09:05:46.817579 argos-nac-0.1.2/tests/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9169 2023-05-26 09:05:46.813061 argos-nac-0.1.2/tests/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1598 2023-05-26 09:05:46.814060 argos-nac-0.1.2/tests/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79285 2023-05-26 09:05:46.810063 argos-nac-0.1.2/tests/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1701 2023-05-26 09:05:46.812060 argos-nac-0.1.2/tests/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30872 2023-05-26 09:05:46.805060 argos-nac-0.1.2/tests/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1662 2023-05-26 09:05:46.806059 argos-nac-0.1.2/tests/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0    90137 2023-05-26 09:05:46.800542 argos-nac-0.1.2/tests/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1625 2023-05-26 09:05:46.802539 argos-nac-0.1.2/tests/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    24995 2023-05-26 09:05:47.186413 argos-nac-0.1.2/tests/.mypy_cache/3.11/errno.data.json
--rw-r--r--   0        0        0     1575 2023-05-26 09:05:47.188413 argos-nac-0.1.2/tests/.mypy_cache/3.11/errno.meta.json
--rw-r--r--   0        0        0     6106 2023-05-26 09:05:47.363241 argos-nac-0.1.2/tests/.mypy_cache/3.11/fnmatch.data.json
--rw-r--r--   0        0        0     1566 2023-05-26 09:05:47.364241 argos-nac-0.1.2/tests/.mypy_cache/3.11/fnmatch.meta.json
--rw-r--r--   0        0        0   132081 2023-05-26 09:05:47.462375 argos-nac-0.1.2/tests/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1634 2023-05-26 09:05:47.464373 argos-nac-0.1.2/tests/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    15974 2023-05-26 09:05:47.358908 argos-nac-0.1.2/tests/.mypy_cache/3.11/gc.data.json
--rw-r--r--   0        0        0     1609 2023-05-26 09:05:47.360292 argos-nac-0.1.2/tests/.mypy_cache/3.11/gc.meta.json
--rw-r--r--   0        0        0    22402 2023-05-26 09:05:46.795539 argos-nac-0.1.2/tests/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1625 2023-05-26 09:05:46.796539 argos-nac-0.1.2/tests/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     3753 2023-05-26 09:05:47.225503 argos-nac-0.1.2/tests/.mypy_cache/3.11/getpass.data.json
--rw-r--r--   0        0        0     1544 2023-05-26 09:05:47.227503 argos-nac-0.1.2/tests/.mypy_cache/3.11/getpass.meta.json
--rw-r--r--   0        0        0    46204 2023-05-26 09:05:47.484892 argos-nac-0.1.2/tests/.mypy_cache/3.11/gettext.data.json
--rw-r--r--   0        0        0     1628 2023-05-26 09:05:47.486893 argos-nac-0.1.2/tests/.mypy_cache/3.11/gettext.meta.json
--rw-r--r--   0        0        0     9518 2023-05-26 09:05:47.412297 argos-nac-0.1.2/tests/.mypy_cache/3.11/glob.data.json
--rw-r--r--   0        0        0     1588 2023-05-26 09:05:47.413780 argos-nac-0.1.2/tests/.mypy_cache/3.11/glob.meta.json
--rw-r--r--   0        0        0     6140 2023-05-26 09:05:46.792062 argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1613 2023-05-26 09:05:46.793062 argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70594 2023-05-26 09:05:46.790058 argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1759 2023-05-26 09:05:46.791059 argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64586 2023-05-26 09:05:46.785060 argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1748 2023-05-26 09:05:46.786059 argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91135 2023-05-26 09:05:46.780542 argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1758 2023-05-26 09:05:46.781540 argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11951 2023-05-26 09:05:46.774542 argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1602 2023-05-26 09:05:46.776541 argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    21587 2023-05-26 09:05:47.191936 argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/util.data.json
--rw-r--r--   0        0        0     1753 2023-05-26 09:05:47.193936 argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/util.meta.json
--rw-r--r--   0        0        0    44376 2023-05-26 09:05:48.098317 argos-nac-0.1.2/tests/.mypy_cache/3.11/iniconfig/__init__.data.json
--rw-r--r--   0        0        0     1667 2023-05-26 09:05:48.100317 argos-nac-0.1.2/tests/.mypy_cache/3.11/iniconfig/__init__.meta.json
--rw-r--r--   0        0        0    22635 2023-05-26 09:05:47.903470 argos-nac-0.1.2/tests/.mypy_cache/3.11/iniconfig/_parse.data.json
--rw-r--r--   0        0        0     1608 2023-05-26 09:05:47.903995 argos-nac-0.1.2/tests/.mypy_cache/3.11/iniconfig/_parse.meta.json
--rw-r--r--   0        0        0     4539 2023-05-26 09:05:47.601195 argos-nac-0.1.2/tests/.mypy_cache/3.11/iniconfig/exceptions.data.json
--rw-r--r--   0        0        0     1588 2023-05-26 09:05:47.602193 argos-nac-0.1.2/tests/.mypy_cache/3.11/iniconfig/exceptions.meta.json
--rw-r--r--   0        0        0   330902 2023-05-26 09:05:48.032452 argos-nac-0.1.2/tests/.mypy_cache/3.11/inspect.data.json
--rw-r--r--   0        0        0     1675 2023-05-26 09:05:48.033451 argos-nac-0.1.2/tests/.mypy_cache/3.11/inspect.meta.json
--rw-r--r--   0        0        0    85351 2023-05-26 09:05:46.771540 argos-nac-0.1.2/tests/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1698 2023-05-26 09:05:46.772540 argos-nac-0.1.2/tests/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   266323 2023-05-26 09:05:47.341384 argos-nac-0.1.2/tests/.mypy_cache/3.11/itertools.data.json
--rw-r--r--   0        0        0     1636 2023-05-26 09:05:47.342384 argos-nac-0.1.2/tests/.mypy_cache/3.11/itertools.meta.json
--rw-r--r--   0        0        0    15394 2023-05-26 09:05:47.867421 argos-nac-0.1.2/tests/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1625 2023-05-26 09:05:47.869419 argos-nac-0.1.2/tests/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14519 2023-05-26 09:05:47.528039 argos-nac-0.1.2/tests/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1578 2023-05-26 09:05:47.529038 argos-nac-0.1.2/tests/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10899 2023-05-26 09:05:47.524037 argos-nac-0.1.2/tests/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1587 2023-05-26 09:05:47.525037 argos-nac-0.1.2/tests/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   144400 2023-05-26 09:05:47.718327 argos-nac-0.1.2/tests/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1712 2023-05-26 09:05:47.720324 argos-nac-0.1.2/tests/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0     6406 2023-05-26 09:05:47.180410 argos-nac-0.1.2/tests/.mypy_cache/3.11/marshal.data.json
--rw-r--r--   0        0        0     1651 2023-05-26 09:05:47.182412 argos-nac-0.1.2/tests/.mypy_cache/3.11/marshal.meta.json
--rw-r--r--   0        0        0    52525 2023-05-26 09:05:47.249502 argos-nac-0.1.2/tests/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1613 2023-05-26 09:05:47.251503 argos-nac-0.1.2/tests/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    23321 2023-05-26 09:05:46.765544 argos-nac-0.1.2/tests/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1653 2023-05-26 09:05:46.767541 argos-nac-0.1.2/tests/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    14094 2023-05-26 09:05:46.762596 argos-nac-0.1.2/tests/.mypy_cache/3.11/ntpath.data.json
--rw-r--r--   0        0        0     1641 2023-05-26 09:05:46.763544 argos-nac-0.1.2/tests/.mypy_cache/3.11/ntpath.meta.json
--rw-r--r--   0        0        0    78996 2023-05-26 09:05:47.236507 argos-nac-0.1.2/tests/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1544 2023-05-26 09:05:47.237506 argos-nac-0.1.2/tests/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0     6108 2023-05-26 09:05:46.961665 argos-nac-0.1.2/tests/.mypy_cache/3.11/opcode.data.json
--rw-r--r--   0        0        0     1596 2023-05-26 09:05:46.962661 argos-nac-0.1.2/tests/.mypy_cache/3.11/opcode.meta.json
--rw-r--r--   0        0        0    49212 2023-05-26 09:05:47.561081 argos-nac-0.1.2/tests/.mypy_cache/3.11/operator.data.json
--rw-r--r--   0        0        0     1617 2023-05-26 09:05:47.562080 argos-nac-0.1.2/tests/.mypy_cache/3.11/operator.meta.json
--rw-r--r--   0        0        0   236998 2023-05-26 09:05:46.759123 argos-nac-0.1.2/tests/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1751 2023-05-26 09:05:46.761125 argos-nac-0.1.2/tests/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4911 2023-05-26 09:05:46.749607 argos-nac-0.1.2/tests/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1570 2023-05-26 09:05:46.750604 argos-nac-0.1.2/tests/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     3198 2023-05-26 09:05:47.115274 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/__init__.data.json
--rw-r--r--   0        0        0     1534 2023-05-26 09:05:47.116271 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/__init__.meta.json
--rw-r--r--   0        0        0    13851 2023-05-26 09:05:47.555081 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_elffile.data.json
--rw-r--r--   0        0        0     1661 2023-05-26 09:05:47.556081 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_elffile.meta.json
--rw-r--r--   0        0        0    26585 2023-05-26 09:05:47.894472 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_manylinux.data.json
--rw-r--r--   0        0        0     1841 2023-05-26 09:05:47.896469 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_manylinux.meta.json
--rw-r--r--   0        0        0    18213 2023-05-26 09:05:47.878945 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_musllinux.data.json
--rw-r--r--   0        0        0     1754 2023-05-26 09:05:47.879944 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_musllinux.meta.json
--rw-r--r--   0        0        0    44044 2023-05-26 09:05:48.246514 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_parser.data.json
--rw-r--r--   0        0        0     1645 2023-05-26 09:05:48.248032 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_parser.meta.json
--rw-r--r--   0        0        0    13952 2023-05-26 09:05:47.109750 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_structures.data.json
--rw-r--r--   0        0        0     1563 2023-05-26 09:05:47.111750 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_structures.meta.json
--rw-r--r--   0        0        0    17549 2023-05-26 09:05:48.231994 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_tokenizer.data.json
--rw-r--r--   0        0        0     1656 2023-05-26 09:05:48.232993 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_tokenizer.meta.json
--rw-r--r--   0        0        0    17587 2023-05-26 09:05:48.265559 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/markers.data.json
--rw-r--r--   0        0        0     1745 2023-05-26 09:05:48.266557 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/markers.meta.json
--rw-r--r--   0        0        0     8566 2023-05-26 09:05:48.276086 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/requirements.data.json
--rw-r--r--   0        0        0     1719 2023-05-26 09:05:48.278082 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/requirements.meta.json
--rw-r--r--   0        0        0    55975 2023-05-26 09:05:48.215472 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/specifiers.data.json
--rw-r--r--   0        0        0     1694 2023-05-26 09:05:48.217467 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/specifiers.meta.json
--rw-r--r--   0        0        0    27792 2023-05-26 09:05:48.079792 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/tags.data.json
--rw-r--r--   0        0        0     1825 2023-05-26 09:05:48.081790 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/tags.meta.json
--rw-r--r--   0        0        0     9833 2023-05-26 09:05:48.167363 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/utils.data.json
--rw-r--r--   0        0        0     1712 2023-05-26 09:05:48.168361 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/utils.meta.json
--rw-r--r--   0        0        0    65183 2023-05-26 09:05:47.797627 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/version.data.json
--rw-r--r--   0        0        0     1741 2023-05-26 09:05:47.798623 argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/version.meta.json
--rw-r--r--   0        0        0    85758 2023-05-26 09:05:46.745603 argos-nac-0.1.2/tests/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1707 2023-05-26 09:05:46.747606 argos-nac-0.1.2/tests/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    92071 2023-05-26 09:05:48.129421 argos-nac-0.1.2/tests/.mypy_cache/3.11/pdb.data.json
--rw-r--r--   0        0        0     1694 2023-05-26 09:05:48.131363 argos-nac-0.1.2/tests/.mypy_cache/3.11/pdb.meta.json
--rw-r--r--   0        0        0    44407 2023-05-26 09:05:46.741085 argos-nac-0.1.2/tests/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1655 2023-05-26 09:05:46.741608 argos-nac-0.1.2/tests/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    31505 2023-05-26 09:05:47.368240 argos-nac-0.1.2/tests/.mypy_cache/3.11/pkgutil.data.json
--rw-r--r--   0        0        0     1631 2023-05-26 09:05:47.369243 argos-nac-0.1.2/tests/.mypy_cache/3.11/pkgutil.meta.json
--rw-r--r--   0        0        0    34966 2023-05-26 09:05:47.389296 argos-nac-0.1.2/tests/.mypy_cache/3.11/platform.data.json
--rw-r--r--   0        0        0     1575 2023-05-26 09:05:47.391297 argos-nac-0.1.2/tests/.mypy_cache/3.11/platform.meta.json
--rw-r--r--   0        0        0    75211 2023-05-26 09:05:46.737084 argos-nac-0.1.2/tests/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1652 2023-05-26 09:05:46.738084 argos-nac-0.1.2/tests/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0    12026 2023-05-26 09:05:47.469375 argos-nac-0.1.2/tests/.mypy_cache/3.11/pprint.data.json
--rw-r--r--   0        0        0     1571 2023-05-26 09:05:47.470375 argos-nac-0.1.2/tests/.mypy_cache/3.11/pprint.meta.json
--rw-r--r--   0        0        0    11121 2023-05-26 09:05:50.076039 argos-nac-0.1.2/tests/.mypy_cache/3.11/pytest/__init__.data.json
--rw-r--r--   0        0        0     2166 2023-05-26 09:05:50.078039 argos-nac-0.1.2/tests/.mypy_cache/3.11/pytest/__init__.meta.json
--rw-r--r--   0        0        0   167559 2023-05-26 09:05:46.732080 argos-nac-0.1.2/tests/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1726 2023-05-26 09:05:46.734083 argos-nac-0.1.2/tests/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    16749 2023-05-26 09:05:47.003716 argos-nac-0.1.2/tests/.mypy_cache/3.11/reprlib.data.json
--rw-r--r--   0        0        0     1649 2023-05-26 09:05:47.004718 argos-nac-0.1.2/tests/.mypy_cache/3.11/reprlib.meta.json
--rw-r--r--   0        0        0    16510 2023-05-26 09:05:47.407298 argos-nac-0.1.2/tests/.mypy_cache/3.11/shlex.data.json
--rw-r--r--   0        0        0     1615 2023-05-26 09:05:47.408297 argos-nac-0.1.2/tests/.mypy_cache/3.11/shlex.meta.json
--rw-r--r--   0        0        0    71126 2023-05-26 09:05:47.353906 argos-nac-0.1.2/tests/.mypy_cache/3.11/shutil.data.json
--rw-r--r--   0        0        0     1626 2023-05-26 09:05:47.354908 argos-nac-0.1.2/tests/.mypy_cache/3.11/shutil.meta.json
--rw-r--r--   0        0        0    14832 2023-05-26 09:05:47.080183 argos-nac-0.1.2/tests/.mypy_cache/3.11/signal.data.json
--rw-r--r--   0        0        0     1639 2023-05-26 09:05:47.082183 argos-nac-0.1.2/tests/.mypy_cache/3.11/signal.meta.json
--rw-r--r--   0        0        0    14387 2023-05-26 09:05:46.723567 argos-nac-0.1.2/tests/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1597 2023-05-26 09:05:46.725566 argos-nac-0.1.2/tests/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28494 2023-05-26 09:05:46.721563 argos-nac-0.1.2/tests/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1609 2023-05-26 09:05:46.722572 argos-nac-0.1.2/tests/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49755 2023-05-26 09:05:46.717566 argos-nac-0.1.2/tests/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1652 2023-05-26 09:05:46.719563 argos-nac-0.1.2/tests/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0     8866 2023-05-26 09:05:47.641735 argos-nac-0.1.2/tests/.mypy_cache/3.11/stat.data.json
--rw-r--r--   0        0        0     1550 2023-05-26 09:05:47.642734 argos-nac-0.1.2/tests/.mypy_cache/3.11/stat.meta.json
--rw-r--r--   0        0        0    27762 2023-05-26 09:05:47.039239 argos-nac-0.1.2/tests/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1637 2023-05-26 09:05:47.040757 argos-nac-0.1.2/tests/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0    15313 2023-05-26 09:05:47.174891 argos-nac-0.1.2/tests/.mypy_cache/3.11/struct.data.json
--rw-r--r--   0        0        0     1634 2023-05-26 09:05:47.176891 argos-nac-0.1.2/tests/.mypy_cache/3.11/struct.meta.json
--rw-r--r--   0        0        0   167815 2023-05-26 09:05:46.713564 argos-nac-0.1.2/tests/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1717 2023-05-26 09:05:46.714564 argos-nac-0.1.2/tests/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   165686 2023-05-26 09:05:46.705254 argos-nac-0.1.2/tests/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1685 2023-05-26 09:05:46.706254 argos-nac-0.1.2/tests/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    14479 2023-05-26 09:05:46.942330 argos-nac-0.1.2/tests/.mypy_cache/3.11/sysconfig.data.json
--rw-r--r--   0        0        0     1601 2023-05-26 09:05:46.943663 argos-nac-0.1.2/tests/.mypy_cache/3.11/sysconfig.meta.json
--rw-r--r--   0        0        0   133952 2023-05-26 09:05:47.443846 argos-nac-0.1.2/tests/.mypy_cache/3.11/tempfile.data.json
--rw-r--r--   0        0        0     1706 2023-05-26 09:05:47.445377 argos-nac-0.1.2/tests/.mypy_cache/3.11/tempfile.meta.json
--rw-r--r--   0        0        0    19567 2023-05-26 09:05:47.475374 argos-nac-0.1.2/tests/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1579 2023-05-26 09:05:47.476373 argos-nac-0.1.2/tests/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0    64729 2023-05-26 09:05:47.063756 argos-nac-0.1.2/tests/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1649 2023-05-26 09:05:47.065757 argos-nac-0.1.2/tests/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    38018 2023-05-26 09:05:47.032238 argos-nac-0.1.2/tests/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1590 2023-05-26 09:05:47.033238 argos-nac-0.1.2/tests/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0    14927 2023-05-26 09:05:46.997773 argos-nac-0.1.2/tests/.mypy_cache/3.11/token.data.json
--rw-r--r--   0        0        0     1570 2023-05-26 09:05:46.998716 argos-nac-0.1.2/tests/.mypy_cache/3.11/token.meta.json
--rw-r--r--   0        0        0    49284 2023-05-26 09:05:47.654251 argos-nac-0.1.2/tests/.mypy_cache/3.11/tokenize.data.json
--rw-r--r--   0        0        0     1651 2023-05-26 09:05:47.655251 argos-nac-0.1.2/tests/.mypy_cache/3.11/tokenize.meta.json
--rw-r--r--   0        0        0     5254 2023-05-26 09:05:47.119278 argos-nac-0.1.2/tests/.mypy_cache/3.11/tomllib.data.json
--rw-r--r--   0        0        0     1582 2023-05-26 09:05:47.121272 argos-nac-0.1.2/tests/.mypy_cache/3.11/tomllib.meta.json
--rw-r--r--   0        0        0    57032 2023-05-26 09:05:47.382297 argos-nac-0.1.2/tests/.mypy_cache/3.11/traceback.data.json
--rw-r--r--   0        0        0     1634 2023-05-26 09:05:47.383300 argos-nac-0.1.2/tests/.mypy_cache/3.11/traceback.meta.json
--rw-r--r--   0        0        0    48912 2023-05-26 09:05:46.979189 argos-nac-0.1.2/tests/.mypy_cache/3.11/tracemalloc.data.json
--rw-r--r--   0        0        0     1646 2023-05-26 09:05:46.980187 argos-nac-0.1.2/tests/.mypy_cache/3.11/tracemalloc.meta.json
--rw-r--r--   0        0        0   239646 2023-05-26 09:05:46.697728 argos-nac-0.1.2/tests/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1663 2023-05-26 09:05:46.699260 argos-nac-0.1.2/tests/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432248 2023-05-26 09:05:46.686727 argos-nac-0.1.2/tests/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1714 2023-05-26 09:05:46.688728 argos-nac-0.1.2/tests/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57859 2023-05-26 09:05:46.671728 argos-nac-0.1.2/tests/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1670 2023-05-26 09:05:46.672729 argos-nac-0.1.2/tests/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    41974 2023-05-26 09:05:47.168893 argos-nac-0.1.2/tests/.mypy_cache/3.11/unicodedata.data.json
--rw-r--r--   0        0        0     1604 2023-05-26 09:05:47.170892 argos-nac-0.1.2/tests/.mypy_cache/3.11/unicodedata.meta.json
--rw-r--r--   0        0        0     6208 2023-05-26 09:05:47.995092 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/__init__.data.json
--rw-r--r--   0        0        0     1769 2023-05-26 09:05:47.996091 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/__init__.meta.json
--rw-r--r--   0        0        0    24083 2023-05-26 09:05:47.966091 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/_log.data.json
--rw-r--r--   0        0        0     1632 2023-05-26 09:05:47.967090 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/_log.meta.json
--rw-r--r--   0        0        0     9283 2023-05-26 09:05:47.978090 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/async_case.data.json
--rw-r--r--   0        0        0     1680 2023-05-26 09:05:47.979091 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/async_case.meta.json
--rw-r--r--   0        0        0   210169 2023-05-26 09:05:47.975092 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/case.data.json
--rw-r--r--   0        0        0     1762 2023-05-26 09:05:47.976096 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/case.meta.json
--rw-r--r--   0        0        0    14633 2023-05-26 09:05:47.988092 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/loader.data.json
--rw-r--r--   0        0        0     1688 2023-05-26 09:05:47.989092 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/loader.meta.json
--rw-r--r--   0        0        0    11741 2023-05-26 09:05:47.991093 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/main.data.json
--rw-r--r--   0        0        0     1697 2023-05-26 09:05:47.993090 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/main.meta.json
--rw-r--r--   0        0        0    20593 2023-05-26 09:05:47.960090 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/result.data.json
--rw-r--r--   0        0        0     1650 2023-05-26 09:05:47.964092 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/result.meta.json
--rw-r--r--   0        0        0    10760 2023-05-26 09:05:47.986090 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/runner.data.json
--rw-r--r--   0        0        0     1690 2023-05-26 09:05:47.987089 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/runner.meta.json
--rw-r--r--   0        0        0    11279 2023-05-26 09:05:47.983092 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/signals.data.json
--rw-r--r--   0        0        0     1648 2023-05-26 09:05:47.984090 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/signals.meta.json
--rw-r--r--   0        0        0    11265 2023-05-26 09:05:47.980091 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/suite.data.json
--rw-r--r--   0        0        0     1667 2023-05-26 09:05:47.982089 argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/suite.meta.json
--rw-r--r--   0        0        0     1510 2023-05-26 09:05:47.083707 argos-nac-0.1.2/tests/.mypy_cache/3.11/urllib/__init__.data.json
--rw-r--r--   0        0        0     1551 2023-05-26 09:05:47.085704 argos-nac-0.1.2/tests/.mypy_cache/3.11/urllib/__init__.meta.json
--rw-r--r--   0        0        0   175327 2023-05-26 09:05:47.100226 argos-nac-0.1.2/tests/.mypy_cache/3.11/urllib/parse.data.json
--rw-r--r--   0        0        0     1642 2023-05-26 09:05:47.102224 argos-nac-0.1.2/tests/.mypy_cache/3.11/urllib/parse.meta.json
--rw-r--r--   0        0        0    33600 2023-05-26 09:05:47.146315 argos-nac-0.1.2/tests/.mypy_cache/3.11/uuid.data.json
--rw-r--r--   0        0        0     1655 2023-05-26 09:05:47.146846 argos-nac-0.1.2/tests/.mypy_cache/3.11/uuid.meta.json
--rw-r--r--   0        0        0    23803 2023-05-26 09:05:47.849892 argos-nac-0.1.2/tests/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1649 2023-05-26 09:05:47.851893 argos-nac-0.1.2/tests/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0   142942 2023-05-26 09:05:47.682282 argos-nac-0.1.2/tests/.mypy_cache/3.11/weakref.data.json
--rw-r--r--   0        0        0     1655 2023-05-26 09:05:47.683283 argos-nac-0.1.2/tests/.mypy_cache/3.11/weakref.meta.json
--rw-r--r--   0        0        0     1400 2023-05-26 09:05:47.531038 argos-nac-0.1.2/tests/.mypy_cache/3.11/work/__init__.data.json
--rw-r--r--   0        0        0     1452 2023-05-26 09:05:47.532036 argos-nac-0.1.2/tests/.mypy_cache/3.11/work/__init__.meta.json
--rw-r--r--   0        0        0     1714 2023-05-26 09:05:47.543551 argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects/argos/controller/tests/__init__.data.json
--rw-r--r--   0        0        0     1532 2023-05-26 09:05:47.545553 argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects/argos/controller/tests/__init__.meta.json
--rw-r--r--   0        0        0     1395 2023-05-26 09:05:47.541036 argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects/argos/controller.data.json
--rw-r--r--   0        0        0     1445 2023-05-26 10:05:52.291632 argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects/argos/controller.meta.json
--rw-r--r--   0        0        0     1317 2023-05-26 09:05:47.538037 argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects/argos.data.json
--rw-r--r--   0        0        0     1422 2023-05-26 09:05:47.539036 argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects/argos.meta.json
--rw-r--r--   0        0        0     1274 2023-05-26 09:05:47.534042 argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects.data.json
--rw-r--r--   0        0        0     1409 2023-05-26 09:05:47.536036 argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects.meta.json
--rw-r--r--   0        0        0      193 2023-05-26 09:05:50.102561 argos-nac-0.1.2/tests/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        0 2023-05-14 17:18:53.063545 argos-nac-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-30 13:13:31.249105 argos-nac-0.1.2/tests/cisco_test.py
--rw-r--r--   0        0        0     2923 2023-05-26 06:59:58.816158 argos-nac-0.1.2/tests/configs/PE1.log
--rw-r--r--   0        0        0     1932 2023-05-30 13:13:31.250157 argos-nac-0.1.2/tests/configs/PE1_expected.log
--rw-r--r--   0        0        0     2802 2023-05-30 13:13:31.250672 argos-nac-0.1.2/tests/configs/PE2.log
--rw-r--r--   0        0        0     1921 2023-05-30 13:13:31.251670 argos-nac-0.1.2/tests/configs/PE2_expected.log
--rw-r--r--   0        0        0    29598 2023-05-30 13:13:31.251670 argos-nac-0.1.2/tests/site_sample_data.json
--rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 argos-nac-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       10 2023-03-21 16:37:52.480936 argos-nac-0.1.3/graphql_schema/.gitignore
+-rw-r--r--   0        0        0      311 2023-04-06 09:35:21.416520 argos-nac-0.1.3/graphql_schema/__init__.py
+-rw-r--r--   0        0        0     1158 2023-03-21 16:37:09.958974 argos-nac-0.1.3/graphql_schema/gen_schema.py
+-rw-r--r--   0        0        0  2602951 2023-03-20 15:36:54.363420 argos-nac-0.1.3/graphql_schema/schema.py
+-rw-r--r--   0        0        0     1440 2023-03-20 13:23:43.292829 argos-nac-0.1.3/graphql_schema/schema_query.gql
+-rw-r--r--   0        0        0       36 2023-05-10 23:04:17.246649 argos-nac-0.1.3/nac/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0        2 2023-05-12 06:43:07.044719 argos-nac-0.1.3/nac/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   180391 2023-05-10 23:04:17.062153 argos-nac-0.1.3/nac/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1601 2023-05-10 23:04:17.063151 argos-nac-0.1.3/nac/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    58135 2023-05-10 23:04:17.054152 argos-nac-0.1.3/nac/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1694 2023-05-10 23:04:17.055653 argos-nac-0.1.3/nac/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18250 2023-05-10 23:04:17.049652 argos-nac-0.1.3/nac/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1620 2023-05-10 23:04:17.051151 argos-nac-0.1.3/nac/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     7234 2023-05-10 23:04:17.046155 argos-nac-0.1.3/nac/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1619 2023-05-10 23:04:17.047655 argos-nac-0.1.3/nac/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    23884 2023-05-10 23:04:17.174654 argos-nac-0.1.3/nac/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1655 2023-05-10 23:04:17.176653 argos-nac-0.1.3/nac/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0    89078 2023-05-10 23:04:17.043152 argos-nac-0.1.3/nac/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1724 2023-05-10 23:04:17.044155 argos-nac-0.1.3/nac/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    62849 2023-05-10 23:04:17.036155 argos-nac-0.1.3/nac/.mypy_cache/3.11/_winapi.data.json
+-rw-r--r--   0        0        0     1680 2023-05-10 23:04:17.038153 argos-nac-0.1.3/nac/.mypy_cache/3.11/_winapi.meta.json
+-rw-r--r--   0        0        0    23359 2023-05-10 23:04:17.031650 argos-nac-0.1.3/nac/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1608 2023-05-10 23:04:17.033154 argos-nac-0.1.3/nac/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60699 2023-05-10 23:04:17.028653 argos-nac-0.1.3/nac/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1663 2023-05-10 23:04:17.030152 argos-nac-0.1.3/nac/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0  1130864 2023-05-10 23:04:17.142151 argos-nac-0.1.3/nac/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1755 2023-05-10 23:04:17.143150 argos-nac-0.1.3/nac/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   124034 2023-05-10 23:04:17.024152 argos-nac-0.1.3/nac/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1705 2023-05-10 23:04:17.025154 argos-nac-0.1.3/nac/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   408012 2023-05-10 23:04:17.018152 argos-nac-0.1.3/nac/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1682 2023-05-10 23:04:17.019652 argos-nac-0.1.3/nac/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3755 2023-05-10 23:04:17.003651 argos-nac-0.1.3/nac/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1593 2023-05-10 23:04:17.005152 argos-nac-0.1.3/nac/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   109227 2023-05-10 23:04:17.001152 argos-nac-0.1.3/nac/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1654 2023-05-10 23:04:17.002157 argos-nac-0.1.3/nac/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0   136839 2023-05-10 23:04:16.995650 argos-nac-0.1.3/nac/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1701 2023-05-10 23:04:16.997152 argos-nac-0.1.3/nac/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    57768 2023-05-10 23:04:16.988915 argos-nac-0.1.3/nac/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1659 2023-05-10 23:04:16.990152 argos-nac-0.1.3/nac/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0     7462 2023-05-10 23:04:16.985151 argos-nac-0.1.3/nac/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1645 2023-05-10 23:04:16.986152 argos-nac-0.1.3/nac/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12224 2023-05-10 23:04:16.982154 argos-nac-0.1.3/nac/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1590 2023-05-10 23:04:16.983652 argos-nac-0.1.3/nac/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7273 2023-05-10 23:04:16.979151 argos-nac-0.1.3/nac/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1622 2023-05-10 23:04:16.980654 argos-nac-0.1.3/nac/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25097 2023-05-10 23:04:16.976152 argos-nac-0.1.3/nac/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1594 2023-05-10 23:04:16.977152 argos-nac-0.1.3/nac/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9178 2023-05-10 23:04:16.973152 argos-nac-0.1.3/nac/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1607 2023-05-10 23:04:16.974652 argos-nac-0.1.3/nac/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79294 2023-05-10 23:04:16.970652 argos-nac-0.1.3/nac/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1710 2023-05-10 23:04:16.971651 argos-nac-0.1.3/nac/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30881 2023-05-10 23:04:16.965152 argos-nac-0.1.3/nac/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1671 2023-05-10 23:04:16.966651 argos-nac-0.1.3/nac/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0    90146 2023-05-10 23:04:16.960655 argos-nac-0.1.3/nac/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1634 2023-05-10 23:04:16.962154 argos-nac-0.1.3/nac/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    22411 2023-05-10 23:04:16.955651 argos-nac-0.1.3/nac/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1634 2023-05-10 23:04:16.956655 argos-nac-0.1.3/nac/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     6149 2023-05-10 23:04:16.952653 argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1622 2023-05-10 23:04:16.953654 argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70603 2023-05-10 23:04:16.946152 argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1768 2023-05-10 23:04:16.947152 argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64595 2023-05-10 23:04:16.941153 argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1757 2023-05-10 23:04:16.942653 argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91144 2023-05-10 23:04:16.936651 argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1767 2023-05-10 23:04:16.938152 argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11960 2023-05-10 23:04:16.930652 argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1611 2023-05-10 23:04:16.932152 argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    85360 2023-05-10 23:04:16.927651 argos-nac-0.1.3/nac/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1707 2023-05-10 23:04:16.928654 argos-nac-0.1.3/nac/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   144294 2023-05-10 23:04:17.226153 argos-nac-0.1.3/nac/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1721 2023-05-10 23:04:17.227652 argos-nac-0.1.3/nac/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0    23330 2023-05-10 23:04:16.922653 argos-nac-0.1.3/nac/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1662 2023-05-10 23:04:16.924155 argos-nac-0.1.3/nac/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    14103 2023-05-10 23:04:16.919151 argos-nac-0.1.3/nac/.mypy_cache/3.11/ntpath.data.json
+-rw-r--r--   0        0        0     1650 2023-05-10 23:04:16.920653 argos-nac-0.1.3/nac/.mypy_cache/3.11/ntpath.meta.json
+-rw-r--r--   0        0        0   237007 2023-05-10 23:04:16.915651 argos-nac-0.1.3/nac/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1760 2023-05-10 23:04:16.916652 argos-nac-0.1.3/nac/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4920 2023-05-10 23:04:16.906151 argos-nac-0.1.3/nac/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1579 2023-05-10 23:04:16.907653 argos-nac-0.1.3/nac/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0    85743 2023-05-10 23:04:16.903653 argos-nac-0.1.3/nac/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1716 2023-05-10 23:04:16.904654 argos-nac-0.1.3/nac/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    44416 2023-05-10 23:04:16.898152 argos-nac-0.1.3/nac/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1664 2023-05-10 23:04:16.899652 argos-nac-0.1.3/nac/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75220 2023-05-10 23:04:16.895151 argos-nac-0.1.3/nac/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1661 2023-05-10 23:04:16.896153 argos-nac-0.1.3/nac/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167568 2023-05-10 23:04:16.890152 argos-nac-0.1.3/nac/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1735 2023-05-10 23:04:16.891651 argos-nac-0.1.3/nac/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14396 2023-05-10 23:04:16.882652 argos-nac-0.1.3/nac/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1606 2023-05-10 23:04:16.883651 argos-nac-0.1.3/nac/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28503 2023-05-10 23:04:16.879651 argos-nac-0.1.3/nac/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1618 2023-05-10 23:04:16.880651 argos-nac-0.1.3/nac/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49764 2023-05-10 23:04:16.876154 argos-nac-0.1.3/nac/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1661 2023-05-10 23:04:16.877652 argos-nac-0.1.3/nac/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0    27771 2023-05-10 23:04:17.157652 argos-nac-0.1.3/nac/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1646 2023-05-10 23:04:17.159151 argos-nac-0.1.3/nac/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0   167824 2023-05-10 23:04:16.872153 argos-nac-0.1.3/nac/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1726 2023-05-10 23:04:16.873153 argos-nac-0.1.3/nac/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   159493 2023-05-10 23:04:16.864652 argos-nac-0.1.3/nac/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1694 2023-05-10 23:04:16.866152 argos-nac-0.1.3/nac/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    64738 2023-05-10 23:04:17.179651 argos-nac-0.1.3/nac/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1658 2023-05-10 23:04:17.181153 argos-nac-0.1.3/nac/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    38027 2023-05-10 23:04:17.151151 argos-nac-0.1.3/nac/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1599 2023-05-10 23:04:17.153154 argos-nac-0.1.3/nac/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0   239655 2023-05-10 23:04:16.857152 argos-nac-0.1.3/nac/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1672 2023-05-10 23:04:16.858652 argos-nac-0.1.3/nac/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432425 2023-05-10 23:04:16.847651 argos-nac-0.1.3/nac/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1723 2023-05-10 23:04:16.848651 argos-nac-0.1.3/nac/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57889 2023-05-10 23:04:16.832150 argos-nac-0.1.3/nac/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1679 2023-05-10 23:04:16.833651 argos-nac-0.1.3/nac/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0     1400 2023-05-10 23:04:17.182651 argos-nac-0.1.3/nac/.mypy_cache/3.11/work/__init__.data.json
+-rw-r--r--   0        0        0     1452 2023-05-10 23:04:17.184152 argos-nac-0.1.3/nac/.mypy_cache/3.11/work/__init__.meta.json
+-rw-r--r--   0        0        0     1698 2023-05-10 23:04:17.193651 argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.data.json
+-rw-r--r--   0        0        0     1528 2023-05-10 23:04:17.194653 argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.meta.json
+-rw-r--r--   0        0        0    49114 2023-05-10 23:04:17.238651 argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/model.data.json
+-rw-r--r--   0        0        0     1656 2023-05-10 23:04:17.240153 argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/model.meta.json
+-rw-r--r--   0        0        0     1395 2023-05-10 23:04:17.190652 argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos/controller.data.json
+-rw-r--r--   0        0        0     1445 2023-05-10 23:04:17.191652 argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos/controller.meta.json
+-rw-r--r--   0        0        0     1317 2023-05-10 23:04:17.188154 argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos.data.json
+-rw-r--r--   0        0        0     1422 2023-05-11 08:05:37.470673 argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos.meta.json
+-rw-r--r--   0        0        0     1274 2023-05-10 23:04:17.185653 argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects.data.json
+-rw-r--r--   0        0        0     1409 2023-05-10 23:04:17.187153 argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects.meta.json
+-rw-r--r--   0        0        0      193 2023-05-10 23:04:17.250652 argos-nac-0.1.3/nac/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        0 2023-05-30 06:35:53.597209 argos-nac-0.1.3/nac/__init__.py
+-rw-r--r--   0        0        0      417 2023-06-02 21:36:52.295500 argos-nac-0.1.3/nac/__main__.py
+-rw-r--r--   0        0        0       22 2023-06-02 19:45:10.978375 argos-nac-0.1.3/nac/__version__.py
+-rw-r--r--   0        0        0       74 2023-05-26 06:59:58.793027 argos-nac-0.1.3/nac/cisco/__init__.py
+-rw-r--r--   0        0        0     3571 2023-05-30 13:13:31.234054 argos-nac-0.1.3/nac/cisco/controller.py
+-rw-r--r--   0        0        0     2650 2023-05-30 13:13:31.235056 argos-nac-0.1.3/nac/cisco/nornir_util.py
+-rw-r--r--   0        0        0       75 2023-05-26 06:59:58.797861 argos-nac-0.1.3/nac/cisco/protocols/__init__.py
+-rw-r--r--   0        0        0     5728 2023-05-30 13:13:31.236055 argos-nac-0.1.3/nac/cisco/protocols/bgp.py
+-rw-r--r--   0        0        0     1880 2023-05-30 13:13:31.236055 argos-nac-0.1.3/nac/cisco/protocols/ldp.py
+-rw-r--r--   0        0        0     2337 2023-05-30 13:13:31.237055 argos-nac-0.1.3/nac/cisco/protocols/vrf.py
+-rw-r--r--   0        0        0       98 2023-05-30 13:13:31.238055 argos-nac-0.1.3/nac/constants.py
+-rw-r--r--   0        0        0     7183 2023-06-02 21:40:57.095176 argos-nac-0.1.3/nac/main.py
+-rw-r--r--   0        0        0     5182 2023-05-30 13:13:31.242743 argos-nac-0.1.3/nac/model.py
+-rw-r--r--   0        0        0     2188 2023-05-30 13:13:31.243293 argos-nac-0.1.3/nac/queries/main.gql
+-rw-r--r--   0        0        0       36 2023-05-28 09:22:24.169770 argos-nac-0.1.3/nac/util/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0        2 2023-05-29 09:23:35.916730 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   180382 2023-05-28 09:22:23.971852 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1645 2023-05-28 09:22:23.972852 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    58126 2023-05-28 09:22:23.963749 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1685 2023-05-28 09:22:23.965862 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18241 2023-05-28 09:22:23.958748 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1611 2023-05-28 09:22:23.960749 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     7225 2023-05-28 09:22:23.955882 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1610 2023-05-28 09:22:23.957753 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    23875 2023-05-28 09:22:24.086799 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1646 2023-05-28 09:22:24.088770 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0    89069 2023-05-28 09:22:23.954330 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1715 2023-05-28 09:22:23.955330 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    62840 2023-05-28 09:22:23.948350 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_winapi.data.json
+-rw-r--r--   0        0        0     1671 2023-05-28 09:22:23.950332 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_winapi.meta.json
+-rw-r--r--   0        0        0    23350 2023-05-28 09:22:23.944352 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1599 2023-05-28 09:22:23.945351 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60690 2023-05-28 09:22:23.941348 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1654 2023-05-28 09:22:23.942349 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0  1130855 2023-05-28 09:22:24.049760 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1736 2023-05-28 09:22:24.051759 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   124025 2023-05-28 09:22:23.937349 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1696 2023-05-28 09:22:23.938351 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   408003 2023-05-28 09:22:23.930336 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1726 2023-05-28 09:22:23.932340 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3746 2023-05-28 09:22:23.916029 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1584 2023-05-28 09:22:23.917028 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   109218 2023-05-28 09:22:23.912028 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1645 2023-05-28 09:22:23.914029 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0   136830 2023-05-28 09:22:23.907027 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1692 2023-05-28 09:22:23.908031 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    57759 2023-05-28 09:22:23.899009 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1650 2023-05-28 09:22:23.901007 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0     7453 2023-05-28 09:22:23.894746 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1636 2023-05-28 09:22:23.896013 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12215 2023-05-28 09:22:23.892746 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1581 2023-05-28 09:22:23.893747 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7264 2023-05-28 09:22:23.889750 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1613 2023-05-28 09:22:23.890748 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25088 2023-05-28 09:22:23.887656 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1585 2023-05-28 09:22:23.888749 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9169 2023-05-28 09:22:23.883658 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1598 2023-05-28 09:22:23.884658 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79285 2023-05-28 09:22:23.880656 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1701 2023-05-28 09:22:23.881657 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30872 2023-05-28 09:22:23.876657 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1662 2023-05-28 09:22:23.877659 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0    90137 2023-05-28 09:22:23.872659 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1625 2023-05-28 09:22:23.873656 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    22402 2023-05-28 09:22:23.867657 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1625 2023-05-28 09:22:23.868657 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     6140 2023-05-28 09:22:23.863779 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1613 2023-05-28 09:22:23.865743 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70594 2023-05-28 09:22:23.861779 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1759 2023-05-28 09:22:23.862779 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64586 2023-05-28 09:22:23.856745 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1748 2023-05-28 09:22:23.858780 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91135 2023-05-28 09:22:23.851745 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1758 2023-05-28 09:22:23.852744 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11951 2023-05-28 09:22:23.845728 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1602 2023-05-28 09:22:23.846728 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    85351 2023-05-28 09:22:23.842728 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1698 2023-05-28 09:22:23.843728 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   144400 2023-05-28 09:22:24.138780 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1712 2023-05-28 09:22:24.139777 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0    23321 2023-05-28 09:22:23.837728 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1653 2023-05-28 09:22:23.838727 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    14094 2023-05-28 09:22:23.834730 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/ntpath.data.json
+-rw-r--r--   0        0        0     1641 2023-05-28 09:22:23.836727 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/ntpath.meta.json
+-rw-r--r--   0        0        0   236998 2023-05-28 09:22:23.831728 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1751 2023-05-28 09:22:23.832730 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4911 2023-05-28 09:22:23.821749 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1570 2023-05-28 09:22:23.822749 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0    85758 2023-05-28 09:22:23.818753 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1707 2023-05-28 09:22:23.819750 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    44407 2023-05-28 09:22:23.813750 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1655 2023-05-28 09:22:23.814749 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75211 2023-05-28 09:22:23.810750 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1652 2023-05-28 09:22:23.811751 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167559 2023-05-28 09:22:23.805751 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1726 2023-05-28 09:22:23.806749 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14387 2023-05-28 09:22:23.798751 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1597 2023-05-28 09:22:23.799750 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28494 2023-05-28 09:22:23.795754 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1609 2023-05-28 09:22:23.797717 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49755 2023-05-28 09:22:23.792746 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1652 2023-05-28 09:22:23.793747 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0    27762 2023-05-28 09:22:24.068900 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1637 2023-05-28 09:22:24.069897 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0   167815 2023-05-28 09:22:23.789745 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1717 2023-05-28 09:22:23.790746 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   165686 2023-05-28 09:22:23.782597 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1685 2023-05-28 09:22:23.783595 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    64729 2023-05-28 09:22:24.090772 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1649 2023-05-28 09:22:24.092773 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    38018 2023-05-28 09:22:24.060158 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1590 2023-05-28 09:22:24.063161 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0   239646 2023-05-28 09:22:23.775599 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1663 2023-05-28 09:22:23.776596 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432248 2023-05-28 09:22:23.765854 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1714 2023-05-28 09:22:23.766848 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57859 2023-05-28 09:22:23.749761 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1670 2023-05-28 09:22:23.750757 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0     1400 2023-05-28 09:22:24.093772 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/__init__.data.json
+-rw-r--r--   0        0        0     1452 2023-05-28 09:22:24.094771 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/__init__.meta.json
+-rw-r--r--   0        0        0     1698 2023-05-28 09:22:24.103771 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.data.json
+-rw-r--r--   0        0        0     1528 2023-05-28 09:22:24.104771 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.meta.json
+-rw-r--r--   0        0        0     5955 2023-05-28 09:22:24.162781 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util/netbox_api.data.json
+-rw-r--r--   0        0        0     1609 2023-05-28 09:22:24.163782 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util/netbox_api.meta.json
+-rw-r--r--   0        0        0     1460 2023-05-28 09:22:24.106782 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util.data.json
+-rw-r--r--   0        0        0     1465 2023-05-29 09:23:32.839349 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util.meta.json
+-rw-r--r--   0        0        0     1395 2023-05-28 09:22:24.101775 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller.data.json
+-rw-r--r--   0        0        0     1445 2023-05-28 09:22:24.102772 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller.meta.json
+-rw-r--r--   0        0        0     1317 2023-05-28 09:22:24.098772 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos.data.json
+-rw-r--r--   0        0        0     1422 2023-05-28 09:22:24.099773 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos.meta.json
+-rw-r--r--   0        0        0     1274 2023-05-28 09:22:24.095772 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects.data.json
+-rw-r--r--   0        0        0     1409 2023-05-28 09:22:24.096775 argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects.meta.json
+-rw-r--r--   0        0        0      193 2023-05-28 09:22:24.173767 argos-nac-0.1.3/nac/util/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        0 2023-05-31 13:41:33.410344 argos-nac-0.1.3/nac/util/__init__.py
+-rw-r--r--   0        0        0     3792 2023-06-02 20:58:06.336927 argos-nac-0.1.3/nac/util/common.py
+-rw-r--r--   0        0        0     2738 2023-05-30 13:13:31.244892 argos-nac-0.1.3/nac/util/graphql_util.py
+-rw-r--r--   0        0        0      369 2023-05-26 06:59:58.806115 argos-nac-0.1.3/nac/util/jinja_util.py
+-rw-r--r--   0        0        0     2092 2023-05-30 13:23:09.225378 argos-nac-0.1.3/nac/util/netbox_api.py
+-rw-r--r--   0        0        0     1339 2023-06-02 21:37:05.316676 argos-nac-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-05-31 13:41:33.812536 argos-nac-0.1.3/README.md
+-rw-r--r--   0        0        0       36 2023-05-26 09:05:50.098560 argos-nac-0.1.3/tests/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0        2 2023-05-26 10:05:55.185213 argos-nac-0.1.3/tests/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7835 2023-05-26 09:05:47.068757 argos-nac-0.1.3/tests/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1575 2023-05-26 09:05:47.069756 argos-nac-0.1.3/tests/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180382 2023-05-26 09:05:46.903810 argos-nac-0.1.3/tests/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1592 2023-05-26 09:05:46.904813 argos-nac-0.1.3/tests/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    43208 2023-05-26 09:05:46.992186 argos-nac-0.1.3/tests/.mypy_cache/3.11/_bisect.data.json
+-rw-r--r--   0        0        0     1594 2023-05-26 09:05:46.993185 argos-nac-0.1.3/tests/.mypy_cache/3.11/_bisect.meta.json
+-rw-r--r--   0        0        0    58126 2023-05-26 09:05:46.895812 argos-nac-0.1.3/tests/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1685 2023-05-26 09:05:46.897807 argos-nac-0.1.3/tests/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18241 2023-05-26 09:05:46.889812 argos-nac-0.1.3/tests/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1611 2023-05-26 09:05:46.891808 argos-nac-0.1.3/tests/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     7225 2023-05-26 09:05:46.886289 argos-nac-0.1.3/tests/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1610 2023-05-26 09:05:46.887288 argos-nac-0.1.3/tests/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171945 2023-05-26 09:05:47.596194 argos-nac-0.1.3/tests/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1649 2023-05-26 09:05:47.597193 argos-nac-0.1.3/tests/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0   113943 2023-05-26 09:05:46.957662 argos-nac-0.1.3/tests/.mypy_cache/3.11/_operator.data.json
+-rw-r--r--   0        0        0     1622 2023-05-26 09:05:46.959665 argos-nac-0.1.3/tests/.mypy_cache/3.11/_operator.meta.json
+-rw-r--r--   0        0        0     2096 2023-05-26 09:05:47.861430 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/__init__.data.json
+-rw-r--r--   0        0        0     1553 2023-05-26 09:05:47.862420 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/__init__.meta.json
+-rw-r--r--   0        0        0     5668 2023-05-26 09:05:47.856892 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_argcomplete.data.json
+-rw-r--r--   0        0        0     1705 2023-05-26 09:05:47.858894 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_argcomplete.meta.json
+-rw-r--r--   0        0        0     2851 2023-05-26 09:05:49.954398 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_code/__init__.data.json
+-rw-r--r--   0        0        0     1595 2023-05-26 09:05:49.956397 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_code/__init__.meta.json
+-rw-r--r--   0        0        0   201366 2023-05-26 09:05:49.952399 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_code/code.data.json
+-rw-r--r--   0        0        0     1984 2023-05-26 09:05:49.953398 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_code/code.meta.json
+-rw-r--r--   0        0        0    18070 2023-05-26 09:05:48.152361 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_code/source.data.json
+-rw-r--r--   0        0        0     1780 2023-05-26 09:05:48.153361 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_code/source.meta.json
+-rw-r--r--   0        0        0     2173 2023-05-26 09:05:49.927884 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/__init__.data.json
+-rw-r--r--   0        0        0     1572 2023-05-26 09:05:49.928884 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/__init__.meta.json
+-rw-r--r--   0        0        0    12069 2023-05-26 09:05:47.665769 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/saferepr.data.json
+-rw-r--r--   0        0        0     1594 2023-05-26 09:05:47.666768 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json
+-rw-r--r--   0        0        0    15783 2023-05-26 09:05:49.916368 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json
+-rw-r--r--   0        0        0     1893 2023-05-26 09:05:49.917369 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json
+-rw-r--r--   0        0        0     2946 2023-05-26 09:05:47.638735 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json
+-rw-r--r--   0        0        0     1582 2023-05-26 09:05:47.640735 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json
+-rw-r--r--   0        0        0     2657 2023-05-26 09:05:47.222503 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_version.data.json
+-rw-r--r--   0        0        0     1539 2023-05-26 09:05:47.223504 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_version.meta.json
+-rw-r--r--   0        0        0    12240 2023-05-26 09:05:50.068039 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/__init__.data.json
+-rw-r--r--   0        0        0     1896 2023-05-26 09:05:50.069038 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json
+-rw-r--r--   0        0        0    58200 2023-05-26 09:05:50.036508 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json
+-rw-r--r--   0        0        0     2318 2023-05-26 09:05:50.037510 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json
+-rw-r--r--   0        0        0     5807 2023-05-26 09:05:49.984915 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/truncate.data.json
+-rw-r--r--   0        0        0     1674 2023-05-26 09:05:49.985914 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json
+-rw-r--r--   0        0        0    22273 2023-05-26 09:05:49.972914 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/util.data.json
+-rw-r--r--   0        0        0     1970 2023-05-26 09:05:49.973912 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/util.meta.json
+-rw-r--r--   0        0        0    49255 2023-05-26 09:05:50.064039 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/cacheprovider.data.json
+-rw-r--r--   0        0        0     2354 2023-05-26 09:05:50.066039 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/cacheprovider.meta.json
+-rw-r--r--   0        0        0   122253 2023-05-26 09:05:50.024052 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/capture.data.json
+-rw-r--r--   0        0        0     1962 2023-05-26 09:05:50.025052 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/capture.meta.json
+-rw-r--r--   0        0        0    30716 2023-05-26 09:05:49.912924 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/compat.data.json
+-rw-r--r--   0        0        0     1886 2023-05-26 09:05:49.914368 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/compat.meta.json
+-rw-r--r--   0        0        0   106084 2023-05-26 09:05:49.962915 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/__init__.data.json
+-rw-r--r--   0        0        0     2763 2023-05-26 09:05:49.964912 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/__init__.meta.json
+-rw-r--r--   0        0        0    38719 2023-05-26 09:05:49.938398 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/argparsing.data.json
+-rw-r--r--   0        0        0     2004 2023-05-26 09:05:49.939397 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/argparsing.meta.json
+-rw-r--r--   0        0        0     4457 2023-05-26 09:05:49.981912 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/compat.data.json
+-rw-r--r--   0        0        0     1690 2023-05-26 09:05:49.982913 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/compat.meta.json
+-rw-r--r--   0        0        0     3004 2023-05-26 09:05:49.918367 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/exceptions.data.json
+-rw-r--r--   0        0        0     1579 2023-05-26 09:05:49.920369 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/exceptions.meta.json
+-rw-r--r--   0        0        0     9287 2023-05-26 09:05:49.944400 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/findpaths.data.json
+-rw-r--r--   0        0        0     1828 2023-05-26 09:05:49.945400 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/findpaths.meta.json
+-rw-r--r--   0        0        0    30461 2023-05-26 09:05:50.018051 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/debugging.data.json
+-rw-r--r--   0        0        0     2135 2023-05-26 09:05:50.019053 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/debugging.meta.json
+-rw-r--r--   0        0        0     7724 2023-05-26 09:05:49.925883 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/deprecated.data.json
+-rw-r--r--   0        0        0     1606 2023-05-26 09:05:49.926883 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/deprecated.meta.json
+-rw-r--r--   0        0        0    49561 2023-05-26 09:05:50.059039 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/doctest.data.json
+-rw-r--r--   0        0        0     2251 2023-05-26 09:05:50.060038 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/doctest.meta.json
+-rw-r--r--   0        0        0   173647 2023-05-26 09:05:49.995430 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/fixtures.data.json
+-rw-r--r--   0        0        0     2322 2023-05-26 09:05:49.996429 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/fixtures.meta.json
+-rw-r--r--   0        0        0     3113 2023-05-26 09:05:48.037452 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/freeze_support.data.json
+-rw-r--r--   0        0        0     1662 2023-05-26 09:05:48.039451 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/freeze_support.meta.json
+-rw-r--r--   0        0        0     8846 2023-05-26 09:05:50.082039 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/helpconfig.data.json
+-rw-r--r--   0        0        0     1782 2023-05-26 09:05:50.083038 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/helpconfig.meta.json
+-rw-r--r--   0        0        0    56857 2023-05-26 09:05:49.931884 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/hookspec.data.json
+-rw-r--r--   0        0        0     2058 2023-05-26 09:05:49.932883 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/hookspec.meta.json
+-rw-r--r--   0        0        0    68092 2023-05-26 09:05:50.073040 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/legacypath.data.json
+-rw-r--r--   0        0        0     2000 2023-05-26 09:05:50.074038 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/legacypath.meta.json
+-rw-r--r--   0        0        0    73622 2023-05-26 09:05:50.055038 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/logging.data.json
+-rw-r--r--   0        0        0     2194 2023-05-26 09:05:50.056038 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/logging.meta.json
+-rw-r--r--   0        0        0    50797 2023-05-26 09:05:50.031055 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/main.data.json
+-rw-r--r--   0        0        0     2264 2023-05-26 09:05:50.033510 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/main.meta.json
+-rw-r--r--   0        0        0    34788 2023-05-26 09:05:49.979914 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/mark/__init__.data.json
+-rw-r--r--   0        0        0     1988 2023-05-26 09:05:49.980912 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/mark/__init__.meta.json
+-rw-r--r--   0        0        0    36117 2023-05-26 09:05:47.923512 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/mark/expression.data.json
+-rw-r--r--   0        0        0     1720 2023-05-26 09:05:47.925041 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/mark/expression.meta.json
+-rw-r--r--   0        0        0   126266 2023-05-26 09:05:49.969912 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/mark/structures.data.json
+-rw-r--r--   0        0        0     2001 2023-05-26 09:05:49.970912 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/mark/structures.meta.json
+-rw-r--r--   0        0        0    24902 2023-05-26 09:05:50.015055 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/monkeypatch.data.json
+-rw-r--r--   0        0        0     1832 2023-05-26 09:05:50.016051 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/monkeypatch.meta.json
+-rw-r--r--   0        0        0    55874 2023-05-26 09:05:49.975915 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/nodes.data.json
+-rw-r--r--   0        0        0     2028 2023-05-26 09:05:49.976912 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/nodes.meta.json
+-rw-r--r--   0        0        0    29287 2023-05-26 09:05:49.935401 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/outcomes.data.json
+-rw-r--r--   0        0        0     1877 2023-05-26 09:05:49.936401 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/outcomes.meta.json
+-rw-r--r--   0        0        0    32236 2023-05-26 09:05:49.941401 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/pathlib.data.json
+-rw-r--r--   0        0        0     2075 2023-05-26 09:05:49.942397 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/pathlib.meta.json
+-rw-r--r--   0        0        0   128647 2023-05-26 09:05:50.050042 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/pytester.data.json
+-rw-r--r--   0        0        0     2554 2023-05-26 09:05:50.051038 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/pytester.meta.json
+-rw-r--r--   0        0        0     4466 2023-05-26 09:05:49.998429 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/pytester_assertions.data.json
+-rw-r--r--   0        0        0     1584 2023-05-26 09:05:50.000430 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json
+-rw-r--r--   0        0        0   130991 2023-05-26 09:05:50.043041 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/python.data.json
+-rw-r--r--   0        0        0     2438 2023-05-26 09:05:50.044039 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/python.meta.json
+-rw-r--r--   0        0        0    49533 2023-05-26 09:05:49.958911 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/python_api.data.json
+-rw-r--r--   0        0        0     1932 2023-05-26 09:05:49.959912 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/python_api.meta.json
+-rw-r--r--   0        0        0    29608 2023-05-26 09:05:50.012054 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/recwarn.data.json
+-rw-r--r--   0        0        0     1807 2023-05-26 09:05:50.013053 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/recwarn.meta.json
+-rw-r--r--   0        0        0    47879 2023-05-26 09:05:49.987916 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/reports.data.json
+-rw-r--r--   0        0        0     1931 2023-05-26 09:05:49.989430 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/reports.meta.json
+-rw-r--r--   0        0        0    49890 2023-05-26 09:05:50.007429 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/runner.data.json
+-rw-r--r--   0        0        0     2162 2023-05-26 09:05:50.009053 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/runner.meta.json
+-rw-r--r--   0        0        0    11134 2023-05-26 09:05:49.909925 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/scope.data.json
+-rw-r--r--   0        0        0     1614 2023-05-26 09:05:49.910924 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/scope.meta.json
+-rw-r--r--   0        0        0    13846 2023-05-26 09:05:47.519041 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/stash.data.json
+-rw-r--r--   0        0        0     1533 2023-05-26 09:05:47.520037 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/stash.meta.json
+-rw-r--r--   0        0        0    98667 2023-05-26 09:05:50.004428 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/terminal.data.json
+-rw-r--r--   0        0        0     2407 2023-05-26 09:05:50.005427 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/terminal.meta.json
+-rw-r--r--   0        0        0     1934 2023-05-26 09:05:47.685284 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/timing.data.json
+-rw-r--r--   0        0        0     1546 2023-05-26 09:05:47.686286 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/timing.meta.json
+-rw-r--r--   0        0        0    23725 2023-05-26 09:05:50.027052 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/tmpdir.data.json
+-rw-r--r--   0        0        0     1899 2023-05-26 09:05:50.029054 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/tmpdir.meta.json
+-rw-r--r--   0        0        0    33752 2023-05-26 09:05:49.922369 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/warning_types.data.json
+-rw-r--r--   0        0        0     1663 2023-05-26 09:05:49.924368 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/warning_types.meta.json
+-rw-r--r--   0        0        0    12293 2023-05-26 09:05:50.079040 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/warnings.data.json
+-rw-r--r--   0        0        0     1904 2023-05-26 09:05:50.080039 argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/warnings.meta.json
+-rw-r--r--   0        0        0    24870 2023-05-26 09:05:46.985187 argos-nac-0.1.3/tests/.mypy_cache/3.11/_stat.data.json
+-rw-r--r--   0        0        0     1594 2023-05-26 09:05:46.986187 argos-nac-0.1.3/tests/.mypy_cache/3.11/_stat.meta.json
+-rw-r--r--   0        0        0    23875 2023-05-26 09:05:47.057756 argos-nac-0.1.3/tests/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1646 2023-05-26 09:05:47.060756 argos-nac-0.1.3/tests/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0     8141 2023-05-26 09:05:46.976189 argos-nac-0.1.3/tests/.mypy_cache/3.11/_tracemalloc.data.json
+-rw-r--r--   0        0        0     1623 2023-05-26 09:05:46.977188 argos-nac-0.1.3/tests/.mypy_cache/3.11/_tracemalloc.meta.json
+-rw-r--r--   0        0        0    89069 2023-05-26 09:05:46.883288 argos-nac-0.1.3/tests/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1715 2023-05-26 09:05:46.884288 argos-nac-0.1.3/tests/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    13092 2023-05-26 09:05:47.218990 argos-nac-0.1.3/tests/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1549 2023-05-26 09:05:47.220505 argos-nac-0.1.3/tests/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    27323 2023-05-26 09:05:47.021238 argos-nac-0.1.3/tests/.mypy_cache/3.11/_weakref.data.json
+-rw-r--r--   0        0        0     1633 2023-05-26 09:05:47.022239 argos-nac-0.1.3/tests/.mypy_cache/3.11/_weakref.meta.json
+-rw-r--r--   0        0        0    50443 2023-05-26 09:05:47.013238 argos-nac-0.1.3/tests/.mypy_cache/3.11/_weakrefset.data.json
+-rw-r--r--   0        0        0     1639 2023-05-26 09:05:47.015237 argos-nac-0.1.3/tests/.mypy_cache/3.11/_weakrefset.meta.json
+-rw-r--r--   0        0        0    62840 2023-05-26 09:05:46.877289 argos-nac-0.1.3/tests/.mypy_cache/3.11/_winapi.data.json
+-rw-r--r--   0        0        0     1671 2023-05-26 09:05:46.878289 argos-nac-0.1.3/tests/.mypy_cache/3.11/_winapi.meta.json
+-rw-r--r--   0        0        0    23350 2023-05-26 09:05:46.872290 argos-nac-0.1.3/tests/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1599 2023-05-26 09:05:46.874288 argos-nac-0.1.3/tests/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0   149848 2023-05-26 09:05:47.511409 argos-nac-0.1.3/tests/.mypy_cache/3.11/argparse.data.json
+-rw-r--r--   0        0        0     1631 2023-05-26 09:05:47.513407 argos-nac-0.1.3/tests/.mypy_cache/3.11/argparse.meta.json
+-rw-r--r--   0        0        0    60690 2023-05-26 09:05:46.868289 argos-nac-0.1.3/tests/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1654 2023-05-26 09:05:46.870288 argos-nac-0.1.3/tests/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0   137634 2023-05-26 09:05:47.214988 argos-nac-0.1.3/tests/.mypy_cache/3.11/ast.data.json
+-rw-r--r--   0        0        0     1685 2023-05-26 09:05:47.215990 argos-nac-0.1.3/tests/.mypy_cache/3.11/ast.meta.json
+-rw-r--r--   0        0        0     8141 2023-05-26 09:05:47.149841 argos-nac-0.1.3/tests/.mypy_cache/3.11/atexit.data.json
+-rw-r--r--   0        0        0     1588 2023-05-26 09:05:47.151841 argos-nac-0.1.3/tests/.mypy_cache/3.11/atexit.meta.json
+-rw-r--r--   0        0        0   203398 2023-05-26 09:05:47.828367 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/__init__.data.json
+-rw-r--r--   0        0        0     1750 2023-05-26 09:05:47.829891 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/__init__.meta.json
+-rw-r--r--   0        0        0     3923 2023-05-26 09:05:47.132796 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/_cmp.data.json
+-rw-r--r--   0        0        0     1525 2023-05-26 09:05:47.134796 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/_cmp.meta.json
+-rw-r--r--   0        0        0     3032 2023-05-26 09:05:47.128798 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/_typing_compat.data.json
+-rw-r--r--   0        0        0     1545 2023-05-26 09:05:47.130796 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/_typing_compat.meta.json
+-rw-r--r--   0        0        0     7021 2023-05-26 09:05:47.125271 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/_version_info.data.json
+-rw-r--r--   0        0        0     1544 2023-05-26 09:05:47.126797 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/_version_info.meta.json
+-rw-r--r--   0        0        0     8304 2023-05-26 09:05:47.841893 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/converters.data.json
+-rw-r--r--   0        0        0     1548 2023-05-26 09:05:47.842892 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/converters.meta.json
+-rw-r--r--   0        0        0    10254 2023-05-26 09:05:47.137314 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/exceptions.data.json
+-rw-r--r--   0        0        0     1537 2023-05-26 09:05:47.139313 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/exceptions.meta.json
+-rw-r--r--   0        0        0     3555 2023-05-26 09:05:47.838891 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/filters.data.json
+-rw-r--r--   0        0        0     1542 2023-05-26 09:05:47.839890 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/filters.meta.json
+-rw-r--r--   0        0        0     7687 2023-05-26 09:05:47.835891 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/setters.data.json
+-rw-r--r--   0        0        0     1542 2023-05-26 09:05:47.837892 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/setters.meta.json
+-rw-r--r--   0        0        0    41655 2023-05-26 09:05:47.831893 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/validators.data.json
+-rw-r--r--   0        0        0     1578 2023-05-26 09:05:47.833893 argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/validators.meta.json
+-rw-r--r--   0        0        0    50473 2023-05-26 09:05:47.401295 argos-nac-0.1.3/tests/.mypy_cache/3.11/bdb.data.json
+-rw-r--r--   0        0        0     1622 2023-05-26 09:05:47.402299 argos-nac-0.1.3/tests/.mypy_cache/3.11/bdb.meta.json
+-rw-r--r--   0        0        0    11215 2023-05-26 09:05:47.645732 argos-nac-0.1.3/tests/.mypy_cache/3.11/bisect.data.json
+-rw-r--r--   0        0        0     1573 2023-05-26 09:05:47.646732 argos-nac-0.1.3/tests/.mypy_cache/3.11/bisect.meta.json
+-rw-r--r--   0        0        0  1130855 2023-05-26 09:05:46.936329 argos-nac-0.1.3/tests/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1736 2023-05-26 09:05:46.938330 argos-nac-0.1.3/tests/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0    20278 2023-05-26 09:05:47.074181 argos-nac-0.1.3/tests/.mypy_cache/3.11/cmd.data.json
+-rw-r--r--   0        0        0     1583 2023-05-26 09:05:47.076181 argos-nac-0.1.3/tests/.mypy_cache/3.11/cmd.meta.json
+-rw-r--r--   0        0        0   124025 2023-05-26 09:05:46.863291 argos-nac-0.1.3/tests/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1696 2023-05-26 09:05:46.865290 argos-nac-0.1.3/tests/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   408003 2023-05-26 09:05:46.858288 argos-nac-0.1.3/tests/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1673 2023-05-26 09:05:46.859289 argos-nac-0.1.3/tests/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3746 2023-05-26 09:05:46.845245 argos-nac-0.1.3/tests/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1584 2023-05-26 09:05:46.846246 argos-nac-0.1.3/tests/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   109218 2023-05-26 09:05:46.842247 argos-nac-0.1.3/tests/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1645 2023-05-26 09:05:46.843246 argos-nac-0.1.3/tests/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0     5423 2023-05-26 09:05:47.415776 argos-nac-0.1.3/tests/.mypy_cache/3.11/copy.data.json
+-rw-r--r--   0        0        0     1538 2023-05-26 09:05:47.416779 argos-nac-0.1.3/tests/.mypy_cache/3.11/copy.meta.json
+-rw-r--r--   0        0        0   136830 2023-05-26 09:05:46.836249 argos-nac-0.1.3/tests/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1692 2023-05-26 09:05:46.837247 argos-nac-0.1.3/tests/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    57759 2023-05-26 09:05:46.829101 argos-nac-0.1.3/tests/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1650 2023-05-26 09:05:46.831100 argos-nac-0.1.3/tests/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142222 2023-05-26 09:05:47.633737 argos-nac-0.1.3/tests/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1610 2023-05-26 09:05:47.634732 argos-nac-0.1.3/tests/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4925 2023-05-26 09:05:47.904994 argos-nac-0.1.3/tests/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1560 2023-05-26 09:05:47.906993 argos-nac-0.1.3/tests/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    58305 2023-05-26 09:05:47.160366 argos-nac-0.1.3/tests/.mypy_cache/3.11/difflib.data.json
+-rw-r--r--   0        0        0     1607 2023-05-26 09:05:47.161365 argos-nac-0.1.3/tests/.mypy_cache/3.11/difflib.meta.json
+-rw-r--r--   0        0        0    62920 2023-05-26 09:05:47.609710 argos-nac-0.1.3/tests/.mypy_cache/3.11/dis.data.json
+-rw-r--r--   0        0        0     1637 2023-05-26 09:05:47.612710 argos-nac-0.1.3/tests/.mypy_cache/3.11/dis.meta.json
+-rw-r--r--   0        0        0    69848 2023-05-26 09:05:48.111837 argos-nac-0.1.3/tests/.mypy_cache/3.11/doctest.data.json
+-rw-r--r--   0        0        0     1679 2023-05-26 09:05:48.112837 argos-nac-0.1.3/tests/.mypy_cache/3.11/doctest.meta.json
+-rw-r--r--   0        0        0     7453 2023-05-26 09:05:46.825578 argos-nac-0.1.3/tests/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1636 2023-05-26 09:05:46.827104 argos-nac-0.1.3/tests/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12215 2023-05-26 09:05:46.822578 argos-nac-0.1.3/tests/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1581 2023-05-26 09:05:46.823578 argos-nac-0.1.3/tests/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7264 2023-05-26 09:05:46.818580 argos-nac-0.1.3/tests/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1613 2023-05-26 09:05:46.820578 argos-nac-0.1.3/tests/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25088 2023-05-26 09:05:46.815580 argos-nac-0.1.3/tests/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1585 2023-05-26 09:05:46.817579 argos-nac-0.1.3/tests/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9169 2023-05-26 09:05:46.813061 argos-nac-0.1.3/tests/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1598 2023-05-26 09:05:46.814060 argos-nac-0.1.3/tests/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79285 2023-05-26 09:05:46.810063 argos-nac-0.1.3/tests/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1701 2023-05-26 09:05:46.812060 argos-nac-0.1.3/tests/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30872 2023-05-26 09:05:46.805060 argos-nac-0.1.3/tests/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1662 2023-05-26 09:05:46.806059 argos-nac-0.1.3/tests/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0    90137 2023-05-26 09:05:46.800542 argos-nac-0.1.3/tests/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1625 2023-05-26 09:05:46.802539 argos-nac-0.1.3/tests/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    24995 2023-05-26 09:05:47.186413 argos-nac-0.1.3/tests/.mypy_cache/3.11/errno.data.json
+-rw-r--r--   0        0        0     1575 2023-05-26 09:05:47.188413 argos-nac-0.1.3/tests/.mypy_cache/3.11/errno.meta.json
+-rw-r--r--   0        0        0     6106 2023-05-26 09:05:47.363241 argos-nac-0.1.3/tests/.mypy_cache/3.11/fnmatch.data.json
+-rw-r--r--   0        0        0     1566 2023-05-26 09:05:47.364241 argos-nac-0.1.3/tests/.mypy_cache/3.11/fnmatch.meta.json
+-rw-r--r--   0        0        0   132081 2023-05-26 09:05:47.462375 argos-nac-0.1.3/tests/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1634 2023-05-26 09:05:47.464373 argos-nac-0.1.3/tests/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    15974 2023-05-26 09:05:47.358908 argos-nac-0.1.3/tests/.mypy_cache/3.11/gc.data.json
+-rw-r--r--   0        0        0     1609 2023-05-26 09:05:47.360292 argos-nac-0.1.3/tests/.mypy_cache/3.11/gc.meta.json
+-rw-r--r--   0        0        0    22402 2023-05-26 09:05:46.795539 argos-nac-0.1.3/tests/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1625 2023-05-26 09:05:46.796539 argos-nac-0.1.3/tests/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     3753 2023-05-26 09:05:47.225503 argos-nac-0.1.3/tests/.mypy_cache/3.11/getpass.data.json
+-rw-r--r--   0        0        0     1544 2023-05-26 09:05:47.227503 argos-nac-0.1.3/tests/.mypy_cache/3.11/getpass.meta.json
+-rw-r--r--   0        0        0    46204 2023-05-26 09:05:47.484892 argos-nac-0.1.3/tests/.mypy_cache/3.11/gettext.data.json
+-rw-r--r--   0        0        0     1628 2023-05-26 09:05:47.486893 argos-nac-0.1.3/tests/.mypy_cache/3.11/gettext.meta.json
+-rw-r--r--   0        0        0     9518 2023-05-26 09:05:47.412297 argos-nac-0.1.3/tests/.mypy_cache/3.11/glob.data.json
+-rw-r--r--   0        0        0     1588 2023-05-26 09:05:47.413780 argos-nac-0.1.3/tests/.mypy_cache/3.11/glob.meta.json
+-rw-r--r--   0        0        0     6140 2023-05-26 09:05:46.792062 argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1613 2023-05-26 09:05:46.793062 argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70594 2023-05-26 09:05:46.790058 argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1759 2023-05-26 09:05:46.791059 argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64586 2023-05-26 09:05:46.785060 argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1748 2023-05-26 09:05:46.786059 argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91135 2023-05-26 09:05:46.780542 argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1758 2023-05-26 09:05:46.781540 argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11951 2023-05-26 09:05:46.774542 argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1602 2023-05-26 09:05:46.776541 argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    21587 2023-05-26 09:05:47.191936 argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/util.data.json
+-rw-r--r--   0        0        0     1753 2023-05-26 09:05:47.193936 argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/util.meta.json
+-rw-r--r--   0        0        0    44376 2023-05-26 09:05:48.098317 argos-nac-0.1.3/tests/.mypy_cache/3.11/iniconfig/__init__.data.json
+-rw-r--r--   0        0        0     1667 2023-05-26 09:05:48.100317 argos-nac-0.1.3/tests/.mypy_cache/3.11/iniconfig/__init__.meta.json
+-rw-r--r--   0        0        0    22635 2023-05-26 09:05:47.903470 argos-nac-0.1.3/tests/.mypy_cache/3.11/iniconfig/_parse.data.json
+-rw-r--r--   0        0        0     1608 2023-05-26 09:05:47.903995 argos-nac-0.1.3/tests/.mypy_cache/3.11/iniconfig/_parse.meta.json
+-rw-r--r--   0        0        0     4539 2023-05-26 09:05:47.601195 argos-nac-0.1.3/tests/.mypy_cache/3.11/iniconfig/exceptions.data.json
+-rw-r--r--   0        0        0     1588 2023-05-26 09:05:47.602193 argos-nac-0.1.3/tests/.mypy_cache/3.11/iniconfig/exceptions.meta.json
+-rw-r--r--   0        0        0   330902 2023-05-26 09:05:48.032452 argos-nac-0.1.3/tests/.mypy_cache/3.11/inspect.data.json
+-rw-r--r--   0        0        0     1675 2023-05-26 09:05:48.033451 argos-nac-0.1.3/tests/.mypy_cache/3.11/inspect.meta.json
+-rw-r--r--   0        0        0    85351 2023-05-26 09:05:46.771540 argos-nac-0.1.3/tests/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1698 2023-05-26 09:05:46.772540 argos-nac-0.1.3/tests/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   266323 2023-05-26 09:05:47.341384 argos-nac-0.1.3/tests/.mypy_cache/3.11/itertools.data.json
+-rw-r--r--   0        0        0     1636 2023-05-26 09:05:47.342384 argos-nac-0.1.3/tests/.mypy_cache/3.11/itertools.meta.json
+-rw-r--r--   0        0        0    15394 2023-05-26 09:05:47.867421 argos-nac-0.1.3/tests/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1625 2023-05-26 09:05:47.869419 argos-nac-0.1.3/tests/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    14519 2023-05-26 09:05:47.528039 argos-nac-0.1.3/tests/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1578 2023-05-26 09:05:47.529038 argos-nac-0.1.3/tests/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    10899 2023-05-26 09:05:47.524037 argos-nac-0.1.3/tests/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1587 2023-05-26 09:05:47.525037 argos-nac-0.1.3/tests/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   144400 2023-05-26 09:05:47.718327 argos-nac-0.1.3/tests/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1712 2023-05-26 09:05:47.720324 argos-nac-0.1.3/tests/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0     6406 2023-05-26 09:05:47.180410 argos-nac-0.1.3/tests/.mypy_cache/3.11/marshal.data.json
+-rw-r--r--   0        0        0     1651 2023-05-26 09:05:47.182412 argos-nac-0.1.3/tests/.mypy_cache/3.11/marshal.meta.json
+-rw-r--r--   0        0        0    52525 2023-05-26 09:05:47.249502 argos-nac-0.1.3/tests/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1613 2023-05-26 09:05:47.251503 argos-nac-0.1.3/tests/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    23321 2023-05-26 09:05:46.765544 argos-nac-0.1.3/tests/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1653 2023-05-26 09:05:46.767541 argos-nac-0.1.3/tests/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    14094 2023-05-26 09:05:46.762596 argos-nac-0.1.3/tests/.mypy_cache/3.11/ntpath.data.json
+-rw-r--r--   0        0        0     1641 2023-05-26 09:05:46.763544 argos-nac-0.1.3/tests/.mypy_cache/3.11/ntpath.meta.json
+-rw-r--r--   0        0        0    78996 2023-05-26 09:05:47.236507 argos-nac-0.1.3/tests/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1544 2023-05-26 09:05:47.237506 argos-nac-0.1.3/tests/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0     6108 2023-05-26 09:05:46.961665 argos-nac-0.1.3/tests/.mypy_cache/3.11/opcode.data.json
+-rw-r--r--   0        0        0     1596 2023-05-26 09:05:46.962661 argos-nac-0.1.3/tests/.mypy_cache/3.11/opcode.meta.json
+-rw-r--r--   0        0        0    49212 2023-05-26 09:05:47.561081 argos-nac-0.1.3/tests/.mypy_cache/3.11/operator.data.json
+-rw-r--r--   0        0        0     1617 2023-05-26 09:05:47.562080 argos-nac-0.1.3/tests/.mypy_cache/3.11/operator.meta.json
+-rw-r--r--   0        0        0   236998 2023-05-26 09:05:46.759123 argos-nac-0.1.3/tests/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1751 2023-05-26 09:05:46.761125 argos-nac-0.1.3/tests/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4911 2023-05-26 09:05:46.749607 argos-nac-0.1.3/tests/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1570 2023-05-26 09:05:46.750604 argos-nac-0.1.3/tests/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     3198 2023-05-26 09:05:47.115274 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/__init__.data.json
+-rw-r--r--   0        0        0     1534 2023-05-26 09:05:47.116271 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/__init__.meta.json
+-rw-r--r--   0        0        0    13851 2023-05-26 09:05:47.555081 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_elffile.data.json
+-rw-r--r--   0        0        0     1661 2023-05-26 09:05:47.556081 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_elffile.meta.json
+-rw-r--r--   0        0        0    26585 2023-05-26 09:05:47.894472 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_manylinux.data.json
+-rw-r--r--   0        0        0     1841 2023-05-26 09:05:47.896469 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_manylinux.meta.json
+-rw-r--r--   0        0        0    18213 2023-05-26 09:05:47.878945 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_musllinux.data.json
+-rw-r--r--   0        0        0     1754 2023-05-26 09:05:47.879944 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_musllinux.meta.json
+-rw-r--r--   0        0        0    44044 2023-05-26 09:05:48.246514 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_parser.data.json
+-rw-r--r--   0        0        0     1645 2023-05-26 09:05:48.248032 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_parser.meta.json
+-rw-r--r--   0        0        0    13952 2023-05-26 09:05:47.109750 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_structures.data.json
+-rw-r--r--   0        0        0     1563 2023-05-26 09:05:47.111750 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_structures.meta.json
+-rw-r--r--   0        0        0    17549 2023-05-26 09:05:48.231994 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_tokenizer.data.json
+-rw-r--r--   0        0        0     1656 2023-05-26 09:05:48.232993 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_tokenizer.meta.json
+-rw-r--r--   0        0        0    17587 2023-05-26 09:05:48.265559 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/markers.data.json
+-rw-r--r--   0        0        0     1745 2023-05-26 09:05:48.266557 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/markers.meta.json
+-rw-r--r--   0        0        0     8566 2023-05-26 09:05:48.276086 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/requirements.data.json
+-rw-r--r--   0        0        0     1719 2023-05-26 09:05:48.278082 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/requirements.meta.json
+-rw-r--r--   0        0        0    55975 2023-05-26 09:05:48.215472 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/specifiers.data.json
+-rw-r--r--   0        0        0     1694 2023-05-26 09:05:48.217467 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/specifiers.meta.json
+-rw-r--r--   0        0        0    27792 2023-05-26 09:05:48.079792 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/tags.data.json
+-rw-r--r--   0        0        0     1825 2023-05-26 09:05:48.081790 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/tags.meta.json
+-rw-r--r--   0        0        0     9833 2023-05-26 09:05:48.167363 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/utils.data.json
+-rw-r--r--   0        0        0     1712 2023-05-26 09:05:48.168361 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/utils.meta.json
+-rw-r--r--   0        0        0    65183 2023-05-26 09:05:47.797627 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/version.data.json
+-rw-r--r--   0        0        0     1741 2023-05-26 09:05:47.798623 argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/version.meta.json
+-rw-r--r--   0        0        0    85758 2023-05-26 09:05:46.745603 argos-nac-0.1.3/tests/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1707 2023-05-26 09:05:46.747606 argos-nac-0.1.3/tests/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    92071 2023-05-26 09:05:48.129421 argos-nac-0.1.3/tests/.mypy_cache/3.11/pdb.data.json
+-rw-r--r--   0        0        0     1694 2023-05-26 09:05:48.131363 argos-nac-0.1.3/tests/.mypy_cache/3.11/pdb.meta.json
+-rw-r--r--   0        0        0    44407 2023-05-26 09:05:46.741085 argos-nac-0.1.3/tests/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1655 2023-05-26 09:05:46.741608 argos-nac-0.1.3/tests/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    31505 2023-05-26 09:05:47.368240 argos-nac-0.1.3/tests/.mypy_cache/3.11/pkgutil.data.json
+-rw-r--r--   0        0        0     1631 2023-05-26 09:05:47.369243 argos-nac-0.1.3/tests/.mypy_cache/3.11/pkgutil.meta.json
+-rw-r--r--   0        0        0    34966 2023-05-26 09:05:47.389296 argos-nac-0.1.3/tests/.mypy_cache/3.11/platform.data.json
+-rw-r--r--   0        0        0     1575 2023-05-26 09:05:47.391297 argos-nac-0.1.3/tests/.mypy_cache/3.11/platform.meta.json
+-rw-r--r--   0        0        0    75211 2023-05-26 09:05:46.737084 argos-nac-0.1.3/tests/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1652 2023-05-26 09:05:46.738084 argos-nac-0.1.3/tests/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0    12026 2023-05-26 09:05:47.469375 argos-nac-0.1.3/tests/.mypy_cache/3.11/pprint.data.json
+-rw-r--r--   0        0        0     1571 2023-05-26 09:05:47.470375 argos-nac-0.1.3/tests/.mypy_cache/3.11/pprint.meta.json
+-rw-r--r--   0        0        0    11121 2023-05-26 09:05:50.076039 argos-nac-0.1.3/tests/.mypy_cache/3.11/pytest/__init__.data.json
+-rw-r--r--   0        0        0     2166 2023-05-26 09:05:50.078039 argos-nac-0.1.3/tests/.mypy_cache/3.11/pytest/__init__.meta.json
+-rw-r--r--   0        0        0   167559 2023-05-26 09:05:46.732080 argos-nac-0.1.3/tests/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1726 2023-05-26 09:05:46.734083 argos-nac-0.1.3/tests/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    16749 2023-05-26 09:05:47.003716 argos-nac-0.1.3/tests/.mypy_cache/3.11/reprlib.data.json
+-rw-r--r--   0        0        0     1649 2023-05-26 09:05:47.004718 argos-nac-0.1.3/tests/.mypy_cache/3.11/reprlib.meta.json
+-rw-r--r--   0        0        0    16510 2023-05-26 09:05:47.407298 argos-nac-0.1.3/tests/.mypy_cache/3.11/shlex.data.json
+-rw-r--r--   0        0        0     1615 2023-05-26 09:05:47.408297 argos-nac-0.1.3/tests/.mypy_cache/3.11/shlex.meta.json
+-rw-r--r--   0        0        0    71126 2023-05-26 09:05:47.353906 argos-nac-0.1.3/tests/.mypy_cache/3.11/shutil.data.json
+-rw-r--r--   0        0        0     1626 2023-05-26 09:05:47.354908 argos-nac-0.1.3/tests/.mypy_cache/3.11/shutil.meta.json
+-rw-r--r--   0        0        0    14832 2023-05-26 09:05:47.080183 argos-nac-0.1.3/tests/.mypy_cache/3.11/signal.data.json
+-rw-r--r--   0        0        0     1639 2023-05-26 09:05:47.082183 argos-nac-0.1.3/tests/.mypy_cache/3.11/signal.meta.json
+-rw-r--r--   0        0        0    14387 2023-05-26 09:05:46.723567 argos-nac-0.1.3/tests/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1597 2023-05-26 09:05:46.725566 argos-nac-0.1.3/tests/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28494 2023-05-26 09:05:46.721563 argos-nac-0.1.3/tests/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1609 2023-05-26 09:05:46.722572 argos-nac-0.1.3/tests/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49755 2023-05-26 09:05:46.717566 argos-nac-0.1.3/tests/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1652 2023-05-26 09:05:46.719563 argos-nac-0.1.3/tests/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0     8866 2023-05-26 09:05:47.641735 argos-nac-0.1.3/tests/.mypy_cache/3.11/stat.data.json
+-rw-r--r--   0        0        0     1550 2023-05-26 09:05:47.642734 argos-nac-0.1.3/tests/.mypy_cache/3.11/stat.meta.json
+-rw-r--r--   0        0        0    27762 2023-05-26 09:05:47.039239 argos-nac-0.1.3/tests/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1637 2023-05-26 09:05:47.040757 argos-nac-0.1.3/tests/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0    15313 2023-05-26 09:05:47.174891 argos-nac-0.1.3/tests/.mypy_cache/3.11/struct.data.json
+-rw-r--r--   0        0        0     1634 2023-05-26 09:05:47.176891 argos-nac-0.1.3/tests/.mypy_cache/3.11/struct.meta.json
+-rw-r--r--   0        0        0   167815 2023-05-26 09:05:46.713564 argos-nac-0.1.3/tests/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1717 2023-05-26 09:05:46.714564 argos-nac-0.1.3/tests/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   165686 2023-05-26 09:05:46.705254 argos-nac-0.1.3/tests/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1685 2023-05-26 09:05:46.706254 argos-nac-0.1.3/tests/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    14479 2023-05-26 09:05:46.942330 argos-nac-0.1.3/tests/.mypy_cache/3.11/sysconfig.data.json
+-rw-r--r--   0        0        0     1601 2023-05-26 09:05:46.943663 argos-nac-0.1.3/tests/.mypy_cache/3.11/sysconfig.meta.json
+-rw-r--r--   0        0        0   133952 2023-05-26 09:05:47.443846 argos-nac-0.1.3/tests/.mypy_cache/3.11/tempfile.data.json
+-rw-r--r--   0        0        0     1706 2023-05-26 09:05:47.445377 argos-nac-0.1.3/tests/.mypy_cache/3.11/tempfile.meta.json
+-rw-r--r--   0        0        0    19567 2023-05-26 09:05:47.475374 argos-nac-0.1.3/tests/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1579 2023-05-26 09:05:47.476373 argos-nac-0.1.3/tests/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0    64729 2023-05-26 09:05:47.063756 argos-nac-0.1.3/tests/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1649 2023-05-26 09:05:47.065757 argos-nac-0.1.3/tests/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    38018 2023-05-26 09:05:47.032238 argos-nac-0.1.3/tests/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1590 2023-05-26 09:05:47.033238 argos-nac-0.1.3/tests/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0    14927 2023-05-26 09:05:46.997773 argos-nac-0.1.3/tests/.mypy_cache/3.11/token.data.json
+-rw-r--r--   0        0        0     1570 2023-05-26 09:05:46.998716 argos-nac-0.1.3/tests/.mypy_cache/3.11/token.meta.json
+-rw-r--r--   0        0        0    49284 2023-05-26 09:05:47.654251 argos-nac-0.1.3/tests/.mypy_cache/3.11/tokenize.data.json
+-rw-r--r--   0        0        0     1651 2023-05-26 09:05:47.655251 argos-nac-0.1.3/tests/.mypy_cache/3.11/tokenize.meta.json
+-rw-r--r--   0        0        0     5254 2023-05-26 09:05:47.119278 argos-nac-0.1.3/tests/.mypy_cache/3.11/tomllib.data.json
+-rw-r--r--   0        0        0     1582 2023-05-26 09:05:47.121272 argos-nac-0.1.3/tests/.mypy_cache/3.11/tomllib.meta.json
+-rw-r--r--   0        0        0    57032 2023-05-26 09:05:47.382297 argos-nac-0.1.3/tests/.mypy_cache/3.11/traceback.data.json
+-rw-r--r--   0        0        0     1634 2023-05-26 09:05:47.383300 argos-nac-0.1.3/tests/.mypy_cache/3.11/traceback.meta.json
+-rw-r--r--   0        0        0    48912 2023-05-26 09:05:46.979189 argos-nac-0.1.3/tests/.mypy_cache/3.11/tracemalloc.data.json
+-rw-r--r--   0        0        0     1646 2023-05-26 09:05:46.980187 argos-nac-0.1.3/tests/.mypy_cache/3.11/tracemalloc.meta.json
+-rw-r--r--   0        0        0   239646 2023-05-26 09:05:46.697728 argos-nac-0.1.3/tests/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1663 2023-05-26 09:05:46.699260 argos-nac-0.1.3/tests/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432248 2023-05-26 09:05:46.686727 argos-nac-0.1.3/tests/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1714 2023-05-26 09:05:46.688728 argos-nac-0.1.3/tests/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57859 2023-05-26 09:05:46.671728 argos-nac-0.1.3/tests/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1670 2023-05-26 09:05:46.672729 argos-nac-0.1.3/tests/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    41974 2023-05-26 09:05:47.168893 argos-nac-0.1.3/tests/.mypy_cache/3.11/unicodedata.data.json
+-rw-r--r--   0        0        0     1604 2023-05-26 09:05:47.170892 argos-nac-0.1.3/tests/.mypy_cache/3.11/unicodedata.meta.json
+-rw-r--r--   0        0        0     6208 2023-05-26 09:05:47.995092 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1769 2023-05-26 09:05:47.996091 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    24083 2023-05-26 09:05:47.966091 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/_log.data.json
+-rw-r--r--   0        0        0     1632 2023-05-26 09:05:47.967090 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/_log.meta.json
+-rw-r--r--   0        0        0     9283 2023-05-26 09:05:47.978090 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1680 2023-05-26 09:05:47.979091 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   210169 2023-05-26 09:05:47.975092 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/case.data.json
+-rw-r--r--   0        0        0     1762 2023-05-26 09:05:47.976096 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/case.meta.json
+-rw-r--r--   0        0        0    14633 2023-05-26 09:05:47.988092 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/loader.data.json
+-rw-r--r--   0        0        0     1688 2023-05-26 09:05:47.989092 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11741 2023-05-26 09:05:47.991093 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/main.data.json
+-rw-r--r--   0        0        0     1697 2023-05-26 09:05:47.993090 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/main.meta.json
+-rw-r--r--   0        0        0    20593 2023-05-26 09:05:47.960090 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/result.data.json
+-rw-r--r--   0        0        0     1650 2023-05-26 09:05:47.964092 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/result.meta.json
+-rw-r--r--   0        0        0    10760 2023-05-26 09:05:47.986090 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/runner.data.json
+-rw-r--r--   0        0        0     1690 2023-05-26 09:05:47.987089 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11279 2023-05-26 09:05:47.983092 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/signals.data.json
+-rw-r--r--   0        0        0     1648 2023-05-26 09:05:47.984090 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11265 2023-05-26 09:05:47.980091 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/suite.data.json
+-rw-r--r--   0        0        0     1667 2023-05-26 09:05:47.982089 argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1510 2023-05-26 09:05:47.083707 argos-nac-0.1.3/tests/.mypy_cache/3.11/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1551 2023-05-26 09:05:47.085704 argos-nac-0.1.3/tests/.mypy_cache/3.11/urllib/__init__.meta.json
+-rw-r--r--   0        0        0   175327 2023-05-26 09:05:47.100226 argos-nac-0.1.3/tests/.mypy_cache/3.11/urllib/parse.data.json
+-rw-r--r--   0        0        0     1642 2023-05-26 09:05:47.102224 argos-nac-0.1.3/tests/.mypy_cache/3.11/urllib/parse.meta.json
+-rw-r--r--   0        0        0    33600 2023-05-26 09:05:47.146315 argos-nac-0.1.3/tests/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1655 2023-05-26 09:05:47.146846 argos-nac-0.1.3/tests/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    23803 2023-05-26 09:05:47.849892 argos-nac-0.1.3/tests/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1649 2023-05-26 09:05:47.851893 argos-nac-0.1.3/tests/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0   142942 2023-05-26 09:05:47.682282 argos-nac-0.1.3/tests/.mypy_cache/3.11/weakref.data.json
+-rw-r--r--   0        0        0     1655 2023-05-26 09:05:47.683283 argos-nac-0.1.3/tests/.mypy_cache/3.11/weakref.meta.json
+-rw-r--r--   0        0        0     1400 2023-05-26 09:05:47.531038 argos-nac-0.1.3/tests/.mypy_cache/3.11/work/__init__.data.json
+-rw-r--r--   0        0        0     1452 2023-05-26 09:05:47.532036 argos-nac-0.1.3/tests/.mypy_cache/3.11/work/__init__.meta.json
+-rw-r--r--   0        0        0     1714 2023-05-26 09:05:47.543551 argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects/argos/controller/tests/__init__.data.json
+-rw-r--r--   0        0        0     1532 2023-05-26 09:05:47.545553 argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects/argos/controller/tests/__init__.meta.json
+-rw-r--r--   0        0        0     1395 2023-05-26 09:05:47.541036 argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects/argos/controller.data.json
+-rw-r--r--   0        0        0     1445 2023-05-26 10:05:52.291632 argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects/argos/controller.meta.json
+-rw-r--r--   0        0        0     1317 2023-05-26 09:05:47.538037 argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects/argos.data.json
+-rw-r--r--   0        0        0     1422 2023-05-26 09:05:47.539036 argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects/argos.meta.json
+-rw-r--r--   0        0        0     1274 2023-05-26 09:05:47.534042 argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects.data.json
+-rw-r--r--   0        0        0     1409 2023-05-26 09:05:47.536036 argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects.meta.json
+-rw-r--r--   0        0        0      193 2023-05-26 09:05:50.102561 argos-nac-0.1.3/tests/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        0 2023-05-14 17:18:53.063545 argos-nac-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-30 13:13:31.249105 argos-nac-0.1.3/tests/cisco_test.py
+-rw-r--r--   0        0        0     2923 2023-05-26 06:59:58.816158 argos-nac-0.1.3/tests/configs/PE1.log
+-rw-r--r--   0        0        0     1932 2023-05-30 13:13:31.250157 argos-nac-0.1.3/tests/configs/PE1_expected.log
+-rw-r--r--   0        0        0     2802 2023-05-30 13:13:31.250672 argos-nac-0.1.3/tests/configs/PE2.log
+-rw-r--r--   0        0        0     1921 2023-05-30 13:13:31.251670 argos-nac-0.1.3/tests/configs/PE2_expected.log
+-rw-r--r--   0        0        0    29598 2023-05-30 13:13:31.251670 argos-nac-0.1.3/tests/site_sample_data.json
+-rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 argos-nac-0.1.3/PKG-INFO
```

### Comparing `argos-nac-0.1.2/graphql_schema/gen_schema.py` & `argos-nac-0.1.3/graphql_schema/gen_schema.py`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/graphql_schema/schema.py` & `argos-nac-0.1.3/graphql_schema/schema.py`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/graphql_schema/schema_query.gql` & `argos-nac-0.1.3/graphql_schema/schema_query.gql`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/_ast.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/_ast.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/_codecs.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/_codecs.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/_collections_abc.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/_collections_abc.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/_ctypes.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/_ctypes.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/_thread.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/_thread.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/_typeshed/__init__.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/_winapi.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/_winapi.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/_winapi.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/_winapi.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/abc.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/abc.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/array.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/array.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/builtins.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/builtins.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/codecs.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/codecs.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/collections/__init__.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/collections/__init__.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/collections/abc.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/collections/abc.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/contextlib.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/contextlib.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/ctypes/__init__.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/ctypes/__init__.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/dataclasses.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/dataclasses.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/email/__init__.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/email/__init__.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/email/charset.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/email/charset.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/email/contentmanager.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/email/contentmanager.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/email/errors.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/email/errors.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/email/header.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/email/header.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/email/message.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/email/message.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/email/policy.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/email/policy.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/enum.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/enum.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/genericpath.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/genericpath.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/__init__.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/__init__.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/abc.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/abc.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/machinery.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/machinery.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/io.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/io.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/logging/__init__.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/logging/__init__.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/mmap.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/mmap.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/ntpath.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/ntpath.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/ntpath.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/ntpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/os/__init__.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/os/__init__.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/os/path.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/os/path.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/pathlib.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/pathlib.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/pickle.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/pickle.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/posixpath.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/posixpath.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/re.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/re.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/sre_compile.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/sre_compile.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/sre_constants.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/sre_constants.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/sre_parse.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/sre_parse.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/string.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/string.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/subprocess.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/subprocess.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/sys.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/sys.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/threading.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/threading.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/time.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/time.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/types.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/types.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/typing.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/typing.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/typing_extensions.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/typing_extensions.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/work/__init__.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/work/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/work/__init__.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/work/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/model.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/model.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/model.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos/controller/nac/model.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos/controller.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos/controller.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos/controller.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos/controller.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects/argos.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects/argos.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects.data.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/.mypy_cache/3.11/work/school_projects.meta.json` & `argos-nac-0.1.3/nac/.mypy_cache/3.11/work/school_projects.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/cisco/controller.py` & `argos-nac-0.1.3/nac/cisco/controller.py`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/cisco/nornir_util.py` & `argos-nac-0.1.3/nac/cisco/nornir_util.py`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/cisco/protocols/bgp.py` & `argos-nac-0.1.3/nac/cisco/protocols/bgp.py`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/cisco/protocols/ldp.py` & `argos-nac-0.1.3/nac/cisco/protocols/ldp.py`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/cisco/protocols/vrf.py` & `argos-nac-0.1.3/nac/cisco/protocols/vrf.py`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/main.py` & `argos-nac-0.1.3/nac/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from dataclasses import dataclass
 from logging import getLogger
 from os import environ, makedirs
 from pathlib import Path
 
 from nornir.core.inventory import Defaults
+from nornir.core.task import AggregatedResult
 
 from nac.cisco import CiscoNAC
 from nac.util.common import HostMapping
 from nac.util.netbox_api import NetBoxAPI
 
 from .model import *
 from .util.graphql_util import GraphQLUtil
+from .__version__ import __version__
 
 LOGGER = getLogger(__name__)
 
 
 @dataclass
 class Settings:
     interactive: bool
@@ -52,16 +54,14 @@
         falsy = proceed in ('n', 'no')
     return truthy
 
 
 def run():
     settings: Settings = parse_cli_arguments()
 
-    LOGGER.info(settings)
-
     NetBoxAPI(settings.netbox_url, token=settings.netbox_token).assert_plugin_installed("argos_netbox", version="0.1")
 
     LOGGER.info(f"Querying site data for site: {settings.site_id}.")
     site: Site = GraphQLUtil.get_site_data(
         graphql_url=f"{settings.netbox_url}/graphql",
         token=settings.netbox_token,
         site_id=settings.site_id,
@@ -75,30 +75,33 @@
         username=settings.ssh_username,
         platform="ios",
     )
 
     # Create host mapping
     host_mapping: HostMapping = HostMapping.from_site(site, defaults)
     LOGGER.info(f"Found {len(host_mapping)} devices to configure: {', '.join((str(x) for x in host_mapping.keys()))}")
+    LOGGER.info(settings)
     if settings.interactive:
         ok = get_confirmation("Please double-check the above information. Does it appear correct to you?")
         if not ok:
             LOGGER.info("Exiting.")
             exit()
 
     # Configure devices
     nac = CiscoNAC(
         host_mapping=host_mapping,
         defaults=defaults,
         dry_run=settings.dry_run,
     )
-    nac.configure_devices(
+    result: AggregatedResult = nac.configure_devices(
         backup_dir=settings.backup_dir,
         output_dir=settings.output_dir,
     )
+    result.raise_on_error()
+    LOGGER.info("Operation completed successfully.")
 
 
 def get_value(env_name: str, interactive: bool, prompt: str = '', critical: bool = False) -> str:
     value = environ.get(env_name, None)
     if value is None:
         if interactive:
             prompt = f'"{env_name}" unset. {prompt} '
@@ -119,15 +122,15 @@
     # Import locally to not clutter scope of caller
     import logging
     from argparse import ArgumentParser, SUPPRESS
 
     # Setup parser
     parser = ArgumentParser(
         prog="argos-deploy",
-        description='Query NetBox via GraphQL and deploy the documented services.',
+        description=f"Query NetBox via GraphQL and deploy the documented services. v{__version__}",
         add_help=False,
     )
     parser.add_argument(
         '-h',
         '--help',
         help='Show this help message and exit.',  # Default implementation is not capitalized
         action='help',
```

### Comparing `argos-nac-0.1.2/nac/model.py` & `argos-nac-0.1.3/nac/model.py`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/queries/main.gql` & `argos-nac-0.1.3/nac/queries/main.gql`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_ast.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_ast.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_codecs.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_codecs.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_collections_abc.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_collections_abc.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_ctypes.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_ctypes.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_thread.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_thread.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_typeshed/__init__.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_winapi.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_winapi.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/_winapi.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/_winapi.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/abc.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/abc.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/array.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/array.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/builtins.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/builtins.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/codecs.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/codecs.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/collections/__init__.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/collections/__init__.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/collections/abc.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/collections/abc.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/contextlib.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/contextlib.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/ctypes/__init__.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/ctypes/__init__.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/dataclasses.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/dataclasses.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/__init__.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/__init__.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/charset.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/charset.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/contentmanager.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/contentmanager.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/errors.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/errors.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/header.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/header.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/message.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/message.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/policy.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/email/policy.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/enum.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/enum.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/genericpath.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/genericpath.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/__init__.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/__init__.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/abc.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/abc.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/machinery.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/machinery.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/io.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/io.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/logging/__init__.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/logging/__init__.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/mmap.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/mmap.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/ntpath.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/ntpath.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/ntpath.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/ntpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/os/__init__.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/os/__init__.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/os/path.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/os/path.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/pathlib.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/pathlib.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/pickle.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/pickle.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/posixpath.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/posixpath.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/re.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/re.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sre_compile.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sre_compile.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sre_constants.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sre_constants.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sre_parse.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sre_parse.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/string.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/string.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/subprocess.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/subprocess.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sys.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/sys.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/threading.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/threading.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/time.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/time.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/types.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/types.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/typing.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/typing.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/typing_extensions.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/typing_extensions.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/__init__.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/__init__.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util/netbox_api.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util/netbox_api.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util/netbox_api.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util/netbox_api.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller/nac/util.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos/controller.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects/argos.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects/argos.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects.data.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/.mypy_cache/3.11/work/school_projects.meta.json` & `argos-nac-0.1.3/nac/util/.mypy_cache/3.11/work/school_projects.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/common.py` & `argos-nac-0.1.3/nac/util/common.py`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/graphql_util.py` & `argos-nac-0.1.3/nac/util/graphql_util.py`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/nac/util/netbox_api.py` & `argos-nac-0.1.3/nac/util/netbox_api.py`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/pyproject.toml` & `argos-nac-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -37,20 +37,20 @@
     "nornir-napalm>=0.3.0",
     "nornir-utils>=0.2.0",
     "pydantic>=1.10.7",
     "semver>=3.0.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
-argos-deploy = "nac.main:run"
+argos-deploy = "nac.__main__:run"
 
 [build-system]
 requires = [
     "pdm-pep517>=1.0",
 ]
 build-backend = "pdm.pep517.api"
```

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/__future__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/__future__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_ast.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_ast.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_bisect.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_bisect.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_bisect.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_bisect.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_codecs.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_codecs.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_collections_abc.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_collections_abc.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_ctypes.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_ctypes.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_decimal.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_decimal.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_operator.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_operator.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_operator.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_operator.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_argcomplete.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_argcomplete.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_argcomplete.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_argcomplete.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_code/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_code/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_code/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_code/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_code/code.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_code/code.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_code/code.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_code/code.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_code/source.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_code/source.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_code/source.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_code/source.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/saferepr.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/saferepr.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/saferepr.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/terminalwriter.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/terminalwriter.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/wcwidth.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_io/wcwidth.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_version.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_version.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/_version.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/_version.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/rewrite.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/rewrite.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/truncate.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/truncate.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/truncate.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/util.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/util.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/assertion/util.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/assertion/util.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/cacheprovider.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/cacheprovider.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/cacheprovider.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/cacheprovider.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/capture.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/capture.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/capture.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/capture.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/compat.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/compat.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/compat.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/compat.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/argparsing.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/argparsing.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/argparsing.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/argparsing.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/compat.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/compat.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/compat.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/compat.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/exceptions.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/exceptions.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/findpaths.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/findpaths.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/config/findpaths.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/config/findpaths.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/debugging.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/debugging.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/debugging.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/debugging.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/deprecated.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/deprecated.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/deprecated.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/deprecated.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/doctest.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/doctest.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/doctest.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/doctest.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/fixtures.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/fixtures.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/fixtures.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/fixtures.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/freeze_support.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/freeze_support.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/freeze_support.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/freeze_support.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/helpconfig.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/helpconfig.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/helpconfig.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/helpconfig.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/hookspec.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/hookspec.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/hookspec.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/hookspec.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/legacypath.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/legacypath.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/legacypath.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/legacypath.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/logging.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/logging.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/logging.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/logging.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/main.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/main.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/main.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/main.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/mark/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/mark/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/mark/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/mark/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/mark/expression.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/mark/expression.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/mark/expression.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/mark/expression.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/mark/structures.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/mark/structures.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/mark/structures.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/mark/structures.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/monkeypatch.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/monkeypatch.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/monkeypatch.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/monkeypatch.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/nodes.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/nodes.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/nodes.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/nodes.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/outcomes.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/outcomes.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/outcomes.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/outcomes.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/pathlib.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/pathlib.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/pytester.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/pytester.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/pytester.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/pytester.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/pytester_assertions.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/pytester_assertions.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/pytester_assertions.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/python.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/python.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/python.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/python.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/python_api.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/python_api.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/python_api.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/python_api.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/recwarn.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/recwarn.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/recwarn.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/recwarn.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/reports.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/reports.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/reports.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/reports.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/runner.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/runner.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/runner.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/scope.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/scope.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/scope.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/scope.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/stash.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/stash.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/stash.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/stash.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/terminal.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/terminal.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/terminal.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/terminal.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/timing.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/timing.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/timing.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/timing.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/tmpdir.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/tmpdir.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/tmpdir.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/tmpdir.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/warning_types.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/warning_types.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/warning_types.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/warning_types.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/warnings.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/warnings.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_pytest/warnings.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_pytest/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_stat.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_stat.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_stat.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_stat.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_thread.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_thread.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_tracemalloc.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_tracemalloc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_tracemalloc.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_tracemalloc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_typeshed/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_warnings.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_warnings.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_weakref.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_weakref.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_weakref.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_weakref.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_weakrefset.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_weakrefset.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_weakrefset.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_weakrefset.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_winapi.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_winapi.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/_winapi.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/_winapi.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/abc.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/abc.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/argparse.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/argparse.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/argparse.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/argparse.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/array.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/array.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/ast.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/ast.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/ast.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/ast.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/atexit.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/atexit.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/atexit.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/atexit.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/_cmp.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/_cmp.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/_cmp.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/_cmp.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/_typing_compat.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/_typing_compat.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/_typing_compat.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/_typing_compat.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/_version_info.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/_version_info.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/_version_info.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/_version_info.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/converters.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/converters.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/converters.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/converters.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/exceptions.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/exceptions.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/filters.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/filters.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/filters.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/filters.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/setters.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/setters.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/setters.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/setters.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/validators.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/validators.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/attr/validators.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/attr/validators.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/bdb.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/bdb.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/bdb.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/bdb.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/bisect.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/bisect.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/bisect.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/bisect.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/builtins.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/builtins.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/cmd.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/cmd.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/cmd.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/cmd.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/codecs.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/codecs.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/collections/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/collections/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/collections/abc.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/collections/abc.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/contextlib.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/contextlib.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/copy.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/copy.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/copy.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/copy.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/ctypes/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/ctypes/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/dataclasses.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/dataclasses.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/datetime.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/datetime.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/decimal.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/decimal.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/difflib.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/difflib.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/difflib.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/difflib.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/dis.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/dis.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/dis.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/dis.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/doctest.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/doctest.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/doctest.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/doctest.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/email/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/email/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/email/charset.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/email/charset.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/email/contentmanager.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/email/contentmanager.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/email/errors.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/email/errors.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/email/header.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/email/header.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/email/message.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/email/message.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/email/policy.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/email/policy.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/enum.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/enum.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/errno.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/errno.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/errno.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/errno.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/fnmatch.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/fnmatch.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/fnmatch.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/fnmatch.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/functools.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/functools.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/gc.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/gc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/gc.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/gc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/genericpath.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/genericpath.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/getpass.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/getpass.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/getpass.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/getpass.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/gettext.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/gettext.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/gettext.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/gettext.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/glob.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/glob.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/glob.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/glob.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/abc.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/abc.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/machinery.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/machinery.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/util.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/util.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/importlib/util.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/importlib/util.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/iniconfig/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/iniconfig/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/iniconfig/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/iniconfig/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/iniconfig/_parse.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/iniconfig/_parse.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/iniconfig/_parse.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/iniconfig/_parse.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/iniconfig/exceptions.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/iniconfig/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/iniconfig/exceptions.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/iniconfig/exceptions.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/inspect.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/inspect.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/inspect.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/inspect.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/io.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/io.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/itertools.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/itertools.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/itertools.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/itertools.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/json/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/json/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/json/decoder.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/json/decoder.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/json/encoder.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/json/encoder.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/logging/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/logging/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/marshal.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/marshal.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/marshal.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/marshal.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/math.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/math.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/math.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/mmap.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/mmap.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/ntpath.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/ntpath.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/ntpath.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/ntpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/numbers.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/numbers.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/opcode.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/opcode.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/opcode.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/opcode.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/operator.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/operator.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/operator.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/operator.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/os/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/os/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/os/path.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/os/path.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_elffile.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_elffile.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_elffile.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_elffile.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_manylinux.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_manylinux.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_manylinux.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_manylinux.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_musllinux.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_musllinux.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_musllinux.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_musllinux.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_parser.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_parser.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_parser.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_parser.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_structures.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_structures.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_structures.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_structures.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_tokenizer.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_tokenizer.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/_tokenizer.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/_tokenizer.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/markers.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/markers.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/markers.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/markers.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/requirements.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/requirements.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/requirements.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/requirements.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/specifiers.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/specifiers.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/specifiers.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/specifiers.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/tags.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/tags.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/tags.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/tags.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/utils.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/utils.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/utils.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/utils.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/version.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/version.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/packaging/version.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/packaging/version.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/pathlib.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/pathlib.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/pdb.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/pdb.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/pdb.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/pdb.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/pickle.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/pickle.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/pkgutil.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/pkgutil.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/pkgutil.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/pkgutil.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/platform.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/platform.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/platform.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/platform.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/posixpath.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/posixpath.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/pprint.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/pprint.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/pprint.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/pprint.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/pytest/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/pytest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/pytest/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/pytest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/re.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/re.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/reprlib.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/reprlib.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/reprlib.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/reprlib.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/shlex.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/shlex.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/shlex.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/shlex.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/shutil.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/shutil.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/shutil.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/shutil.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/signal.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/signal.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/signal.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/signal.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/sre_compile.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/sre_compile.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/sre_constants.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/sre_constants.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/sre_parse.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/sre_parse.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/stat.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/stat.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/stat.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/stat.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/string.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/string.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/struct.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/struct.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/struct.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/struct.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/subprocess.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/subprocess.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/sys.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/sys.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/sysconfig.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/sysconfig.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/sysconfig.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/sysconfig.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/tempfile.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/tempfile.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/tempfile.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/textwrap.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/textwrap.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/threading.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/threading.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/time.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/time.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/token.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/token.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/token.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/token.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/tokenize.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/tokenize.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/tokenize.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/tokenize.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/tomllib.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/tomllib.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/tomllib.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/tomllib.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/traceback.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/traceback.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/traceback.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/traceback.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/tracemalloc.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/tracemalloc.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/tracemalloc.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/tracemalloc.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/types.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/types.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/typing.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/typing.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/typing_extensions.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/typing_extensions.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unicodedata.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unicodedata.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unicodedata.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unicodedata.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/_log.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/_log.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/async_case.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/async_case.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/case.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/case.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/loader.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/loader.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/main.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/main.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/result.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/result.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/runner.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/runner.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/signals.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/signals.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/suite.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/unittest/suite.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/urllib/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/urllib/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/urllib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/urllib/parse.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/urllib/parse.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/urllib/parse.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/urllib/parse.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/uuid.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/uuid.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/uuid.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/uuid.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/warnings.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/warnings.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/weakref.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/weakref.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/weakref.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/weakref.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/work/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/work/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/work/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/work/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects/argos/controller/tests/__init__.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects/argos/controller/tests/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects/argos/controller/tests/__init__.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects/argos/controller/tests/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects/argos/controller.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects/argos/controller.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects/argos/controller.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects/argos/controller.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects/argos.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects/argos.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects/argos.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects/argos.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects.data.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects.data.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/.mypy_cache/3.11/work/school_projects.meta.json` & `argos-nac-0.1.3/tests/.mypy_cache/3.11/work/school_projects.meta.json`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/cisco_test.py` & `argos-nac-0.1.3/tests/cisco_test.py`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/configs/PE1.log` & `argos-nac-0.1.3/tests/configs/PE1.log`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/configs/PE1_expected.log` & `argos-nac-0.1.3/tests/configs/PE1_expected.log`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/configs/PE2.log` & `argos-nac-0.1.3/tests/configs/PE2.log`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/configs/PE2_expected.log` & `argos-nac-0.1.3/tests/configs/PE2_expected.log`

 * *Files identical despite different names*

### Comparing `argos-nac-0.1.2/tests/site_sample_data.json` & `argos-nac-0.1.3/tests/site_sample_data.json`

 * *Files identical despite different names*

