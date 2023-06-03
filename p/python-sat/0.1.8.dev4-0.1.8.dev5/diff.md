# Comparing `tmp/python-sat-0.1.8.dev4.tar.gz` & `tmp/python-sat-0.1.8.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sat-0.1.8.dev4.tar", last modified: Thu May 25 02:35:20 2023, max compression
+gzip compressed data, was "python-sat-0.1.8.dev5.tar", last modified: Sat Jun  3 01:33:44 2023, max compression
```

## Comparing `python-sat-0.1.8.dev4.tar` & `python-sat-0.1.8.dev5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.969249 python-sat-0.1.8.dev4/
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1109 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/LICENSE.txt
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      217 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/MANIFEST.in
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1193 2023-05-25 02:35:20.969327 python-sat-0.1.8.dev4/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    14137 2023-04-21 08:05:23.000000 python-sat-0.1.8.dev4/README.rst
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.953835 python-sat-0.1.8.dev4/allies/
--rw-------   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-14 00:41:27.000000 python-sat-0.1.8.dev4/allies/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    13572 2023-05-09 14:01:54.000000 python-sat-0.1.8.dev4/allies/approxmc.py
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.955968 python-sat-0.1.8.dev4/cardenc/
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1375 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/bitwise.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2468 2023-03-02 05:23:11.000000 python-sat-0.1.8.dev4/cardenc/card.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1874 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/clset.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1303 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/common.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     4646 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/itot.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2325 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/ladder.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    11355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/mto.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1008 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/pairwise.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      918 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/ptypes.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    15865 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/pycard.cc
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     4851 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/seqcounter.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     8355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/sortcard.hh
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     5117 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/cardenc/utils.hh
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.957965 python-sat-0.1.8.dev4/examples/
--rw-------   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    17968 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/fm.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    18986 2023-03-04 22:56:50.000000 python-sat-0.1.8.dev4/examples/genhard.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    20609 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/hitman.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    21295 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/lbx.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    15523 2023-01-20 20:56:31.000000 python-sat-0.1.8.dev4/examples/lsu.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    20320 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/mcsls.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)     5724 2023-01-13 10:54:03.000000 python-sat-0.1.8.dev4/examples/models.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    10563 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/musx.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    23950 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/optux.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    66919 2023-05-25 02:24:53.000000 python-sat-0.1.8.dev4/examples/rc2.py
--rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2183 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/examples/usage.py
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.959266 python-sat-0.1.8.dev4/pysat/
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      653 2023-05-25 02:26:56.000000 python-sat-0.1.8.dev4/pysat/__init__.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     5814 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/pysat/_fileio.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1340 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/pysat/_utils.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    30043 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/pysat/card.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    95959 2023-05-19 07:25:29.000000 python-sat-0.1.8.dev4/pysat/formula.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    15657 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/pysat/pb.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    11968 2023-03-05 06:22:14.000000 python-sat-0.1.8.dev4/pysat/process.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   169376 2023-03-05 04:20:33.000000 python-sat-0.1.8.dev4/pysat/solvers.py
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.960147 python-sat-0.1.8.dev4/python_sat.egg-info/
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1193 2023-05-25 02:35:20.000000 python-sat-0.1.8.dev4/python_sat.egg-info/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1863 2023-05-25 02:35:20.000000 python-sat-0.1.8.dev4/python_sat.egg-info/SOURCES.txt
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)        1 2023-05-25 02:35:20.000000 python-sat-0.1.8.dev4/python_sat.egg-info/dependency_links.txt
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)       87 2023-05-25 02:35:20.000000 python-sat-0.1.8.dev4/python_sat.egg-info/requires.txt
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)       23 2023-05-25 02:35:20.000000 python-sat-0.1.8.dev4/python_sat.egg-info/top_level.txt
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)       39 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/requirements.txt
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      107 2023-05-25 02:35:20.969586 python-sat-0.1.8.dev4/setup.cfg
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     6549 2023-04-21 07:47:02.000000 python-sat-0.1.8.dev4/setup.py
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.964551 python-sat-0.1.8.dev4/solvers/
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   547031 2023-03-02 05:10:30.000000 python-sat-0.1.8.dev4/solvers/cadical103.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   596433 2023-03-03 10:16:48.000000 python-sat-0.1.8.dev4/solvers/cadical153.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    50813 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/glucose30.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    82779 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/glucose41.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   501731 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/lingeling.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    82656 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/maplechrono.zip
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    94949 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/maplecm.zip
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    77088 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/maplesat.zip
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   179223 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/mergesat3.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)  1529188 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/minicard.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    43879 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/minisat22.tar.gz
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    75209 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/minisatgh.zip
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.967531 python-sat-0.1.8.dev4/solvers/patches/
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    51588 2023-03-02 05:15:52.000000 python-sat-0.1.8.dev4/solvers/patches/cadical103.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    66092 2023-03-06 01:41:40.000000 python-sat-0.1.8.dev4/solvers/patches/cadical153.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    93207 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/glucose30.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    89206 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/glucose41.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   117955 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/gluecard30.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   137342 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/gluecard41.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    54848 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/lingeling.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    90618 2023-01-14 22:24:35.000000 python-sat-0.1.8.dev4/solvers/patches/maplechrono.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   114715 2023-01-14 21:29:08.000000 python-sat-0.1.8.dev4/solvers/patches/maplecm.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    82379 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/maplesat.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    88893 2023-01-14 22:24:31.000000 python-sat-0.1.8.dev4/solvers/patches/mergesat3.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    51757 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/minicard.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    42627 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/minisat22.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    60626 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/solvers/patches/minisatgh.patch
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    25391 2023-03-06 01:41:50.000000 python-sat-0.1.8.dev4/solvers/prepare.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   214965 2023-03-05 04:21:31.000000 python-sat-0.1.8.dev4/solvers/pysolvers.cc
-drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-05-25 02:35:20.969106 python-sat-0.1.8.dev4/tests/
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      948 2023-03-05 08:16:22.000000 python-sat-0.1.8.dev4/tests/test_accum_stats.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      429 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/tests/test_atmost.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      707 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/tests/test_atmost1.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      998 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/tests/test_atmostk.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2408 2023-03-05 08:17:09.000000 python-sat-0.1.8.dev4/tests/test_cnfplus.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      784 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/tests/test_equals1.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1007 2023-03-05 06:31:37.000000 python-sat-0.1.8.dev4/tests/test_process.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      866 2023-03-05 08:17:46.000000 python-sat-0.1.8.dev4/tests/test_unique_model.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      937 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev4/tests/test_unique_mus.py
--rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      643 2023-01-14 22:33:39.000000 python-sat-0.1.8.dev4/tests/test_warmstart.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.233020 python-sat-0.1.8.dev5/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1109 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/LICENSE.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      217 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/MANIFEST.in
+-rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-06-03 01:33:44.233115 python-sat-0.1.8.dev5/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) 907548567    14137 2023-04-21 08:05:23.000000 python-sat-0.1.8.dev5/README.rst
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.203440 python-sat-0.1.8.dev5/allies/
+-rw-------   0 aign0002 (892519254) 907548567        0 2023-04-14 00:41:27.000000 python-sat-0.1.8.dev5/allies/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    13572 2023-05-09 14:01:54.000000 python-sat-0.1.8.dev5/allies/approxmc.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.206274 python-sat-0.1.8.dev5/cardenc/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1375 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/bitwise.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     2468 2023-03-02 05:23:11.000000 python-sat-0.1.8.dev5/cardenc/card.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1874 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/clset.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1303 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/common.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     4646 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/itot.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     2325 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/ladder.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567    11355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/mto.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1008 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/pairwise.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567      918 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/ptypes.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567    15865 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/pycard.cc
+-rw-r--r--   0 aign0002 (892519254) 907548567     4851 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/seqcounter.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     8355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/sortcard.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     5117 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/cardenc/utils.hh
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.210505 python-sat-0.1.8.dev5/examples/
+-rw-------   0 aign0002 (892519254) 907548567        0 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/examples/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    17968 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/examples/fm.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    18986 2023-03-04 22:56:50.000000 python-sat-0.1.8.dev5/examples/genhard.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    24012 2023-06-02 13:29:16.000000 python-sat-0.1.8.dev5/examples/hitman.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    21295 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/examples/lbx.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    15523 2023-01-20 20:56:31.000000 python-sat-0.1.8.dev5/examples/lsu.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    20320 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/examples/mcsls.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567     5724 2023-01-13 10:54:03.000000 python-sat-0.1.8.dev5/examples/models.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    10563 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/examples/musx.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    23950 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/examples/optux.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    67020 2023-05-25 10:53:45.000000 python-sat-0.1.8.dev5/examples/rc2.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567     2183 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/examples/usage.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.212751 python-sat-0.1.8.dev5/pysat/
+-rw-r--r--   0 aign0002 (892519254) 907548567      653 2023-06-03 01:29:39.000000 python-sat-0.1.8.dev5/pysat/__init__.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     5814 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/pysat/_fileio.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1340 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/pysat/_utils.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    30043 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/pysat/card.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    95959 2023-05-19 07:25:29.000000 python-sat-0.1.8.dev5/pysat/formula.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    15657 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/pysat/pb.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    11968 2023-03-05 06:22:14.000000 python-sat-0.1.8.dev5/pysat/process.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   174192 2023-06-03 01:28:00.000000 python-sat-0.1.8.dev5/pysat/solvers.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.214048 python-sat-0.1.8.dev5/python_sat.egg-info/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-06-03 01:33:44.000000 python-sat-0.1.8.dev5/python_sat.egg-info/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) 907548567     1863 2023-06-03 01:33:44.000000 python-sat-0.1.8.dev5/python_sat.egg-info/SOURCES.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567        1 2023-06-03 01:33:44.000000 python-sat-0.1.8.dev5/python_sat.egg-info/dependency_links.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       87 2023-06-03 01:33:44.000000 python-sat-0.1.8.dev5/python_sat.egg-info/requires.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       23 2023-06-03 01:33:44.000000 python-sat-0.1.8.dev5/python_sat.egg-info/top_level.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       39 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/requirements.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      107 2023-06-03 01:33:44.233388 python-sat-0.1.8.dev5/setup.cfg
+-rw-r--r--   0 aign0002 (892519254) 907548567     6549 2023-04-21 07:47:02.000000 python-sat-0.1.8.dev5/setup.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.222854 python-sat-0.1.8.dev5/solvers/
+-rw-r--r--   0 aign0002 (892519254) 907548567   547031 2023-03-02 05:10:30.000000 python-sat-0.1.8.dev5/solvers/cadical103.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   596433 2023-03-03 10:16:48.000000 python-sat-0.1.8.dev5/solvers/cadical153.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    50813 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/glucose30.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    82779 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/glucose41.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   501731 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/lingeling.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    82656 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/maplechrono.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567    94949 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/maplecm.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567    77088 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/maplesat.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567   179223 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/mergesat3.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567  1529188 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/minicard.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    43879 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/minisat22.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    75209 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/minisatgh.zip
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.229963 python-sat-0.1.8.dev5/solvers/patches/
+-rw-r--r--   0 aign0002 (892519254) 907548567    51588 2023-03-02 05:15:52.000000 python-sat-0.1.8.dev5/solvers/patches/cadical103.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    66092 2023-06-03 01:29:02.000000 python-sat-0.1.8.dev5/solvers/patches/cadical153.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    93207 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/glucose30.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    89206 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/glucose41.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   117955 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/gluecard30.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   137342 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/gluecard41.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    54848 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/lingeling.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    90618 2023-01-14 22:24:35.000000 python-sat-0.1.8.dev5/solvers/patches/maplechrono.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   114715 2023-01-14 21:29:08.000000 python-sat-0.1.8.dev5/solvers/patches/maplecm.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    82379 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/maplesat.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    88893 2023-01-14 22:24:31.000000 python-sat-0.1.8.dev5/solvers/patches/mergesat3.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    51757 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/minicard.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    42627 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/minisat22.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    60626 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/solvers/patches/minisatgh.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    25391 2023-06-03 01:04:24.000000 python-sat-0.1.8.dev5/solvers/prepare.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   222394 2023-06-03 01:27:14.000000 python-sat-0.1.8.dev5/solvers/pysolvers.cc
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-03 01:33:44.232748 python-sat-0.1.8.dev5/tests/
+-rw-r--r--   0 aign0002 (892519254) 907548567      948 2023-03-05 08:16:22.000000 python-sat-0.1.8.dev5/tests/test_accum_stats.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      429 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/tests/test_atmost.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      707 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/tests/test_atmost1.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      998 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/tests/test_atmostk.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     2408 2023-03-05 08:17:09.000000 python-sat-0.1.8.dev5/tests/test_cnfplus.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      784 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/tests/test_equals1.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1007 2023-03-05 06:31:37.000000 python-sat-0.1.8.dev5/tests/test_process.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      866 2023-03-05 08:17:46.000000 python-sat-0.1.8.dev5/tests/test_unique_model.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      937 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev5/tests/test_unique_mus.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      643 2023-01-14 22:33:39.000000 python-sat-0.1.8.dev5/tests/test_warmstart.py
```

### Comparing `python-sat-0.1.8.dev4/LICENSE.txt` & `python-sat-0.1.8.dev5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/PKG-INFO` & `python-sat-0.1.8.dev5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 0.1.8.dev4
+Version: 0.1.8.dev5
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: aiger
```

### Comparing `python-sat-0.1.8.dev4/README.rst` & `python-sat-0.1.8.dev5/README.rst`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/allies/approxmc.py` & `python-sat-0.1.8.dev5/allies/approxmc.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/cardenc/bitwise.hh` & `python-sat-0.1.8.dev5/cardenc/bitwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/cardenc/card.hh` & `python-sat-0.1.8.dev5/cardenc/card.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/cardenc/clset.hh` & `python-sat-0.1.8.dev5/cardenc/clset.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/cardenc/common.hh` & `python-sat-0.1.8.dev5/cardenc/common.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/cardenc/itot.hh` & `python-sat-0.1.8.dev5/cardenc/itot.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/cardenc/ladder.hh` & `python-sat-0.1.8.dev5/cardenc/ladder.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/cardenc/mto.hh` & `python-sat-0.1.8.dev5/cardenc/mto.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/cardenc/pairwise.hh` & `python-sat-0.1.8.dev5/cardenc/pairwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/cardenc/ptypes.hh` & `python-sat-0.1.8.dev5/cardenc/ptypes.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/cardenc/pycard.cc` & `python-sat-0.1.8.dev5/cardenc/pycard.cc`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/cardenc/seqcounter.hh` & `python-sat-0.1.8.dev5/cardenc/seqcounter.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/cardenc/sortcard.hh` & `python-sat-0.1.8.dev5/cardenc/sortcard.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/cardenc/utils.hh` & `python-sat-0.1.8.dev5/cardenc/utils.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/examples/fm.py` & `python-sat-0.1.8.dev5/examples/fm.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/examples/genhard.py` & `python-sat-0.1.8.dev5/examples/genhard.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/examples/hitman.py` & `python-sat-0.1.8.dev5/examples/hitman.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,14 +46,18 @@
 
     Taking into account this problem formulation as MaxSAT, ordered hitting
     enumeration is done with the use of the state-of-the-art MaxSAT solver
     called :class:`.RC2` [2]_ [3]_ [4]_ while unordered hitting set enumeration
     is done through the *minimal correction subset* (MCS) enumeration, e.g.
     using the :class:`.LBX`- [5]_ or :class:`.MCSls`-like [6]_ MCS enumerators.
 
+    Note that this implementation additionally supports *pure* SAT-based
+    minimal hitting set enumeration with the use of preferred variable
+    polarity setting following the approach of [7]_.
+
     .. [1] Erick Moreno-Centeno, Richard M. Karp. *The Implicit Hitting Set
         Approach to Solve Combinatorial Optimization Problems with an
         Application to Multigenome Alignment*. Operations Research 61(2). 2013.
         pp. 453-468
 
     .. [2] António Morgado, Carmine Dodaro, Joao Marques-Silva. *Core-Guided
         MaxSAT with Soft Cardinality Constraints*. CP 2014. pp. 564-573
@@ -67,14 +71,17 @@
     .. [5] Carlos Mencía, Alessandro Previti, Joao Marques-Silva.
         *Literal-Based MCS Extraction*. IJCAI. 2015. pp. 1973-1979
 
     .. [6] Joao Marques-Silva, Federico Heras, Mikolás Janota,
         Alessandro Previti, Anton Belov. *On Computing Minimal Correction
         Subsets*. IJCAI. 2013. pp. 615-622
 
+    .. [7] Enrico Giunchiglia, Marco Maratea. *Solving Optimization Problems
+        with DLL*. ECAI 2006. pp. 377-381
+
     :class:`Hitman` supports hitting set enumeration in the *implicit* manner,
     i.e. when sets to hit can be added on the fly as well as hitting sets can
     be blocked on demand.
 
     An example usage of :class:`Hitman` through the Python ``import`` interface
     is shown below. Here we target unordered subset-minimal hitting set
     enumeration.
@@ -117,15 +124,15 @@
         [2, 4, 7]
         [3, 4, 6]
         [3, 4, 5]
         [2, 4, 6]
         [2, 4, 5]
 
     Finally, implicit hitting set enumeration can be used in practical problem
-    solving. As an example, let us show the basic flow of a MaxHS-like [7]_
+    solving. As an example, let us show the basic flow of a MaxHS-like [8]_
     algorithm for MaxSAT:
 
     .. code-block:: python
 
         >>> from pysat.examples.hitman import Hitman
         >>> from pysat.solvers import Solver
         >>>
@@ -144,28 +151,30 @@
         ...         print('s OPTIMUM FOUND')
         ...         print('o', len(hs))
         ...         break
         ...     else:
         ...         core = oracle.get_core()
         ...         hitman.hit(core)
 
-    .. [7] Jessica Davies, Fahiem Bacchus. *Solving MAXSAT by Solving a
+    .. [8] Jessica Davies, Fahiem Bacchus. *Solving MAXSAT by Solving a
         Sequence of Simpler SAT Instances*. CP 2011. pp. 225-239
 
     ==============
     Module details
     ==============
 """
 
 #
 #==============================================================================
-from pysat.formula import IDPool, WCNFPlus
+import collections
 from pysat.examples.rc2 import RC2, RC2Stratified
 from pysat.examples.lbx import LBX
 from pysat.examples.mcsls import MCSls
+from pysat.formula import IDPool, WCNFPlus
+from pysat.solvers import Solver, SolverNames
 import six
 
 
 #
 #==============================================================================
 class Atom(object):
     """
@@ -182,33 +191,39 @@
         self.sign = sign
 
 
 #
 #==============================================================================
 class Hitman(object):
     """
+
         A cardinality-/subset-minimal hitting set enumerator. The enumerator
         can be set up to use either a MaxSAT solver :class:`.RC2` or an MCS
         enumerator (either :class:`.LBX` or :class:`.MCSls`). In the former
         case, the hitting sets enumerated are ordered by size (smallest size
         hitting sets are computed first), i.e. *sorted*. In the latter case,
         subset-minimal hitting are enumerated in an arbitrary order, i.e.
-        *unsorted*.
+        *unsorted*. Additionally, Hitman supports pure SAT-based minimal
+        hitting set enumeration with the use of polarity preferences.
 
-        This is handled with the use of parameter ``htype``, which is set to be
-        ``'sorted'`` by default. The MaxSAT-based enumerator can be chosen by
-        setting ``htype`` to one of the following values: ``'maxsat'``,
-        ``'mxsat'``, or ``'rc2'``. Alternatively, by setting it to ``'mcs'`` or
-        ``'lbx'``, a user can enforce using the :class:`.LBX` MCS enumerator.
-        If ``htype`` is set to ``'mcsls'``, the :class:`.MCSls` enumerator is
-        used.
-
-        In either case, an underlying problem solver can use a SAT oracle
-        specified as an input parameter ``solver``. The default SAT solver is
-        Glucose3 (specified as ``g3``, see :class:`.SolverNames` for details).
+        This is handled with the use of parameter ``htype``, which is set to
+        be ``'sorted'`` by default. The MaxSAT-based enumerator can be chosen
+        by setting ``htype`` to one of the following values: ``'maxsat'``,
+        ``'mxsat'``, or ``'rc2'``. Alternatively, by setting it to ``'mcs'``
+        or ``'lbx'``, a user can enforce using the :class:`.LBX` MCS
+        enumerator. If ``htype`` is set to ``'mcsls'``, the :class:`.MCSls`
+        enumerator is used. Finally, value ``'sat'`` can be given, in which
+        case minimal hitting set enumeration will performed by means of a SAT
+        solver (can be either MiniSat-GH or Lingeling) with polarity setting.
+
+        In either case, unless pure SAT-based hitting set enumeration is
+        selected, an underlying problem solver can use a SAT oracle specified
+        as an input parameter ``solver``. The default SAT solver is Glucose3
+        (specified as ``g3``, see :class:`.SolverNames` for details). For
+        SAT-based enumeration, MinisatGH is used as an underlying SAT solver.
 
         Objects of class :class:`Hitman` can be bootstrapped with an iterable
         of iterables, e.g. a list of lists. This is handled using the
         ``bootstrap_with`` parameter. Each set to hit can comprise elements of
         any type, e.g. integers, strings or objects of any Python class, as
         well as their combinations. The bootstrapping phase is done in
         :func:`init`.
@@ -270,16 +285,18 @@
         self.usecld   = mcs_usecld
 
         # hitman type: either a MaxSAT solver or an MCS enumerator
         if htype in ('maxsat', 'mxsat', 'rc2', 'sorted'):
             self.htype = 'rc2'
         elif htype in ('mcs', 'lbx'):
             self.htype = 'lbx'
-        else:  # 'mcsls'
+        elif htype == 'mcsls':
             self.htype = 'mcsls'
+        else:  # 'sat'
+            self.htype = 'sat'
 
         # pool of variable identifiers (for objects to hit)
         self.idpool = IDPool()
 
         # initialize hitting set solver
         self.init(bootstrap_with, weights=weights, subject_to=subject_to)
 
@@ -362,17 +379,45 @@
             else:
                 self.oracle = RC2Stratified(formula, solver=self.solver,
                         adapt=self.adapt, exhaust=self.exhaust, minz=self.minz,
                         nohard=True, trim=self.trim)
         elif self.htype == 'lbx':
             self.oracle = LBX(formula, solver_name=self.solver,
                     use_cld=self.usecld)
-        else:
+        elif self.htype == 'mcsls':
             self.oracle = MCSls(formula, solver_name=self.solver,
                     use_cld=self.usecld)
+        else:  # 'sat'
+            assert self.solver in SolverNames.minisatgh + SolverNames.lingeling, \
+                    'Hard polarity setting is unsupported by {0}'.format(self.solver)
+
+            assert formula.atms == [], 'Native AtMostK constraints aren\'t' \
+            'supported by MinisatGH, Lingeling'
+
+            # setting up a SAT solver, so that it supports the same interface
+            self.oracle = Solver(name=self.solver, bootstrap_with=formula.hard,
+                                 use_timer=True)
+
+            # MinisatGH supports warm start mode
+            if self.solver in SolverNames.minisatgh:
+                self.oracle.start_mode(warm=True)
+
+            # soft clauses are enforced by means of setting polarities
+            self.oracle.set_phases(literals=[cl[0] for cl in formula.soft])
+
+            # "adding" the missing compute() and oracle_time() methods
+            self.oracle.compute = lambda: [self.oracle.solve(), self.oracle.get_model()][-1]
+            self.oracle.oracle_time = self.oracle.time_accum
+
+            # adding a dummy VariableMap, as is in RC2 and LBX/MCSls
+            VariableMap = collections.namedtuple('VariableMap', ['e2i', 'i2e'])
+            self.oracle.vmap = VariableMap(e2i={}, i2e={})
+            for vid in self.idpool.id2obj.keys():
+                self.oracle.vmap.e2i[vid] = vid
+                self.oracle.vmap.i2e[vid] = vid
 
     def add_hard(self, clause, weights=None):
         """
             Add a hard constraint, which can be either a pure clause or an
             AtMostK constraint.
 
             Note that an optional parameter that can be passed to this method
@@ -405,17 +450,26 @@
 
         # some of the literals may also have the opposite polarity
         new_obj = [l if l in self.idpool.obj2id else -l for l in new_obj]
 
         # adding the hard clause
         self.oracle.add_clause(clause)
 
-        # new soft clauses
-        for vid in new_obj:
-            self.oracle.add_clause([-vid], 1 if not weights else weights[self.idpool.obj(vid)])
+        if self.htype != 'sat':
+            # new soft clauses
+            for vid in new_obj:
+                self.oracle.add_clause([-vid], 1 if not weights else weights[self.idpool.obj(vid)])
+        else:
+            # dummy variable id mapping
+            for vid in new_obj:
+                self.oracle.vmap.e2i[vid] = vid
+                self.oracle.vmap.i2e[vid] = vid
+
+            # setting variable polarities
+            self.oracle.set_phases(literals=[-vid for vid in new_obj])
 
     def delete(self):
         """
             Explicit destructor of the internal hitting set oracle.
         """
 
         if self.oracle:
@@ -431,15 +485,15 @@
 
             :rtype: list(obj)
         """
 
         model = self.oracle.compute()
 
         if model is not None:
-            if self.htype == 'rc2':
+            if self.htype in ('rc2', 'sat'):
                 # extracting a hitting set
                 self.hset = filter(lambda v: v > 0, model)
             else:
                 self.hset = model
 
             return list(map(lambda vid: self.idpool.id2obj[vid], self.hset))
 
@@ -467,16 +521,26 @@
         # a soft clause should be added for each new object
         new_obj = list(filter(lambda vid: vid not in self.oracle.vmap.e2i, to_hit))
 
         # new hard clause
         self.oracle.add_clause(to_hit)
 
         # new soft clauses
-        for vid in new_obj:
-            self.oracle.add_clause([-vid], 1 if not weights else weights[self.idpool.obj(vid)])
+        if self.htype != 'sat':
+            # new soft clauses
+            for vid in new_obj:
+                self.oracle.add_clause([-vid], 1 if not weights else weights[self.idpool.obj(vid)])
+        else:
+            # dummy variable id mapping
+            for vid in new_obj:
+                self.oracle.vmap.e2i[vid] = vid
+                self.oracle.vmap.i2e[vid] = vid
+
+            # setting variable polarities
+            self.oracle.set_phases(literals=[-vid for vid in new_obj])
 
     def block(self, to_block, weights=None):
         """
             The method serves for imposing a constraint forbidding the hitting
             set solver to compute a given hitting set. Each set to block is
             encoded as a hard clause in the MaxSAT problem formulation, which
             is then added to the underlying oracle.
@@ -499,16 +563,25 @@
         # a soft clause should be added for each new object
         new_obj = list(filter(lambda vid: vid not in self.oracle.vmap.e2i, to_block))
 
         # new hard clause
         self.oracle.add_clause([-vid for vid in to_block])
 
         # new soft clauses
-        for vid in new_obj:
-            self.oracle.add_clause([-vid], 1 if not weights else weights[self.idpool.obj(vid)])
+        if self.htype != 'sat':
+            for vid in new_obj:
+                self.oracle.add_clause([-vid], 1 if not weights else weights[self.idpool.obj(vid)])
+        else:
+            # dummy variable id mapping
+            for vid in new_obj:
+                self.oracle.vmap.e2i[vid] = vid
+                self.oracle.vmap.i2e[vid] = vid
+
+            # setting variable polarities
+            self.oracle.set_phases(literals=[-vid for vid in new_obj])
 
     def enumerate(self):
         """
             The method can be used as a simple iterator computing and blocking
             the hitting sets on the fly. It essentially calls :func:`get`
             followed by :func:`block`. Each hitting set is reported as a list
             of objects in the original problem domain, i.e. it is mapped back
```

### Comparing `python-sat-0.1.8.dev4/examples/lbx.py` & `python-sat-0.1.8.dev5/examples/lbx.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/examples/lsu.py` & `python-sat-0.1.8.dev5/examples/lsu.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/examples/mcsls.py` & `python-sat-0.1.8.dev5/examples/mcsls.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/examples/models.py` & `python-sat-0.1.8.dev5/examples/models.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/examples/musx.py` & `python-sat-0.1.8.dev5/examples/musx.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/examples/optux.py` & `python-sat-0.1.8.dev5/examples/optux.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/examples/rc2.py` & `python-sat-0.1.8.dev5/examples/rc2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1119,23 +1119,25 @@
                 amb = [[-t.rhs[b]] * (rhs - b) + t.lits, rhs]
                 self.oracle.add_atmost(*amb)
 
         return t, b
 
     def set_bound(self, tobj, rhs, weight):
         """
-            Given a totalizer sum and its right-hand side to be
-            enforced, the method creates a new sum assumption literal,
-            which will be used in the following SAT oracle calls.
+            Given a totalizer sum, its right-hand side to be enforced, and a
+            weight, the method creates a new sum assumption literal, which
+            will be used in the following SAT oracle calls.
 
             :param tobj: totalizer sum
             :param rhs: right-hand side
+            :param weight: numeric weight of the assumption
 
             :type tobj: :class:`.ITotalizer`
             :type rhs: int
+            :type weight: int
         """
 
         # saving the sum and its weight in a mapping
         self.tobj[-tobj.rhs[rhs]] = tobj
         self.bnds[-tobj.rhs[rhs]] = rhs
         self.wght[-tobj.rhs[rhs]] = weight
         self.swgt[-tobj.rhs[rhs]] = weight
```

### Comparing `python-sat-0.1.8.dev4/examples/usage.py` & `python-sat-0.1.8.dev5/examples/usage.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/pysat/__init__.py` & `python-sat-0.1.8.dev5/pysat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ##  Created on: Mar 4, 2017
 ##      Author: Alexey S. Ignatiev
 ##      E-mail: aignatiev@ciencias.ulisboa.pt
 ##
 
 # current version
 #==============================================================================
-VERSION = (0, 1, 8, "dev", 4)
+VERSION = (0, 1, 8, "dev", 5)
 
 
 # PEP440 Format
 #==============================================================================
 __version__ = "%d.%d.%d.%s%d" % VERSION if len(VERSION) == 5 else \
               "%d.%d.%d" % VERSION
```

### Comparing `python-sat-0.1.8.dev4/pysat/_fileio.py` & `python-sat-0.1.8.dev5/pysat/_fileio.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/pysat/_utils.py` & `python-sat-0.1.8.dev5/pysat/_utils.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/pysat/card.py` & `python-sat-0.1.8.dev5/pysat/card.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/pysat/formula.py` & `python-sat-0.1.8.dev5/pysat/formula.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/pysat/pb.py` & `python-sat-0.1.8.dev5/pysat/pb.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/pysat/process.py` & `python-sat-0.1.8.dev5/pysat/process.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/pysat/solvers.py` & `python-sat-0.1.8.dev5/pysat/solvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -630,15 +630,15 @@
 
     def prop_budget(self, budget=-1):
         """
             Set limit (i.e. the upper bound) on the number of propagations in
             the next limited SAT call (see :meth:`solve_limited`). The limit
             value is given as a ``budget`` variable and is an integer greater
             than ``0``. If the budget is set to ``0`` or ``-1``, the upper
-            bound on the number of conflicts is disabled.
+            bound on the number of propagations is disabled.
 
             :param budget: the upper bound on the number of propagations.
             :type budget: int
 
             Example:
 
             .. code-block:: python
@@ -654,14 +654,47 @@
                 None
                 >>> m.delete()
         """
 
         if self.solver:
             self.solver.prop_budget(budget)
 
+    def dec_budget(self, budget):
+        """
+            Set limit (i.e. the upper bound) on the number of decisions in
+            the next limited SAT call (see :meth:`solve_limited`). The limit
+            value is given as a ``budget`` variable and is an integer greater
+            than ``0``. If the budget is set to ``0`` or ``-1``, the upper
+            bound on the number of decisions is disabled.
+
+            Note that this functionality is supported by :class:`Cadical103`
+            and :class:`Cadical153` only!
+
+            :param budget: the upper bound on the number of decisions.
+            :type budget: int
+
+            Example:
+
+            .. code-block:: python
+
+                >>> from pysat.solvers import Cadical153
+                >>> from pysat.examples.genhard import Parity
+                >>>
+                >>> cnf = Parity(size=10)  # too hard for a SAT solver
+                >>> c = Cadical153(bootstrap_with=cnf.clauses)
+                >>>
+                >>> c.dec_budget(500)  # doing at most 500 decisions
+                >>> print(c.solve_limited())  # making a limited oracle call
+                None
+                >>> c.delete()
+        """
+
+        if self.solver:
+            self.solver.dec_budget(budget)
+
     def interrupt(self):
         """
             Interrupt the execution of the current *limited* SAT call (see
             :meth:`solve_limited`). Can be used to enforce time limits using
             timer objects. The interrupt must be cleared before performing
             another SAT call (see :meth:`clear_interrupt`).
 
@@ -1302,42 +1335,64 @@
             if self.use_timer:
                 self.call_time = process_time() - start_time
                 self.accu_time += self.call_time
 
             self.prev_assumps = assumptions
             return self.status
 
-    def start_mode(self, warm=False):
-        """
-            Set start mode: either warm or standard.
-        """
-
-        raise NotImplementedError('Warm-start mode is currently unsupported by CaDiCaL.')
-
     def solve_limited(self, assumptions=[], expect_interrupt=False):
         """
             Solve internal formula using given budgets for conflicts and
-            propagations.
+            decisions.
         """
 
-        raise NotImplementedError('Limited solve is currently unsupported by CaDiCaL.')
+        if self.cadical:
+            if self.use_timer:
+                 start_time = process_time()
+
+            self.status = pysolvers.cadical103_solve_lim(self.cadical,
+                    assumptions, int(MainThread.check()))
+
+            self.status = None if self.status == 0 else bool((self.status + 1) / 2)
+
+            if self.use_timer:
+                self.call_time = process_time() - start_time
+                self.accu_time += self.call_time
+
+            return self.status
 
     def conf_budget(self, budget):
         """
             Set limit on the number of conflicts.
         """
 
-        raise NotImplementedError('Limited solve is currently unsupported by CaDiCaL.')
+        if self.cadical:
+            pysolvers.cadical103_cbudget(self.cadical, budget)
+
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        if self.cadical:
+            pysolvers.cadical103_dbudget(self.cadical, budget)
+
+    def start_mode(self, warm=False):
+        """
+            Set start mode: either warm or standard.
+        """
+
+        raise NotImplementedError('Warm-start mode is currently unsupported by CaDiCaL.')
 
     def prop_budget(self, budget):
         """
             Set limit on the number of propagations.
         """
 
-        raise NotImplementedError('Limited solve is currently unsupported by CaDiCaL.')
+        raise NotImplementedError('Limit on propagations is currently unsupported by CaDiCaL.')
 
     def interrupt(self):
         """
             Interrupt solver execution.
         """
 
         raise NotImplementedError('Limited solve is currently unsupported by CaDiCaL.')
@@ -1598,14 +1653,51 @@
             if self.use_timer:
                 self.call_time = process_time() - start_time
                 self.accu_time += self.call_time
 
             self.prev_assumps = assumptions
             return self.status
 
+    def solve_limited(self, assumptions=[], expect_interrupt=False):
+        """
+            Solve internal formula using given budgets for conflicts and
+            decisions.
+        """
+
+        if self.cadical:
+            if self.use_timer:
+                 start_time = process_time()
+
+            self.status = pysolvers.cadical153_solve_lim(self.cadical,
+                    assumptions, int(MainThread.check()))
+
+            self.status = None if self.status == 0 else bool((self.status + 1) / 2)
+
+            if self.use_timer:
+                self.call_time = process_time() - start_time
+                self.accu_time += self.call_time
+
+            return self.status
+
+    def conf_budget(self, budget):
+        """
+            Set limit on the number of conflicts.
+        """
+
+        if self.cadical:
+            pysolvers.cadical153_cbudget(self.cadical, budget)
+
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        if self.cadical:
+            pysolvers.cadical153_dbudget(self.cadical, budget)
+
     def process(self, rounds=1, block=False, cover=False, condition=False,
                 decompose=True, elim=True, probe=True, probehbr=True,
                 subsume=True, vivify=True):
         """
             Apply the preprocessor for the internal formula. See the
             documentation for the ``process`` module for details.
         """
@@ -1632,35 +1724,20 @@
     def start_mode(self, warm=False):
         """
             Set start mode: either warm or standard.
         """
 
         raise NotImplementedError('Warm-start mode is currently unsupported by CaDiCaL.')
 
-    def solve_limited(self, assumptions=[], expect_interrupt=False):
-        """
-            Solve internal formula using given budgets for conflicts and
-            propagations.
-        """
-
-        raise NotImplementedError('Limited solve is currently unsupported by CaDiCaL.')
-
-    def conf_budget(self, budget):
-        """
-            Set limit on the number of conflicts.
-        """
-
-        raise NotImplementedError('Limited solve is currently unsupported by CaDiCaL.')
-
     def prop_budget(self, budget):
         """
             Set limit on the number of propagations.
         """
 
-        raise NotImplementedError('Limited solve is currently unsupported by CaDiCaL.')
+        raise NotImplementedError('Limit on propagations is currently unsupported by CaDiCaL.')
 
     def interrupt(self):
         """
             Interrupt solver execution.
         """
 
         raise NotImplementedError('Limited solve is currently unsupported by CaDiCaL.')
@@ -1966,14 +2043,21 @@
         """
             Set limit on the number of propagations.
         """
 
         if self.gluecard:
             pysolvers.gluecard3_pbudget(self.gluecard, budget)
 
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        raise NotImplementedError('Limit on decisions is unsupported by Gluecard3.')
+
     def interrupt(self):
         """
             Interrupt solver execution.
         """
 
         if self.gluecard:
             pysolvers.gluecard3_interrupt(self.gluecard)
@@ -2298,14 +2382,21 @@
         """
             Set limit on the number of propagations.
         """
 
         if self.gluecard:
             pysolvers.gluecard41_pbudget(self.gluecard, budget)
 
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        raise NotImplementedError('Limit on decisions is unsupported by Gluecard4.')
+
     def interrupt(self):
         """
             Interrupt solver execution.
         """
 
         if self.gluecard:
             pysolvers.gluecard41_interrupt(self.gluecard)
@@ -2630,14 +2721,21 @@
         """
             Set limit on the number of propagations.
         """
 
         if self.glucose:
             pysolvers.glucose3_pbudget(self.glucose, budget)
 
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        raise NotImplementedError('Limit on decisions is unsupported by Glucose3.')
+
     def interrupt(self):
         """
             Interrupt solver execution.
         """
 
         if self.glucose:
             pysolvers.glucose3_interrupt(self.glucose)
@@ -2954,14 +3052,21 @@
         """
             Set limit on the number of propagations.
         """
 
         if self.glucose:
             pysolvers.glucose41_pbudget(self.glucose, budget)
 
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        raise NotImplementedError('Limit on decisions is unsupported by Glucose4.')
+
     def interrupt(self):
         """
             Interrupt solver execution.
         """
 
         if self.glucose:
             pysolvers.glucose41_interrupt(self.glucose)
@@ -3262,14 +3367,21 @@
     def prop_budget(self, budget):
         """
             Set limit on the number of propagations.
         """
 
         raise NotImplementedError('Limited solve is currently unsupported by Lingeling.')
 
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        raise NotImplementedError('Limited solve is currently unsupported by Lingeling.')
+
     def interrupt(self):
         """
             Interrupt solver execution.
         """
 
         raise NotImplementedError('Limited solve is currently unsupported by Lingeling.')
 
@@ -3555,14 +3667,21 @@
         """
             Set limit on the number of propagations.
         """
 
         if self.maplesat:
             pysolvers.maplechrono_pbudget(self.maplesat, budget)
 
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        raise NotImplementedError('Limit on decisions is unsupported by MapleChrono.')
+
     def interrupt(self):
         """
             Interrupt solver execution.
         """
 
         if self.maplesat:
             pysolvers.maplechrono_interrupt(self.maplesat)
@@ -3877,14 +3996,21 @@
         """
             Set limit on the number of propagations.
         """
 
         if self.maplesat:
             pysolvers.maplecm_pbudget(self.maplesat, budget)
 
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        raise NotImplementedError('Limit on decisions is unsupported by MapleCM.')
+
     def interrupt(self):
         """
             Interrupt solver execution.
         """
 
         if self.maplesat:
             pysolvers.maplecm_interrupt(self.maplesat)
@@ -4199,14 +4325,21 @@
         """
             Set limit on the number of propagations.
         """
 
         if self.maplesat:
             pysolvers.maplesat_pbudget(self.maplesat, budget)
 
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        raise NotImplementedError('Limit on decisions is unsupported by Maplesat.')
+
     def interrupt(self):
         """
             Interrupt solver execution.
         """
 
         if self.maplesat:
             pysolvers.maplesat_interrupt(self.maplesat)
@@ -4504,14 +4637,21 @@
         """
             Set limit on the number of propagations.
         """
 
         if self.mergesat:
             pysolvers.mergesat3_pbudget(self.mergesat, budget)
 
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        raise NotImplementedError('Limit on decisions is unsupported by Mergesat3.')
+
     def interrupt(self):
         """
             Interrupt solver execution.
         """
 
         if self.mergesat:
             pysolvers.mergesat3_interrupt(self.mergesat)
@@ -4818,14 +4958,21 @@
         """
             Set limit on the number of propagations.
         """
 
         if self.minicard:
             pysolvers.minicard_pbudget(self.minicard, budget)
 
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        raise NotImplementedError('Limit on decisions is unsupported by Minicard.')
+
     def interrupt(self):
         """
             Interrupt solver execution.
         """
 
         if self.minicard:
             pysolvers.minicard_interrupt(self.minicard)
@@ -5140,14 +5287,21 @@
         """
             Set limit on the number of propagations.
         """
 
         if self.minisat:
             pysolvers.minisat22_pbudget(self.minisat, budget)
 
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        raise NotImplementedError('Limit on decisions is unsupported by Minisat22.')
+
     def interrupt(self):
         """
             Interrupt solver execution.
         """
 
         if self.minisat:
             pysolvers.minisat22_interrupt(self.minisat)
@@ -5454,14 +5608,21 @@
         """
             Set limit on the number of propagations.
         """
 
         if self.minisat:
             pysolvers.minisatgh_pbudget(self.minisat, budget)
 
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        raise NotImplementedError('Limit on decisions is unsupported by MinisatGH.')
+
     def interrupt(self):
         """
             Interrupt solver execution.
         """
 
         if self.minisat:
             pysolvers.minisatgh_interrupt(self.minisat)
```

### Comparing `python-sat-0.1.8.dev4/python_sat.egg-info/PKG-INFO` & `python-sat-0.1.8.dev5/python_sat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 0.1.8.dev4
+Version: 0.1.8.dev5
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: aiger
```

### Comparing `python-sat-0.1.8.dev4/python_sat.egg-info/SOURCES.txt` & `python-sat-0.1.8.dev5/python_sat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/setup.py` & `python-sat-0.1.8.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/cadical103.tar.gz` & `python-sat-0.1.8.dev5/solvers/cadical103.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/cadical153.tar.gz` & `python-sat-0.1.8.dev5/solvers/cadical153.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/glucose30.tar.gz` & `python-sat-0.1.8.dev5/solvers/glucose30.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/glucose41.tar.gz` & `python-sat-0.1.8.dev5/solvers/glucose41.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/lingeling.tar.gz` & `python-sat-0.1.8.dev5/solvers/lingeling.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/maplechrono.zip` & `python-sat-0.1.8.dev5/solvers/maplechrono.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/maplecm.zip` & `python-sat-0.1.8.dev5/solvers/maplecm.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/maplesat.zip` & `python-sat-0.1.8.dev5/solvers/maplesat.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/mergesat3.tar.gz` & `python-sat-0.1.8.dev5/solvers/mergesat3.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/minicard.tar.gz` & `python-sat-0.1.8.dev5/solvers/minicard.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/minisat22.tar.gz` & `python-sat-0.1.8.dev5/solvers/minisat22.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/minisatgh.zip` & `python-sat-0.1.8.dev5/solvers/minisatgh.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/patches/cadical103.patch` & `python-sat-0.1.8.dev5/solvers/patches/cadical103.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/patches/cadical153.patch` & `python-sat-0.1.8.dev5/solvers/patches/cadical153.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/patches/glucose30.patch` & `python-sat-0.1.8.dev5/solvers/patches/glucose30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/patches/glucose41.patch` & `python-sat-0.1.8.dev5/solvers/patches/glucose41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/patches/gluecard30.patch` & `python-sat-0.1.8.dev5/solvers/patches/gluecard30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/patches/gluecard41.patch` & `python-sat-0.1.8.dev5/solvers/patches/gluecard41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/patches/lingeling.patch` & `python-sat-0.1.8.dev5/solvers/patches/lingeling.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/patches/maplechrono.patch` & `python-sat-0.1.8.dev5/solvers/patches/maplechrono.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/patches/maplecm.patch` & `python-sat-0.1.8.dev5/solvers/patches/maplecm.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/patches/maplesat.patch` & `python-sat-0.1.8.dev5/solvers/patches/maplesat.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/patches/mergesat3.patch` & `python-sat-0.1.8.dev5/solvers/patches/mergesat3.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/patches/minicard.patch` & `python-sat-0.1.8.dev5/solvers/patches/minicard.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/patches/minisat22.patch` & `python-sat-0.1.8.dev5/solvers/patches/minisat22.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/patches/minisatgh.patch` & `python-sat-0.1.8.dev5/solvers/patches/minisatgh.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/prepare.py` & `python-sat-0.1.8.dev5/solvers/prepare.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/solvers/pysolvers.cc` & `python-sat-0.1.8.dev5/solvers/pysolvers.cc`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,16 @@
                                     "the CaDiCaL 1.5.3 preprocessor";
 static char   restore_docstring[] = "Reconstruct the model to a CNF formula "
                                     "from the model for its processed version";
 static char      prop_docstring[] = "Propagate a given set of literals.";
 static char    phases_docstring[] = "Set variable polarities.";
 static char   cbudget_docstring[] = "Set limit on the number of conflicts.";
 static char   pbudget_docstring[] = "Set limit on the number of propagations.";
+static char   dbudget_docstring[] = "Set limit on the number of decisions "
+                                    "(CaDiCaL only).";
 static char interrupt_docstring[] = "Interrupt SAT solver execution "
                                     "(not supported by lingeling and CaDiCaL).";
 static char  clearint_docstring[] = "Clear interrupt indicator flag.";
 static char   setincr_docstring[] = "Set incremental mode (for Glucose3 only).";
 static char   tracepr_docstring[] = "Trace resolution proof.";
 static char      core_docstring[] = "Get an unsatisfiable core if formula is UNSAT.";
 static char     model_docstring[] = "Get a model if formula is SAT.";
@@ -112,28 +114,35 @@
 // function declaration for functions available in module
 //=============================================================================
 extern "C" {
 #ifdef WITH_CADICAL103
 	static PyObject *py_cadical103_new       (PyObject *, PyObject *);
 	static PyObject *py_cadical103_add_cl    (PyObject *, PyObject *);
 	static PyObject *py_cadical103_solve     (PyObject *, PyObject *);
+	static PyObject *py_cadical103_solve_lim (PyObject *, PyObject *);
+	static PyObject *py_cadical103_cbudget   (PyObject *, PyObject *);
+	static PyObject *py_cadical103_dbudget   (PyObject *, PyObject *);
 	static PyObject *py_cadical103_tracepr   (PyObject *, PyObject *);
 	static PyObject *py_cadical103_core      (PyObject *, PyObject *);
 	static PyObject *py_cadical103_model     (PyObject *, PyObject *);
 	static PyObject *py_cadical103_nof_vars  (PyObject *, PyObject *);
 	static PyObject *py_cadical103_nof_cls   (PyObject *, PyObject *);
 	static PyObject *py_cadical103_del       (PyObject *, PyObject *);
 	static PyObject *py_cadical103_acc_stats (PyObject *, PyObject *);
 #endif
 #ifdef WITH_CADICAL153
 	static PyObject *py_cadical153_new       (PyObject *, PyObject *);
 	static PyObject *py_cadical153_add_cl    (PyObject *, PyObject *);
 	static PyObject *py_cadical153_process   (PyObject *, PyObject *);
 	static PyObject *py_cadical153_restore   (PyObject *, PyObject *);
 	static PyObject *py_cadical153_solve     (PyObject *, PyObject *);
+	static PyObject *py_cadical153_solve_lim (PyObject *, PyObject *);
+	/* static PyObject *py_cadical153_setphases (PyObject *, PyObject *); */
+	static PyObject *py_cadical153_cbudget   (PyObject *, PyObject *);
+	static PyObject *py_cadical153_dbudget   (PyObject *, PyObject *);
 	static PyObject *py_cadical153_tracepr   (PyObject *, PyObject *);
 	static PyObject *py_cadical153_core      (PyObject *, PyObject *);
 	static PyObject *py_cadical153_model     (PyObject *, PyObject *);
 	static PyObject *py_cadical153_nof_vars  (PyObject *, PyObject *);
 	static PyObject *py_cadical153_nof_cls   (PyObject *, PyObject *);
 	static PyObject *py_cadical153_del       (PyObject *, PyObject *);
 	static PyObject *py_cadical153_acc_stats (PyObject *, PyObject *);
@@ -377,26 +386,33 @@
 // module specification
 //=============================================================================
 static PyMethodDef module_methods[] = {
 #ifdef WITH_CADICAL103
 	{ "cadical103_new",       py_cadical103_new,       METH_VARARGS,      new_docstring },
 	{ "cadical103_add_cl",    py_cadical103_add_cl,    METH_VARARGS,    addcl_docstring },
 	{ "cadical103_solve",     py_cadical103_solve,     METH_VARARGS,    solve_docstring },
+	{ "cadical103_solve_lim", py_cadical103_solve_lim, METH_VARARGS,      lim_docstring },
+	{ "cadical103_cbudget",   py_cadical103_cbudget,   METH_VARARGS,  cbudget_docstring },
+	{ "cadical103_dbudget",   py_cadical103_dbudget,   METH_VARARGS,  dbudget_docstring },
 	{ "cadical103_tracepr",   py_cadical103_tracepr,   METH_VARARGS,  tracepr_docstring },
 	{ "cadical103_core",      py_cadical103_core,      METH_VARARGS,     core_docstring },
 	{ "cadical103_model",     py_cadical103_model,     METH_VARARGS,    model_docstring },
 	{ "cadical103_nof_vars",  py_cadical103_nof_vars,  METH_VARARGS,    nvars_docstring },
 	{ "cadical103_nof_cls",   py_cadical103_nof_cls,   METH_VARARGS,     ncls_docstring },
 	{ "cadical103_del",       py_cadical103_del,       METH_VARARGS,      del_docstring },
 	{ "cadical103_acc_stats", py_cadical103_acc_stats, METH_VARARGS, acc_stat_docstring },
 #endif
 #ifdef WITH_CADICAL153
 	{ "cadical153_new",       py_cadical153_new,       METH_VARARGS,      new_docstring },
 	{ "cadical153_add_cl",    py_cadical153_add_cl,    METH_VARARGS,    addcl_docstring },
 	{ "cadical153_solve",     py_cadical153_solve,     METH_VARARGS,    solve_docstring },
+	{ "cadical153_solve_lim", py_cadical153_solve_lim, METH_VARARGS,      lim_docstring },
+	/* { "cadical153_setphases", py_cadical153_setphases, METH_VARARGS,   phases_docstring }, */
+	{ "cadical153_cbudget",   py_cadical153_cbudget,   METH_VARARGS,  cbudget_docstring },
+	{ "cadical153_dbudget",   py_cadical153_dbudget,   METH_VARARGS,  dbudget_docstring },
 	{ "cadical153_process",   py_cadical153_process,   METH_VARARGS,  process_docstring },
 	{ "cadical153_restore",   py_cadical153_restore,   METH_VARARGS,  restore_docstring },
 	{ "cadical153_tracepr",   py_cadical153_tracepr,   METH_VARARGS,  tracepr_docstring },
 	{ "cadical153_core",      py_cadical153_core,      METH_VARARGS,     core_docstring },
 	{ "cadical153_model",     py_cadical153_model,     METH_VARARGS,    model_docstring },
 	{ "cadical153_nof_vars",  py_cadical153_nof_vars,  METH_VARARGS,    nvars_docstring },
 	{ "cadical153_nof_cls",   py_cadical153_nof_cls,   METH_VARARGS,     ncls_docstring },
@@ -975,14 +991,121 @@
 
 	PyObject *ret = PyBool_FromLong((long)res);
 	return ret;
 }
 
 //
 //=============================================================================
+static PyObject *py_cadical103_solve_lim(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	PyObject *a_obj;  // assumptions
+	int main_thread;
+
+	if (!PyArg_ParseTuple(args, "OOi", &s_obj, &a_obj, &main_thread))
+		return NULL;
+
+	// get pointer to solver
+	CaDiCaL103::Solver *s = (CaDiCaL103::Solver *)pyobj_to_void(s_obj);
+
+	// assumptions iterator
+	PyObject *i_obj = PyObject_GetIter(a_obj);
+	if (i_obj == NULL) {
+		PyErr_SetString(PyExc_RuntimeError,
+				"Object does not seem to be an iterable.");
+		return NULL;
+	}
+
+	PyObject *l_obj;
+	while ((l_obj = PyIter_Next(i_obj)) != NULL) {
+		if (!pyint_check(l_obj)) {
+			Py_DECREF(l_obj);
+			Py_DECREF(i_obj);
+			PyErr_SetString(PyExc_TypeError, "integer expected");
+			return NULL;
+		}
+
+		int l = pyint_to_cint(l_obj);
+		Py_DECREF(l_obj);
+
+		if (l == 0) {
+			Py_DECREF(i_obj);
+			PyErr_SetString(PyExc_ValueError, "non-zero integer expected");
+			return NULL;
+		}
+
+		s->assume(l);
+	}
+
+	Py_DECREF(i_obj);
+
+	PyOS_sighandler_t sig_save;
+	if (main_thread) {
+		sig_save = PyOS_setsig(SIGINT, sigint_handler);
+
+		if (setjmp(env) != 0) {
+			PyErr_SetString(SATError, "Caught keyboard interrupt");
+			return NULL;
+		}
+	}
+
+	int res = s->solve();
+	res = (res == 10 ? 1 : (res == 20 ? -1 : 0));
+
+	if (main_thread)
+		PyOS_setsig(SIGINT, sig_save);
+
+	PyObject *ret = pyint_from_cint(res);
+	return ret;
+}
+
+//
+//=============================================================================
+static PyObject *py_cadical103_cbudget(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	int64_t budget;
+
+	if (!PyArg_ParseTuple(args, "Ol", &s_obj, &budget))
+		return NULL;
+
+	// get pointer to solver
+	CaDiCaL103::Solver *s = (CaDiCaL103::Solver *)pyobj_to_void(s_obj);
+
+	if (budget != 0 && budget != -1)  // it is 0 by default
+		s->limit("conflicts", (int)budget);
+	else
+		s->limit("conflicts", -1);
+
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
+static PyObject *py_cadical103_dbudget(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	int64_t budget;
+
+	if (!PyArg_ParseTuple(args, "Ol", &s_obj, &budget))
+		return NULL;
+
+	// get pointer to solver
+	CaDiCaL103::Solver *s = (CaDiCaL103::Solver *)pyobj_to_void(s_obj);
+
+	if (budget != 0 && budget != -1)  // it is 0 by default
+		s->limit("decisions", (int)budget);
+	else
+		s->limit("decisions", -1);
+
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
 static PyObject *py_cadical103_core(PyObject *self, PyObject *args)
 {
 	PyObject *s_obj;
 	PyObject *a_obj;  // assumptions
 
 	if (!PyArg_ParseTuple(args, "OO", &s_obj, &a_obj))
 		return NULL;
@@ -1405,14 +1528,167 @@
 
 	PyObject *ret = PyBool_FromLong((long)res);
 	return ret;
 }
 
 //
 //=============================================================================
+static PyObject *py_cadical153_solve_lim(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	PyObject *a_obj;  // assumptions
+	int main_thread;
+
+	if (!PyArg_ParseTuple(args, "OOi", &s_obj, &a_obj, &main_thread))
+		return NULL;
+
+	// get pointer to solver
+	CaDiCaL153::Solver *s = (CaDiCaL153::Solver *)pyobj_to_void(s_obj);
+
+	// assumptions iterator
+	PyObject *i_obj = PyObject_GetIter(a_obj);
+	if (i_obj == NULL) {
+		PyErr_SetString(PyExc_RuntimeError,
+				"Object does not seem to be an iterable.");
+		return NULL;
+	}
+
+	PyObject *l_obj;
+	while ((l_obj = PyIter_Next(i_obj)) != NULL) {
+		if (!pyint_check(l_obj)) {
+			Py_DECREF(l_obj);
+			Py_DECREF(i_obj);
+			PyErr_SetString(PyExc_TypeError, "integer expected");
+			return NULL;
+		}
+
+		int l = pyint_to_cint(l_obj);
+		Py_DECREF(l_obj);
+
+		if (l == 0) {
+			Py_DECREF(i_obj);
+			PyErr_SetString(PyExc_ValueError, "non-zero integer expected");
+			return NULL;
+		}
+
+		s->assume(l);
+	}
+
+	Py_DECREF(i_obj);
+
+	PyOS_sighandler_t sig_save;
+	if (main_thread) {
+		sig_save = PyOS_setsig(SIGINT, sigint_handler);
+
+		if (setjmp(env) != 0) {
+			PyErr_SetString(SATError, "Caught keyboard interrupt");
+			return NULL;
+		}
+	}
+
+	int res = s->solve();
+	res = (res == 10 ? 1 : (res == 20 ? -1 : 0));
+
+	if (main_thread)
+		PyOS_setsig(SIGINT, sig_save);
+
+	PyObject *ret = pyint_from_cint(res);
+	return ret;
+}
+
+// calling phase() does not seem to work for now!
+//=============================================================================
+/* static PyObject *py_cadical153_setphases(PyObject *self, PyObject *args) */
+/* { */
+/* 	PyObject *s_obj; */
+/* 	PyObject *p_obj;  // polarities given as a list of integer literals */
+
+/* 	if (!PyArg_ParseTuple(args, "OO", &s_obj, &p_obj)) */
+/* 		return NULL; */
+
+/* 	// get pointer to solver */
+/* 	CaDiCaL153::Solver *s = (CaDiCaL153::Solver *)pyobj_to_void(s_obj); */
+
+/* 	// assumptions iterator */
+/* 	PyObject *i_obj = PyObject_GetIter(p_obj); */
+/* 	if (i_obj == NULL) { */
+/* 		PyErr_SetString(PyExc_RuntimeError, */
+/* 				"Object does not seem to be an iterable."); */
+/* 		return NULL; */
+/* 	} */
+
+/* 	PyObject *l_obj; */
+/* 	while ((l_obj = PyIter_Next(i_obj)) != NULL) { */
+/* 		if (!pyint_check(l_obj)) { */
+/* 			Py_DECREF(l_obj); */
+/* 			Py_DECREF(i_obj); */
+/* 			PyErr_SetString(PyExc_TypeError, "integer expected"); */
+/* 			return NULL; */
+/* 		} */
+
+/* 		int l = pyint_to_cint(l_obj); */
+/* 		Py_DECREF(l_obj); */
+
+/* 		if (l == 0) { */
+/* 			Py_DECREF(i_obj); */
+/* 			PyErr_SetString(PyExc_ValueError, "non-zero integer expected"); */
+/* 			return NULL; */
+/* 		} */
+
+/* 		s->phase(l); */
+/* 	} */
+
+/* 	Py_DECREF(i_obj); */
+/* 	Py_RETURN_NONE; */
+/* } */
+
+//
+//=============================================================================
+static PyObject *py_cadical153_cbudget(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	int64_t budget;
+
+	if (!PyArg_ParseTuple(args, "Ol", &s_obj, &budget))
+		return NULL;
+
+	// get pointer to solver
+	CaDiCaL153::Solver *s = (CaDiCaL153::Solver *)pyobj_to_void(s_obj);
+
+	if (budget != 0 && budget != -1)  // it is 0 by default
+		s->limit("conflicts", (int)budget);
+	else
+		s->limit("conflicts", -1);
+
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
+static PyObject *py_cadical153_dbudget(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	int64_t budget;
+
+	if (!PyArg_ParseTuple(args, "Ol", &s_obj, &budget))
+		return NULL;
+
+	// get pointer to solver
+	CaDiCaL153::Solver *s = (CaDiCaL153::Solver *)pyobj_to_void(s_obj);
+
+	if (budget != 0 && budget != -1)  // it is 0 by default
+		s->limit("decisions", (int)budget);
+	else
+		s->limit("decisions", -1);
+
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
 static PyObject *py_cadical153_core(PyObject *self, PyObject *args)
 {
 	PyObject *s_obj;
 	PyObject *a_obj;  // assumptions
 
 	if (!PyArg_ParseTuple(args, "OO", &s_obj, &a_obj))
 		return NULL;
```

### Comparing `python-sat-0.1.8.dev4/tests/test_accum_stats.py` & `python-sat-0.1.8.dev5/tests/test_accum_stats.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/tests/test_atmost1.py` & `python-sat-0.1.8.dev5/tests/test_atmost1.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/tests/test_atmostk.py` & `python-sat-0.1.8.dev5/tests/test_atmostk.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/tests/test_cnfplus.py` & `python-sat-0.1.8.dev5/tests/test_cnfplus.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/tests/test_equals1.py` & `python-sat-0.1.8.dev5/tests/test_equals1.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/tests/test_process.py` & `python-sat-0.1.8.dev5/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/tests/test_unique_model.py` & `python-sat-0.1.8.dev5/tests/test_unique_model.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/tests/test_unique_mus.py` & `python-sat-0.1.8.dev5/tests/test_unique_mus.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev4/tests/test_warmstart.py` & `python-sat-0.1.8.dev5/tests/test_warmstart.py`

 * *Files identical despite different names*

