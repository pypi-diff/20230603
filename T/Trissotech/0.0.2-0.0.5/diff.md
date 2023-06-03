# Comparing `tmp/trissotech-0.0.2.tar.gz` & `tmp/trissotech-0.0.5.tar.gz`

## Comparing `trissotech-0.0.2.tar` & `trissotech-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 trissotech-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 trissotech-0.0.2/.idea/Libreria_Trisso.iml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 trissotech-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 trissotech-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 trissotech-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 trissotech-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 trissotech-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 trissotech-0.0.2/src/Trissotech/API.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trissotech-0.0.2/src/Trissotech/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 trissotech-0.0.2/LICENSE
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 trissotech-0.0.2/README.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 trissotech-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 trissotech-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 trissotech-0.0.5/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 trissotech-0.0.5/.idea/Libreria_Trisso.iml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 trissotech-0.0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 trissotech-0.0.5/.idea/modules.xml
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 trissotech-0.0.5/.idea/workspace.xml
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 trissotech-0.0.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 trissotech-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 trissotech-0.0.5/src/Trissotech/API.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trissotech-0.0.5/src/Trissotech/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 trissotech-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 trissotech-0.0.5/README.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 trissotech-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 trissotech-0.0.5/PKG-INFO
```

### Comparing `trissotech-0.0.2/.idea/workspace.xml` & `trissotech-0.0.5/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `trissotech-0.0.2/.idea/workspace.xml` & `trissotech-0.0.5/.idea/workspace.xml`

```diff
@@ -22,26 +22,27 @@
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
-    "WebServerToolWindowFactoryState": "false"
+    "WebServerToolWindowFactoryState": "false",
+    "nodejs_package_manager_path": "npm"
   }
 }]]></component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="bc3f8460-bde2-43f1-ac31-a6d2c8e074fd" name="Changes" comment=""/>
       <created>1685737594004</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1685737594004</updated>
-      <workItem from="1685737616821" duration="2739000"/>
+      <workItem from="1685737616821" duration="5180000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
 </project>
```

### Comparing `trissotech-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `trissotech-0.0.5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `trissotech-0.0.2/src/Trissotech/API.py` & `trissotech-0.0.5/src/Trissotech/API.py`

 * *Files identical despite different names*

### Comparing `trissotech-0.0.2/LICENSE` & `trissotech-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trissotech-0.0.2/pyproject.toml` & `trissotech-0.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Trissotech"
-version = "0.0.2"
+version = "0.0.5"
 authors = [
   { name="Facu", email="facundonieto@mi.unc.edu.ar" },
 ]
 description = "Trissotech library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,8 +19,8 @@
 
 dependencies = [
   "pillow",
 ]
 
 [project.urls]
 "Homepage" = "https://www.trissotech.com/"
-"Bug Tracker" = "https://www.facundonieto.com/Contact"
+"Bug Tracker" = "https://www.facundonieto.com/contact"
```

