# Comparing `tmp/py2sambvca-1.3.4.tar.gz` & `tmp/py2sambvca-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2sambvca-1.3.4.tar", last modified: Tue Mar 28 15:12:18 2023, max compression
+gzip compressed data, was "py2sambvca-1.4.0.tar", last modified: Sat Jun  3 19:47:04 2023, max compression
```

## Comparing `py2sambvca-1.3.4.tar` & `py2sambvca-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-03-28 15:12:18.937850 py2sambvca-1.3.4/
--rw-r--r--   0 jackson    (501) staff       (20)    35129 2023-03-28 13:10:27.000000 py2sambvca-1.3.4/LICENSE
--rw-r--r--   0 jackson    (501) staff       (20)     7954 2023-03-28 15:12:18.937305 py2sambvca-1.3.4/PKG-INFO
--rw-r--r--   0 jackson    (501) staff       (20)     7311 2023-03-28 13:10:27.000000 py2sambvca-1.3.4/README.md
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-03-28 15:12:18.917519 py2sambvca-1.3.4/py2sambvca/
--rw-r--r--   0 jackson    (501) staff       (20)       84 2023-03-28 14:55:58.000000 py2sambvca-1.3.4/py2sambvca/__init__.py
--rw-r--r--   0 jackson    (501) staff       (20)    20362 2023-03-28 14:36:21.000000 py2sambvca-1.3.4/py2sambvca/py2sambvca.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-03-28 15:12:18.929750 py2sambvca-1.3.4/py2sambvca.egg-info/
--rw-r--r--   0 jackson    (501) staff       (20)     7954 2023-03-28 15:12:18.000000 py2sambvca-1.3.4/py2sambvca.egg-info/PKG-INFO
--rw-r--r--   0 jackson    (501) staff       (20)      261 2023-03-28 15:12:18.000000 py2sambvca-1.3.4/py2sambvca.egg-info/SOURCES.txt
--rw-r--r--   0 jackson    (501) staff       (20)        1 2023-03-28 15:12:18.000000 py2sambvca-1.3.4/py2sambvca.egg-info/dependency_links.txt
--rw-r--r--   0 jackson    (501) staff       (20)       11 2023-03-28 15:12:18.000000 py2sambvca-1.3.4/py2sambvca.egg-info/top_level.txt
--rw-r--r--   0 jackson    (501) staff       (20)       38 2023-03-28 15:12:18.938149 py2sambvca-1.3.4/setup.cfg
--rw-r--r--   0 jackson    (501) staff       (20)     1483 2023-03-28 13:10:27.000000 py2sambvca-1.3.4/setup.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-03-28 15:12:18.935285 py2sambvca-1.3.4/test/
--rw-r--r--   0 jackson    (501) staff       (20)    13591 2023-03-28 14:28:25.000000 py2sambvca-1.3.4/test/test_py2sambvca.py
--rw-r--r--   0 jackson    (501) staff       (20)     1783 2023-03-28 14:26:44.000000 py2sambvca-1.3.4/test/test_static_output.py
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-06-03 19:47:04.459173 py2sambvca-1.4.0/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)    35129 2023-02-05 17:11:46.000000 py2sambvca-1.4.0/LICENSE
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)     8111 2023-06-03 19:47:04.459173 py2sambvca-1.4.0/PKG-INFO
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     7468 2023-06-03 19:01:26.000000 py2sambvca-1.4.0/README.md
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-06-03 19:47:04.459173 py2sambvca-1.4.0/py2sambvca/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)       84 2023-06-03 19:45:53.000000 py2sambvca-1.4.0/py2sambvca/__init__.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)    18655 2023-06-03 19:38:22.000000 py2sambvca-1.4.0/py2sambvca/py2sambvca.py
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-06-03 19:47:04.459173 py2sambvca-1.4.0/py2sambvca.egg-info/
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)     8111 2023-06-03 19:47:04.000000 py2sambvca-1.4.0/py2sambvca.egg-info/PKG-INFO
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)      261 2023-06-03 19:47:04.000000 py2sambvca-1.4.0/py2sambvca.egg-info/SOURCES.txt
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)        1 2023-06-03 19:47:04.000000 py2sambvca-1.4.0/py2sambvca.egg-info/dependency_links.txt
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)       11 2023-06-03 19:47:04.000000 py2sambvca-1.4.0/py2sambvca.egg-info/top_level.txt
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)       38 2023-06-03 19:47:04.459173 py2sambvca-1.4.0/setup.cfg
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1483 2023-06-03 16:19:52.000000 py2sambvca-1.4.0/setup.py
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-06-03 19:47:04.459173 py2sambvca-1.4.0/test/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)    13614 2023-06-03 19:13:59.000000 py2sambvca-1.4.0/test/test_py2sambvca.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1783 2023-06-03 16:19:52.000000 py2sambvca-1.4.0/test/test_static_output.py
```

### Comparing `py2sambvca-1.3.4/LICENSE` & `py2sambvca-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py2sambvca-1.3.4/PKG-INFO` & `py2sambvca-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2sambvca
-Version: 1.3.4
+Version: 1.4.0
 Summary: Simple thin client to interface python scripts with SambVca catalytic pocket Fortran calculator.
 Home-page: https://github.com/JacksonBurns/py2sambvca
 Author: Jackson Burns
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -35,20 +35,20 @@
 
 ## Installation
 `py2sambvca` is available on PyPI and can be installed like so:
 ```python
 pip install py2sambvca
 ```
 
-`py2sambvca` has __zero__ external depdencies.
+`py2sambvca` has __zero__ external dependencies.
 
-### Downloading and Compiling `Sambvca`
-`py2sambvca` can read and write input and output files for `Sambvca` without the actual program in place, but in order to run input files you must have an executable `sambvca21.exe` (or similar) somewhere on your machine.
+### Downloading and Compiling `SambVca`
+`py2sambvca` can read and write input and output files for `SambVca` without the actual program in place, but in order to run input files you must have an executable `sambvca21.exe` (or similar) somewhere on your machine.
 
-You can download the source code [on the `Sambvca` webserver](https://www.molnac.unisa.it/OMtools/sambvca2.1/download/download.html) and compile it using [`gfortran`](https://gcc.gnu.org/wiki/GFortranBinaries).
+You can download the source code [on the `SambVca` webserver](https://www.molnac.unisa.it/OMtools/sambvca2.1/download/download.html) and compile it using [`gfortran`](https://gcc.gnu.org/wiki/GFortranBinaries).
 
 By default, `py2sambvca` expects the executable to be present in the `cwd` and named `sambvca21.exe` on Windows or `sambvca21.x` on Unix-based systems. optionally, the filepath to your executable can be specified as shown below.
 
 ## Usage
 After installation, `py2sambvca` can be added to a Python script via `import` and instantiated:
 ```python
 from py2sambvca import p2s
@@ -75,14 +75,15 @@
  - `mesh_size` (float): Mesh size for numerical integration (default 0.10)
  - `remove_H` (int): 0/1 Do not remove/remove H atoms from Vbur calculation (default 1)
  - `orient_z` (int): 0/1 Molecule oriented along negative/positive Z-axis (default 1)
  - `write_surf_files` (int): 0/1 Do not write/write files for top and bottom surfaces (default 1)
  - `path_to_sambvcax` (str): Path to the SambVca executable. Only needed to use py2sambvca.calc()(default "sambvca.exe")
  - `working_dir` (path): Path to the working directory where the output and input files are generated (default os.getcwd())
  - `verbose` (int): 0 for no output, 1 for some output, 2 for the most output (default 1)
+ - `radii_table` (dict or str): a dictionary of atomic symbols and their radii (angstroms), or "default" for the radii used in the original implementation
 
 
 From here, running can be done stepwise or with a single function:
 ```python
 nhc_p2s.run()
 # equivalent to
 nhc_p2s.write_input()
```

### Comparing `py2sambvca-1.3.4/README.md` & `py2sambvca-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 
 ## Installation
 `py2sambvca` is available on PyPI and can be installed like so:
 ```python
 pip install py2sambvca
 ```
 
-`py2sambvca` has __zero__ external depdencies.
+`py2sambvca` has __zero__ external dependencies.
 
-### Downloading and Compiling `Sambvca`
-`py2sambvca` can read and write input and output files for `Sambvca` without the actual program in place, but in order to run input files you must have an executable `sambvca21.exe` (or similar) somewhere on your machine.
+### Downloading and Compiling `SambVca`
+`py2sambvca` can read and write input and output files for `SambVca` without the actual program in place, but in order to run input files you must have an executable `sambvca21.exe` (or similar) somewhere on your machine.
 
-You can download the source code [on the `Sambvca` webserver](https://www.molnac.unisa.it/OMtools/sambvca2.1/download/download.html) and compile it using [`gfortran`](https://gcc.gnu.org/wiki/GFortranBinaries).
+You can download the source code [on the `SambVca` webserver](https://www.molnac.unisa.it/OMtools/sambvca2.1/download/download.html) and compile it using [`gfortran`](https://gcc.gnu.org/wiki/GFortranBinaries).
 
 By default, `py2sambvca` expects the executable to be present in the `cwd` and named `sambvca21.exe` on Windows or `sambvca21.x` on Unix-based systems. optionally, the filepath to your executable can be specified as shown below.
 
 ## Usage
 After installation, `py2sambvca` can be added to a Python script via `import` and instantiated:
 ```python
 from py2sambvca import p2s
@@ -58,14 +58,15 @@
  - `mesh_size` (float): Mesh size for numerical integration (default 0.10)
  - `remove_H` (int): 0/1 Do not remove/remove H atoms from Vbur calculation (default 1)
  - `orient_z` (int): 0/1 Molecule oriented along negative/positive Z-axis (default 1)
  - `write_surf_files` (int): 0/1 Do not write/write files for top and bottom surfaces (default 1)
  - `path_to_sambvcax` (str): Path to the SambVca executable. Only needed to use py2sambvca.calc()(default "sambvca.exe")
  - `working_dir` (path): Path to the working directory where the output and input files are generated (default os.getcwd())
  - `verbose` (int): 0 for no output, 1 for some output, 2 for the most output (default 1)
+ - `radii_table` (dict or str): a dictionary of atomic symbols and their radii (angstroms), or "default" for the radii used in the original implementation
 
 
 From here, running can be done stepwise or with a single function:
 ```python
 nhc_p2s.run()
 # equivalent to
 nhc_p2s.write_input()
```

### Comparing `py2sambvca-1.3.4/py2sambvca/py2sambvca.py` & `py2sambvca-1.4.0/py2sambvca/py2sambvca.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import subprocess
 import re
 import glob
 import os
-from typing import List
+from typing import List, Union
 from warnings import warn
 
+from py2sambvca.radii_tables import table_lookup, format_radii_table
+
 
 class py2sambvca:
     """
     Wrapper class for py2sambvca functions.
 
     Call this class to instantiate a py2sambvca object, which has methods to write input, call SambVca,
     and retrieve output.
@@ -24,14 +26,15 @@
     mesh_size (float): Mesh size for numerical integration (default 0.10)
     remove_H (int): 0/1 Do not remove/remove H atoms from Vbur calculation (default 1)
     orient_z (int): 0/1 Molecule oriented along negative/positive Z-axis (default 1)
     write_surf_files (int): 0/1 Do not write/write files for top and bottom surfaces (default 1)
     path_to_sambvcax (str): Path to the SambVca executable. Only needed to use py2sambvca.calc()( default "/path/to/executable/sambvca.x")
     working_dir (path): Path to the working directory where the output and input files are generated (default os.getcwd())
     verbose (int): 0 for no output, 1 for some output, 2 for the most output
+    radii_table (dict or str): atomic symbols (ie. H, LI) and radii (Angstrom), "default" (bondii radii*1.17), or "vdw" for van Der Waals
     """
 
     def __init__(
         self,
         xyz_filepath: str,
         sphere_center_atom_ids: List[int],
         z_ax_atom_ids: List[int],
@@ -42,14 +45,15 @@
         mesh_size: float = 0.10,
         remove_H: int = 1,
         orient_z: int = 1,
         write_surf_files: int = 1,
         path_to_sambvcax: str = "sambvca.exe",
         working_dir: str = os.getcwd(),
         verbose: int = 1,
+        radii_table: Union[str, dict] = "default",
     ):
         """
         Wrapper class for py2sambvca functions.
 
         Call this class to instantiate a py2sambvca object, which has methods to write input, call SambVca,
         and retrieve output.
 
@@ -64,14 +68,15 @@
         mesh_size (float): Mesh size for numerical integration (default 0.10)
         remove_H (int): 0/1 Do not remove/remove H atoms from Vbur calculation (default 1)
         orient_z (int): 0/1 Molecule oriented along negative/positive Z-axis (default 1)
         write_surf_files (int): 0/1 Do not write/write files for top and bottom surfaces (default 1)
         path_to_sambvcax (str): Path to the SambVca executable. Only needed to use py2sambvca.calc()( default "/path/to/executable/sambvca.x")
         working_dir (path): Path to the working directory where the output and input files are generated (default os.getcwd())
         verbose (int): 0 for no output, 1 for some output, 2 for the most output
+        radii_table (dict or str): atomic symbols (ie. H, LI) and radii (Angstrom), "default" (bondii radii*1.17), or "vdw" for van Der Waals
         """
         # if atoms are requested to be deleted, assign them and the number of them
         if atoms_to_delete_ids is not None:
             self.n_atoms_to_delete = len(atoms_to_delete_ids)
             self.atoms_to_delete_ids = atoms_to_delete_ids
         else:  # otherwise, set to none to avoid bad writes in the future
             self.n_atoms_to_delete = None
@@ -110,14 +115,19 @@
         self.verbose = verbose
 
         # make results accesible from object directly
         self.total_results = None
         self.quadrant_results = None
         self.octant_results = None
 
+        # data table
+        self.__radii_table = format_radii_table(
+            table_lookup[radii_table] if type(radii_table) is str else radii_table
+        )
+
     def write_input(self):
         """
         Write input for the Sambvca buried-volume Fortran calculator based on the data entered
         when object was initialized.
 
         """
         # make file in the same cwd, which is where sambvca will look
@@ -163,15 +173,15 @@
                     str(self.remove_H) + "\n",
                     str(self.orient_z) + "\n",
                     str(self.write_surf_files) + "\n",
                     "103\n",
                 ]
             )
             # write radii
-            file.writelines(radii_table)
+            file.writelines(self.__radii_table)
             # write the atom coordinates
             file.writelines(self.xyz_data)
 
     def calc(self):
         """
         Call SambVca based on the executable path given on initialization of py2sambvca.
 
@@ -507,114 +517,7 @@
 
     def run(self):
         self.write_input()
         self.calc()
         self.parse_output()
         self.clean_files()
         return self.total_results, self.quadrant_results, self.octant_results
-
-
-radii_table = [
-    "H       1.28\n",
-    "HE      1.64\n",
-    "LI      2.13\n",
-    "BE      1.79\n",
-    "B       2.25\n",
-    "C       1.99\n",
-    "N       1.81\n",
-    "O       1.78\n",
-    "F       1.72\n",
-    "NE      1.80\n",
-    "NA      2.66\n",
-    "MG      2.02\n",
-    "AL      2.15\n",
-    "SI      2.46\n",
-    "P       2.11\n",
-    "S       2.11\n",
-    "CL      2.05\n",
-    "AR      2.20\n",
-    "K       3.22\n",
-    "CA      2.70\n",
-    "SC      2.52\n",
-    "TI      2.47\n",
-    "V       2.42\n",
-    "CR      2.41\n",
-    "MN      2.40\n",
-    "FE      2.39\n",
-    "CO      2.34\n",
-    "NI      1.91\n",
-    "CU      1.64\n",
-    "ZN      1.63\n",
-    "GA      2.19\n",
-    "GE      2.47\n",
-    "AS      2.16\n",
-    "SE      2.22\n",
-    "BR      2.16\n",
-    "KR      2.36\n",
-    "RB      3.55\n",
-    "SR      2.91\n",
-    "Y       2.71\n",
-    "ZR      2.61\n",
-    "NB      2.55\n",
-    "MO      2.54\n",
-    "TC      2.53\n",
-    "RU      2.49\n",
-    "RH      2.46\n",
-    "PD      1.91\n",
-    "AG      2.01\n",
-    "CD      1.85\n",
-    "IN      2.26\n",
-    "SN      2.54\n",
-    "SB      2.41\n",
-    "TE      2.41\n",
-    "I       2.32\n",
-    "XE      2.53\n",
-    "CS      4.01\n",
-    "BA      3.14\n",
-    "LA      2.84\n",
-    "CE      2.83\n",
-    "PR      2.81\n",
-    "ND      2.80\n",
-    "PM      2.78\n",
-    "SM      2.76\n",
-    "EU      2.75\n",
-    "GD      2.74\n",
-    "TB      2.73\n",
-    "DY      2.70\n",
-    "HO      2.69\n",
-    "ER      2.68\n",
-    "TM      2.66\n",
-    "YB      2.64\n",
-    "LU      2.62\n",
-    "HF      2.61\n",
-    "TA      2.60\n",
-    "W       2.55\n",
-    "RE      2.53\n",
-    "OS      2.53\n",
-    "IR      2.49\n",
-    "PT      2.01\n",
-    "AU      1.94\n",
-    "HG      1.81\n",
-    "TL      2.29\n",
-    "PB      2.36\n",
-    "BI      2.42\n",
-    "PO      2.30\n",
-    "AT      2.36\n",
-    "RN      2.57\n",
-    "FR      4.07\n",
-    "RA      3.31\n",
-    "AC      2.89\n",
-    "TH      2.87\n",
-    "PA      2.84\n",
-    "U       2.18\n",
-    "NP      2.80\n",
-    "PU      2.84\n",
-    "AM      2.85\n",
-    "CM      2.87\n",
-    "BK      2.85\n",
-    "CF      2.87\n",
-    "ES      2.87\n",
-    "FM      2.87\n",
-    "M       2.88\n",
-    "NO      2.88\n",
-    "LR      2.88\n",
-]
```

### Comparing `py2sambvca-1.3.4/py2sambvca.egg-info/PKG-INFO` & `py2sambvca-1.4.0/py2sambvca.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2sambvca
-Version: 1.3.4
+Version: 1.4.0
 Summary: Simple thin client to interface python scripts with SambVca catalytic pocket Fortran calculator.
 Home-page: https://github.com/JacksonBurns/py2sambvca
 Author: Jackson Burns
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -35,20 +35,20 @@
 
 ## Installation
 `py2sambvca` is available on PyPI and can be installed like so:
 ```python
 pip install py2sambvca
 ```
 
-`py2sambvca` has __zero__ external depdencies.
+`py2sambvca` has __zero__ external dependencies.
 
-### Downloading and Compiling `Sambvca`
-`py2sambvca` can read and write input and output files for `Sambvca` without the actual program in place, but in order to run input files you must have an executable `sambvca21.exe` (or similar) somewhere on your machine.
+### Downloading and Compiling `SambVca`
+`py2sambvca` can read and write input and output files for `SambVca` without the actual program in place, but in order to run input files you must have an executable `sambvca21.exe` (or similar) somewhere on your machine.
 
-You can download the source code [on the `Sambvca` webserver](https://www.molnac.unisa.it/OMtools/sambvca2.1/download/download.html) and compile it using [`gfortran`](https://gcc.gnu.org/wiki/GFortranBinaries).
+You can download the source code [on the `SambVca` webserver](https://www.molnac.unisa.it/OMtools/sambvca2.1/download/download.html) and compile it using [`gfortran`](https://gcc.gnu.org/wiki/GFortranBinaries).
 
 By default, `py2sambvca` expects the executable to be present in the `cwd` and named `sambvca21.exe` on Windows or `sambvca21.x` on Unix-based systems. optionally, the filepath to your executable can be specified as shown below.
 
 ## Usage
 After installation, `py2sambvca` can be added to a Python script via `import` and instantiated:
 ```python
 from py2sambvca import p2s
@@ -75,14 +75,15 @@
  - `mesh_size` (float): Mesh size for numerical integration (default 0.10)
  - `remove_H` (int): 0/1 Do not remove/remove H atoms from Vbur calculation (default 1)
  - `orient_z` (int): 0/1 Molecule oriented along negative/positive Z-axis (default 1)
  - `write_surf_files` (int): 0/1 Do not write/write files for top and bottom surfaces (default 1)
  - `path_to_sambvcax` (str): Path to the SambVca executable. Only needed to use py2sambvca.calc()(default "sambvca.exe")
  - `working_dir` (path): Path to the working directory where the output and input files are generated (default os.getcwd())
  - `verbose` (int): 0 for no output, 1 for some output, 2 for the most output (default 1)
+ - `radii_table` (dict or str): a dictionary of atomic symbols and their radii (angstroms), or "default" for the radii used in the original implementation
 
 
 From here, running can be done stepwise or with a single function:
 ```python
 nhc_p2s.run()
 # equivalent to
 nhc_p2s.write_input()
```

### Comparing `py2sambvca-1.3.4/setup.py` & `py2sambvca-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `py2sambvca-1.3.4/test/test_py2sambvca.py` & `py2sambvca-1.4.0/test/test_py2sambvca.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,15 @@
             self.radius,
             self.displacement,
             self.mesh_size,
             self.remove_H,
             self.orient_Z,
             self.write_surf_files,
             self.exe_path,
+            "default",
         )
         self.assertEqual(
             self.sphere_ids,
             test_p2s.sphere_center_atom_ids,
             "sphere_center_atom_ids not set correctly.",
         )
         self.assertEqual(
```

### Comparing `py2sambvca-1.3.4/test/test_static_output.py` & `py2sambvca-1.4.0/test/test_static_output.py`

 * *Files identical despite different names*

