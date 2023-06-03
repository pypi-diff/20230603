# Comparing `tmp/PySupercell-0.0.4.tar.gz` & `tmp/PySupercell-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySupercell-0.0.4.tar", last modified: Sat Jun  3 14:51:34 2023, max compression
+gzip compressed data, was "PySupercell-0.0.5.tar", last modified: Sat Jun  3 15:43:00 2023, max compression
```

## Comparing `PySupercell-0.0.4.tar` & `PySupercell-0.0.5.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:51:34.207877 PySupercell-0.0.4/
--rwxrw-r--   0 zsh       (1000) zsh       (1000)     1058 2023-06-03 11:10:34.000000 PySupercell-0.0.4/LICENSE.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      294 2023-06-03 11:24:12.000000 PySupercell-0.0.4/MANIFEST.in
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      484 2023-06-03 14:51:34.207877 PySupercell-0.0.4/PKG-INFO
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:51:34.199877 PySupercell-0.0.4/PySupercell.egg-info/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      484 2023-06-03 14:51:34.000000 PySupercell-0.0.4/PySupercell.egg-info/PKG-INFO
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     1017 2023-06-03 14:51:34.000000 PySupercell-0.0.4/PySupercell.egg-info/SOURCES.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-06-03 14:51:34.000000 PySupercell-0.0.4/PySupercell.egg-info/dependency_links.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       33 2023-06-03 14:51:34.000000 PySupercell-0.0.4/PySupercell.egg-info/requires.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       92 2023-06-03 14:51:34.000000 PySupercell-0.0.4/PySupercell.egg-info/top_level.txt
--rw-r--r--   0 zsh       (1000) zsh       (1000)     2282 2023-06-03 13:25:16.000000 PySupercell-0.0.4/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:51:34.199877 PySupercell-0.0.4/bin/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)    10109 2023-06-03 14:33:14.000000 PySupercell-0.0.4/bin/pysc.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     9870 2023-06-03 14:48:56.000000 PySupercell-0.0.4/bin/v2qe.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:51:34.199877 PySupercell-0.0.4/examples/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      266 2023-06-03 13:05:58.000000 PySupercell-0.0.4/examples/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:51:34.199877 PySupercell-0.0.4/examples/example1/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      364 2023-06-03 11:32:21.000000 PySupercell-0.0.4/examples/example1/POSCAR
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      691 2023-06-03 14:49:50.000000 PySupercell-0.0.4/examples/example1/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:51:34.199877 PySupercell-0.0.4/examples/example1/reference/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      704 2023-06-03 11:32:28.000000 PySupercell-0.0.4/examples/example1/reference/POSCAR_redefine
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     1312 2023-06-03 12:58:44.000000 PySupercell-0.0.4/examples/example1/reference/POSCAR_slab
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:51:34.199877 PySupercell-0.0.4/examples/example2/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      437 2023-06-03 13:07:30.000000 PySupercell-0.0.4/examples/example2/POSCAR
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       40 2023-06-03 13:09:42.000000 PySupercell-0.0.4/examples/example2/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:51:34.199877 PySupercell-0.0.4/examples/example2/reference/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     9732 2023-06-03 13:09:46.000000 PySupercell-0.0.4/examples/example2/reference/POSCAR_sc
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     9738 2023-06-03 13:09:46.000000 PySupercell-0.0.4/examples/example2/reference/POSCAR_tube
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:51:34.203877 PySupercell-0.0.4/examples/example3/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      948 2023-06-03 14:16:16.000000 PySupercell-0.0.4/examples/example3/POSCAR
--rw-rw-r--   0 zsh       (1000) zsh       (1000)    54936 2023-06-03 14:23:45.000000 PySupercell-0.0.4/examples/example3/POSCAR_redefine
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      569 2023-06-03 14:16:10.000000 PySupercell-0.0.4/examples/example3/README
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     9854 2023-06-03 14:03:09.000000 PySupercell-0.0.4/examples/example3/make_screw_diamond.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:51:34.203877 PySupercell-0.0.4/examples/example3/reference/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)    44136 2023-06-03 14:01:17.000000 PySupercell-0.0.4/examples/example3/reference/POSCAR_redefine
--rw-rw-r--   0 zsh       (1000) zsh       (1000)    54957 2023-06-03 14:06:32.000000 PySupercell-0.0.4/examples/example3/reference/POSCAR_screw
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:51:34.203877 PySupercell-0.0.4/examples/example4/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      534 2023-06-03 13:02:08.000000 PySupercell-0.0.4/examples/example4/POSCAR
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      124 2023-06-03 13:04:39.000000 PySupercell-0.0.4/examples/example4/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:51:34.203877 PySupercell-0.0.4/examples/example4/reference/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     2176 2023-06-03 13:02:46.000000 PySupercell-0.0.4/examples/example4/reference/POSCAR_bending
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     2168 2023-06-03 13:02:46.000000 PySupercell-0.0.4/examples/example4/reference/POSCAR_flat
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:51:34.203877 PySupercell-0.0.4/pysupercell/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     8621 2023-06-03 10:12:44.000000 PySupercell-0.0.4/pysupercell/QE_ibrav_lib.py
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      293 2023-06-03 14:37:15.000000 PySupercell-0.0.4/pysupercell/__init__.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     4589 2023-06-03 13:26:30.000000 PySupercell-0.0.4/pysupercell/arguments.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)    44652 2023-06-03 14:37:08.000000 PySupercell-0.0.4/pysupercell/pysupercell.py
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-06-03 14:51:34.207877 PySupercell-0.0.4/setup.cfg
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3621 2023-06-03 14:51:27.000000 PySupercell-0.0.4/setup.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 14:51:34.207877 PySupercell-0.0.4/tests_basic/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       40 2023-06-03 10:27:02.000000 PySupercell-0.0.4/tests_basic/README
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       72 2023-06-03 10:30:27.000000 PySupercell-0.0.4/tests_basic/test_1.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.470323 PySupercell-0.0.5/
+-rwxrw-r--   0 zsh       (1000) zsh       (1000)     1058 2023-06-03 11:10:34.000000 PySupercell-0.0.5/LICENSE.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      294 2023-06-03 11:24:12.000000 PySupercell-0.0.5/MANIFEST.in
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      484 2023-06-03 15:43:00.470323 PySupercell-0.0.5/PKG-INFO
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.462323 PySupercell-0.0.5/PySupercell.egg-info/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      484 2023-06-03 15:43:00.000000 PySupercell-0.0.5/PySupercell.egg-info/PKG-INFO
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1076 2023-06-03 15:43:00.000000 PySupercell-0.0.5/PySupercell.egg-info/SOURCES.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-06-03 15:43:00.000000 PySupercell-0.0.5/PySupercell.egg-info/dependency_links.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       33 2023-06-03 15:43:00.000000 PySupercell-0.0.5/PySupercell.egg-info/requires.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       92 2023-06-03 15:43:00.000000 PySupercell-0.0.5/PySupercell.egg-info/top_level.txt
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     2282 2023-06-03 13:25:16.000000 PySupercell-0.0.5/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.462323 PySupercell-0.0.5/bin/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)    10109 2023-06-03 14:54:46.000000 PySupercell-0.0.5/bin/pysc.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)    10425 2023-06-03 15:13:38.000000 PySupercell-0.0.5/bin/v2qe.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.462323 PySupercell-0.0.5/examples/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      266 2023-06-03 13:05:58.000000 PySupercell-0.0.5/examples/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.466323 PySupercell-0.0.5/examples/example1/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      364 2023-06-03 11:32:21.000000 PySupercell-0.0.5/examples/example1/POSCAR
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      376 2023-06-03 15:13:42.000000 PySupercell-0.0.5/examples/example1/POSCAR_Primitive
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      691 2023-06-03 14:49:50.000000 PySupercell-0.0.5/examples/example1/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.466323 PySupercell-0.0.5/examples/example1/reference/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      704 2023-06-03 11:32:28.000000 PySupercell-0.0.5/examples/example1/reference/POSCAR_redefine
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1312 2023-06-03 12:58:44.000000 PySupercell-0.0.5/examples/example1/reference/POSCAR_slab
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      456 2023-06-03 15:13:45.000000 PySupercell-0.0.5/examples/example1/rx.in
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.466323 PySupercell-0.0.5/examples/example2/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      437 2023-06-03 13:07:30.000000 PySupercell-0.0.5/examples/example2/POSCAR
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       40 2023-06-03 13:09:42.000000 PySupercell-0.0.5/examples/example2/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.466323 PySupercell-0.0.5/examples/example2/reference/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     9732 2023-06-03 13:09:46.000000 PySupercell-0.0.5/examples/example2/reference/POSCAR_sc
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     9738 2023-06-03 13:09:46.000000 PySupercell-0.0.5/examples/example2/reference/POSCAR_tube
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.466323 PySupercell-0.0.5/examples/example3/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      948 2023-06-03 14:16:16.000000 PySupercell-0.0.5/examples/example3/POSCAR
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)    54936 2023-06-03 14:23:45.000000 PySupercell-0.0.5/examples/example3/POSCAR_redefine
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      569 2023-06-03 14:16:10.000000 PySupercell-0.0.5/examples/example3/README
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     9854 2023-06-03 14:03:09.000000 PySupercell-0.0.5/examples/example3/make_screw_diamond.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.466323 PySupercell-0.0.5/examples/example3/reference/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)    44136 2023-06-03 14:01:17.000000 PySupercell-0.0.5/examples/example3/reference/POSCAR_redefine
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)    54957 2023-06-03 14:06:32.000000 PySupercell-0.0.5/examples/example3/reference/POSCAR_screw
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.470323 PySupercell-0.0.5/examples/example4/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      534 2023-06-03 13:02:08.000000 PySupercell-0.0.5/examples/example4/POSCAR
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      124 2023-06-03 13:04:39.000000 PySupercell-0.0.5/examples/example4/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.470323 PySupercell-0.0.5/examples/example4/reference/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     2176 2023-06-03 13:02:46.000000 PySupercell-0.0.5/examples/example4/reference/POSCAR_bending
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     2168 2023-06-03 13:02:46.000000 PySupercell-0.0.5/examples/example4/reference/POSCAR_flat
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.470323 PySupercell-0.0.5/pysupercell/
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     8665 2023-06-03 15:06:12.000000 PySupercell-0.0.5/pysupercell/QE_ibrav_lib.py
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      293 2023-06-03 15:06:18.000000 PySupercell-0.0.5/pysupercell/__init__.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     4589 2023-06-03 13:26:30.000000 PySupercell-0.0.5/pysupercell/arguments.py
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)    44613 2023-06-03 15:41:34.000000 PySupercell-0.0.5/pysupercell/pysupercell.py
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-06-03 15:43:00.470323 PySupercell-0.0.5/setup.cfg
+-rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3621 2023-06-03 15:42:52.000000 PySupercell-0.0.5/setup.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.470323 PySupercell-0.0.5/tests_basic/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       40 2023-06-03 10:27:02.000000 PySupercell-0.0.5/tests_basic/README
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       72 2023-06-03 10:30:27.000000 PySupercell-0.0.5/tests_basic/test_1.py
```

### Comparing `PySupercell-0.0.4/LICENSE.txt` & `PySupercell-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/PySupercell.egg-info/SOURCES.txt` & `PySupercell-0.0.5/PySupercell.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 PySupercell.egg-info/dependency_links.txt
 PySupercell.egg-info/requires.txt
 PySupercell.egg-info/top_level.txt
 bin/pysc.py
 bin/v2qe.py
 examples/README.md
 examples/example1/POSCAR
+examples/example1/POSCAR_Primitive
 examples/example1/README.md
+examples/example1/rx.in
 examples/example1/reference/POSCAR_redefine
 examples/example1/reference/POSCAR_slab
 examples/example2/POSCAR
 examples/example2/README.md
 examples/example2/reference/POSCAR_sc
 examples/example2/reference/POSCAR_tube
 examples/example3/POSCAR
```

### Comparing `PySupercell-0.0.4/README.md` & `PySupercell-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/bin/pysc.py` & `PySupercell-0.0.5/bin/pysc.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/bin/v2qe.py` & `PySupercell-0.0.5/bin/v2qe.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 #  Dependence: pysupercell.py                                               #
 #  Usage:      convert the POSCAR file to part of input file for PWscf(QE)  #      
 #  Author:     Shunhong Zhang <szhang2@ustc.edu.cn>                         #
 #  Date:       Jun 03, 2023                                                 #
 #                                                                           #
 #===========================================================================#
 
-from astk.utility.dict_common import *
 import sys
 import numpy as np
+from pysupercell.QE_ibrav_lib import *
+from pysupercell import __version__
 from pysupercell.pysupercell import cryst_struct
 try: from termcolor import cprint,colored
 except: pass
 import os
+import shutil
 
 pyver=sys.version_info[0]
 
 Note='''
 This file can be used to generate input file for PWscf (Quantum ESPRESSO) by using VASP-POSCAR as input.
 The definition of primitive cell basis vectors follows the Quantum ESPRESSO code, please refer to:
 http://www.quantum-espresso.org/wp-content/uploads/Doc/INPUT_PW.html#idm6425376
@@ -227,9 +229,28 @@
 
     print ("\n{0}\nSample input for PWscf(Quantum ESPRESSO),Start\n{0}\n".format('-'*60))
     write_pwi(pw_setup_dic,ibrav,struct_std,struct_pm,filename=None)
     write_pwi(pw_setup_dic,ibrav,struct_std,struct_pm,filename="rx.in")
     print ("\n{0}\nSample input for PWscf(Quantum ESPRESSO),End\n{0}\n".format('-'*60))
     #struct._visualize_struct()
 
+    for file in ['BPOSCAR','PPOSCAR','phonopy_symm.yaml','POSCAR_standardized','POSCAR_for_symm_analysis']:
+        if os.path.isfile(file): os.remove(file)
+
+
+
+desc_str = 'Convert POSCAR into QE pwscf input'
+
 if __name__=='__main__':
+    try:
+        from pyfiglet import Figlet
+        f = Figlet()
+        pysc_text = f.renderText('PySupercell')
+        print (pysc_text)
+    except:
+        pass
+
+    print ('{:>53s}'.format('version {}\n'.format(__version__)))
+    try: cprint (desc_str,'green')
+    except: print (desc_str)
+
     main()
```

### Comparing `PySupercell-0.0.4/examples/example1/README.md` & `PySupercell-0.0.5/examples/example1/README.md`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/examples/example1/reference/POSCAR_redefine` & `PySupercell-0.0.5/examples/example1/reference/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/examples/example1/reference/POSCAR_slab` & `PySupercell-0.0.5/examples/example1/reference/POSCAR_slab`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/examples/example2/reference/POSCAR_sc` & `PySupercell-0.0.5/examples/example2/reference/POSCAR_sc`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/examples/example2/reference/POSCAR_tube` & `PySupercell-0.0.5/examples/example2/reference/POSCAR_tube`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/examples/example3/POSCAR` & `PySupercell-0.0.5/examples/example3/POSCAR`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/examples/example3/POSCAR_redefine` & `PySupercell-0.0.5/examples/example3/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/examples/example3/README` & `PySupercell-0.0.5/examples/example3/README`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/examples/example3/make_screw_diamond.py` & `PySupercell-0.0.5/examples/example3/make_screw_diamond.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/examples/example3/reference/POSCAR_redefine` & `PySupercell-0.0.5/examples/example3/reference/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/examples/example3/reference/POSCAR_screw` & `PySupercell-0.0.5/examples/example3/reference/POSCAR_screw`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/examples/example4/POSCAR` & `PySupercell-0.0.5/examples/example4/POSCAR`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/examples/example4/reference/POSCAR_bending` & `PySupercell-0.0.5/examples/example4/reference/POSCAR_bending`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/examples/example4/reference/POSCAR_flat` & `PySupercell-0.0.5/examples/example4/reference/POSCAR_flat`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/pysupercell/QE_ibrav_lib.py` & `PySupercell-0.0.5/pysupercell/QE_ibrav_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,32 +47,33 @@
     c=latt['c']
     alpha=latt['alpha']
     beta=latt['beta']
     gamma=latt['gamma']
     alpha_r, beta_r,gamma_r = np.deg2rad(alpha), np.deg2rad(beta), np.deg2rad(gamma)
     if angle_unit=='rad': alpha_r,beta_r,gamma_r = alpha,beta,gamma
     v1=[a,0,0]
-    v2=[b*cos(gamma_r),b*np.sin(gamma_r),0]
-    v3=[c*cos(beta_r),c*cos(beta_r)*cos(gamma_r)/np.sin(gamma_r),
-        c*np.sqrt( 1 + 2*cos(alpha_r)*cos(beta_r)*cos(gamma_r)- cos(alpha_r)**2 -cos(beta_r)**2-cos(gamma_r)**2)/np.sin(gamma_r)]
+    v2=[b*np.cos(gamma_r),b*np.sin(gamma_r),0]
+    v3=[c*np.cos(beta_r),
+        c*np.cos(beta_r)*np.cos(gamma_r)/np.sin(gamma_r),
+        c*np.sqrt( 1 + 2*np.cos(alpha_r)*np.cos(beta_r)*np.cos(gamma_r) - np.cos(alpha_r)**2 - np.cos(beta_r)**2-np.cos(gamma_r)**2)/np.sin(gamma_r)]
     cell = np.array([v1,v2,v3],float)
     return cell
 
 
 def get_connect(ibrav,spg,latt):
     connect_dic={
                   2 : np.array(([-1./2.,  0.0,1./2.],[   0.0,1./2.,1./2.],[-1./2., 1./2.,  0.0]),float),
                   3 : np.array(([1./2., 1./2.,1./2.],[-1./2.,1./2.,1./2.],[-1./2.,-1./2.,1./2.]),float),
                   7 : np.array(([1./2.,-1./2.,1./2.],[ 1./2.,1./2.,1./2.],[-1./2.,-1./2.,1./2.]),float),
                   9 : np.array(([1./2., 1./2.,  0.0],[-1./2.,1./2.,  0.0],[   0.0,   0.0,  1.0]),float),
                  -9 : np.array(([1./2.,-1./2.,  0.0],[ 1./2.,1./2.,1./2.],[   0.0,   0.0,  1.0]),float),
                  10 : np.array(([1./2.,   0.0,1./2.],[ 1./2.,1./2.,  0.0],[   0.0, 1./2.,1./2.]),float),
                  11 : np.array(([1./2., 1./2.,1./2.],[-1./2.,1./2.,1./2.],[-1./2.,-1./2.,1./2.]),float),
                  13 : np.array(([1./2,    0.0,-1./2],[ 0.0,    1.0,  0.0],[ 1./2.,  0.0,  1./2]),float),
-                 14: build_cell_from_latt_constants(latt),
+                 14: build_cell_from_lattice_constants(latt),
                  }
 
     if abs(ibrav)==5:
         a=latt['a'];c=latt['c']
         R_cosalpha=(2*c**2-3*a**2)/(2*c**2+6*a**2)
         print ( "cosalpha(celldm4)=",R_cosalpha)
         tx=np.sqrt((1-R_cosalpha)/2)
```

### Comparing `PySupercell-0.0.4/pysupercell/arguments.py` & `PySupercell-0.0.5/pysupercell/arguments.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.4/pysupercell/pysupercell.py` & `PySupercell-0.0.5/pysupercell/pysupercell.py`

 * *Files 1% similar despite different names*

```diff
@@ -659,25 +659,25 @@
                 print ('\n'.join(['{0:18s}'.format('')+' '.join(['{0:10.8f}'.format(item) for item in line]) for line in local_rot[1:]]), file=fw)
             fw.write('  {0:2d}      NUMBER OF SYMMETRY OPERATIONS \n'.format(len(op)))
             for iop in range(nrotate):
                 fw.write('\n'.join([' '.join(['{0:2d}'.format(rot[iop,i,j]) for j in range(3)])+' {0:10.8f}'.format(trans[iop,i]) for i in range(3)]))
                 fw.write('\n{0:8d}\n'.format(iop+1))
         return 0
 
-    @property
+
     def get_mass(self):
         amass=[get_element_info_phonopy(sym)[-1] for sym in self._symbols]
         return amass
 
-    @property
+
     def get_mass_density(self):
         amass=self.get_mass()
         return sum(amass)/(self.real_cell_volume()*1e-24*scipy.constants.Avogadro)
 
-    @property
+
     def get_volume_density(self):
         return self.real_cell_volume()/self._natom
 
 
     def visualize_struct(self):
         try: import matplotlib.pyplot as plt
         except: exit('cannot import matplotlib!')
```

### Comparing `PySupercell-0.0.4/setup.py` & `PySupercell-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 core_modules = ['pysupercell/{}'.format(item) for item in core_modules]
 
 
 
 kwargs_setup=dict(
 name='PySupercell',
-version='0.0.4',
+version='0.0.5',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
 url='https://to_be_posted',
 download_url='https://on_request',
 keywords=['Python','Crystal structure','supercell'],
 py_modules=core_modules,
 license="MIT License",
```

