# Comparing `tmp/yt_idefix-2.1.0.tar.gz` & `tmp/yt_idefix-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_idefix-2.1.0.tar", last modified: Fri Jun  2 09:37:00 2023, max compression
+gzip compressed data, was "yt_idefix-2.2.0.tar", last modified: Sat Jun  3 16:23:07 2023, max compression
```

## Comparing `yt_idefix-2.1.0.tar` & `yt_idefix-2.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:37:00.050260 yt_idefix-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-02 09:37:00.050260 yt_idefix-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:37:00.050260 yt_idefix-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:37:00.038260 yt_idefix-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:37:00.042260 yt_idefix-2.1.0/src/yt_idefix/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:37:00.046259 yt_idefix-2.1.0/src/yt_idefix/_io/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/_io/C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/_io/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/_io/dmp_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/_io/h5_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/_io/vtk_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34740 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:36:50.000000 yt_idefix-2.1.0/src/yt_idefix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:37:00.046259 yt_idefix-2.1.0/src/yt_idefix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-02 09:37:00.000000 yt_idefix-2.1.0/src/yt_idefix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-02 09:37:00.000000 yt_idefix-2.1.0/src/yt_idefix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:37:00.000000 yt_idefix-2.1.0/src/yt_idefix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-02 09:37:00.000000 yt_idefix-2.1.0/src/yt_idefix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-02 09:37:00.000000 yt_idefix-2.1.0/src/yt_idefix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:37:00.000000 yt_idefix-2.1.0/src/yt_idefix.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:37:00.050260 yt_idefix-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-02 09:36:51.000000 yt_idefix-2.1.0/tests/test_C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-02 09:36:51.000000 yt_idefix-2.1.0/tests/test_dmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-02 09:36:51.000000 yt_idefix-2.1.0/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-06-02 09:36:51.000000 yt_idefix-2.1.0/tests/test_vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-02 09:36:51.000000 yt_idefix-2.1.0/tests/test_xdmf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:23:07.492503 yt_idefix-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-03 16:23:07.492503 yt_idefix-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 16:23:07.492503 yt_idefix-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:23:07.484503 yt_idefix-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:23:07.488503 yt_idefix-2.2.0/src/yt_idefix/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:23:07.492503 yt_idefix-2.2.0/src/yt_idefix/_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/_io/C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/_io/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/_io/dmp_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/_io/h5_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/_io/vtk_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34740 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:22:49.000000 yt_idefix-2.2.0/src/yt_idefix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:23:07.492503 yt_idefix-2.2.0/src/yt_idefix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-03 16:23:07.000000 yt_idefix-2.2.0/src/yt_idefix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-03 16:23:07.000000 yt_idefix-2.2.0/src/yt_idefix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:23:07.000000 yt_idefix-2.2.0/src/yt_idefix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-03 16:23:07.000000 yt_idefix-2.2.0/src/yt_idefix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-03 16:23:07.000000 yt_idefix-2.2.0/src/yt_idefix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 16:23:07.000000 yt_idefix-2.2.0/src/yt_idefix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:23:07.492503 yt_idefix-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-03 16:22:50.000000 yt_idefix-2.2.0/tests/test_C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-03 16:22:50.000000 yt_idefix-2.2.0/tests/test_dmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-03 16:22:50.000000 yt_idefix-2.2.0/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-06-03 16:22:50.000000 yt_idefix-2.2.0/tests/test_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-03 16:22:50.000000 yt_idefix-2.2.0/tests/test_xdmf.py
```

### Comparing `yt_idefix-2.1.0/LICENSE` & `yt_idefix-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/PKG-INFO` & `yt_idefix-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt_idefix
-Version: 2.1.0
+Version: 2.2.0
 Summary: An extension module for yt, adding a frontend for Idefix and Pluto
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
```

### Comparing `yt_idefix-2.1.0/README.md` & `yt_idefix-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/pyproject.toml` & `yt_idefix-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/src/yt_idefix/_backports.py` & `yt_idefix-2.2.0/src/yt_idefix/_backports.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/src/yt_idefix/_io/commons.py` & `yt_idefix-2.2.0/src/yt_idefix/_io/commons.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/src/yt_idefix/_io/dmp_io.py` & `yt_idefix-2.2.0/src/yt_idefix/_io/dmp_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/src/yt_idefix/_io/h5_io.py` & `yt_idefix-2.2.0/src/yt_idefix/_io/h5_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/src/yt_idefix/_io/vtk_io.py` & `yt_idefix-2.2.0/src/yt_idefix/_io/vtk_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,15 +197,40 @@
 
         data_type = next(fh).decode().split()[0]  # CELL_DATA (NX-1)(NY-1)(NZ-1)
         next(fh)
 
         array_shape = shape.to_cell_centered()
         assert data_type == "CELL_DATA"
 
-    return Coordinates(coords[0], coords[1], coords[2], array_shape)
+    def warn_invalid(arr):
+        bulk_msg = (
+            "This may result from uninitialized data being written to disk, "
+            "as is a known bug in PLUTO up to version 4.4.patch2 "
+            "in 1D spherical simulations. "
+            "If you are seeing this warning in a different situation, "
+            "please report this."
+        )
+        if any(np.isnan(arr)):
+            warnings.warn(
+                f"NaNs found in coordinate array, behaviour is undefined. {bulk_msg}",
+                stacklevel=8,
+            )
+        elif not np.all(arr[:-1] <= arr[1:]):
+            warnings.warn(
+                f"Coordinate array is not sorted, behaviour is undefined. {bulk_msg}",
+                stacklevel=8,
+            )
+        return arr
+
+    return Coordinates(
+        warn_invalid(coords[0]),
+        warn_invalid(coords[1]),
+        warn_invalid(coords[2]),
+        array_shape,
+    )
 
 
 def read_field_offset_index(
     fh: BinaryIO, shape: Shape, *, default_field_list: list[str]
 ) -> dict[str, int]:
     # assuming fh is correctly positioned (read_grid_coordinates must be called first)
     retv: dict[str, int] = {}
```

### Comparing `yt_idefix-2.1.0/src/yt_idefix/data_structures.py` & `yt_idefix-2.2.0/src/yt_idefix/data_structures.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/src/yt_idefix/definitions.py` & `yt_idefix-2.2.0/src/yt_idefix/definitions.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/src/yt_idefix/fields.py` & `yt_idefix-2.2.0/src/yt_idefix/fields.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 from yt.fields.field_info_container import FieldInfoContainer
 from yt.fields.magnetic_field import setup_magnetic_field_aliases
 
 
-class BaseFields(FieldInfoContainer):
-    # This class can be used later to add functions and attributes common to all fields
-    pass
-
-
-class IdefixVtkFields(BaseFields):
+class IdefixVtkFields(FieldInfoContainer):
     known_other_fields = (
         ("RHO", ("code_mass / code_length**3", ["density"], None)),  # type: ignore
         ("VX1", ("code_length / code_time", ["velocity_x"], None)),
         ("VX2", ("code_length / code_time", ["velocity_y"], None)),
         ("VX3", ("code_length / code_time", ["velocity_z"], None)),
         ("BX1", ("code_magnetic", [], None)),
         ("BX2", ("code_magnetic", [], None)),
         ("BX3", ("code_magnetic", [], None)),
         ("PRS", ("code_pressure", ["pressure"], None)),
+        (
+            "PART_RHO",
+            ("code_mass / code_length**3", ["deposited_particle_density"], None),
+        ),
+        (
+            "PART_VX1",
+            ("code_length / code_time", ["deposited_particle_velocity_x"], None),
+        ),
+        (
+            "PART_VX2",
+            ("code_length / code_time", ["deposited_particle_velocity_y"], None),
+        ),
+        (
+            "PART_VX3",
+            ("code_length / code_time", ["deposited_particle_velocity_z"], None),
+        ),
     )
 
     def setup_fluid_fields(self):
         setup_magnetic_field_aliases(
             self, "idefix-vtk", [f"BX{idir}" for idir in "123"]
         )
 
 
-class IdefixDmpFields(BaseFields):
+class IdefixDmpFields(FieldInfoContainer):
     known_other_fields = (
         ("Vc-RHO", ("code_mass / code_length**3", ["density"], None)),  # type: ignore
         ("Vc-VX1", ("code_length / code_time", ["velocity_x"], None)),
         ("Vc-VX2", ("code_length / code_time", ["velocity_y"], None)),
         ("Vc-VX3", ("code_length / code_time", ["velocity_z"], None)),
         ("Vc-BX1", ("code_magnetic", [], None)),
         ("Vc-BX2", ("code_magnetic", [], None)),
@@ -43,15 +54,15 @@
 
     def setup_fluid_fields(self):
         setup_magnetic_field_aliases(
             self, "idefix-dmp", [f"Vc-BX{idir}" for idir in "123"]
         )
 
 
-class PlutoFields(BaseFields):
+class PlutoFields(FieldInfoContainer):
     known_other_fields = (
         # PLUTO 4 standard variable names normalized in upper case,
         # Referring to Tools/IDL/pload.pro in Pluto v4.2-patch2
         # Field names of ion fractions are normalized to upper case
         # Each entry here is of the form
         # ( "name", ("code_unit", ["alias1", "alias2", ...], "display_name")),
         # where alias should be set with yt-standard-name or pluto-macro-name
```

### Comparing `yt_idefix-2.1.0/src/yt_idefix/io.py` & `yt_idefix-2.2.0/src/yt_idefix/io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/src/yt_idefix.egg-info/PKG-INFO` & `yt_idefix-2.2.0/src/yt_idefix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-idefix
-Version: 2.1.0
+Version: 2.2.0
 Summary: An extension module for yt, adding a frontend for Idefix and Pluto
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
```

### Comparing `yt_idefix-2.1.0/src/yt_idefix.egg-info/SOURCES.txt` & `yt_idefix-2.2.0/src/yt_idefix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/tests/test_C_io.py` & `yt_idefix-2.2.0/tests/test_C_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/tests/test_dmp.py` & `yt_idefix-2.2.0/tests/test_dmp.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/tests/test_loading.py` & `yt_idefix-2.2.0/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/tests/test_vtk.py` & `yt_idefix-2.2.0/tests/test_vtk.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.1.0/tests/test_xdmf.py` & `yt_idefix-2.2.0/tests/test_xdmf.py`

 * *Files identical despite different names*

