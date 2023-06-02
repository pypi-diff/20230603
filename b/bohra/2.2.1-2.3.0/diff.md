# Comparing `tmp/bohra-2.2.1.tar.gz` & `tmp/bohra-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bohra-2.2.1.tar", last modified: Mon May  1 07:21:22 2023, max compression
+gzip compressed data, was "dist/bohra-2.3.0.tar", last modified: Fri Jun  2 23:54:39 2023, max compression
```

## Comparing `bohra-2.2.1.tar` & `bohra-2.3.0.tar`

### file list

```diff
@@ -1,157 +1,198 @@
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    35149 2019-07-28 01:44:48.000000 bohra-2.2.1/LICENSE.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      202 2021-08-27 05:57:12.000000 bohra-2.2.1/MANIFEST.in
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    12805 2023-05-01 07:21:22.000000 bohra-2.2.1/PKG-INFO
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    10272 2023-04-24 05:05:44.000000 bohra-2.2.1/README.md
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      769 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/CustomLog.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    30708 2023-04-24 03:55:45.000000 bohra-2.2.1/bohra/SnpDetection.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     8434 2020-03-12 06:16:45.000000 bohra-2.2.1/bohra/Utils.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      216 2019-08-07 06:34:59.000000 bohra-2.2.1/bohra/__init__.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     9065 2023-04-24 05:09:25.000000 bohra-2.2.1/bohra/bohra.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     5409 2023-04-04 03:44:06.000000 bohra-2.2.1/bohra/main.nf
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/collation/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/collation/bin/
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      710 2021-11-18 03:36:53.000000 bohra-2.2.1/bohra/modules/collation/bin/add_header_mlst.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1480 2021-12-19 02:04:48.000000 bohra-2.2.1/bohra/modules/collation/bin/collate_asm.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      664 2021-11-09 04:29:51.000000 bohra-2.2.1/bohra/modules/collation/bin/collate_kraken2.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      343 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/collation/bin/collate_plasmids.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     2517 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/collation/bin/collate_stats.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)    13486 2022-03-05 01:26:46.000000 bohra-2.2.1/bohra/modules/collation/bin/compile.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1405 2021-10-05 07:55:10.000000 bohra-2.2.1/bohra/modules/collation/bin/snippy_qc.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      598 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/collation/bin/wrangle_mobsuite.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/collation/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     7114 2023-03-31 02:12:30.000000 bohra-2.2.1/bohra/modules/collation/main.nf
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/csvtk/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/csvtk/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1140 2023-03-31 01:20:40.000000 bohra-2.2.1/bohra/modules/csvtk/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/csvtk/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/gubbins/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/gubbins/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1021 2023-05-01 06:55:31.000000 bohra-2.2.1/bohra/modules/gubbins/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/gubbins/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/iqtree/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/iqtree/bin/
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1212 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/iqtree/bin/iqtree_generator.sh
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/iqtree/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1229 2023-03-31 01:20:24.000000 bohra-2.2.1/bohra/modules/iqtree/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/iqtree/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/kraken2/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/kraken2/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1282 2023-03-31 01:20:15.000000 bohra-2.2.1/bohra/modules/kraken2/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/kraken2/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/mash/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/mash/sketch/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mash/sketch/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1415 2023-03-31 01:20:11.000000 bohra-2.2.1/bohra/modules/mash/sketch/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mash/sketch/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/mash/triangle/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mash/triangle/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1069 2023-03-31 01:20:06.000000 bohra-2.2.1/bohra/modules/mash/triangle/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mash/triangle/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/mlst/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mlst/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1427 2023-03-31 06:32:25.000000 bohra-2.2.1/bohra/modules/mlst/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1721 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mlst/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/mobsuite/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mobsuite/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1349 2023-03-31 01:19:55.000000 bohra-2.2.1/bohra/modules/mobsuite/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/mobsuite/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/panaroo/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-09-03 10:18:11.000000 bohra-2.2.1/bohra/modules/panaroo/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1414 2023-04-24 03:58:15.000000 bohra-2.2.1/bohra/modules/panaroo/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-09-03 10:18:11.000000 bohra-2.2.1/bohra/modules/panaroo/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/prokka/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/prokka/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1285 2023-03-31 01:19:42.000000 bohra-2.2.1/bohra/modules/prokka/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/prokka/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/quicktree/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/quicktree/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1090 2023-03-31 01:19:37.000000 bohra-2.2.1/bohra/modules/quicktree/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/quicktree/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/resistome/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/resistome/bin/
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1118 2021-11-11 03:19:28.000000 bohra-2.2.1/bohra/modules/resistome/bin/combine.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      656 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/resistome/bin/concat.py
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1789 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/resistome/bin/meta.yaml
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/resistome/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2940 2023-03-31 01:19:31.000000 bohra-2.2.1/bohra/modules/resistome/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1834 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/resistome/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/roary2svg/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/roary2svg/bin/
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     5179 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/roary2svg/bin/roary2svg.pl
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/roary2svg/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      712 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/roary2svg/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/roary2svg/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/seqkit/
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/seqkit/fx2tab/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/seqkit/fx2tab/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1461 2023-03-31 01:19:19.000000 bohra-2.2.1/bohra/modules/seqkit/fx2tab/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/seqkit/fx2tab/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/seqkit/stats/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/seqkit/stats/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1570 2023-03-31 01:19:14.000000 bohra-2.2.1/bohra/modules/seqkit/stats/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/seqkit/stats/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/seqtk/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/seqtk/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1132 2023-03-31 01:21:08.000000 bohra-2.2.1/bohra/modules/seqtk/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/seqtk/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/shovill/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/shovill/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1295 2023-03-31 01:21:34.000000 bohra-2.2.1/bohra/modules/shovill/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/shovill/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/skesa/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/skesa/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1277 2023-03-31 01:21:53.000000 bohra-2.2.1/bohra/modules/skesa/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/skesa/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/snippy/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-28 02:54:18.000000 bohra-2.2.1/bohra/modules/snippy/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1663 2023-04-13 00:09:28.000000 bohra-2.2.1/bohra/modules/snippy/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/snippy/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/snippy_clean/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-03-31 00:49:55.000000 bohra-2.2.1/bohra/modules/snippy_clean/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      944 2023-03-31 01:22:37.000000 bohra-2.2.1/bohra/modules/snippy_clean/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2023-03-31 00:49:55.000000 bohra-2.2.1/bohra/modules/snippy_clean/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/snippy_core/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/snippy_core/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1350 2023-03-31 01:22:43.000000 bohra-2.2.1/bohra/modules/snippy_core/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/snippy_core/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/snp_dists/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/snp_dists/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1095 2023-03-31 01:23:35.000000 bohra-2.2.1/bohra/modules/snp_dists/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/snp_dists/meta.yml
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/modules/spades/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/spades/functions.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1406 2023-03-31 01:23:33.000000 bohra-2.2.1/bohra/modules/spades/main.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/modules/spades/meta.yml
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1963 2023-03-31 01:27:18.000000 bohra-2.2.1/bohra/nextflow.config
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/templates/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      932 2019-09-21 05:50:22.000000 bohra-2.2.1/bohra/templates/cluster.tmpl
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      806 2021-02-23 06:36:40.000000 bohra-2.2.1/bohra/templates/config_snippy.yaml
--rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)    17031 2021-11-23 01:23:44.000000 bohra-2.2.1/bohra/templates/index.html
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    17104 2021-11-22 01:20:59.000000 bohra-2.2.1/bohra/templates/report_analysis.json
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/tests/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        0 2019-07-28 01:44:48.000000 bohra-2.2.1/bohra/tests/test.bed
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)  7163607 2019-07-28 01:44:48.000000 bohra-2.2.1/bohra/tests/test.gbk
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      788 2019-07-28 01:44:48.000000 bohra-2.2.1/bohra/tests/test.tab
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2172 2021-08-29 03:00:41.000000 bohra-2.2.1/bohra/tests/test_bohra.py
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        0 2019-07-28 01:44:48.000000 bohra-2.2.1/bohra/tests/test_file.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       17 2023-05-01 07:12:48.000000 bohra-2.2.1/bohra/version.py
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra/workflows/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2577 2023-03-31 06:22:16.000000 bohra-2.2.1/bohra/workflows/assemble_typing.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      656 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/workflows/collation.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1519 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/workflows/common.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     4714 2023-03-31 06:22:16.000000 bohra-2.2.1/bohra/workflows/default.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      375 2021-10-05 08:04:23.000000 bohra-2.2.1/bohra/workflows/pangenome.nf
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      402 2021-08-24 07:45:44.000000 bohra-2.2.1/bohra/workflows/preview.nf
-drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra.egg-info/
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    12805 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra.egg-info/PKG-INFO
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     3728 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra.egg-info/SOURCES.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        1 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra.egg-info/dependency_links.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       44 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra.egg-info/entry_points.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        1 2019-08-07 06:36:45.000000 bohra-2.2.1/bohra.egg-info/not-zip-safe
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      108 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra.egg-info/requires.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        6 2023-05-01 07:21:22.000000 bohra-2.2.1/bohra.egg-info/top_level.txt
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1122 2023-05-01 07:21:22.000000 bohra-2.2.1/setup.cfg
--rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       69 2020-03-06 03:52:01.000000 bohra-2.2.1/setup.py
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:39.000000 bohra-2.3.0/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    35149 2019-07-28 01:44:48.000000 bohra-2.3.0/LICENSE.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      233 2023-06-02 23:10:48.000000 bohra-2.3.0/MANIFEST.in
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     3440 2023-06-02 23:54:39.000000 bohra-2.3.0/PKG-INFO
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2347 2023-06-02 23:10:48.000000 bohra-2.3.0/README.md
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      769 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/CustomLog.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    35519 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/SnpDetection.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     8434 2020-03-12 06:16:45.000000 bohra-2.3.0/bohra/Utils.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      216 2019-08-07 06:34:59.000000 bohra-2.3.0/bohra/__init__.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     9183 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/bohra.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    13336 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/bohra_install.sh
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     6511 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/main.nf
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:35.000000 bohra-2.3.0/bohra/modules/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/collation/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/collation/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      710 2021-11-18 03:36:53.000000 bohra-2.3.0/bohra/modules/collation/bin/add_header_mlst.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1492 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/collation/bin/collate_asm.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      664 2021-11-09 04:29:51.000000 bohra-2.3.0/bohra/modules/collation/bin/collate_kraken2.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1978 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/collation/bin/collate_stats.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      362 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/collation/bin/collate_tables.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)    12892 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/collation/bin/compile.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1405 2021-10-05 07:55:10.000000 bohra-2.3.0/bohra/modules/collation/bin/snippy_qc.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      598 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/collation/bin/wrangle_mobsuite.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/collation/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     7098 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/collation/main.nf
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/csvtk/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/csvtk/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1146 2023-05-09 02:53:48.000000 bohra-2.3.0/bohra/modules/csvtk/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/csvtk/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/ectyper/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/ectyper/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1285 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/ectyper/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/ectyper/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/emmtyper/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/emmtyper/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1304 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/emmtyper/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/emmtyper/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/gubbins/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/gubbins/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1033 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/gubbins/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/gubbins/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/iqtree/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/iqtree/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1201 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/iqtree/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/iqtree/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/kleborate/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/kleborate/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1339 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/kleborate/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/kleborate/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/kmc/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/kmc/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      899 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/kmc/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1513 2023-06-02 23:10:48.000000 bohra-2.3.0/bohra/modules/kmc/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/kraken2/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/kraken2/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1289 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/kraken2/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/kraken2/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/lissero/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/lissero/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1358 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/lissero/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1511 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/lissero/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:35.000000 bohra-2.3.0/bohra/modules/mash/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/mash/sketch/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/mash/sketch/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1068 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/mash/sketch/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/mash/sketch/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/mash/triangle/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/mash/triangle/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1075 2023-05-09 02:53:48.000000 bohra-2.3.0/bohra/modules/mash/triangle/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/mash/triangle/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/meningotype/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/meningotype/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1349 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/meningotype/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/meningotype/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/mlst/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/mlst/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1433 2023-05-09 02:53:48.000000 bohra-2.3.0/bohra/modules/mlst/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1535 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/mlst/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/mobsuite/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/mobsuite/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1361 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/mobsuite/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/mobsuite/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra/modules/ngmaster/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/ngmaster/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1135 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/ngmaster/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/ngmaster/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/panaroo/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-09-03 10:18:11.000000 bohra-2.3.0/bohra/modules/panaroo/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1226 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/panaroo/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-09-03 10:18:11.000000 bohra-2.3.0/bohra/modules/panaroo/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/prokka/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/prokka/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1150 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/prokka/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/prokka/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/quicktree/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/quicktree/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1109 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/quicktree/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/quicktree/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/resistome/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/resistome/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1118 2021-11-11 03:19:28.000000 bohra-2.3.0/bohra/modules/resistome/bin/combine.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      656 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/resistome/bin/concat.py
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     1789 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/resistome/bin/meta.yaml
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/resistome/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2944 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/resistome/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1834 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/resistome/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/roary2svg/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/roary2svg/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)     5179 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/roary2svg/bin/roary2svg.pl
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/roary2svg/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      712 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/roary2svg/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/roary2svg/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:35.000000 bohra-2.3.0/bohra/modules/seqkit/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/seqkit/fx2tab/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/seqkit/fx2tab/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1467 2023-05-09 02:53:48.000000 bohra-2.3.0/bohra/modules/seqkit/fx2tab/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/seqkit/fx2tab/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/seqkit/stats/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/seqkit/stats/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1576 2023-05-09 02:53:48.000000 bohra-2.3.0/bohra/modules/seqkit/stats/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/seqkit/stats/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/seqtk/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/seqtk/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1138 2023-05-09 02:53:48.000000 bohra-2.3.0/bohra/modules/seqtk/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1594 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/seqtk/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/shovill/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/shovill/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1301 2023-05-29 01:29:00.000000 bohra-2.3.0/bohra/modules/shovill/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/shovill/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/skesa/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/skesa/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1283 2023-05-09 02:53:48.000000 bohra-2.3.0/bohra/modules/skesa/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/skesa/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/snippy/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-28 02:54:18.000000 bohra-2.3.0/bohra/modules/snippy/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1669 2023-05-09 02:53:48.000000 bohra-2.3.0/bohra/modules/snippy/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/snippy/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/snippy_clean/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-03-31 00:49:55.000000 bohra-2.3.0/bohra/modules/snippy_clean/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      950 2023-05-09 02:53:48.000000 bohra-2.3.0/bohra/modules/snippy_clean/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2023-03-31 00:49:55.000000 bohra-2.3.0/bohra/modules/snippy_clean/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/snippy_core/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/snippy_core/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1356 2023-05-09 02:53:48.000000 bohra-2.3.0/bohra/modules/snippy_core/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/snippy_core/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/snp_dists/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/snp_dists/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1101 2023-05-09 02:53:48.000000 bohra-2.3.0/bohra/modules/snp_dists/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/snp_dists/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/spades/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/spades/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1368 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/spades/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1870 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/modules/spades/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/stype/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/stype/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1433 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/stype/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1644 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/stype/meta.yml
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/utils/
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:37.000000 bohra-2.3.0/bohra/modules/utils/bin/
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)      258 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/utils/bin/extract_species.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2025 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/utils/functions.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    19267 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/utils/main.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1844 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/modules/utils/meta.yml
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1955 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/nextflow.config
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:38.000000 bohra-2.3.0/bohra/templates/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      932 2019-09-21 05:50:22.000000 bohra-2.3.0/bohra/templates/cluster.tmpl
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      806 2021-02-23 06:36:40.000000 bohra-2.3.0/bohra/templates/config_snippy.yaml
+-rwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)    17087 2023-06-02 23:10:49.000000 bohra-2.3.0/bohra/templates/index.html
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)    34714 2023-06-02 23:10:50.000000 bohra-2.3.0/bohra/templates/report_analysis.json
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:38.000000 bohra-2.3.0/bohra/tests/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        0 2019-07-28 01:44:48.000000 bohra-2.3.0/bohra/tests/test.bed
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)  7163607 2019-07-28 01:44:48.000000 bohra-2.3.0/bohra/tests/test.gbk
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      788 2019-07-28 01:44:48.000000 bohra-2.3.0/bohra/tests/test.tab
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     2172 2021-08-29 03:00:41.000000 bohra-2.3.0/bohra/tests/test_bohra.py
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        0 2019-07-28 01:44:48.000000 bohra-2.3.0/bohra/tests/test_file.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       17 2023-06-02 23:12:15.000000 bohra-2.3.0/bohra/version.py
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:39.000000 bohra-2.3.0/bohra/workflows/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1566 2023-06-02 23:10:50.000000 bohra-2.3.0/bohra/workflows/assemble.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      656 2021-08-24 07:45:44.000000 bohra-2.3.0/bohra/workflows/collation.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     4662 2023-06-02 23:10:50.000000 bohra-2.3.0/bohra/workflows/default.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      375 2021-10-05 08:04:23.000000 bohra-2.3.0/bohra/workflows/pangenome.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      542 2023-06-02 23:10:50.000000 bohra-2.3.0/bohra/workflows/preview.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      941 2023-06-02 23:10:50.000000 bohra-2.3.0/bohra/workflows/read_assessment.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1555 2023-06-02 23:10:50.000000 bohra-2.3.0/bohra/workflows/snps.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      578 2023-06-02 23:10:50.000000 bohra-2.3.0/bohra/workflows/species.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     4401 2023-06-02 23:10:50.000000 bohra-2.3.0/bohra/workflows/typing.nf
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     9848 2023-06-02 23:10:50.000000 bohra-2.3.0/bohra/workflows/versions.nf
+drwxr-xr-x   0 khhor    (638696329) domain_users (1388800513)        0 2023-06-02 23:54:36.000000 bohra-2.3.0/bohra.egg-info/
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     3440 2023-06-02 23:54:32.000000 bohra-2.3.0/bohra.egg-info/PKG-INFO
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     4718 2023-06-02 23:54:33.000000 bohra-2.3.0/bohra.egg-info/SOURCES.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        1 2023-06-02 23:54:32.000000 bohra-2.3.0/bohra.egg-info/dependency_links.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       44 2023-06-02 23:54:32.000000 bohra-2.3.0/bohra.egg-info/entry_points.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        1 2019-08-07 06:36:45.000000 bohra-2.3.0/bohra.egg-info/not-zip-safe
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)      108 2023-06-02 23:54:32.000000 bohra-2.3.0/bohra.egg-info/requires.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)        6 2023-06-02 23:54:32.000000 bohra-2.3.0/bohra.egg-info/top_level.txt
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)     1122 2023-06-02 23:54:39.000000 bohra-2.3.0/setup.cfg
+-rw-r--r--   0 khhor    (638696329) domain_users (1388800513)       69 2020-03-06 03:52:01.000000 bohra-2.3.0/setup.py
```

### Comparing `bohra-2.2.1/LICENSE.txt` & `bohra-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/CustomLog.py` & `bohra-2.3.0/bohra/CustomLog.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/SnpDetection.py` & `bohra-2.3.0/bohra/SnpDetection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pathlib
-import os, getpass, shutil, re, psutil
+import os, getpass, shutil, re, psutil, string, random
 import pandas
-# from bohra.bohra import check_deps
+from collections import namedtuple
 # import sh
 import logging
 # import filecmp
 import datetime
 # import numpy
 # import itertools
 import subprocess
@@ -23,14 +23,30 @@
 fh = logging.FileHandler('bohra.log')
 fh.setLevel(logging.DEBUG)
 formatter = logging.Formatter('[%(levelname)s:%(asctime)s] %(message)s', datefmt='%m/%d/%Y %I:%M:%S %p') 
 fh.setFormatter(formatter)
 LOGGER.addHandler(ch) 
 LOGGER.addHandler(fh)
 
+class InitBohra(object):
+
+    def __init__(self):
+
+        self.script_path = f"{pathlib.Path(__file__).parent}"
+    
+    def init(self):
+
+        LOGGER.info(f"Will now try to install dependencies. Please be patient this may take some time!!... Maybe get coffee.")
+        process = subprocess.Popen(['bash', f"{self.script_path}/bohra_install.sh"], stdout=subprocess.PIPE, encoding='utf-8')
+        while process.poll() is None:
+            l = process.stdout.readline().strip() # This blocks until it receives a newline.
+            print(f"{l}")
+        
+
+
 class RunSnpDetection(object):
     '''
     A class for Bohra pipeline object
     '''
     
     def __init__(self, args):
         
@@ -52,25 +68,20 @@
         # path to pipeline resources
         self.pipeline = args.pipeline
         self.preview = True if self.pipeline == 'preview' else False
         LOGGER.info(f"You are running bohra in {self.pipeline} mode.")
         self.job_id =args.job_id
         LOGGER.info(f"Job ID is set {self.job_id}")
         # path to reference and mask
-        self.ref = pathlib.Path(args.reference)
+        self.ref = args.reference
         # LOGGER.info(f"The reference is {self.ref}")
         # self.link_file(self.ref)
         self.mask = args.mask
         # path to input file
-        if args.input_file == '':
-            LOGGER.critical('`read` file can not be empty, please set -r path_to_input to try again')
-            raise SystemExit()
-        else:
-            self.reads = pathlib.Path(args.input_file)
-        self.contigs = args.contigs
+        self.reads,self.contigs = self._check_input_files(_input = args.input_file, contigs = args.contigs, pipeline = self.pipeline)
 
         self.keep = True if args.keep == 'Y' else False
         # snippy args
         self.minmap = args.minmap
         self.mincov = args.mincov
         self.basequal = args.basequal
         self.minqual = args.minqual
@@ -81,20 +92,34 @@
         self.cpus = args.cpus
         self.config = args.config
         self.profile_config = os.getenv('BOHRA_PROFILES','')
         self.profile = self._get_profile() if args.profile == '' else args.profile
         self.run_kraken = 'false'
         self.no_phylo = args.no_phylo
         self.abritamr_args = args.abritamr_args
+        self.spades_args = args.spades_args
         self.proceed = args.proceed
         self.use_conda = True if args.no_conda == False else False
         self.conda_path = args.conda_path
         
         
-    
+    def _check_input_files(self, _input, contigs, pipeline):
+        
+        if _input == '':
+            LOGGER.critical(f"You must supply and input file. Please see help and try again.")
+            raise SystemExit
+
+        # if _input == '':
+        #     if pipeline in ['preview', 'snps','phylogeny','default','full']:
+        #         LOGGER.critical(f"You are trying to run the {pipeline} bohra pipeline - you must supply an input file with paths to reads.")
+        #         raise SystemExit
+        
+        return pathlib.Path(_input), contigs
+
+
     def _get_profile(self):
 
         # get hostname
         LOGGER.info(f"Tyring to find your profile.")
         profile = 'lcl'
         if self.profile_config != '' and self._path_exists(pathlib.Path(self.profile_config)):
             with open(self.profile_config, 'r') as j:
@@ -134,35 +159,30 @@
                 else:
                     LOGGER.warning(f"Profile : {self.profile} is not found in {config}. I hope you know what you are doing!")
                 return config
         else:
             LOGGER.critical(f"You have provided the path to an alternative config file, which does not exist. Please try again.")
             raise SystemExit
 
-    def _remove_core(self):
-        '''
-        Need to remove core_isolates.txt to get snakemake to redo snippy core step
-        '''
-        LOGGER.info(f"Removing previous snippy-core output.")
-        corefiles = sorted(pathlib.Path(self.workdir, self.job_id).glob('core*'))
-        if corefiles:
-            for core in corefiles:
-                core.unlink()
+    def _generate_random_string(self):
+
+        letters = string.ascii_lowercase
+        result_str = ''.join(random.choice(letters) for i in range(10))
+
+        return result_str
     
     def setup_for_rerun(self):
-        report_path_orig = self.workdir / self.job_id / 'report'
-        report_path_preview =  self.workdir / self.job_id / f'report_{self.day}'
-        if self.keep == 'Y' and report_path_orig.exists():
+        
+        report_path_orig = self.workdir / 'report'
+        report_path_preview =  self.workdir / f'report_archived_{self.day}_{self._generate_random_string()}'
+        if self.keep and report_path_orig.exists():
             cmd = f"mv {report_path_orig} {report_path_preview}"
             LOGGER.info(f"Archiving previous report directory...")
-            subprocess.run(cmd, shell = True, encoding = "utf-8", capture_output= True)
-        elif self.keep == 'N' and report_path_orig.exists():
-            cmd = f"rm {report_path_orig}"
-            LOGGER.info(f"Removing previous report files")
-            subprocess.run(cmd, shell = True, encoding = "utf-8", capture_output= True)
+            self._run_subprocess(cmd  = cmd)
+        
 
 
     def _path_exists(self,path, v = True):
         '''
         ensure files are present, if so continues if not quits with FileNotFoundError
         input:
             :path: patht to files for pipeline
@@ -193,24 +213,38 @@
             else:
                 return name
         else:
             LOGGER.warning('Job id ca not be empty, please set -j job_id to try again')
             raise SystemExit()
    
 
-    def _check_ref(self, ref):
-
-        LOGGER.info(f"Checking if reference is a valid reference file.")
-        p = subprocess.run(f"any2fasta {ref}", shell = True, capture_output = True, encoding = "utf-8")
-        if p.returncode == 0:
-            LOGGER.info(f"Reference is in a valid format.")
+    def _check_ref(self, ref, pipeline):
+        
+        if pipeline in ['snps','default','full','phylogeny']:
+            if self.ref == '':
+                LOGGER.critical(f"Reference file must be provided. Please try again.")
+                raise SystemExit
+            elif not self._path_exists(pathlib.Path(self.ref), v = True):
+                LOGGER.critical(f"A valid reference file must be provided. Please try again.")
+                raise SystemExit
+            
+            LOGGER.info(f"Reference {self.ref} has been found. Will now copy to running directory.")
+            reference = self._copy_files(_file = self.ref)
+            LOGGER.info(f"Checking if reference is a valid reference file.")
+            p = subprocess.run(f"any2fasta {ref}", shell = True, capture_output = True, encoding = "utf-8")
+            if p.returncode == 0:
+                LOGGER.info(f"Reference is in a valid format.")
+            
+            else:
+                LOGGER.critical(f"There is something wrong with your reference file. Valid file types are .fasta, .gbk, .fasta.gz, .gbk.gz. Please check your inputs and try again.")
+                raise SystemExit
+            return reference
         else:
-            LOGGER.critical(f"There is something wrong with your reference file. Valid file types are .fasta, .gbk, .fasta.gz, .gbk.gz. Please check your inputs and try again.")
-            raise SystemExit
-
+            return 'no_ref_req'
+        
     def _check_gzip(self,read):
         """
         ensure that gz file is true gz
         input:
             read: path to read file
         """
         LOGGER.info(f"Checking if file is valid gzip.")
@@ -366,15 +400,15 @@
             else:
                 LOGGER.critical(f"{sft} is not installed.")
                 raise SystemExit
         LOGGER.info(f"Now checking kraken2 DB")
         self._check_kraken2DB(checking = checking)
         software_versions.append(f"kraken2 DB: {self.kraken_db}")
         if not checking:
-            print(checking)
+            # print(checking)
             self._check_mlstdb()
             software_versions.append(f"mlst blast db: {self.blast_db}")
             software_versions.append(f"mlst data dir: {self.data_dir}")
         # write software_versions.tab
         
             LOGGER.info(f"Writing software_versions.txt")
             if not pathlib.Path('report').exists():
@@ -405,23 +439,25 @@
                 raise SystemExit
             return True
         else:
             True
    
     def _check_reads(self,reads):
 
-        if self._path_exists(reads):
+        if reads != '' and self._path_exists(reads):
             
             tab = pandas.read_csv(reads, sep = '\t', header = None)
             if self._check_shape(tab.shape[1]):
                 LOGGER.info(f"File {reads} is in correct format.")
             else:
                 LOGGER.critical(f"{reads} is not in the correct format. Please check your inputs and try again.")
                 raise SystemExit
             return tab
+        # elif self.pipeline in ['assemble','amr_typing']:
+        #     return pandas.DataFrame()
         else:
             LOGGER.critical(f"Something is wrong with {reads}. Please try again.")
             raise SystemExit
 
 
     def _check_contigs(self, contigs):
 
@@ -438,22 +474,26 @@
             return False
 
     def _check_phylo(self, isolates_list):
         LOGGER.info(f"Checking if phylo needs to be run.")
         LOGGER.info(f"Your analysis contains {len(isolates_list)}")
         if self.pipeline == 'preivew' and len(isolates_list) > 2:
             LOGGER.info(f"You are running in preview mode, a mash tree will be output")
-        if len(isolates_list) < 3 and self.pipeline in ['default', 'all']:
+        if self.pipeline in ['amr_typing', 'assemble']:
+            LOGGER.info(f"Your are running the {self.pipeline} bohra pipeline. No tree will be generated.")
+            self.no_phylo = True
+        elif len(isolates_list) < 3 and self.pipeline in ['phylogeny', 'default', 'all']:
             LOGGER.warning(f"You have less than 3 isolates in your dataset, no phylogenetic tree will be generated.")
             self.no_phylo = True
         elif not self.no_phylo:
             LOGGER.info(f"A phylogenetic tree will be generated.")
-        if self.pipeline == 'all' and len(isolates_list) < 4:
-            LOGGER.warning(f"You can not run roary with less the 4 isolates.")
+        elif self.pipeline == 'all' and len(isolates_list) < 4:
+            LOGGER.warning(f"You can not run panaroo with less than 4 isolates.")
             self.pipeline = 'default'
+        
         # if self.no_phylo:
         #     LOGGER.info(f"You have selected no_phylo option so no phylogenetic tree will be generated.")
         
     def _copy_files(self, _file):
 
         p = pathlib.Path(_file)
         name = p.name
@@ -462,44 +502,58 @@
         else:
             cmd = f"cp {p} {pathlib.Path(self.workdir, name)}"
             LOGGER.info(f"Running : {cmd}")
             subprocess.run(cmd, shell = True)
 
         return f"{name}"
     
-    def _link_reads(self, iso_dir,read, target):
+    def _link_input_files(self, iso_dir,read, target):
 
         if read.exists() and not pathlib.Path(f"{iso_dir}/{target}").exists():
                     subprocess.run(f"ln -sf {read} {iso_dir}/{target}", shell = True)
         elif not read.exists():
             LOGGER.critical(f"{read} is not a valid path. All read files must be valid path. Please try again.")
             raise SystemExit
         
     def _setup_directory(self, reads):
         
         isolates_list = []
-        # if not pathlib.Path(self.job_id).exists():
-        #     LOGGER.info(f"Creating job directory")
-        #     subprocess.run(f"mkdir {self.workdir}", shell = True)
-        LOGGER.info(f"Setting up isolate directories.")
-        for row in reads.iterrows():
-            if not row[1][0].startswith('#'):
-                isolates_list.append(row[1][0])
-                iso_dir = self.workdir/ f"{row[1][0]}" 
-                if not iso_dir.exists():
-                    subprocess.run(f"mkdir {iso_dir}", shell = True)
-                # for r in [row[1][1],row[1][2]]:
-                read1 = pathlib.Path(row[1][1])
-                read2 =pathlib.Path(row[1][2])
-                target1 = 'R1.fastq.gz'
-                target2 = 'R2.fastq.gz'
-                self._link_reads(iso_dir = iso_dir, read = read1, target = target1)
-                self._link_reads(iso_dir = iso_dir, read = read2, target = target2)
-                
+        if not reads.empty:
+            LOGGER.info(f"Setting up isolate directories.")
+            for row in reads.iterrows():
+                if not row[1][0].startswith('#'):
+                    isolates_list.append(row[1][0])
+                    iso_dir = self.workdir/ f"{row[1][0]}" 
+                    if not iso_dir.exists():
+                        subprocess.run(f"mkdir {iso_dir}", shell = True)
+                    # for r in [row[1][1],row[1][2]]:
+                    read1 = pathlib.Path(row[1][1])
+                    read2 =pathlib.Path(row[1][2])
+                    target1 = 'R1.fastq.gz'
+                    target2 = 'R2.fastq.gz'
+                    self._link_input_files(iso_dir = iso_dir, read = read1, target = target1)
+                    self._link_input_files(iso_dir = iso_dir, read = read2, target = target2)       
+            # self._check_phylo(isolates_list = isolates_list)
+        
+        elif self.contigs != '' and pathlib.Path(self.contigs).exists():
+            tab = pandas.read_csv(self.contigs, sep = '\t', header = None, names = ['Isolate','Path'])
+            for row in tab.iterrows():
+                if not row[1][0].startswith('#'):
+                    isolates_list.append(row[1][0])
+                    iso_dir = self.workdir/ f"{row[1][0]}" 
+                    if not iso_dir.exists():
+                        subprocess.run(f"mkdir {iso_dir}", shell = True)
+                    # for r in [row[1][1],row[1][2]]:
+                    contig = pathlib.Path(row[1][1])
+                    target = 'contigs.fa'
+                    self._link_input_files(iso_dir = iso_dir, read = contig, target = target)
         
+        else:
+            LOGGER.critical(f"There seems to be a problem with your input files... not isolates can be extracted. Please check you inputs and try again.")
+            raise SystemExit
         self._check_phylo(isolates_list = isolates_list)
         LOGGER.info(f"Updating isolate list.")
         pathlib.Path(f"isolates.list").write_text('\n'.join(isolates_list))
         return f"isolates.list"
         
     def _check_snippy_defaults(self, snippy_arg, val):
         
@@ -530,86 +584,92 @@
         snippy_opts = []
 
         for d in _dict:
             if self._check_snippy_defaults(snippy_arg=d, val = _dict[d]):
                 snippy_opts.append(f"--{d} {_dict[d]}")
         
         return ' '.join(snippy_opts)
-        
+    
+    def _generate_spades_args(self):
+
+        if self.assembler == 'spades':
+            return f"--spades_opt '{self.spades_args}'"
+        else:
+            return ''
+
     def _generate_cmd(self, mode, run_kraken, kraken2_db,assembler, mask_string, reference, 
                         isolates, user, day, contigs, run_iqtree, species, cpus, config, profile, gubbins,blast_db,data_dir, job_id):
         
         stub = f"nextflow -Dnxf.pool.type=sync run {self.script_path}/main.nf"
         resume = '' if self.force else "-resume"
         cpu = f'-executor.cpus={int(cpus)}' if cpus != '' else ''
         config = f'-c {config}' if config != '' else ''
-        conda = '--enable_conda' if self.use_conda else ''
+        conda = '--enable_conda true' if self.use_conda else ''
+        conda_path = f"--conda_path {self.conda_path}" if self.conda_path != '' else ''
         snippy_opts = self._generate_snippy_params()
-        parameters = f"--job_id {job_id} --mode {mode} --run_iqtree {run_iqtree} --run_kraken {run_kraken} --kraken2_db {kraken2_db} --assembler {assembler} --mask_string {mask_string} --reference {reference} --contigs_file {contigs} --species {species if species != '' else 'no_species'} --outdir {self.workdir} --isolates {isolates} --user {user} --day {day} --gubbins {gubbins} --blast_db {blast_db} --data_dir {data_dir} {conda} {snippy_opts}"
+        spades_opts = self._generate_spades_args()
+        parameters = f"--job_id {job_id} --mode {mode} --run_iqtree {run_iqtree} --run_kraken {run_kraken} --kraken2_db {kraken2_db} --assembler {assembler} --mask_string {mask_string} --reference {reference} --contigs_file {contigs} --species {species if species != '' else 'no_species'} --outdir {self.workdir} --isolates {isolates} --user {user} --day {day} --gubbins {gubbins} --blast_db {blast_db} --data_dir {data_dir} {conda} {conda_path} {snippy_opts} {spades_opts}"
         options = f"-with-report bohra_{day}_report.html -with-trace -profile {profile} {resume} {cpu} {config} {'-with-conda' if self.use_conda else ''}"
 
         cmd = f"{stub} {parameters} {options}"
         return cmd
         
-        
+    def _run_subprocess(self, cmd):
+
+        LOGGER.info(f"Running:\n\033[1m{cmd}\033[0m")
+        p = subprocess.run(cmd, shell = True)
+        return p
+    
     def _run_cmd(self, cmd):
         
         if self.proceed:
-            LOGGER.info(f"Running:\n\033[1m{cmd}\033[0m")
-            p = subprocess.run(cmd, shell = True)
-            return p
+            return self._run_subprocess(cmd= cmd)
+        
         else:
 
             try:
                 LOGGER.info(f"Please paste the following command to run the pipeline:\n\033[1m{cmd}\033[0m")
             except NameError:
                 LOGGER.critical(f"It seems something has gone wrong with your inputs. \
 Please select a mode to run, choices are 'analysis' or 'finish'")
                 raise SystemExit
 
 
     def run_pipeline(self):
         '''
         run pipeline, if workflow runs to completion print out a thank you message.
         '''
+        self.setup_for_rerun()
         # run checks for inputs
         if self.use_conda == False:
             LOGGER.warning(f"You are using a pre-configured conda environment - please note the results may be unexpected.")
             self.check_dependencies(checking=False)
         else:
             LOGGER.info(f"You are running with conda - wise decision!! Will now ensure that kraken DB is configured properly.")
             self._check_kraken2DB(checking = False)
             LOGGER.info(f"Now looking for MLST setup")
             self._check_mlstdb()
         # input files
         reads = self._check_reads(reads = self.reads)
         contigs = self._check_contigs(contigs = self.contigs)
         
         # reference
-        if self.ref == '':
-            LOGGER.critical(f"Reference file must be provided. Please try again.")
-            raise SystemExit
-        elif not self._path_exists(self.ref, v = True):
-            LOGGER.critical(f"A valid reference file must be provided. Please try again.")
-            raise SystemExit
-        else:
-            LOGGER.info(f"Reference {self.ref} has been found. Will now copy to running directory.")
-            reference = self._copy_files(_file = self.ref)
-            self._check_ref(ref = reference)
+        
+        reference = self._check_ref(ref = self.ref,pipeline=self.pipeline)
         # mask
         if self.mask != '' and not self._path_exists(pathlib.Path(self.mask)):
             LOGGER.critical(f"{self.mask} is not a valid path please try again.")
             raise SystemExit
         elif self.mask != '' and  self._path_exists(pathlib.Path(self.mask, v = False)):
             self.mask = self._copy_files(_file = self.mask)
             LOGGER.info(f"Mask file {self.mask} has been provided.")
         else:
             LOGGER.info(f"No mask file has been provided.")
 
-        isolates_list = self._setup_directory(reads = reads)
+        isolates_list = self._setup_directory(reads = reads) 
 
         if contigs:
             contigs_file = self.contigs
         else:
             contigs_file = 'no_contigs'
             
         run_iqtree = 'false' if self.no_phylo else 'true'
@@ -625,29 +685,16 @@
         cmd = self._generate_cmd(mode = self.pipeline, run_kraken = self.run_kraken, kraken2_db = self.kraken_db,
                         contigs = contigs_file, cpus = cpus, config = config, assembler = self.assembler, 
                         mask_string = mask_string, reference = reference, run_iqtree = run_iqtree,profile = self.profile,
                         isolates = isolates_list, day = self.day, user = self.user, 
                         species = self.abritamr_args, gubbins = self.gubbins, blast_db = self.blast_db if self.blast_db != '' else 'no_db', data_dir = self.data_dir if self.data_dir != '' else 'no_db', job_id = self.job_id)
         self._run_cmd(cmd)
 
-# class CheckBohra(RunSnpDetection):
 
-#     def __init__(self):
-        
-#         # user
-#         self.user = getpass.getuser()
-#         # get date and time
-#         self.now = datetime.datetime.today().strftime("%d_%m_%y_%H")
-#         self.day = datetime.datetime.today().strftime('%Y-%m-%d')
-#         self.script_path = f"{pathlib.Path(__file__).parent}"
-#         self.check = True
-#         self.check_dependencies(checking = self.check)
-
-
-class SetupInputFiles():
+class SetupInputFiles(RunSnpDetection):
 
     def __init__(self, args):
 
         self.read_path = args.read_path
         self.isolate_list = args.isolate_list
         self.now = datetime.datetime.today().strftime("%d_%m_%y_%H")
         self.day = datetime.datetime.today().strftime('%Y-%m-%d')
@@ -662,14 +709,15 @@
         LOGGER.info(f"Checking for {path}")
         if pathlib.Path(path).exists():
             LOGGER.info(f"{path} exists.")
             return True
         else:
             LOGGER.critical(f"Path provided : {path} does not exist - please try again.")
             return False
+        
     def _extract_isolates(self, isolate_file):
         
         with open(isolate_file, 'r') as f:
             isolates = f.read().strip().split('\n')
         
         return isolates
     
@@ -749,11 +797,76 @@
             else:
                 isolates = []
             self._glob_data(path = self.read_path, isolates= isolates)
         else:
             LOGGER.critical(f"There seems to be a problem with your read path. Please provide a valid path to the reads you wish to include")
             raise SystemExit
 
+class TestBohra(SetupInputFiles):
+
+    def __init__(self,args):
 
+        self.isolate_list = ['ERR1102348','ERR1102353','ERR1102355','ERR1102356']
+        self.download_stub = "https://raw.githubusercontent.com/MDU-PHL/bohra/master/data"
+        self.reference = self._check_reference_test(args.reference)
+        self.read_path = f"{pathlib.Path.cwd() / 'test_data'}"
+
+    def _download_reads_from_github(self):
+
+        for isolate in self.isolate_list:
+            
+            for r in [1,2]:
+                cmd = f"mkdir -p test_data/{isolate} && wget -O test_data/{isolate}/{isolate}_{r}.fastq.gz {self.download_stub}/{isolate}/{isolate}_{r}.fastq.gz"
+                self._run_subprocess(cmd = cmd)
+            
+
+    def _download_reference_from_github(self):
+
+        cmd = f"wget -O Lm_Cluster1_J1-108.fa {self.download_stub}/Lm_Cluster1_J1-108.fa"
+        self._run_subprocess(cmd = cmd)
+        return 'Lm_Cluster1_J1-108.fa'
+    
+    def _check_reference_test(self, path):
+
+        if not pathlib.Path(path).exists():
+
+            return self._download_reference_from_github()
+
+        else:
+            return path
+
+    def _check_test_data(self,path):
+
+        for i in self.isolate_list:
+            reads = sorted(pathlib.Path(path).glob(f"{i}/{i}*.f*q.gz"))
+            if len(reads) != 2:
+                LOGGER.warning(f"Reads for {i} are not found. Will try to get them for you!")
+                return False
+        LOGGER.info(f"All reads are found at {path}")
+        return True
     
+    def _make_test_input(self, path):
 
+        LOGGER.info(f"Now generating input file for bohra.")
+        self._glob_data(path = path)
+
+    def run_tests(self):
+        
+        LOGGER.info(f"Checking availability of data.")
+        if not pathlib.Path(self.read_path).exists():
+            LOGGER.info(f"Will now download some reads for testing - this may take a little while - it might be coffee time.")
+            self._download_reads_from_github()
+        elif self._check_test_data(path = self.read_path):
+            self._make_test_input(path = self.read_path)
+        else:
+            LOGGER.info(f"Will now download some reads for testing - this may take a little while - it might be coffee time.")
+            self._download_reads_from_github()
+            self._make_test_input(path = self.read_path)
+            
+        cmd = f"bohra run -i isolates.tab -r {self.reference} -p full --proceed"
+        proc = self._run_subprocess(cmd=cmd)
+
+        if proc.returncode == 0:
+            LOGGER.info(f"bohra test has completed successfully!!")
+        else:
+            LOGGER.critical(f"bohra run was not successful... please raise an issue on github.")
```

### Comparing `bohra-2.2.1/bohra/Utils.py` & `bohra-2.3.0/bohra/Utils.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/bohra.py` & `bohra-2.3.0/bohra/bohra.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 The pipline is based on nullarbor (https://github.com/tseemann/nullarbor) and is designed to be run in high performance computing environment.
 
 Bohra is modular allowing the user to choose between calling SNPs and generating a phylogenetic tree, perform assemblies and detect AMR, perform typing etc; Or use the full pipeline to call SNPs, generate phylogenies, assemble, type and detect the pan-geneome. The output of Bohra is a html report that can be distributed, with downloadable tables and data.
 """
 
 
-import logging
+# import logging
 import argparse
 import pathlib
 import sys
 import os
 import shutil
-from bohra.SnpDetection import RunSnpDetection, SetupInputFiles
+from bohra.SnpDetection import RunSnpDetection, SetupInputFiles, InitBohra, TestBohra
 from bohra.version import version
 
 
 def run_pipeline(args):
     '''
     Run the pipeline for the first time
     '''
@@ -31,98 +31,99 @@
 
 def find_reads(args):
 
     S = SetupInputFiles(args)
     S.find_reads()
 
 def init_bohra():
-    pass
+    
+    I = InitBohra()
+    I.init()
+
+def test_bohra(args):
+    
+    S = TestBohra(args)
+    S.run_tests()
+    # run_pipeline(inputs)
 
 def main():
     # setup the parser
   
     parser = argparse.ArgumentParser(description=f'Bohra - a bacterial genomics pipeline - version {version}',formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('-v', '--version', action='version', version='%(prog)s ' + version)
     # options for running
-
     subparsers = parser.add_subparsers(help="Task to perform")
     # run bohra pipeline
     parser_run = subparsers.add_parser('run', help='Run bohra', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
     parser_run.add_argument('--check',action="store_true", help = "Check that dependencies are installed correctly.")
     parser_run.add_argument('--input_file','-i',help='Path to reads file, which is a tab-delimited with 3 columns <isolatename>  <path_to_read1> <path_to_read2>. REQUIRED', default='')
     parser_run.add_argument('--contigs','-c',help='Path to contigs file, which is a tab-delimited with 3 columns <isolatename>  <path_to_contigs>. OPTIONAL if you already have assemblies.', default='')
     parser_run.add_argument('--job_id','-j',help='Job ID is the name that will be displayed on your report', default='Bohra microbial genomics pipeline')
     parser_run.add_argument('--reference','-r',help='Path to reference (.gbk or .fa)', default = '')
     parser_run.add_argument('--mask','-m',default = '', help='Path to mask file if used (.bed)')
     parser_run.add_argument("--abritamr_args",default="",help="Set if you would like to use point mutations, please provide a valid species.", choices= ['Neisseria', 'Acinetobacter_baumannii', "Campylobacter", "Enterococcus_faecalis", "Enterococcus_faecium", "Escherichia", "Klebsiella", "Salmonella", "Staphylococcus_aureus", "Staphylococcus_pseudintermedius", "Streptococcus_agalactiae", "Streptococcus_pneumoniae", "Streptococcus_pyogenes", "Vibrio_cholerae"])
     parser_run.add_argument('--kraken_db', '-k', default="KRAKEN2_DEFAULT_DB", help="Path to DB for use with kraken2, if no DB present speciation will not be performed.")
-    parser_run.add_argument('--pipeline','-p', default = 'preview', choices=['preview','default','pluspan'], help=f"The pipeline to run. `preview` - generates a rapid tree using mash distances | `default` - runs snippy, phylogenetic tree (if > 3 sequences), assemblies, mlst and amr gene detection | `all` - same as default but includes roary pangenome analysis")
-    parser_run.add_argument('--assembler','-a', default = 'shovill', choices=['shovill','skesa','spades'], help=f"Assembler to use.")
+    parser_run.add_argument('--pipeline','-p', default = 'preview', choices=['preview','default','full','snps','phylogeny','assemble','amr_typing'], help=f"The pipeline to run. `preview` - generates a rapid tree using mash distances | `default` - runs snippy, phylogenetic tree (if > 3 sequences), assemblies, mlst and amr gene detection | `all` - same as default but includes roary pangenome analysis")
+    parser_run.add_argument('--assembler','-a', default = 'shovill', choices=['shovill','skesa','spades'], help=f"Assembler to use (shovill uses spades > 3.14 with --isolate mode).")
+    parser_run.add_argument('--spades_args', default = "", help="Use to add arguments to spades (when running with --assembler spades) for example: '--cov-cutoff auto' ")
     parser_run.add_argument('--cpus',help='Number of max CPU cores to run, will define how many rules are run at a time, if 0 then the avail cpus will be determined at time of launch', default=0) # need to change
     parser_run.add_argument('--minmap','-mp',help='Snippy - minimum read mapping quality to consider.', default='60')
     parser_run.add_argument('--basequal','-bq',help='Snippy - Minimum base quality to consider.', default='13')
     parser_run.add_argument('--minqual','-mq',help='Snippy - minumum QUALITY in VCF column 6', default='100')
     parser_run.add_argument('--minfrac','-mf',help='Snippy - minumum proportion for variant evidence ', default='0')
     parser_run.add_argument('--mincov','-mc',help='Snippy - minimum site depth to for calling alleles.', default='10')
     parser_run.add_argument('--workdir','-w', default = f"{pathlib.Path.cwd().absolute()}", help='The directory where Bohra will be run, default is current directory') # don't need this
     parser_run.add_argument('--force','-f', action="store_true", help = "Add if you would like to force a complete restart of the pipeline. All previous logs will be lost.")
     parser_run.add_argument('--no_phylo',action="store_true", help = "Set if you do NOT want to generate a phylogentic tree.")
     parser_run.add_argument('--config', default = f"", help='An additional config file, required if running on a non-local machine, ie slurm, cloud. For help see documentation at https://github.com/MDU-PHL/bohra or https://www.nextflow.io/docs/latest/executor.html') # don't need this
     parser_run.add_argument('--profile', default = f"", help='The resource profile to use. Defaults to local, if using an alternative config file, this calue should represent the name of a profile provided') 
-    parser_run.add_argument('--conda_path', default = f"", help='The path to where your pre-installed conda envs are stored, defaults to installing conda envs in your work directory. This can be provided in your profiles settings as well - it assumes you have pre-configured all of your conda environments for each process run by bohra, this is an advanced setting. Please take care.') 
+    parser_run.add_argument('--conda_path', default = f"{pathlib.Path(os.getenv('CONDA_PREFIX')).parent}", help='The path to where your pre-installed conda envs are stored, defaults to installing conda envs in your work directory. This can be provided in your profiles settings as well - it assumes you have pre-configured all of your conda environments for each process run by bohra, this is an advanced setting. Please take care.') 
     parser_run.add_argument('--blast_db', default = f"{os.getenv('BLAST_DB', '')}", help='Path to the mlst blast_db, defaults to what is installed in the environment.') 
     parser_run.add_argument('--data_dir', default = f"{os.getenv('PUBMLST_DB','')}", help='Path to the mlst datadir, defaults to what is installed in the environment.') 
     parser_run.add_argument('--mlst_exclude',default = f"", help='Space delimited list of mlst schemes to exclude.', nargs='+')
     parser_run.add_argument('--proceed', action="store_true", help = "If you would like to proceed straigt to the pipeline.")
     parser_run.add_argument('--gubbins',  action = 'store_true', help = 'Set to use gubbins for recombination correction.')
     parser_run.add_argument('--keep', default = 'N', choices= ['Y', 'N'], help = 'If you are rerunning bohra over an exisiting directory set --keep to \'Y\' to archive report files - otherwise previous reprot files will be removed.')
     parser_run.add_argument('--no-conda',action="store_true", help="Set if you DO NOT WANT to use separate conda environments for each nextflow process.")
 
-    # parser_check = subparsers.add_parser('check', help='Check bohra installation', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-
     parser_setup = subparsers.add_parser('generate_input', help='Generate input files for bohra', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser_setup.add_argument(
         '--read_path',
         '-r',
         default='',
         help = 'Path to look for read files')
     parser_setup.add_argument(
         '--isolate_list',
         '-i',
         default= '',
         help = 'List of isolates (one isolate name per line) to include in input file. If not provided all sequences in found will be included.'
     )
 
-        
+    parser_init = subparsers.add_parser('init', help='Setup bohra dependencies', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser_check = subparsers.add_parser('check', help='Check for bohra dependencies', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+
+    parser_test = subparsers.add_parser('test', help='Test bohra', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser_test.add_argument(
+        '--reference',
+        '-r',help='Reference to be used in test.', 
+        default='Lm_Cluster1_J1-108.fa'
+    )
+    
     parser_run.set_defaults(func=run_pipeline)
     parser_setup.set_defaults(func=find_reads)
+    parser_test.set_defaults(func=test_bohra)
+    
 
         
     args = parser.parse_args()
-    
-    if len(sys.argv) <= 2 and sys.argv[1] != 'check':
+    print(len(sys.argv))
+    if len(sys.argv) < 2:
         parser.print_help(sys.stderr)
-    # elif sys.argv[1] == 'check':
-    #     check_deps()
+    elif sys.argv[1] in ['init', 'check']:
+        init_bohra()
     else:
-        # logger = logging.getLogger(__name__)
-        # logger.setLevel(logging.INFO)
-        # # create file handler which logs even debug messages
-        # fh = logging.FileHandler('bohra.log')
-        # fh.setLevel(logging.INFO)
-        # # create console handler with a higher log level
-        # ch = logging.StreamHandler()
-        # ch.setLevel(logging.INFO)
-        # # create formatter and add it to the handlers
-        # formatter = logging.Formatter('[%(levelname)s:%(asctime)s] %(message)s', datefmt='%m/%d/%Y %I:%M:%S %p')
-        # fh.setFormatter(formatter)
-        # ch.setFormatter(formatter)
-        # # add the handlers to the logger
-        # logger.addHandler(ch)
-        # logger.addHandler(fh)
-        # logger.info(f"Starting bohra pipeline using {' '.join(sys.argv)}")
         args.func(args)
 	
 if __name__ == '__main__':
     main()
```

### Comparing `bohra-2.2.1/bohra/modules/collation/bin/add_header_mlst.py` & `bohra-2.3.0/bohra/modules/collation/bin/add_header_mlst.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/collation/bin/collate_asm.py` & `bohra-2.3.0/bohra/modules/collation/bin/collate_asm.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 import pandas, pathlib
 
 HEADER = [f"Isolate\tbp\t# Contigs\t# Gaps\tMin Contig size\tMax Contig size\tAvg Contig size\tN50\tCDS\trRNA"]
 
 def combine(prokka, asm, isolate, output):
 
     gff = pandas.read_csv(prokka, sep = ':', header = None, names = ['cond', isolate])
-    print(gff)
+    # print(gff)
     df = pandas.read_csv(asm, sep = '\t')
     gff = gff[gff['cond'].isin(['CDS', 'rRNA'])]
-    print(gff)
+    # print(gff)
     rrna = gff[gff['cond'] == 'rRNA'][isolate].values[0].replace("\"","").strip() if not gff[gff['cond'] == 'rRNA'].empty else ''
     cds = gff[gff['cond'] == 'CDS'][isolate].values[0].replace("\"","").strip()
-    print(rrna)
-    print(cds)
-    print(df)
+    # print(rrna)
+    # print(cds)
+    # print(df)
     bp = df['sum_len'].values[0]
     contigs = df['num_seqs'].values[0]
     mincontigs = df['min_len'].values[0]
     avgcontigs = df['avg_len'].values[0]
     maxcontigs = df['max_len'].values[0]
     gaps= df['sum_gap'].values[0]
     n50 = df['N50'].values[0]
 
     result = f"{isolate}\t{bp}\t{contigs}\t{gaps}\t{mincontigs}\t{avgcontigs}\t{maxcontigs}\t{n50}\t{cds}\t{rrna}"
-    print(result)
+    # print(result)
     HEADER.append(result)
     out = pathlib.Path(output)
     out.write_text('\n'.join(HEADER))
 
 def main(isolate,asm,prokka, output):
     combine(prokka=prokka, asm = asm, isolate=isolate, output = output)
```

### Comparing `bohra-2.2.1/bohra/modules/collation/bin/collate_kraken2.py` & `bohra-2.3.0/bohra/modules/collation/bin/collate_kraken2.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/collation/bin/collate_stats.py` & `bohra-2.3.0/bohra/modules/collation/bin/collate_stats.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 #!/usr/bin/env python3
 import sys, json, datetime, subprocess, pathlib,pandas
 
-# Isolate\tMatch 1\t%\tMatch 2\t%\tMatch 3\t%
-
-STATS_TEXT = ["Isolate\tReads\tYield\tGC content\tMin len\tAvg len\tMax len\tAvg qual\tEstimated average depth\tQuality (>Q30)"]
-
 
 def get_vals_seqtk(f):
 
     with open(f, 'r') as inputfile:
         lines = inputfile.read().split('\n')
         qscore = lines[1].split('\t')[3]
         bases = lines[1].split('\t')[0]
@@ -26,49 +22,40 @@
     reads = sum_stats(f, 'sum', 4)
     minval = sum_stats(f, 'mean', 6)
     avgval = sum_stats(f, 'mean', 7)
     maxval = sum_stats(f, 'mean', 8)
 
     return int(reads.strip()), float(minval.strip()), float(avgval.strip()), float(maxval.strip())
 
-def get_length(ref):
+def get_length(genome_size):
 
-    p = subprocess.run(f"any2fasta {ref} | seqkit stats -a -T | cut -f5 | sed 1d", shell = True, capture_output = True, encoding = "utf-8")
-    length = int(p.stdout.strip())
-    print(p)
-    return length
-
-def get_dpth(ref,bases):
-    length = get_length(ref)
+    with open(genome_size, 'r') as f:
+        x = f.read().strip().split('\n')[0].strip()
+        try:
+            return int(x)
+        except:
+            print(f"Something has gone horribly wrong {x} can not be parsed to an int!!")
+            raise SystemExit
+    
+def get_dpth(genome_size,bases):
+    length = get_length(genome_size)
     dpth = int(bases)/length
     
     return round(dpth, 1)
 
-def get_qual(min_qscore, min_dpth, qscore, dpth):
-
-    if dpth > min_dpth and qscore > min_qscore:
-        return 'PASS'
-    else:
-        return 'FAIL'
-
-# STATS_TEXT = ["Isolate\tReads\tYield\tGC content\tMin len\tAvg len\tMax len\tAvg qual\tEstimated average depth\tQuality (>Q30)"]
 gcs = pandas.read_csv(sys.argv[3], sep = '\t')
 tab = pandas.read_csv(sys.argv[2], sep = '\t')
 tab['Isolate'] = sys.argv[1]
-print(tab)
-print(gcs)
-# file   format   type   num_seqs   sum_len     min_len   avg_len   max_len   Q1      Q2      Q3      sum_gap   N50   Q20(%)   Q30(%)
 tab = tab.rename(columns = {'num_seqs': 'Reads', 'sum_len': 'Yield','min_len':'Min len','max_len':'Max len', 'avg_len':'Avg len', 'Q30(%)': 'Average quality (% >Q30)'})
-tab['Estimated average depth'] = get_dpth(ref = sys.argv[4], bases = tab['Yield'].values[0])
+tab['Estimated average depth'] = get_dpth(genome_size = sys.argv[4], bases = tab['Yield'].values[0])
 tab['GC content'] = gcs[gcs.columns[0]].values[0]
 tab['Avgerage quality'] = gcs[gcs.columns[1]].values[0]
 tab = tab[['Isolate','Reads','Yield','GC content','Min len','Avg len','Max len','Average quality (% >Q30)','Estimated average depth']]
 tab.to_csv('read_assessment.txt', sep = '\t', index = False)
-# 
-# print(ROW)
+
```

### Comparing `bohra-2.2.1/bohra/modules/collation/bin/compile.py` & `bohra-2.3.0/bohra/modules/collation/bin/compile.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     '''
     tree_file = pathlib.Path(wd, 'report','preview.newick') if pipeline == 'preview' else pathlib.Path(wd, 'report','core.newick')
     if tree_file.exists() and phylo == 'true':
         with open(f"{tree_file}", 'r') as t:
             tree = t.read().strip()
     else:
         tree = 'No tree available'
-    print(tree)
+    # print(tree)
     return tree
 
 
 def _get_offset(reference):
     # print(reference)
     d = {}
     offset = 0
@@ -125,34 +125,14 @@
         col1 = df.columns[0]
         
         # if the there is no snp in the isolate (ie same as ref then mak na - then easy to drop)
         
         # collect positions to get allow for histogram and dropna (no snp)
         melted_df = pandas.melt(df, id_vars=[col1], value_vars=names)
         melted_df = melted_df[melted_df[col1]!= melted_df['variable']]
-        # brush = alt.selection_interval(encodings=['x'])
-        # base = alt.Chart(melted_df).mark_bar().encode(
-        #                         y='count():Q'
-        #                     ).properties(
-        #                         width=1200,
-        #                         height=100
-        #                     )
-        # chart = alt.vconcat(
-        #             base.encode(
-        #                 alt.X('value:Q',
-        #                 bin=alt.Bin(maxbins=30, extent=brush),
-        #                 scale=alt.Scale(domain=brush)
-        #                 )
-        #             ),
-        #             base.encode(
-        #                 alt.X('value:Q', bin=alt.Bin(maxbins=30)),
-        #             ).add_selection(brush)
-        #             )
-        
-        # chart = chart.to_json()
         chart = alt.Chart(melted_df).mark_bar().encode(
                             alt.X('value', axis = alt.Axis(title = 'Pairwise SNP distance')),
                             y=alt.Y('count()', axis= alt.Axis(title = "Frequency"))
                         ).properties(
                                 width=1200,
                                 height=200
                             )
@@ -238,15 +218,15 @@
     
     elif 'snp-distances' in d['link']:
         _c = [{'title':'Isolate','field':'Isolate',"headerFilter":"input","headerFilterPlaceholder":"Search isolate"}]
         _cls = sorted([c for c in cols if c not in ['Isolate']])
         for i in _cls:
             _c.append({'title':f"{i}",'field':f"{i}", "headerVertical":"true", "vertAlign":"bottom"})
         columns[d['link']] = _c
-    
+
     else:
         _c = [{'title':'Isolate','field':'Isolate',"headerFilter":"input","headerFilterPlaceholder":"Search isolate"}]
         _cls = sorted([c for c in cols if c not in ['Isolate']])
         for i in _cls:
             _c.append({'title':f"{i}",'field':f"{i}","headerFilter":"input","headerFilterPlaceholder":f"Search {i}"})
         columns[d['link']] = _c
     
@@ -266,14 +246,16 @@
     columns = {}
     comment = {}
     
     for d in _data:
         # print(d)
         if d['link'] == 'pan-genome':
             id_col = 'Genes'
+        elif d['link'] == 'software-versions':
+            id_col = 'tool'
         elif d['type'] == 'table' or d['type'] == 'matrix':
             id_col = 'Isolate'
         else:
             id_col = ''
         # print(id_col)
         tables,columns,comment = _generate_table(d = d, wd = wd, iso_dict= iso_dict, columns= columns,tables=tables,comment=comment,id_col=id_col)
     
@@ -288,15 +270,15 @@
     _dict = json.load(open(f"{pathlib.Path(args.template_dir, 'report_analysis.json')}", 'r'))
     # print(_dict[args.pipeline])
     # for d in _dict[args.pipeline]:
         # print(d)
     
     isos = _get_isos(wd = args.launchdir, iso_list=args.isolates)
     # print(isos)
-    reporthtml = pathlib.Path('report.html')
+    reporthtml = pathlib.Path(f'report_{args.pipeline}.html')
     # # path to html template
     indexhtml = pathlib.Path(args.template_dir,'index.html') 
     tables,columns,comment = _get_tables(_data = _dict[args.pipeline], wd = args.launchdir, isos = isos)
     version_head,version_body = _get_versions(wd = args.launchdir)
     data = {
         'newick' :'',
         'job_id':args.job_id[0],
@@ -304,19 +286,19 @@
         'date':args.day,
         'user':args.user,
         'tables':tables,
         'columns': columns,
         'comment':comment,
         'phylo': 'phylo' if args.iqtree == 'true' else 'no_phylo',
         'num_isos':len(isos),
-        'version_head': version_head,
-        'version_body':version_body,
-        'snp_distances': _plot_distances(wd = args.launchdir),
-        'snp_density': _plot_snpdensity(reference=args.reference, wd = args.launchdir, isos = isos),
-        'pan_svg': _get_pan_genome(d = _dict[args.pipeline], wd = args.launchdir) if args.pipeline == 'pluspan' else ''
+        # 'version_head': version_head,
+        # 'version_body':version_body,
+        'snp_distances': _plot_distances(wd = args.launchdir) if args.pipeline not in ['preview', 'assemble','amr_typing'] else {0:0},
+        'snp_density': _plot_snpdensity(reference=args.reference, wd = args.launchdir, isos = isos) if args.pipeline not in ['preview', 'assemble','amr_typing'] else {0:0},
+        'pan_svg': _get_pan_genome(d = _dict[args.pipeline], wd = args.launchdir) if args.pipeline == 'full' else ''
         }
     
     data['newick'] = _get_tree_string(pipeline = args.pipeline, wd = args.launchdir, phylo = args.iqtree)
     
     print("rendering html")
     report_template = jinja2.Template(pathlib.Path(indexhtml).read_text())
     reporthtml.write_text(report_template.render(data))
```

### Comparing `bohra-2.2.1/bohra/modules/collation/bin/snippy_qc.py` & `bohra-2.3.0/bohra/modules/collation/bin/snippy_qc.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/collation/bin/wrangle_mobsuite.py` & `bohra-2.3.0/bohra/modules/collation/bin/wrangle_mobsuite.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/collation/functions.nf` & `bohra-2.3.0/bohra/modules/collation/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/collation/main.nf` & `bohra-2.3.0/bohra/modules/collation/main.nf`

 * *Files 2% similar despite different names*

```diff
@@ -42,23 +42,23 @@
         } else {
             conda 'csvtk seqkit=2.1.0 pandas numpy=1.23.1 any2fasta'
         }
     } else {
         conda null
     }
     input:
-    tuple val(meta), path(seqkit_stats), path(seqkit_qual), path(reference)
+    tuple val(meta), path(seqkit_stats), path(seqkit_qual), path(genome_size)
 
     output:
     tuple val(meta), path ("read_assessment.txt"), emit: read_assessment
     
     script:
     """
     ${module_dir}/collate_stats.py $meta.id $seqkit_stats  \
-    $seqkit_qual $launchDir/$params.reference read_assessment.txt
+    $seqkit_qual $genome_size read_assessment.txt
     """
     
 }
 
 
 process SNIPPY_QC {
     tag "$meta.id"
@@ -183,15 +183,15 @@
 
     output:
     path "plasmid.txt", emit: collated_plasmid
     
     script:
     def plasmids = input.join(' ')
     """
-    $module_dir/collate_plasmids.py $output_name $plasmids
+    $module_dir/collate_tables.py $output_name $plasmids
     """
 
 }
 
 process COLLATE_SNIPPY_QCS {
     label 'process_medium'
     publishDir "${params.outdir}",
@@ -243,15 +243,15 @@
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:'report', publish_id:'report') }
         
     cache 'lenient'
     input:
     val(results) 
 
     output:
-    path "report.html", emit: html
+    path "report_*.html", emit: html
     
     script:
     def res = results.join(' ')
     """
     $module_dir/compile.py --pipeline $params.mode --launchdir $launchDir \
     --template_dir $params.template_dir  --day ${params.day} --user ${params.user} \
     --isolates $params.isolates --reference $params.reference --job_id $params.job_id \
@@ -271,11 +271,11 @@
 
     output:
     path "${output_name}.txt", emit: collated
     
     script:
     def resistomes = input.join(' ')
     """
-    $module_dir/collate_plasmids.py $output_name $resistomes
+    $module_dir/collate_tables.py $output_name $resistomes
     """
 
 }
```

### Comparing `bohra-2.2.1/bohra/modules/csvtk/functions.nf` & `bohra-2.3.0/bohra/modules/csvtk/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/csvtk/main.nf` & `bohra-2.3.0/bohra/modules/csvtk/main.nf`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         mode: params.publish_dir_mode,
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:'report', publish_id:'report') }
     
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/csvtk" : 'bioconda::csvtk') : null)
     
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/csvtk"
+            conda "${params.conda_path}/bohra-csvtk"
         } else {
             conda 'bioconda::csvtk'
         }
     } else {
         conda null
     }
```

### Comparing `bohra-2.2.1/bohra/modules/csvtk/meta.yml` & `bohra-2.3.0/bohra/modules/csvtk/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/gubbins/functions.nf` & `bohra-2.3.0/bohra/modules/ectyper/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/gubbins/main.nf` & `bohra-2.3.0/bohra/modules/gubbins/main.nf`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     publishDir "${params.outdir}",
         mode: params.publish_dir_mode
     
     cache 'lenient'
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/gubbins" : 'gubbins=2.4.1 snp-sites=2.5.1') : null)
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/gubbins"
+            conda "${params.conda_path}/bohra-gubbins"
         } else {
-            conda 'gubbins=2.4.1 snp-sites=2.5.1'
+            conda 'gubbins=2.4.1 snp-sites=2.5.1 csvtk'
         }
     } else {
         conda null
     }
     input:
     path(cleaned)
```

### Comparing `bohra-2.2.1/bohra/modules/gubbins/meta.yml` & `bohra-2.3.0/bohra/modules/gubbins/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/iqtree/functions.nf` & `bohra-2.3.0/bohra/modules/emmtyper/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/iqtree/main.nf` & `bohra-2.3.0/bohra/modules/iqtree/main.nf`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 // Import generic module functions
 include { initOptions; saveFiles; getSoftwareName } from './functions'
 
 params.options = [:]
 def options    = initOptions(params.options)
 
-def module_dir = moduleDir + "/bin"
-
 
 process IQTREE {
 
     label 'process_high'
     publishDir "${params.outdir}",
         mode: params.publish_dir_mode,
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:'report', publish_id:'report') }
     
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/iqtree2" : 'iqtree=2.1.4 snp-sites=2.5.1') : null)
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/iqtree2"
+            conda "${params.conda_path}/bohra-iqtree"
         } else {
             conda 'iqtree=2.1.4 snp-sites=2.5.1'
         }
     } else {
         conda null
     }
 
@@ -30,15 +28,15 @@
       
     input:
         path(aln)
         path(full_aln)
 
     output:
         path('core.newick'), emit: newick
-
+    
     script:    
     """
     iqtree -fconst \$(snp-sites -C $full_aln) \\
     -s $aln -pre core \\
     -m GTR+G4 -bb 1000 -ntmax $task.cpus \\
     -nt AUTO -st DNA
     cp core.treefile core.newick
```

### Comparing `bohra-2.2.1/bohra/modules/iqtree/meta.yml` & `bohra-2.3.0/bohra/modules/iqtree/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/kraken2/functions.nf` & `bohra-2.3.0/bohra/modules/gubbins/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/kraken2/main.nf` & `bohra-2.3.0/bohra/modules/kraken2/main.nf`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     publishDir "${params.outdir}",
         mode: params.publish_dir_mode,
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:"${meta.id}", publish_id:meta.id) }
     
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/kraken2" : 'kraken2=2.1.2') : null) 
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/kraken2"
+            conda "${params.conda_path}/bohra-kraken2"
         } else {
             conda 'kraken2=2.1.2'
         }
     } else {
         conda null
     }
     cache 'lenient'
@@ -27,14 +27,15 @@
     
     input:
     tuple val(meta), path(reads), path(kraken)
 
     output:
     tuple val(meta), path('kraken2.tab'), emit: kraken2
 
+
     script:
     def read_files = meta.single_end ?"$reads" : "--paired ${reads[0]} ${reads[1]}"
     """
     kraken2  $read_files \
     --threads $task.cpus \
     --report kraken2.tab \
     --memory-mapping \
```

### Comparing `bohra-2.2.1/bohra/modules/kraken2/meta.yml` & `bohra-2.3.0/bohra/modules/kraken2/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/mash/sketch/functions.nf` & `bohra-2.3.0/bohra/modules/iqtree/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/mash/sketch/main.nf` & `bohra-2.3.0/bohra/modules/lissero/main.nf`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,42 @@
 // Import generic module functions
 include { initOptions; saveFiles; getSoftwareName } from './functions'
 
 params.options = [:]
 def options    = initOptions(params.options)
 
-process MASH_SKETCH {
+process LISSERO {
     tag "$meta.id"
-    label 'process_medium'
+    label 'process_high'
     publishDir "${params.outdir}",
         mode: params.publish_dir_mode,
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:meta.id, publish_id:meta.id) }
     
-    
-    // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/mash" : 'mash') : null) 
-    
+    cpus options.args2// args2 needs to be cpus for shovill
+    cache 'lenient'
+    // errorStrategy 'ignore'
+    // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/spades" : 'bioconda::spades=3.15.2') : null) 
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/mash"
+            conda "${params.conda_path}/bohra-lissero"
         } else {
-            conda 'mash'
+            conda 'lissero csvtk'
         }
+        
     } else {
         conda null
     }
-
-    scratch true
-    
-    cache 'lenient'
-    // conda (params.enable_conda ? 'bioconda::shovill=1.1.0' : null)
-    // if (workflow.containerEngine == 'singularity' && !params.singularity_pull_docker_container) {
-    //     container 'https://depot.galaxyproject.org/singularity/fastp:0.20.1--h8b12597_0'
-    // } else {
-    //     container 'quay.io/biocontainers/fastp:0.20.1--h8b12597_0'
-    // }
-
     input:
-    tuple val(meta), path(reads)
+    tuple val(meta), path(contigs), val(species_obs)
 
     output:
-    tuple val(meta), path('*.msh'), emit: sketch
+    tuple val(meta), path('typer.txt'), emit: typer
 
     script:
     """
-    mash sketch -r ${reads[0]} -m 5 -k 21 -C $meta.id -o ${meta.id}
+    echo -e Isolate'\n'${meta.id} >> tmp.tab
+    lissero $contigs | sed 's/contigs\\.fa/$meta.id/g'  > lissero.tab
+    paste tmp.tab lissero.tab | csvtk -t rename -f SEROTYPE -n Serotype | csvtk -t cut -f -ID,-COMMENT > typer.txt
+    rm -f tmp.tab
     """
     
 }
```

### Comparing `bohra-2.2.1/bohra/modules/mash/sketch/meta.yml` & `bohra-2.3.0/bohra/modules/mash/sketch/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/mash/triangle/functions.nf` & `bohra-2.3.0/bohra/modules/kleborate/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/mash/triangle/main.nf` & `bohra-2.3.0/bohra/modules/mash/triangle/main.nf`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:'report', publish_id:'report') }
     
     
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/mash" : 'mash') : null) 
     
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/mash"
+            conda "${params.conda_path}/bohra-mash"
         } else {
             conda 'mash'
         }
     } else {
         conda null
     }
```

### Comparing `bohra-2.2.1/bohra/modules/mash/triangle/meta.yml` & `bohra-2.3.0/bohra/modules/mash/triangle/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/mlst/functions.nf` & `bohra-2.3.0/bohra/modules/kmc/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/mlst/main.nf` & `bohra-2.3.0/bohra/modules/mlst/main.nf`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     
     cache 'lenient'
     
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/mlst" : 'bioconda::mlst=2.19.0') : null) 
     
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/mlst"
+            conda "${params.conda_path}/bohra-mlst"
         } else {
             conda 'bioconda::mlst=2.19.0'
         }
     } else {
         conda null
     }
```

### Comparing `bohra-2.2.1/bohra/modules/mlst/meta.yml` & `bohra-2.3.0/bohra/modules/kmc/meta.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-name: mlst
-description: in silico MLST against pubmlst database
+name: kmc
+description: determine genome size
 keywords:
-  - mlst
+  - kmc
 tools:
-  - shovill:
+  - kmc:
       description: |
-        Scan contig files against PubMLST typing schemes
-      documentation: https://github.com/tseemann/mlst
+        none
+      documentation: 
       doi: 
 params:
   - outdir:
       type: string
       description: |
         The pipeline's output directory. By default, the module will
         output files into `$params.outdir/<SOFTWARE>`
@@ -44,18 +44,15 @@
 
 output:
   - meta:
       type: map
       description: |
         Groovy Map containing sample information
         e.g. [ id:'test', single_end:false ]
-  - mlst:
+  - genome_size:
       type: file
-      description: The report file from kraken2
-      pattern: "*.mlst.tab"
-  - version:
-      type: file
-      description: File containing software version
-      pattern: "*.{version.txt}"
+      description: genome size
+      pattern: "est_genome_size_kmer.txt"
+  
 authors:
   - "@kristyhoran"
```

### Comparing `bohra-2.2.1/bohra/modules/mobsuite/functions.nf` & `bohra-2.3.0/bohra/modules/kraken2/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/mobsuite/main.nf` & `bohra-2.3.0/bohra/modules/mobsuite/main.nf`

 * *Files 9% similar despite different names*

```diff
@@ -12,17 +12,17 @@
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:meta.id, publish_id:meta.id) }
     
     cache 'lenient'
     
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/mob_suite" : 'bioconda::mob_suite=3.0.2') : null) 
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/mob_suite"
+            conda "${params.conda_path}/bohra-mob_suite"
         } else {
-            conda 'bioconda::mob_suite=3.0.2'
+            conda 'bioconda::mob_suite=3.0.2 csvtk'
         }
     } else {
         conda null
     }
 
     input:
     tuple val(meta), path(asm)
```

### Comparing `bohra-2.2.1/bohra/modules/mobsuite/meta.yml` & `bohra-2.3.0/bohra/modules/mobsuite/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/panaroo/functions.nf` & `bohra-2.3.0/bohra/modules/lissero/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/panaroo/main.nf` & `bohra-2.3.0/bohra/modules/panaroo/main.nf`

 * *Files 10% similar despite different names*

```diff
@@ -6,31 +6,28 @@
 
 process PANAROO {
     label 'process_high'
     publishDir "${params.outdir}",
         mode: 'copy',
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:"report", publish_id:'report') }
     
-    
-    // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/panaroo" : 'bioconda::panaroos=1.2.9') : null) 
-    
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/panaroo"
+            conda "${params.conda_path}/bohra-panaroo"
         } else {
             conda 'bioconda::panaroo=1.2.9 csvtk'
         }
     } else {
         conda null
     }
     
 
     cache 'lenient'
     scratch true
-    // afterScript "rm -fr /tmp/\$USER/*"
+    
     
     input:
     val(gffs)
 
     output:
     path('summary_statistics.txt'), emit: pangenome_summary
     path('gene_presence_absence_roary.csv'), emit: pangenome_csv
```

### Comparing `bohra-2.2.1/bohra/modules/panaroo/meta.yml` & `bohra-2.3.0/bohra/modules/panaroo/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/prokka/functions.nf` & `bohra-2.3.0/bohra/modules/mash/sketch/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/prokka/main.nf` & `bohra-2.3.0/bohra/modules/prokka/main.nf`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     label 'process_high'
     publishDir "${params.outdir}",
         mode: params.publish_dir_mode,
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:meta.id, publish_id:meta.id) }
 
     cache 'lenient'
     
-    // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/prokka" : 'bioconda::prokka=1.14.6') : null) 
+   
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/prokka"
+            conda "${params.conda_path}/bohra-prokka"
         } else {
             conda 'bioconda::prokka'
         }
     } else {
         conda null
     }
```

### Comparing `bohra-2.2.1/bohra/modules/prokka/meta.yml` & `bohra-2.3.0/bohra/modules/prokka/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/quicktree/functions.nf` & `bohra-2.3.0/bohra/modules/mash/triangle/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/quicktree/main.nf` & `bohra-2.3.0/bohra/modules/snp_dists/main.nf`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 // Import generic module functions
 include { initOptions; saveFiles; getSoftwareName } from './functions'
 
 params.options = [:]
 def options    = initOptions(params.options)
 
-process QUICKTREE {
-
+process SNP_DISTS {
+    
     label 'process_medium'
     publishDir "${params.outdir}",
         mode: params.publish_dir_mode,
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:'report', publish_id:'report') }
     
     
-    // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/quicktree" : 'bioconda::quicktree=2.5') : null) 
+    // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/snpdists" : 'bioconda::snp-dists=0.8.2 bioconda::csvtk') : null) 
     
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/quicktree"
+            conda "${params.conda_path}/bohra-snpdists"
         } else {
-            conda 'bioconda::bioconda::quicktree=2.5'
+            conda 'bioconda::snp-dists=0.8.2 bioconda::csvtk'
         }
     } else {
         conda null
     }
-
+    
     cache 'lenient'
     
     input:
-    path(preview_distances)
+    path(core) 
 
     output:
-    path('preview.newick'), emit: preveiw_tree
+    path('distances.tab'), emit: distances
 
     script:
+    
     """
-    quicktree -in m -out t $preview_distances  | nw_order -c n - > preview.newick
+    snp-dists $core | csvtk rename -t -f 1 -n Isolate > distances.tab
     """
-        
+    
 }
```

### Comparing `bohra-2.2.1/bohra/modules/quicktree/meta.yml` & `bohra-2.3.0/bohra/modules/quicktree/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/resistome/bin/combine.py` & `bohra-2.3.0/bohra/modules/resistome/bin/combine.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/resistome/bin/concat.py` & `bohra-2.3.0/bohra/modules/resistome/bin/concat.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/resistome/bin/meta.yaml` & `bohra-2.3.0/bohra/modules/resistome/bin/meta.yaml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/resistome/functions.nf` & `bohra-2.3.0/bohra/modules/meningotype/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/resistome/main.nf` & `bohra-2.3.0/bohra/modules/resistome/main.nf`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     // publishDir "abritamr",
     //     mode: 'link',
     //     saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:meta.id, publish_id:meta.id) }
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/abritamr" : 'bioconda::abritamr') : null) 
     
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/abritamr"
+            conda "${params.conda_path}/bohra-abritamr"
         } else {
             conda 'bioconda::bioconda::abritamr'
         }
     } else {
         conda null
     }
 
@@ -107,9 +107,7 @@
     script:
     
     """
     $module_dir/concat.py summary_partials.txt $abritamr_partials_isolates
     """
     
 }
-
-
```

### Comparing `bohra-2.2.1/bohra/modules/resistome/meta.yml` & `bohra-2.3.0/bohra/modules/resistome/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/roary2svg/bin/roary2svg.pl` & `bohra-2.3.0/bohra/modules/roary2svg/bin/roary2svg.pl`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/roary2svg/functions.nf` & `bohra-2.3.0/bohra/modules/mlst/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/roary2svg/main.nf` & `bohra-2.3.0/bohra/modules/roary2svg/main.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/roary2svg/meta.yml` & `bohra-2.3.0/bohra/modules/roary2svg/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/seqkit/fx2tab/functions.nf` & `bohra-2.3.0/bohra/modules/mobsuite/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/seqkit/fx2tab/main.nf` & `bohra-2.3.0/bohra/modules/seqkit/fx2tab/main.nf`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:meta.id, publish_id:meta.id) }
     
     cache 'lenient'
     
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/seqkit" : 'csvtk seqkit=2.1.0') : null) 
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/seqkit"
+            conda "${params.conda_path}/bohra-seqkit"
         } else {
             conda 'csvtk seqkit=2.1.0'
         }
     } else {
         conda null
     }
     // if (workflow.containerEngine == 'singularity' && !params.singularity_pull_docker_container) {
```

### Comparing `bohra-2.2.1/bohra/modules/seqkit/fx2tab/meta.yml` & `bohra-2.3.0/bohra/modules/seqkit/fx2tab/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/seqkit/stats/functions.nf` & `bohra-2.3.0/bohra/modules/ngmaster/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/seqkit/stats/main.nf` & `bohra-2.3.0/bohra/modules/seqkit/stats/main.nf`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:meta.id, publish_id:meta.id) }
     
     cache 'lenient'
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/seqkit" : 'csvtk seqkit=2.1.0') : null) 
     
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/seqkit"
+            conda "${params.conda_path}/bohra-seqkit"
         } else {
             conda 'csvtk seqkit=2.1.0'
         }
     } else {
         conda null
     }
```

### Comparing `bohra-2.2.1/bohra/modules/seqkit/stats/meta.yml` & `bohra-2.3.0/bohra/modules/seqkit/stats/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/seqtk/functions.nf` & `bohra-2.3.0/bohra/modules/panaroo/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/seqtk/main.nf` & `bohra-2.3.0/bohra/modules/seqtk/main.nf`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         mode: params.publish_dir_mode,
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:meta.id, publish_id:meta.id) }
     
     cache 'lenient'
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/seqtk" : 'seqtk') : null) 
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/seqtk"
+            conda "${params.conda_path}/bohra-seqtk"
         } else {
             conda 'bioconda::seqtk'
         }
     } else {
         conda null
     }
     input:
```

### Comparing `bohra-2.2.1/bohra/modules/seqtk/meta.yml` & `bohra-2.3.0/bohra/modules/seqtk/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/shovill/functions.nf` & `bohra-2.3.0/bohra/modules/prokka/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/shovill/main.nf` & `bohra-2.3.0/bohra/modules/shovill/main.nf`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:"${meta.id}", publish_id:meta.id) }
     
     
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/shovill" : 'shovill=1.1.0') : null) 
     
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/shovill"
+            conda "${params.conda_path}/bohra-shovill"
         } else {
             conda 'bioconda::shovill=1.1.0'
         }
     } else {
         conda null
     }
```

### Comparing `bohra-2.2.1/bohra/modules/shovill/meta.yml` & `bohra-2.3.0/bohra/modules/shovill/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/skesa/functions.nf` & `bohra-2.3.0/bohra/modules/quicktree/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/skesa/main.nf` & `bohra-2.3.0/bohra/modules/skesa/main.nf`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:"${meta.id}", publish_id:meta.id) }
     
     
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/skesa" : 'bioconda::skesa=2.4.0') : null) 
     
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/skesa"
+            conda "${params.conda_path}/bohra-skesa"
         } else {
             conda 'bioconda::skesa=2.4'
         }
     } else {
         conda null
     }
```

### Comparing `bohra-2.2.1/bohra/modules/skesa/meta.yml` & `bohra-2.3.0/bohra/modules/skesa/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/snippy/functions.nf` & `bohra-2.3.0/bohra/modules/resistome/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/snippy/main.nf` & `bohra-2.3.0/bohra/modules/snippy/main.nf`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     
     // scratch true
     cache 'lenient'
     
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/snippy" : 'bioconda::snippy=4.4.5') : null) 
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/snippy"
+            conda "${params.conda_path}/bohra-snippy"
         } else {
             conda 'bioconda::snippy=4.4.5'
         }
     } else {
         conda null
     }
     input:
```

### Comparing `bohra-2.2.1/bohra/modules/snippy/meta.yml` & `bohra-2.3.0/bohra/modules/snippy/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/snippy_clean/functions.nf` & `bohra-2.3.0/bohra/modules/roary2svg/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/snippy_clean/main.nf` & `bohra-2.3.0/bohra/modules/snippy_clean/main.nf`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         mode: params.publish_dir_mode
     
     cache 'lenient'
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/snippy" : 'snippy=4.4.5') : null)
     
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/snippy"
+            conda "${params.conda_path}/bohra-snippy"
         } else {
             conda 'bioconda::snippy=4.4.5'
         }
     } else {
         conda null
     }
```

### Comparing `bohra-2.2.1/bohra/modules/snippy_clean/meta.yml` & `bohra-2.3.0/bohra/modules/snippy_clean/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/snippy_core/functions.nf` & `bohra-2.3.0/bohra/modules/seqkit/fx2tab/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/snippy_core/main.nf` & `bohra-2.3.0/bohra/modules/snippy_core/main.nf`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     label 'process_medium'
     publishDir "${params.outdir}",
         mode: params.publish_dir_mode
     
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/snippy" : 'bioconda::snippy=4.4.5') : null) 
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/snippy"
+            conda "${params.conda_path}/bohra-snippy"
         } else {
             conda 'bioconda::snippy=4.4.5'
         }
     } else {
         conda null
     }
     cpus options.args2// args2 needs to be cpus for shovill
```

### Comparing `bohra-2.2.1/bohra/modules/snippy_core/meta.yml` & `bohra-2.3.0/bohra/modules/snippy_core/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/snp_dists/functions.nf` & `bohra-2.3.0/bohra/modules/seqkit/stats/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/snp_dists/meta.yml` & `bohra-2.3.0/bohra/modules/snp_dists/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/spades/functions.nf` & `bohra-2.3.0/bohra/modules/seqtk/functions.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/modules/spades/main.nf` & `bohra-2.3.0/bohra/modules/spades/main.nf`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 
 process SPADES {
     tag "$meta.id"
     label 'process_high'
     publishDir "${params.outdir}",
         mode: params.publish_dir_mode,
         saveAs: { filename -> saveFiles(filename:filename, options:params.options, publish_dir:meta.id, publish_id:meta.id) }
-    
-    cpus options.args2// args2 needs to be cpus for shovill
+
     cache 'lenient'
     
     // conda (params.enable_conda ? (file("${params.conda_path}").exists() ? "${params.conda_path}/spades" : 'bioconda::spades=3.15.2') : null) 
     if ( params.enable_conda ) {
         if (file("${params.conda_path}").exists()) {
-            conda "${params.conda_path}/spades"
+            conda "${params.conda_path}/bohra-spades"
         } else {
-            conda 'bioconda::spades=3.15.2'
+            conda 'bioconda::spades=3.13 csvtk python=3.7'
         }
     } else {
         conda null
     }
     input:
     tuple val(meta), path(reads)
 
@@ -34,14 +33,14 @@
     script:
     """
     if [ -e $meta.contigs ]
     then
         cp $meta.contigs contigs.fa
     else
         tmp_dir=\$(mktemp -d)
-        spades.py -1 ${reads[0]} -2 ${reads[1]} -o current -t $task.cpus --isolate --tmp-dir \$tmp_dir
+        spades.py -1 ${reads[0]} -2 ${reads[1]} -o current -t $task.cpus $options.args2 --tmp-dir \$tmp_dir
         cp current/contigs.fasta contigs.fa
         rm -rf \$tmp_dir
     fi
     """
     
 }
```

### Comparing `bohra-2.2.1/bohra/modules/spades/meta.yml` & `bohra-2.3.0/bohra/modules/spades/meta.yml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/nextflow.config` & `bohra-2.3.0/bohra/nextflow.config`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,14 @@
     run_kraken = true
     run_iqtree = true
     kraken2_db = "$KRAKEN2_DEFAULT_DB"
     assembler = "spades"
     mask_string = ""
     mlst_exclude = ""
 
-    
-
 }
 
 
 profiles {
 
    lcl {
       params.publish_dir_mode = 'copy'
@@ -42,15 +40,15 @@
            cpus= 8
         }
       }
     }
    mdu_binfie {
       params.publish_dir_mode = 'link'
       params.mlst_exclude = 'ecoli,abaumannii'
-      params.conda_path = '/home/khhor/conda/envs'
+      params.conda_path = '/home/mdu/conda/envs'
       executor {
          name = 'local'
          cpus = 256
       }
       process {
       
         withLabel: process_low {
```

### Comparing `bohra-2.2.1/bohra/templates/cluster.tmpl` & `bohra-2.3.0/bohra/templates/cluster.tmpl`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/templates/config_snippy.yaml` & `bohra-2.3.0/bohra/templates/config_snippy.yaml`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/templates/index.html` & `bohra-2.3.0/bohra/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -191,67 +191,67 @@
           <p style="margin:10px;">Select the parent node to display pariwise SNP distances</p>
         </ul>
         </div>
       </div>
     </div>
 
 <div id="help-button" style = "float:right;">
-  <button type="button" class="btn btn-sm btn-outline-secondary zoom-button" id = "help" data-toggle="modal" data-target="#myModal3" data-placement="top" title="Select"> Helpful tips </button>    
-  <button type="button" class="btn btn-sm btn-outline-secondary version-button" id = "version"> Software versions </button>    
+  <!-- <button type="button" class="btn btn-sm btn-outline-secondary zoom-button" id = "help" data-toggle="modal" data-target="#myModal3" data-placement="top" title="Select"> Helpful tips </button>     -->
+  <!-- <button type="button" class="btn btn-sm btn-outline-secondary version-button" id = "version"> Software versions </button>     -->
   <!-- <button type="button" class="btn btn-sm btn-outline-secondary" id = "nwk" ><span data-feather="arrow-down"> Download newick </button>         -->
 </div>
 <!-- div for summary table and phylogenetic tree -->
 <div class= "container-fluid">
 <!-- buttons -->
 {% if phylo == 'phylo' %}
-<button type="button" class="btn btn-primary btn-xlg btn-outline-primary btn-lg phylogeny-button">Phylogeny</button>
+<button type="button" class="btn btn-primary btn-xlg btn-outline-primary btn-lg phylogeny-button">Tree</button>
 {% endif %}
 {% for t,v in tables.items() %}
   <button type="button" class="btn btn-primary btn-xlg btn-outline-primary btn-lg detail-button {{v.link}}-button">{{v.name}}</button>
 {% endfor %}
 
-<div id = "software-versions" class = "versions" style = "display: none;">
+<!-- <div id = "software-versions" class = "versions" style = "display: none;">
   <table class="table" id = "version-table">     
     <thead>
       <tr>
         {{version_head}}
       </tr>
     </thead>
     <tbody>
       {{version_body}}
     </tbody>
   </table>
-</div>
+</div> -->
 <div id = "empty-table"></div>
 <div id="comment"></div>
 <div id = "snp-distances-graph" class = "hidden-graph" style="display:none;">  <!-- placeholder for graphs  --> </div>
 <div id = "snp-density-graph" class = "hidden-graph" style="display: none;">  <!-- placeholder for graphs  --> </div>
 <div id="table-download" style="display: none;">
   <button type="button" class="btn btn-sm btn-outline-secondary csv-download-button" id = "download-csv"> download csv </button>    
   <!-- <button type="button" class="btn btn-sm btn-outline-secondary excel-download-button" id = "download-excel"> download xlsx </button>     -->
 </div>  
 <div id="current-table">
     <!-- placeholder for selected table = put selected table in this div -->    
   </div>
   <div id = "pan-svg" style = "display:none;margin:10px;">
     {{ pan_svg }}
   </div>
-
+{% if phylo == 'phylo' %}
   <div id = "phylogeny">
     <button type="button" class="btn btn-sm btn-outline-secondary back-button" id = "step-back"> back </button>    
     <button type="button" class="btn btn-sm btn-outline-secondary reset-button" id = "reset-tree"> reset </button> 
     <button type="button" class="btn btn-sm btn-outline-secondary download-button" id = "download-tree"> download </button> 
     <button type="button" class="btn btn-sm btn-outline-secondary export-button" id = "export-tree"> export png </button> 
     <button type="button" class="btn btn-sm btn-outline-secondary search-tree-button" id = "get-iso" style="float: right;"> search </button>   
     <input type = "text" id = "search-iso" placeholder="Search for sample" style="float: right;">
        
     <div id="tree_string" style="display: none;">{{newick}}</div>
     <div id = "phylocanvas" style = "width: 100%; margin:5px; border: 1px solid lightgray;" ></div>
   </div>
-    
+  {% endif %}
   </div>         
   
         
 <!-- Datatables (to sort tables) -->
 <!-- <script src="https://cdn.datatables.net/1.10.19/js/jquery.dataTables.min.js"></script> -->
 <!-- <script src="https://cdn.datatables.net/1.10.19/js/dataTables.bootstrap.min.js"></script> -->
 <!-- <script src="https://cdn.datatables.net/1.10.19/js/dataTables.bootstrap4.min.js"></script> -->
```

#### html2text {}

```diff
@@ -16,17 +16,19 @@
 ***** Information *****
     * **** Download tree ****
       To download a newick file right click on tree and select export as newick
     * **** Isolate details ****
       Select an isolate node from the tree to see isolate specific details
     * **** SNP distances ****
       Select the parent node to display pariwise SNP distances
- Helpful tips   Software versions
- {% if phylo == 'phylo' %} Phylogeny {% endif %} {% for t,v in tables.items()
-%} {{v.name}} {% endfor %}
+
+ {% if phylo == 'phylo' %} Tree {% endif %} {% for t,v in tables.items() %} {
+{v.name}} {% endfor %}
  download csv
 {{ pan_svg }}
+{% if phylo == 'phylo' %}
  back   reset   download   export png   search  [                    ]
 {{newick}}
+{% endif %}
 
  {% block script %}
  {% endblock %}
```

### Comparing `bohra-2.2.1/bohra/tests/test.gbk` & `bohra-2.3.0/bohra/tests/test.gbk`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/tests/test.tab` & `bohra-2.3.0/bohra/tests/test.tab`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/tests/test_bohra.py` & `bohra-2.3.0/bohra/tests/test_bohra.py`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/workflows/collation.nf` & `bohra-2.3.0/bohra/workflows/collation.nf`

 * *Files identical despite different names*

### Comparing `bohra-2.2.1/bohra/workflows/default.nf` & `bohra-2.3.0/bohra/workflows/default.nf`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,14 @@
         contigs
         assembly_stats = SEQKIT_STATS.out.stats
         resistome = COMBINE_AMR.out.resistome
         virulome = ABRITAMR.out.abritamr_virulence
         mlst = ADD_HEADER_MLST.out.mlst
         gff = PROKKA.out.gff
         prokka_txt = PROKKA.out.prokka_txt
-        // add the result file emmitted by new rule
         plasmid = MOBSUITE_WRANGLE.out.plasmid
 }
 
 workflow CONCAT_MLST {
     take:
         mlsts
     main:
```

### Comparing `bohra-2.2.1/setup.cfg` & `bohra-2.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = bohra
 author = Kristy Horan
 author_email = kristyhoran15@gmail.com
 description = A bioinformatics pipeline for analysing short read Illumina data microbiological public health.
-version = 2.2.1
+version = 2.3.0
 url = https://github.com/kristyhoran/bohra
 classifiers = 
 	Programming Language :: Python :: 3.9
 	Operating System :: OS Independent
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering :: Bio-Informatics
```

