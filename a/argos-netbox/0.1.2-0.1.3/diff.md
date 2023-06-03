# Comparing `tmp/argos_netbox-0.1.2.tar.gz` & `tmp/argos_netbox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argos_netbox-0.1.2.tar", last modified: Fri Jun  2 06:47:44 2023, max compression
+gzip compressed data, was "argos_netbox-0.1.3.tar", last modified: Sat Jun  3 09:40:37 2023, max compression
```

## Comparing `argos_netbox-0.1.2.tar` & `argos_netbox-0.1.3.tar`

### file list

```diff
@@ -1,140 +1,140 @@
--rw-r--r--   0        0        0      364 2023-05-31 13:41:33.817429 argos_netbox-0.1.2/README.md
--rw-r--r--   0        0        0        7 2023-05-31 13:41:34.021950 argos_netbox-0.1.2/argos_netbox/README.md
--rw-r--r--   0        0        0      332 2023-05-31 13:41:34.026949 argos_netbox-0.1.2/argos_netbox/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 13:41:34.030951 argos_netbox-0.1.2/argos_netbox/api/__init__.py
--rw-r--r--   0        0        0     6272 2023-05-31 13:41:34.030951 argos_netbox-0.1.2/argos_netbox/api/serializers.py
--rw-r--r--   0        0        0      545 2023-05-31 13:41:34.031949 argos_netbox-0.1.2/argos_netbox/api/urls.py
--rw-r--r--   0        0        0      976 2023-05-31 13:41:34.035949 argos_netbox-0.1.2/argos_netbox/api/views.py
--rw-r--r--   0        0        0      382 2023-05-31 13:41:34.036950 argos_netbox-0.1.2/argos_netbox/filtersets.py
--rw-r--r--   0        0        0     4624 2023-06-02 06:47:08.124520 argos_netbox-0.1.2/argos_netbox/forms.py
--rw-r--r--   0        0        0     1772 2023-05-31 13:41:34.040948 argos_netbox-0.1.2/argos_netbox/graphql.py
--rw-r--r--   0        0        0       36 2023-05-14 13:01:57.587396 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/.gitignore
--rw-r--r--   0        0        0        2 2023-05-14 13:01:57.582314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   190035 2023-05-14 13:01:57.524313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1775 2023-05-14 13:01:57.525315 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    61715 2023-05-14 13:01:57.516313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1821 2023-05-14 13:01:57.518314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    19501 2023-05-14 13:01:57.513313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1729 2023-05-14 13:01:57.514313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     7729 2023-05-14 13:01:57.510313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1731 2023-05-14 13:01:57.512313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    92896 2023-05-14 13:01:57.508314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1832 2023-05-14 13:01:57.509315 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    67142 2023-05-14 13:01:57.504314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_winapi.data.json
--rw-r--r--   0        0        0     1804 2023-05-14 13:01:57.505313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_winapi.meta.json
--rw-r--r--   0        0        0    21692 2023-05-14 13:01:57.500312 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1717 2023-05-14 13:01:57.501313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    62974 2023-05-14 13:01:57.497384 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1784 2023-05-14 13:01:57.498312 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0  1147461 2023-05-14 13:01:57.558313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1881 2023-05-14 13:01:57.559313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   127544 2023-05-14 13:01:57.493313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1821 2023-05-14 13:01:57.493313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   390750 2023-05-14 13:01:57.487312 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1800 2023-05-14 13:01:57.488313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     4044 2023-05-14 13:01:57.474316 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1696 2023-05-14 13:01:57.475314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   115814 2023-05-14 13:01:57.472313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1772 2023-05-14 13:01:57.472313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0   144027 2023-05-14 13:01:57.467383 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1828 2023-05-14 13:01:57.468313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8126 2023-05-14 13:01:57.461314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1757 2023-05-14 13:01:57.462314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12853 2023-05-14 13:01:57.458313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1693 2023-05-14 13:01:57.459314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7713 2023-05-14 13:01:57.456315 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1728 2023-05-14 13:01:57.457369 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25497 2023-05-14 13:01:57.454314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1700 2023-05-14 13:01:57.455314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9703 2023-05-14 13:01:57.451313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1713 2023-05-14 13:01:57.452313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    62361 2023-05-14 13:01:57.449314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1850 2023-05-14 13:01:57.450313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    32702 2023-05-14 13:01:57.445312 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1786 2023-05-14 13:01:57.446313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0    95101 2023-05-14 13:01:57.441314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1749 2023-05-14 13:01:57.443313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    23882 2023-05-14 13:01:57.436314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1746 2023-05-14 13:01:57.437378 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     6520 2023-05-14 13:01:57.433314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1731 2023-05-14 13:01:57.434314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    73613 2023-05-14 13:01:57.430314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1879 2023-05-14 13:01:57.431313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    68149 2023-05-14 13:01:57.425315 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1890 2023-05-14 13:01:57.426313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    95589 2023-05-14 13:01:57.421314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1869 2023-05-14 13:01:57.422315 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12491 2023-05-14 13:01:57.417314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1714 2023-05-14 13:01:57.418313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    88673 2023-05-14 13:01:57.414314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1840 2023-05-14 13:01:57.415313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    24368 2023-05-14 13:01:57.409313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1756 2023-05-14 13:01:57.410312 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    15200 2023-05-14 13:01:57.406313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/ntpath.data.json
--rw-r--r--   0        0        0     1768 2023-05-14 13:01:57.407373 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/ntpath.meta.json
--rw-r--r--   0        0        0   248783 2023-05-14 13:01:57.403312 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1899 2023-05-14 13:01:57.405314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     5311 2023-05-14 13:01:57.394317 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1685 2023-05-14 13:01:57.395314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0    90374 2023-05-14 13:01:57.390314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1849 2023-05-14 13:01:57.392313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    47610 2023-05-14 13:01:57.384314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1785 2023-05-14 13:01:57.386314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    80910 2023-05-14 13:01:57.380314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1779 2023-05-14 13:01:57.381316 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   151627 2023-05-14 13:01:57.375314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1871 2023-05-14 13:01:57.377373 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    15014 2023-05-14 13:01:57.369314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1715 2023-05-14 13:01:57.370314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    29571 2023-05-14 13:01:57.366314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1699 2023-05-14 13:01:57.368315 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    52535 2023-05-14 13:01:57.363314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1779 2023-05-14 13:01:57.365313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   181048 2023-05-14 13:01:57.359313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1859 2023-05-14 13:01:57.360314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   168592 2023-05-14 13:01:57.351314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1818 2023-05-14 13:01:57.353315 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0   254573 2023-05-14 13:01:57.345313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1790 2023-05-14 13:01:57.346312 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   446716 2023-05-14 13:01:57.336313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1857 2023-05-14 13:01:57.337460 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    54822 2023-05-14 13:01:57.320394 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1780 2023-05-14 13:01:57.321394 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0     1528 2023-05-14 13:01:57.564314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/__init__.data.json
--rw-r--r--   0        0        0     1564 2023-05-14 13:01:57.565313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/__init__.meta.json
--rw-r--r--   0        0        0     1381 2023-05-14 13:01:57.566969 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects.data.json
--rw-r--r--   0        0        0     1521 2023-05-14 13:01:57.567314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects.meta.json
--rw-r--r--   0        0        0     1424 2023-05-14 13:01:57.569314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos.data.json
--rw-r--r--   0        0        0     1534 2023-05-14 13:01:57.570315 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos.meta.json
--rw-r--r--   0        0        0     1523 2023-05-14 13:01:57.571314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.data.json
--rw-r--r--   0        0        0     1563 2023-05-14 13:01:57.572316 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.meta.json
--rw-r--r--   0        0        0     5506 2023-05-14 13:01:57.580315 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.data.json
--rw-r--r--   0        0        0     1738 2023-05-14 13:01:57.581314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.meta.json
--rw-r--r--   0        0        0     4680 2023-05-14 13:01:57.576315 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.data.json
--rw-r--r--   0        0        0     1740 2023-05-14 13:01:57.577314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.meta.json
--rw-r--r--   0        0        0     1955 2023-05-14 13:01:57.573314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.data.json
--rw-r--r--   0        0        0     1673 2023-05-14 13:01:57.574314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.meta.json
--rw-r--r--   0        0        0     1904 2023-05-14 13:01:57.562314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.data.json
--rw-r--r--   0        0        0     1658 2023-05-14 13:01:57.563314 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.meta.json
--rw-r--r--   0        0        0      193 2023-05-14 13:01:57.591313 argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     8975 2023-05-31 13:41:34.041949 argos_netbox-0.1.2/argos_netbox/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-31 13:41:34.042950 argos_netbox-0.1.2/argos_netbox/migrations/__init__.py
--rw-r--r--   0        0        0     6889 2023-05-31 13:41:34.042950 argos_netbox-0.1.2/argos_netbox/models.py
--rw-r--r--   0        0        0     2412 2023-05-31 13:41:34.043949 argos_netbox-0.1.2/argos_netbox/navigation.py
--rw-r--r--   0        0        0        0 2023-05-31 13:41:34.043949 argos_netbox-0.1.2/argos_netbox/requirements.txt
--rw-r--r--   0        0        0     3334 2023-05-31 13:41:34.043949 argos_netbox-0.1.2/argos_netbox/tables.py
--rw-r--r--   0        0        0     1810 2023-05-31 13:41:34.044948 argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/address_family.html
--rw-r--r--   0        0        0     1067 2023-05-31 13:41:34.045948 argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/address_family_edit.html
--rw-r--r--   0        0        0     1249 2023-05-31 13:41:34.046948 argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/bgp_ce.html
--rw-r--r--   0        0        0     2510 2023-05-31 13:41:34.046948 argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/bgp_mesh.html
--rw-r--r--   0        0        0     1852 2023-05-31 13:41:34.047949 argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/bgp_pe.html
--rw-r--r--   0        0        0     1421 2023-05-31 13:41:34.047949 argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/ldp.html
--rw-r--r--   0        0        0     1106 2023-05-31 13:41:34.048952 argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/ldp_edit.html
--rw-r--r--   0        0        0     1328 2023-05-31 13:41:34.049949 argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/mpls_instance.html
--rw-r--r--   0        0        0      680 2023-05-31 13:41:34.049949 argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/util/hide_if_checked.html
--rw-r--r--   0        0        0      326 2023-05-31 13:41:34.050950 argos_netbox-0.1.2/argos_netbox/templatetags/argos_macros.py
--rw-r--r--   0        0        0     3925 2023-05-31 13:41:34.054948 argos_netbox-0.1.2/argos_netbox/urls.py
--rw-r--r--   0        0        0       20 2023-06-02 06:47:22.681782 argos_netbox-0.1.2/argos_netbox/version.py
--rw-r--r--   0        0        0     2981 2023-05-31 13:41:34.059947 argos_netbox-0.1.2/argos_netbox/views.py
--rw-r--r--   0        0        0     1399 2023-06-02 06:47:44.989792 argos_netbox-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 argos_netbox-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      364 2023-05-31 13:41:33.817429 argos_netbox-0.1.3/README.md
+-rw-r--r--   0        0        0        7 2023-05-31 13:41:34.021950 argos_netbox-0.1.3/argos_netbox/README.md
+-rw-r--r--   0        0        0      320 2023-06-02 11:56:32.302361 argos_netbox-0.1.3/argos_netbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:41:34.030951 argos_netbox-0.1.3/argos_netbox/api/__init__.py
+-rw-r--r--   0        0        0     6272 2023-05-31 13:41:34.030951 argos_netbox-0.1.3/argos_netbox/api/serializers.py
+-rw-r--r--   0        0        0      545 2023-05-31 13:41:34.031949 argos_netbox-0.1.3/argos_netbox/api/urls.py
+-rw-r--r--   0        0        0      976 2023-05-31 13:41:34.035949 argos_netbox-0.1.3/argos_netbox/api/views.py
+-rw-r--r--   0        0        0      382 2023-05-31 13:41:34.036950 argos_netbox-0.1.3/argos_netbox/filtersets.py
+-rw-r--r--   0        0        0     4624 2023-06-02 06:56:43.807811 argos_netbox-0.1.3/argos_netbox/forms.py
+-rw-r--r--   0        0        0     1772 2023-05-31 13:41:34.040948 argos_netbox-0.1.3/argos_netbox/graphql.py
+-rw-r--r--   0        0        0       36 2023-05-14 13:01:57.587396 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0        2 2023-05-14 13:01:57.582314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   190035 2023-05-14 13:01:57.524313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1775 2023-05-14 13:01:57.525315 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    61715 2023-05-14 13:01:57.516313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1821 2023-05-14 13:01:57.518314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    19501 2023-05-14 13:01:57.513313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1729 2023-05-14 13:01:57.514313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     7729 2023-05-14 13:01:57.510313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1731 2023-05-14 13:01:57.512313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    92896 2023-05-14 13:01:57.508314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1832 2023-05-14 13:01:57.509315 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    67142 2023-05-14 13:01:57.504314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_winapi.data.json
+-rw-r--r--   0        0        0     1804 2023-05-14 13:01:57.505313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_winapi.meta.json
+-rw-r--r--   0        0        0    21692 2023-05-14 13:01:57.500312 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1717 2023-05-14 13:01:57.501313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    62974 2023-05-14 13:01:57.497384 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1784 2023-05-14 13:01:57.498312 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0  1147461 2023-05-14 13:01:57.558313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1881 2023-05-14 13:01:57.559313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   127544 2023-05-14 13:01:57.493313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1821 2023-05-14 13:01:57.493313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   390750 2023-05-14 13:01:57.487312 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1800 2023-05-14 13:01:57.488313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4044 2023-05-14 13:01:57.474316 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1696 2023-05-14 13:01:57.475314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   115814 2023-05-14 13:01:57.472313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1772 2023-05-14 13:01:57.472313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0   144027 2023-05-14 13:01:57.467383 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1828 2023-05-14 13:01:57.468313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     8126 2023-05-14 13:01:57.461314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1757 2023-05-14 13:01:57.462314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12853 2023-05-14 13:01:57.458313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1693 2023-05-14 13:01:57.459314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7713 2023-05-14 13:01:57.456315 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1728 2023-05-14 13:01:57.457369 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25497 2023-05-14 13:01:57.454314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1700 2023-05-14 13:01:57.455314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9703 2023-05-14 13:01:57.451313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1713 2023-05-14 13:01:57.452313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    62361 2023-05-14 13:01:57.449314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1850 2023-05-14 13:01:57.450313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    32702 2023-05-14 13:01:57.445312 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1786 2023-05-14 13:01:57.446313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0    95101 2023-05-14 13:01:57.441314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1749 2023-05-14 13:01:57.443313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    23882 2023-05-14 13:01:57.436314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1746 2023-05-14 13:01:57.437378 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     6520 2023-05-14 13:01:57.433314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1731 2023-05-14 13:01:57.434314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    73613 2023-05-14 13:01:57.430314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1879 2023-05-14 13:01:57.431313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    68149 2023-05-14 13:01:57.425315 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1890 2023-05-14 13:01:57.426313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    95589 2023-05-14 13:01:57.421314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1869 2023-05-14 13:01:57.422315 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12491 2023-05-14 13:01:57.417314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1714 2023-05-14 13:01:57.418313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    88673 2023-05-14 13:01:57.414314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1840 2023-05-14 13:01:57.415313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    24368 2023-05-14 13:01:57.409313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1756 2023-05-14 13:01:57.410312 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    15200 2023-05-14 13:01:57.406313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/ntpath.data.json
+-rw-r--r--   0        0        0     1768 2023-05-14 13:01:57.407373 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/ntpath.meta.json
+-rw-r--r--   0        0        0   248783 2023-05-14 13:01:57.403312 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1899 2023-05-14 13:01:57.405314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     5311 2023-05-14 13:01:57.394317 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1685 2023-05-14 13:01:57.395314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0    90374 2023-05-14 13:01:57.390314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1849 2023-05-14 13:01:57.392313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    47610 2023-05-14 13:01:57.384314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1785 2023-05-14 13:01:57.386314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    80910 2023-05-14 13:01:57.380314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1779 2023-05-14 13:01:57.381316 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   151627 2023-05-14 13:01:57.375314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1871 2023-05-14 13:01:57.377373 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    15014 2023-05-14 13:01:57.369314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1715 2023-05-14 13:01:57.370314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    29571 2023-05-14 13:01:57.366314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1699 2023-05-14 13:01:57.368315 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    52535 2023-05-14 13:01:57.363314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1779 2023-05-14 13:01:57.365313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   181048 2023-05-14 13:01:57.359313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1859 2023-05-14 13:01:57.360314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   168592 2023-05-14 13:01:57.351314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1818 2023-05-14 13:01:57.353315 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0   254573 2023-05-14 13:01:57.345313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1790 2023-05-14 13:01:57.346312 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   446716 2023-05-14 13:01:57.336313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1857 2023-05-14 13:01:57.337460 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    54822 2023-05-14 13:01:57.320394 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1780 2023-05-14 13:01:57.321394 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0     1528 2023-05-14 13:01:57.564314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/__init__.data.json
+-rw-r--r--   0        0        0     1564 2023-05-14 13:01:57.565313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/__init__.meta.json
+-rw-r--r--   0        0        0     1381 2023-05-14 13:01:57.566969 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects.data.json
+-rw-r--r--   0        0        0     1521 2023-05-14 13:01:57.567314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects.meta.json
+-rw-r--r--   0        0        0     1424 2023-05-14 13:01:57.569314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos.data.json
+-rw-r--r--   0        0        0     1534 2023-05-14 13:01:57.570315 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos.meta.json
+-rw-r--r--   0        0        0     1523 2023-05-14 13:01:57.571314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.data.json
+-rw-r--r--   0        0        0     1563 2023-05-14 13:01:57.572316 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.meta.json
+-rw-r--r--   0        0        0     5506 2023-05-14 13:01:57.580315 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.data.json
+-rw-r--r--   0        0        0     1738 2023-05-14 13:01:57.581314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.meta.json
+-rw-r--r--   0        0        0     4680 2023-05-14 13:01:57.576315 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.data.json
+-rw-r--r--   0        0        0     1740 2023-05-14 13:01:57.577314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.meta.json
+-rw-r--r--   0        0        0     1955 2023-05-14 13:01:57.573314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.data.json
+-rw-r--r--   0        0        0     1673 2023-05-14 13:01:57.574314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.meta.json
+-rw-r--r--   0        0        0     1904 2023-05-14 13:01:57.562314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.data.json
+-rw-r--r--   0        0        0     1658 2023-05-14 13:01:57.563314 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.meta.json
+-rw-r--r--   0        0        0      193 2023-05-14 13:01:57.591313 argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     8975 2023-05-31 13:41:34.041949 argos_netbox-0.1.3/argos_netbox/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:41:34.042950 argos_netbox-0.1.3/argos_netbox/migrations/__init__.py
+-rw-r--r--   0        0        0     6889 2023-05-31 13:41:34.042950 argos_netbox-0.1.3/argos_netbox/models.py
+-rw-r--r--   0        0        0     2412 2023-05-31 13:41:34.043949 argos_netbox-0.1.3/argos_netbox/navigation.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:41:34.043949 argos_netbox-0.1.3/argos_netbox/requirements.txt
+-rw-r--r--   0        0        0     3334 2023-05-31 13:41:34.043949 argos_netbox-0.1.3/argos_netbox/tables.py
+-rw-r--r--   0        0        0     1810 2023-05-31 13:41:34.044948 argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/address_family.html
+-rw-r--r--   0        0        0     1067 2023-05-31 13:41:34.045948 argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/address_family_edit.html
+-rw-r--r--   0        0        0     1249 2023-05-31 13:41:34.046948 argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/bgp_ce.html
+-rw-r--r--   0        0        0     2510 2023-05-31 13:41:34.046948 argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/bgp_mesh.html
+-rw-r--r--   0        0        0     1852 2023-05-31 13:41:34.047949 argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/bgp_pe.html
+-rw-r--r--   0        0        0     1421 2023-05-31 13:41:34.047949 argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/ldp.html
+-rw-r--r--   0        0        0     1106 2023-05-31 13:41:34.048952 argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/ldp_edit.html
+-rw-r--r--   0        0        0     1328 2023-05-31 13:41:34.049949 argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/mpls_instance.html
+-rw-r--r--   0        0        0      680 2023-05-31 13:41:34.049949 argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/util/hide_if_checked.html
+-rw-r--r--   0        0        0      326 2023-05-31 13:41:34.050950 argos_netbox-0.1.3/argos_netbox/templatetags/argos_macros.py
+-rw-r--r--   0        0        0     3925 2023-05-31 13:41:34.054948 argos_netbox-0.1.3/argos_netbox/urls.py
+-rw-r--r--   0        0        0       22 2023-06-03 09:37:29.410109 argos_netbox-0.1.3/argos_netbox/version.py
+-rw-r--r--   0        0        0     2981 2023-05-31 13:41:34.059947 argos_netbox-0.1.3/argos_netbox/views.py
+-rw-r--r--   0        0        0     1399 2023-06-03 09:40:37.757029 argos_netbox-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 argos_netbox-0.1.3/PKG-INFO
```

### Comparing `argos_netbox-0.1.2/argos_netbox/api/serializers.py` & `argos_netbox-0.1.3/argos_netbox/api/serializers.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/api/urls.py` & `argos_netbox-0.1.3/argos_netbox/api/urls.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/api/views.py` & `argos_netbox-0.1.3/argos_netbox/api/views.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/forms.py` & `argos_netbox-0.1.3/argos_netbox/forms.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/graphql.py` & `argos_netbox-0.1.3/argos_netbox/graphql.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_ast.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_ast.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_codecs.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_codecs.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_collections_abc.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_collections_abc.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_ctypes.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_ctypes.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_typeshed/__init__.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_winapi.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_winapi.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/_winapi.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/_winapi.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/abc.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/abc.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/array.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/array.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/builtins.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/builtins.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/codecs.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/codecs.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/collections/__init__.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/collections/__init__.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/collections/abc.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/collections/abc.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/contextlib.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/contextlib.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/ctypes/__init__.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/ctypes/__init__.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/__init__.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/__init__.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/charset.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/charset.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/contentmanager.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/contentmanager.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/errors.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/errors.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/header.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/header.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/message.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/message.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/policy.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/email/policy.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/enum.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/enum.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/genericpath.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/genericpath.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/__init__.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/__init__.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/abc.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/abc.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/machinery.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/machinery.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/io.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/io.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/mmap.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/mmap.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/ntpath.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/ntpath.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/ntpath.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/ntpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/os/__init__.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/os/__init__.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/os/path.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/os/path.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/pathlib.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/pathlib.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/pickle.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/pickle.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/posixpath.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/posixpath.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/re.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/re.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sre_compile.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sre_compile.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sre_constants.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sre_constants.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sre_parse.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sre_parse.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/subprocess.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/subprocess.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sys.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/sys.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/types.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/types.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/typing.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/typing.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/typing_extensions.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/typing_extensions.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/__init__.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/__init__.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.data.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.meta.json` & `argos_netbox-0.1.3/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/migrations/0001_initial.py` & `argos_netbox-0.1.3/argos_netbox/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/models.py` & `argos_netbox-0.1.3/argos_netbox/models.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/navigation.py` & `argos_netbox-0.1.3/argos_netbox/navigation.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/tables.py` & `argos_netbox-0.1.3/argos_netbox/tables.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/address_family.html` & `argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/address_family.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/address_family_edit.html` & `argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/address_family_edit.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/bgp_ce.html` & `argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/bgp_ce.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/bgp_mesh.html` & `argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/bgp_mesh.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/bgp_pe.html` & `argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/bgp_pe.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/ldp.html` & `argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/ldp.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/ldp_edit.html` & `argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/ldp_edit.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/mpls_instance.html` & `argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/mpls_instance.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/templates/argos_netbox/util/hide_if_checked.html` & `argos_netbox-0.1.3/argos_netbox/templates/argos_netbox/util/hide_if_checked.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/urls.py` & `argos_netbox-0.1.3/argos_netbox/urls.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/argos_netbox/views.py` & `argos_netbox-0.1.3/argos_netbox/views.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.2/pyproject.toml` & `argos_netbox-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 requires-python = ">=3.9"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
 ]
-version = "0.1.2"
+version = "0.1.3"
 
 [project.urls]
 Repository = "https://gitlab.ost.ch/pydantic-sa/netboxify"
 
 [project.optional-dependencies]
 
 [tool.pdm.version]
```

### Comparing `argos_netbox-0.1.2/PKG-INFO` & `argos_netbox-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argos-netbox
-Version: 0.1.2
+Version: 0.1.3
 Author-Email: Dominic Walther <dominic.walther@ost.ch>, Dejan Jovicic <dejan.jovicic@ost.ch>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Project-URL: Repository, https://gitlab.ost.ch/pydantic-sa/netboxify
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

