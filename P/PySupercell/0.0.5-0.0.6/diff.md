# Comparing `tmp/PySupercell-0.0.5.tar.gz` & `tmp/PySupercell-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySupercell-0.0.5.tar", last modified: Sat Jun  3 15:43:00 2023, max compression
+gzip compressed data, was "PySupercell-0.0.6.tar", last modified: Sat Jun  3 15:56:45 2023, max compression
```

## Comparing `PySupercell-0.0.5.tar` & `PySupercell-0.0.6.tar`

### file list

```diff
@@ -1,54 +1,60 @@
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.470323 PySupercell-0.0.5/
--rwxrw-r--   0 zsh       (1000) zsh       (1000)     1058 2023-06-03 11:10:34.000000 PySupercell-0.0.5/LICENSE.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      294 2023-06-03 11:24:12.000000 PySupercell-0.0.5/MANIFEST.in
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      484 2023-06-03 15:43:00.470323 PySupercell-0.0.5/PKG-INFO
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.462323 PySupercell-0.0.5/PySupercell.egg-info/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      484 2023-06-03 15:43:00.000000 PySupercell-0.0.5/PySupercell.egg-info/PKG-INFO
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     1076 2023-06-03 15:43:00.000000 PySupercell-0.0.5/PySupercell.egg-info/SOURCES.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-06-03 15:43:00.000000 PySupercell-0.0.5/PySupercell.egg-info/dependency_links.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       33 2023-06-03 15:43:00.000000 PySupercell-0.0.5/PySupercell.egg-info/requires.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       92 2023-06-03 15:43:00.000000 PySupercell-0.0.5/PySupercell.egg-info/top_level.txt
--rw-r--r--   0 zsh       (1000) zsh       (1000)     2282 2023-06-03 13:25:16.000000 PySupercell-0.0.5/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.462323 PySupercell-0.0.5/bin/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)    10109 2023-06-03 14:54:46.000000 PySupercell-0.0.5/bin/pysc.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)    10425 2023-06-03 15:13:38.000000 PySupercell-0.0.5/bin/v2qe.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.462323 PySupercell-0.0.5/examples/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      266 2023-06-03 13:05:58.000000 PySupercell-0.0.5/examples/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.466323 PySupercell-0.0.5/examples/example1/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      364 2023-06-03 11:32:21.000000 PySupercell-0.0.5/examples/example1/POSCAR
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      376 2023-06-03 15:13:42.000000 PySupercell-0.0.5/examples/example1/POSCAR_Primitive
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      691 2023-06-03 14:49:50.000000 PySupercell-0.0.5/examples/example1/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.466323 PySupercell-0.0.5/examples/example1/reference/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      704 2023-06-03 11:32:28.000000 PySupercell-0.0.5/examples/example1/reference/POSCAR_redefine
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     1312 2023-06-03 12:58:44.000000 PySupercell-0.0.5/examples/example1/reference/POSCAR_slab
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      456 2023-06-03 15:13:45.000000 PySupercell-0.0.5/examples/example1/rx.in
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.466323 PySupercell-0.0.5/examples/example2/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      437 2023-06-03 13:07:30.000000 PySupercell-0.0.5/examples/example2/POSCAR
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       40 2023-06-03 13:09:42.000000 PySupercell-0.0.5/examples/example2/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.466323 PySupercell-0.0.5/examples/example2/reference/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     9732 2023-06-03 13:09:46.000000 PySupercell-0.0.5/examples/example2/reference/POSCAR_sc
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     9738 2023-06-03 13:09:46.000000 PySupercell-0.0.5/examples/example2/reference/POSCAR_tube
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.466323 PySupercell-0.0.5/examples/example3/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      948 2023-06-03 14:16:16.000000 PySupercell-0.0.5/examples/example3/POSCAR
--rw-rw-r--   0 zsh       (1000) zsh       (1000)    54936 2023-06-03 14:23:45.000000 PySupercell-0.0.5/examples/example3/POSCAR_redefine
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      569 2023-06-03 14:16:10.000000 PySupercell-0.0.5/examples/example3/README
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     9854 2023-06-03 14:03:09.000000 PySupercell-0.0.5/examples/example3/make_screw_diamond.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.466323 PySupercell-0.0.5/examples/example3/reference/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)    44136 2023-06-03 14:01:17.000000 PySupercell-0.0.5/examples/example3/reference/POSCAR_redefine
--rw-rw-r--   0 zsh       (1000) zsh       (1000)    54957 2023-06-03 14:06:32.000000 PySupercell-0.0.5/examples/example3/reference/POSCAR_screw
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.470323 PySupercell-0.0.5/examples/example4/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      534 2023-06-03 13:02:08.000000 PySupercell-0.0.5/examples/example4/POSCAR
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      124 2023-06-03 13:04:39.000000 PySupercell-0.0.5/examples/example4/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.470323 PySupercell-0.0.5/examples/example4/reference/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     2176 2023-06-03 13:02:46.000000 PySupercell-0.0.5/examples/example4/reference/POSCAR_bending
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     2168 2023-06-03 13:02:46.000000 PySupercell-0.0.5/examples/example4/reference/POSCAR_flat
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.470323 PySupercell-0.0.5/pysupercell/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     8665 2023-06-03 15:06:12.000000 PySupercell-0.0.5/pysupercell/QE_ibrav_lib.py
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      293 2023-06-03 15:06:18.000000 PySupercell-0.0.5/pysupercell/__init__.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     4589 2023-06-03 13:26:30.000000 PySupercell-0.0.5/pysupercell/arguments.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)    44613 2023-06-03 15:41:34.000000 PySupercell-0.0.5/pysupercell/pysupercell.py
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-06-03 15:43:00.470323 PySupercell-0.0.5/setup.cfg
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3621 2023-06-03 15:42:52.000000 PySupercell-0.0.5/setup.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-06-03 15:43:00.470323 PySupercell-0.0.5/tests_basic/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       40 2023-06-03 10:27:02.000000 PySupercell-0.0.5/tests_basic/README
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       72 2023-06-03 10:30:27.000000 PySupercell-0.0.5/tests_basic/test_1.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1058 2023-06-03 15:54:33.000000 PySupercell-0.0.6/LICENSE.txt
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      294 2023-06-03 15:54:33.000000 PySupercell-0.0.6/MANIFEST.in
+-rw-r--r--   0 shz       (1000) shz       (1000)      484 2023-06-03 15:56:45.226954 PySupercell-0.0.6/PKG-INFO
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/PySupercell.egg-info/
+-rw-r--r--   0 shz       (1000) shz       (1000)      484 2023-06-03 15:56:45.000000 PySupercell-0.0.6/PySupercell.egg-info/PKG-INFO
+-rw-r--r--   0 shz       (1000) shz       (1000)     1297 2023-06-03 15:56:45.000000 PySupercell-0.0.6/PySupercell.egg-info/SOURCES.txt
+-rw-r--r--   0 shz       (1000) shz       (1000)        1 2023-06-03 15:56:45.000000 PySupercell-0.0.6/PySupercell.egg-info/dependency_links.txt
+-rw-r--r--   0 shz       (1000) shz       (1000)       33 2023-06-03 15:56:45.000000 PySupercell-0.0.6/PySupercell.egg-info/requires.txt
+-rw-r--r--   0 shz       (1000) shz       (1000)       92 2023-06-03 15:56:45.000000 PySupercell-0.0.6/PySupercell.egg-info/top_level.txt
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     2282 2023-06-03 15:54:33.000000 PySupercell-0.0.6/README.md
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/bin/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    10217 2023-06-03 15:54:33.000000 PySupercell-0.0.6/bin/pysc.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    10425 2023-06-03 15:54:33.000000 PySupercell-0.0.6/bin/v2qe.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      266 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/README.md
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example1/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      364 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/POSCAR
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      376 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/POSCAR_Primitive
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      378 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/POSCAR_for_symm_analysis
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      691 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/README.md
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1739 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/phonopy_symcells.yaml
+-rwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/phonopy_symm.yaml
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example1/reference/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      704 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/reference/POSCAR_redefine
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1312 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/reference/POSCAR_slab
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      456 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example1/rx.in
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example2/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)       20 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example2/53s}'.format('version
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      437 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example2/POSCAR
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    12072 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example2/POSCAR_sc
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    12078 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example2/POSCAR_tube_4_6
+-rwxr-xr-x   0 shz       (1000) shz       (1000)       37 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example2/README.md
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example2/reference/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     9732 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example2/reference/POSCAR_sc
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     9738 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example2/reference/POSCAR_tube
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example3/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      948 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example3/POSCAR
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    54936 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example3/POSCAR_redefine
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      569 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example3/README
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     9854 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example3/make_screw_diamond.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example3/reference/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    44136 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example3/reference/POSCAR_redefine
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    54957 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example3/reference/POSCAR_screw
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example4/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      534 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example4/POSCAR
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      124 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example4/README.md
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/examples/example4/reference/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     2176 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example4/reference/POSCAR_bending
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     2168 2023-06-03 15:54:34.000000 PySupercell-0.0.6/examples/example4/reference/POSCAR_flat
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/pysupercell/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     8665 2023-06-03 15:54:34.000000 PySupercell-0.0.6/pysupercell/QE_ibrav_lib.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      293 2023-06-03 15:55:22.000000 PySupercell-0.0.6/pysupercell/__init__.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     4589 2023-06-03 15:54:34.000000 PySupercell-0.0.6/pysupercell/arguments.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    44613 2023-06-03 15:54:34.000000 PySupercell-0.0.6/pysupercell/pysupercell.py
+-rw-r--r--   0 shz       (1000) shz       (1000)       38 2023-06-03 15:56:45.226954 PySupercell-0.0.6/setup.cfg
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     3621 2023-06-03 15:56:37.000000 PySupercell-0.0.6/setup.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-03 15:56:45.226954 PySupercell-0.0.6/tests_basic/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)       40 2023-06-03 15:54:34.000000 PySupercell-0.0.6/tests_basic/README
+-rwxr-xr-x   0 shz       (1000) shz       (1000)       72 2023-06-03 15:54:34.000000 PySupercell-0.0.6/tests_basic/test_1.py
```

### Comparing `PySupercell-0.0.5/LICENSE.txt` & `PySupercell-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/PySupercell.egg-info/SOURCES.txt` & `PySupercell-0.0.6/PySupercell.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,25 @@
 PySupercell.egg-info/requires.txt
 PySupercell.egg-info/top_level.txt
 bin/pysc.py
 bin/v2qe.py
 examples/README.md
 examples/example1/POSCAR
 examples/example1/POSCAR_Primitive
+examples/example1/POSCAR_for_symm_analysis
 examples/example1/README.md
+examples/example1/phonopy_symcells.yaml
+examples/example1/phonopy_symm.yaml
 examples/example1/rx.in
 examples/example1/reference/POSCAR_redefine
 examples/example1/reference/POSCAR_slab
+examples/example2/53s}'.format('version
 examples/example2/POSCAR
+examples/example2/POSCAR_sc
+examples/example2/POSCAR_tube_4_6
 examples/example2/README.md
 examples/example2/reference/POSCAR_sc
 examples/example2/reference/POSCAR_tube
 examples/example3/POSCAR
 examples/example3/POSCAR_redefine
 examples/example3/README
 examples/example3/make_screw_diamond.py
```

### Comparing `PySupercell-0.0.5/README.md` & `PySupercell-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/bin/pysc.py` & `PySupercell-0.0.6/bin/pysc.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,38 +147,41 @@
         a=struct.latt_param()['a']
         b=struct.latt_param()['b']
         gamma=struct.latt_param()['gamma']
         cell_1=[a*cos((args.angle)/180*np.pi),a*np.sin((args.angle)/180*np.pi),0]
         cell_2=[b*cos((gamma+args.angle)/180*np.pi),b*np.sin((gamma+args.angle)/180*np.pi),0]
         struct._cell=np.array([cell_1,cell_2,struct._cell[2]])
         struct._system='POSCAR_rotate_z'
+        flpos='POSCAR_rotate_z'
         struct.write_poscar_head(filename=flpos)
         struct.write_poscar_atoms(filename=flpos,mode='add')
 
     elif args.task=='slab':
         hkl=args.hkl
         if len(hkl)>3:
             exit('we do not allow negative index!')
         h,k,l=list(map(int,hkl))
         struct_slab = struct.build_slab(h,k,l,args.thickness,args.vacuum,args.atom_shift)
         struct_slab._system='slab'
+        flpos='POSCAR_slab_{}'.format(hkl)
         struct_slab.write_poscar_head(filename=flpos)
         struct_slab.write_poscar_atoms(filename=flpos,mode='a')
 
     elif args.task=='tube':
         n,m=args.chiral_num
         struct_tube = struct.build_tube(n,m,negative_R=args.negative_R)
         fltube = "POSCAR_tube_{0}_{1}".format(n,m)
         struct_tube._system=system='{0}_{1}_nanotube'.format(n,m)
-        struct_tube.write_poscar_head(filename=flpos)
-        struct_tube.write_poscar_atoms(filename=flpos,mode='a')
+        struct_tube.write_poscar_head(filename=fltube)
+        struct_tube.write_poscar_atoms(filename=fltube,mode='a')
 
     elif args.task=='bending':
         struct_bend = struct.build_bending_supercell(args.nn,args.amp,args.idir_per,args.idir_bend,args.central_z)
         struct_bend._system = 'bending struct'
+        flpos='POSCAR_bending'
         struct_bend.write_poscar_head(filename=flpos)
         struct_bend.write_poscar_atoms(filename=flpos,mode='a')
 
     elif args.task=='strain':
         for idir in args.strain_dirs:
             struct._cell[idir] *= 1+args.strain
         struct._pos_cart=np.dot(struct._pos,struct._cell)
```

### Comparing `PySupercell-0.0.5/bin/v2qe.py` & `PySupercell-0.0.6/bin/v2qe.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/examples/example1/README.md` & `PySupercell-0.0.6/examples/example1/README.md`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/examples/example1/reference/POSCAR_redefine` & `PySupercell-0.0.6/examples/example1/reference/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/examples/example1/reference/POSCAR_slab` & `PySupercell-0.0.6/examples/example1/reference/POSCAR_slab`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/examples/example2/reference/POSCAR_sc` & `PySupercell-0.0.6/examples/example2/reference/POSCAR_sc`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/examples/example2/reference/POSCAR_tube` & `PySupercell-0.0.6/examples/example2/reference/POSCAR_tube`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/examples/example3/POSCAR` & `PySupercell-0.0.6/examples/example3/POSCAR`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/examples/example3/POSCAR_redefine` & `PySupercell-0.0.6/examples/example3/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/examples/example3/README` & `PySupercell-0.0.6/examples/example3/README`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/examples/example3/make_screw_diamond.py` & `PySupercell-0.0.6/examples/example3/make_screw_diamond.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/examples/example3/reference/POSCAR_redefine` & `PySupercell-0.0.6/examples/example3/reference/POSCAR_redefine`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/examples/example3/reference/POSCAR_screw` & `PySupercell-0.0.6/examples/example3/reference/POSCAR_screw`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/examples/example4/POSCAR` & `PySupercell-0.0.6/examples/example4/POSCAR`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/examples/example4/reference/POSCAR_bending` & `PySupercell-0.0.6/examples/example4/reference/POSCAR_bending`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/examples/example4/reference/POSCAR_flat` & `PySupercell-0.0.6/examples/example4/reference/POSCAR_flat`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/pysupercell/QE_ibrav_lib.py` & `PySupercell-0.0.6/pysupercell/QE_ibrav_lib.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/pysupercell/arguments.py` & `PySupercell-0.0.6/pysupercell/arguments.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/pysupercell/pysupercell.py` & `PySupercell-0.0.6/pysupercell/pysupercell.py`

 * *Files identical despite different names*

### Comparing `PySupercell-0.0.5/setup.py` & `PySupercell-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 core_modules = ['pysupercell/{}'.format(item) for item in core_modules]
 
 
 
 kwargs_setup=dict(
 name='PySupercell',
-version='0.0.5',
+version='0.0.6',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
 url='https://to_be_posted',
 download_url='https://on_request',
 keywords=['Python','Crystal structure','supercell'],
 py_modules=core_modules,
 license="MIT License",
```

