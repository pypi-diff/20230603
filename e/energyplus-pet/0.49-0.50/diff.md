# Comparing `tmp/energyplus_pet-0.49.tar.gz` & `tmp/energyplus_pet-0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_pet-0.49.tar", last modified: Fri Apr 14 16:20:53 2023, max compression
+gzip compressed data, was "energyplus_pet-0.50.tar", last modified: Fri Jun  2 22:04:22 2023, max compression
```

## Comparing `energyplus_pet-0.49.tar` & `energyplus_pet-0.50.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:20:53.488829 energyplus_pet-0.49/
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-04-14 16:20:25.000000 energyplus_pet-0.49/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-04-14 16:20:53.488829 energyplus_pet-0.49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-14 16:20:25.000000 energyplus_pet-0.49/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:20:53.484829 energyplus_pet-0.49/energyplus_pet/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/configure.py
--rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/correction_factor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5776 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/data_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:20:53.484829 energyplus_pet-0.49/energyplus_pet/equipment/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13066 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/column_header.py
--rw-r--r--   0 runner    (1001) docker     (122)     2291 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/common_curves.py
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/equip_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    20165 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/wahp_cooling_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)    15424 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/wahp_heating_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)    15053 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/wwhp_cooling_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)    15053 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/wwhp_heating_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:20:53.488829 energyplus_pet-0.49/energyplus_pet/forms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16776 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/base_data_form.py
--rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/basic_message_form.py
--rw-r--r--   0 runner    (1001) docker     (122)     4170 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/catalog_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/comparison_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     8198 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/constant_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)    22194 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/correction_detail_form.py
--rw-r--r--   0 runner    (1001) docker     (122)     9698 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/correction_summary_form.py
--rw-r--r--   0 runner    (1001) docker     (122)     6408 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/correction_summary_widget.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/header_preview.py
--rw-r--r--   0 runner    (1001) docker     (122)    31620 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/main.py
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)    12745 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/units.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:20:53.484829 energyplus_pet-0.49/energyplus_pet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-04-14 16:20:53.000000 energyplus_pet-0.49/energyplus_pet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-04-14 16:20:53.000000 energyplus_pet-0.49/energyplus_pet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 16:20:53.000000 energyplus_pet-0.49/energyplus_pet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-14 16:20:53.000000 energyplus_pet-0.49/energyplus_pet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-14 16:20:53.000000 energyplus_pet-0.49/energyplus_pet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-14 16:20:53.000000 energyplus_pet-0.49/energyplus_pet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-14 16:20:53.488829 energyplus_pet-0.49/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-04-14 16:20:25.000000 energyplus_pet-0.49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:04:22.443636 energyplus_pet-0.50/
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-06-02 22:03:51.000000 energyplus_pet-0.50/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-06-02 22:04:22.443636 energyplus_pet-0.50/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-02 22:03:51.000000 energyplus_pet-0.50/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:04:22.439636 energyplus_pet-0.50/energyplus_pet/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/configure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/correction_factor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5776 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/data_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:04:22.443636 energyplus_pet-0.50/energyplus_pet/equipment/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13066 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/column_header.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2291 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/common_curves.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/equip_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20165 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/wahp_cooling_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15424 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/wahp_heating_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15053 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/wwhp_cooling_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15053 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/wwhp_heating_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:04:22.443636 energyplus_pet-0.50/energyplus_pet/forms/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16776 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/base_data_form.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/basic_message_form.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4170 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/catalog_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/comparison_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8198 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/constant_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22194 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/correction_detail_form.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9698 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/correction_summary_form.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6408 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/correction_summary_widget.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/header_preview.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31620 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12745 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/units.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:04:22.443636 energyplus_pet-0.50/energyplus_pet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-06-02 22:04:22.000000 energyplus_pet-0.50/energyplus_pet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-06-02 22:04:22.000000 energyplus_pet-0.50/energyplus_pet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 22:04:22.000000 energyplus_pet-0.50/energyplus_pet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-02 22:04:22.000000 energyplus_pet-0.50/energyplus_pet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-02 22:04:22.000000 energyplus_pet-0.50/energyplus_pet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-02 22:04:22.000000 energyplus_pet-0.50/energyplus_pet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-02 22:04:22.447636 energyplus_pet-0.50/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-06-02 22:03:51.000000 energyplus_pet-0.50/setup.py
```

### Comparing `energyplus_pet-0.49/LICENSE.txt` & `energyplus_pet-0.50/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/PKG-INFO` & `energyplus_pet-0.50/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus_pet
-Version: 0.49
+Version: 0.50
 Summary: Parameter Estimation Tools for Generating EnergyPlus Inputs from Raw Performance Data
 Home-page: https://github.com/Myoldmopar/EnergyPlusPet
 Author: Edwin Lee, for NREL, for United States Department of Energy
 License: ModifiedBSD
 Description: # EnergyPlus "PET"
         
         This project is a cross platform Python (Tk) GUI and tool kit for generating EnergyPlus inputs from component performance data.
```

### Comparing `energyplus_pet-0.49/README.md` & `energyplus_pet-0.50/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/correction_factor.py` & `energyplus_pet-0.50/energyplus_pet/correction_factor.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/data_manager.py` & `energyplus_pet-0.50/energyplus_pet/data_manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/equipment/base.py` & `energyplus_pet-0.50/energyplus_pet/equipment/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/equipment/column_header.py` & `energyplus_pet-0.50/energyplus_pet/equipment/column_header.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/equipment/common_curves.py` & `energyplus_pet-0.50/energyplus_pet/equipment/common_curves.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/equipment/equip_types.py` & `energyplus_pet-0.50/energyplus_pet/equipment/equip_types.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/equipment/manager.py` & `energyplus_pet-0.50/energyplus_pet/equipment/manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/equipment/wahp_cooling_curve.py` & `energyplus_pet-0.50/energyplus_pet/equipment/wahp_cooling_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/equipment/wahp_heating_curve.py` & `energyplus_pet-0.50/energyplus_pet/equipment/wahp_heating_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/equipment/wwhp_cooling_curve.py` & `energyplus_pet-0.50/energyplus_pet/equipment/wwhp_cooling_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/equipment/wwhp_heating_curve.py` & `energyplus_pet-0.50/energyplus_pet/equipment/wwhp_heating_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/forms/base_data_form.py` & `energyplus_pet-0.50/energyplus_pet/forms/base_data_form.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/forms/basic_message_form.py` & `energyplus_pet-0.50/energyplus_pet/forms/basic_message_form.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/forms/catalog_plot.py` & `energyplus_pet-0.50/energyplus_pet/forms/catalog_plot.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/forms/comparison_plot.py` & `energyplus_pet-0.50/energyplus_pet/forms/comparison_plot.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/forms/constant_parameters.py` & `energyplus_pet-0.50/energyplus_pet/forms/constant_parameters.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/forms/correction_detail_form.py` & `energyplus_pet-0.50/energyplus_pet/forms/correction_detail_form.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/forms/correction_summary_form.py` & `energyplus_pet-0.50/energyplus_pet/forms/correction_summary_form.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/forms/correction_summary_widget.py` & `energyplus_pet-0.50/energyplus_pet/forms/correction_summary_widget.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/forms/header_preview.py` & `energyplus_pet-0.50/energyplus_pet/forms/header_preview.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet/forms/main.py` & `energyplus_pet-0.50/energyplus_pet/forms/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     """This form is the primary GUI entry point for the program; all control runs through here"""
 
     def __init__(self):
         """
         The main window of the parameter estimation tool GUI workflow.
         This window is an instance of a tk.Tk object
         """
+        fixup_taskbar_icon_on_windows(NICE_NAME)
         super().__init__(className=NAME)
 
         # set some basic program information like title and an icon
         self._program_name = NICE_NAME
         program_name_with_version = f"{self._program_name} {VERSION}"
         self.title(program_name_with_version)
         # add the taskbar icon, but its having issues reading the png on Mac, not sure.
@@ -61,15 +62,14 @@
         else:  # Linux
             self.icon_path = Path(__file__).resolve().parent.parent / 'icons' / 'icon.png'
             img = PhotoImage(file=str(self.icon_path))
             if self.icon_path.exists():
                 self.iconphoto(False, img)
             else:
                 print(f"Could not set icon for Windows, expecting to find it at {self.icon_path}")
-        fixup_taskbar_icon_on_windows(NICE_NAME)
 
         # setup event listeners
         self._gui_queue = Queue()
         self._check_queue()
 
         # define the Tk.Variable instances that will be used to communicate with the GUI widgets
         self._define_tk_variables()
```

### Comparing `energyplus_pet-0.49/energyplus_pet/units.py` & `energyplus_pet-0.50/energyplus_pet/units.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/energyplus_pet.egg-info/PKG-INFO` & `energyplus_pet-0.50/energyplus_pet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus-pet
-Version: 0.49
+Version: 0.50
 Summary: Parameter Estimation Tools for Generating EnergyPlus Inputs from Raw Performance Data
 Home-page: https://github.com/Myoldmopar/EnergyPlusPet
 Author: Edwin Lee, for NREL, for United States Department of Energy
 License: ModifiedBSD
 Description: # EnergyPlus "PET"
         
         This project is a cross platform Python (Tk) GUI and tool kit for generating EnergyPlus inputs from component performance data.
```

### Comparing `energyplus_pet-0.49/energyplus_pet.egg-info/SOURCES.txt` & `energyplus_pet-0.50/energyplus_pet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.49/setup.py` & `energyplus_pet-0.50/setup.py`

 * *Files identical despite different names*

