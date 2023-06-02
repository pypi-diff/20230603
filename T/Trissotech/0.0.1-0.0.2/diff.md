# Comparing `tmp/trissotech-0.0.1.tar.gz` & `tmp/trissotech-0.0.2.tar.gz`

## Comparing `trissotech-0.0.1.tar` & `trissotech-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 trissotech-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 trissotech-0.0.1/.idea/Libreria_Trisso.iml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 trissotech-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 trissotech-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 trissotech-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 trissotech-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 trissotech-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 trissotech-0.0.1/src/Trissotech/API.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trissotech-0.0.1/src/Trissotech/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 trissotech-0.0.1/LICENSE
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 trissotech-0.0.1/README.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 trissotech-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 trissotech-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 trissotech-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 trissotech-0.0.2/.idea/Libreria_Trisso.iml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 trissotech-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 trissotech-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 trissotech-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 trissotech-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 trissotech-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 trissotech-0.0.2/src/Trissotech/API.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trissotech-0.0.2/src/Trissotech/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 trissotech-0.0.2/LICENSE
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 trissotech-0.0.2/README.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 trissotech-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 trissotech-0.0.2/PKG-INFO
```

### Comparing `trissotech-0.0.1/.idea/workspace.xml` & `trissotech-0.0.2/.idea/workspace.xml`

 * *Files 0% similar despite different names*

#### Comparing `trissotech-0.0.1/.idea/workspace.xml` & `trissotech-0.0.2/.idea/workspace.xml`

```diff
@@ -33,15 +33,15 @@
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="bc3f8460-bde2-43f1-ac31-a6d2c8e074fd" name="Changes" comment=""/>
       <created>1685737594004</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1685737594004</updated>
-      <workItem from="1685737616821" duration="2082000"/>
+      <workItem from="1685737616821" duration="2739000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
 </project>
```

### Comparing `trissotech-0.0.1/.idea/inspectionProfiles/Project_Default.xml` & `trissotech-0.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `trissotech-0.0.1/src/Trissotech/API.py` & `trissotech-0.0.2/src/Trissotech/API.py`

 * *Files identical despite different names*

### Comparing `trissotech-0.0.1/LICENSE` & `trissotech-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trissotech-0.0.1/pyproject.toml` & `trissotech-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Trissotech"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Facu", email="facundonieto@mi.unc.edu.ar" },
 ]
 description = "Trissotech library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-  "base64",
   "pillow",
-  "base64",
-  "io",
 ]
 
 [project.urls]
 "Homepage" = "https://www.trissotech.com/"
 "Bug Tracker" = "https://www.facundonieto.com/Contact"
```

### Comparing `trissotech-0.0.1/PKG-INFO` & `trissotech-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: Trissotech
-Version: 0.0.1
+Version: 0.0.2
 Summary: Trissotech library
 Project-URL: Homepage, https://www.trissotech.com/
 Project-URL: Bug Tracker, https://www.facundonieto.com/Contact
 Author-email: Facu <facundonieto@mi.unc.edu.ar>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: base64
-Requires-Dist: io
 Requires-Dist: pillow
 Description-Content-Type: text/markdown
 
 Librería de la empresa Trissotech
```

