# Comparing `tmp/ScriptCollection-3.3.95-py3-none-any.whl.zip` & `tmp/ScriptCollection-3.3.96-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 59179 bytes, number of entries: 14
+Zip file size: 59631 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat    18064 b- defN 23-Mar-05 15:39 ScriptCollection/Executables.py
 -rw-rw-rw-  2.0 fat    34151 b- defN 23-May-26 16:46 ScriptCollection/GeneralUtilities.py
 -rw-rw-rw-  2.0 fat     1937 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerBase.py
 -rw-rw-rw-  2.0 fat     6275 b- defN 23-May-26 16:46 ScriptCollection/ProgramRunnerEpew.py
 -rw-rw-rw-  2.0 fat     3023 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerPopen.py
--rw-rw-rw-  2.0 fat    89376 b- defN 23-May-26 16:47 ScriptCollection/ScriptCollectionCore.py
--rw-rw-rw-  2.0 fat   133454 b- defN 23-May-26 16:46 ScriptCollection/TasksForCommonProjectStructure.py
+-rw-rw-rw-  2.0 fat    90646 b- defN 23-Jun-03 11:06 ScriptCollection/ScriptCollectionCore.py
+-rw-rw-rw-  2.0 fat   133998 b- defN 23-Jun-03 11:06 ScriptCollection/TasksForCommonProjectStructure.py
 -rw-rw-rw-  2.0 fat     7918 b- defN 22-Aug-30 21:59 ScriptCollection/UpdateCertificates.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-29 05:45 ScriptCollection/__init__.py
--rw-rw-rw-  2.0 fat     7795 b- defN 23-May-26 16:47 ScriptCollection-3.3.95.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-26 16:47 ScriptCollection-3.3.95.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1968 b- defN 23-May-26 16:47 ScriptCollection-3.3.95.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-26 16:47 ScriptCollection-3.3.95.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1295 b- defN 23-May-26 16:47 ScriptCollection-3.3.95.dist-info/RECORD
-14 files, 305365 bytes uncompressed, 56987 bytes compressed:  81.3%
+-rw-rw-rw-  2.0 fat     7795 b- defN 23-Jun-03 11:07 ScriptCollection-3.3.96.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-03 11:07 ScriptCollection-3.3.96.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1968 b- defN 23-Jun-03 11:07 ScriptCollection-3.3.96.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-03 11:07 ScriptCollection-3.3.96.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1295 b- defN 23-Jun-03 11:07 ScriptCollection-3.3.96.dist-info/RECORD
+14 files, 307179 bytes uncompressed, 57439 bytes compressed:  81.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: ScriptCollection/UpdateCertificates.py
 Comment: 
 
 Filename: ScriptCollection/__init__.py
 Comment: 
 
-Filename: ScriptCollection-3.3.95.dist-info/METADATA
+Filename: ScriptCollection-3.3.96.dist-info/METADATA
 Comment: 
 
-Filename: ScriptCollection-3.3.95.dist-info/WHEEL
+Filename: ScriptCollection-3.3.96.dist-info/WHEEL
 Comment: 
 
-Filename: ScriptCollection-3.3.95.dist-info/entry_points.txt
+Filename: ScriptCollection-3.3.96.dist-info/entry_points.txt
 Comment: 
 
-Filename: ScriptCollection-3.3.95.dist-info/top_level.txt
+Filename: ScriptCollection-3.3.96.dist-info/top_level.txt
 Comment: 
 
-Filename: ScriptCollection-3.3.95.dist-info/RECORD
+Filename: ScriptCollection-3.3.96.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScriptCollection/ScriptCollectionCore.py

```diff
@@ -10,27 +10,27 @@
 from random import randrange
 from subprocess import Popen
 import re
 import shutil
 import traceback
 import uuid
 import io
-import ntplib
 import requests
+import ntplib
 import qrcode
 import pycdlib
 import send2trash
 from PyPDF2 import PdfFileMerger
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 from .ProgramRunnerPopen import ProgramRunnerPopen
 from .ProgramRunnerEpew import ProgramRunnerEpew, CustomEpewArgument
 
 
-version = "3.3.95"
+version = "3.3.96"
 __version__ = version
 
 
 class ScriptCollectionCore:
 
     # The purpose of this property is to use it when testing your code which uses scriptcollection for external program-calls.
     # Do not change this value for productive environments.
@@ -1027,14 +1027,34 @@
                     os.remove(file)
                     os.rename(file + ".modified", file)
             self.SCFilenameObfuscator(inputfolder, printtableheadline, namemappingfile, extensions)
         else:
             raise ValueError(f"Directory not found: '{inputfolder}'")
 
     @GeneralUtilities.check_arguments
+    def get_docker_debian_version(self, image_tag: str) -> str:
+        result = ScriptCollectionCore().run_program_argsasarray(
+            "docker", ['run', f'debian:{image_tag}', 'bash', '-c', 'apt-get -y update && apt-get -y install lsb-release && lsb_release -cs'])
+        result_line = GeneralUtilities.string_to_lines(result[1])[-2]
+        return result_line
+
+    @GeneralUtilities.check_arguments
+    def get_latest_tor_version_of_debian_repository(self, debian_version: str) -> str:
+        package_url: str = f"https://deb.torproject.org/torproject.org/dists/{debian_version}/main/binary-amd64/Packages"
+        r = requests.get(package_url, timeout=5)
+        if r.status_code != 200:
+            raise ValueError(f"Checking for latest tor package resulted in HTTP-response-code {r.status_code}.")
+        lines = GeneralUtilities.string_to_lines(GeneralUtilities.bytes_to_string(r.content))
+        version_line_prefix = "Version: "
+        version_content_line = [line for line in lines if line.startswith(version_line_prefix)][1]
+        version_with_overhead = version_content_line[len(version_line_prefix):]
+        tor_version = version_with_overhead.split("~")[0]
+        return tor_version
+
+    @GeneralUtilities.check_arguments
     def upload_file_to_file_host(self, file: str, host: str) -> int:
         if (host is None):
             return self.upload_file_to_random_filesharing_service(file)
         elif host == "anonfiles.com":
             return self.upload_file_to_anonfiles(file)
         elif host == "bayfiles.com":
             return self.upload_file_to_bayfiles(file)
```

## ScriptCollection/TasksForCommonProjectStructure.py

```diff
@@ -1739,14 +1739,21 @@
     def __check_if_changelog_exists(self, repository_folder: str, project_version: str):
         changelog_folder = os.path.join(repository_folder, "Other", "Resources", "Changelog")
         changelog_file = os.path.join(changelog_folder, f"v{project_version}.md")
         if not os.path.isfile(changelog_file):
             raise ValueError(f"Changelog-file '{changelog_file}' does not exist.")
 
     @GeneralUtilities.check_arguments
+    def update_dependency_in_resources_folder(self, update_dependencies_file, dependency_name: str, latest_version_function: str):
+        version_file = GeneralUtilities.resolve_relative_path(f"../Resources/Dependencies/{dependency_name}/Version.txt", update_dependencies_file)
+        current_version = GeneralUtilities.read_text_from_file(version_file)
+        if current_version != latest_version_function:
+            GeneralUtilities.write_text_to_file(version_file, latest_version_function)
+
+    @GeneralUtilities.check_arguments
     def ensure_grylibrary_is_available(self, codeunit_folder: str):
         grylibrary_folder = os.path.join(codeunit_folder, "Other", "Resources", "GRYLibrary")
         grylibrary_dll_file = os.path.join(grylibrary_folder, "BuildResult_DotNet_win-x64", "GRYLibrary.dll")
         internet_connection_is_available = GeneralUtilities.internet_connection_is_available()
         grylibrary_dll_file_exists = os.path.isfile(grylibrary_dll_file)
         if internet_connection_is_available:  # Load/Update GRYLibrary
             grylibrary_latest_codeunit_file = "https://raw.githubusercontent.com/anionDev/GRYLibrary/stable/GRYLibrary/GRYLibrary.codeunit.xml"
```

## Comparing `ScriptCollection-3.3.95.dist-info/METADATA` & `ScriptCollection-3.3.96.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScriptCollection
-Version: 3.3.95
+Version: 3.3.96
 Summary: The ScriptCollection is the place for reusable scripts.
 Home-page: https://github.com/anionDev/ScriptCollection
 Author: Marius Göcke
 Author-email: marius.goecke@gmail.com
 Project-URL: Documentation, https://aniondev.github.io/ScriptCollectionReference/index.html
 Project-URL: Changelog, https://github.com/anionDev/ScriptCollection/tree/main/Other/Resources/Changelog
 Keywords: package release build management
```

## Comparing `ScriptCollection-3.3.95.dist-info/entry_points.txt` & `ScriptCollection-3.3.96.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ScriptCollection-3.3.95.dist-info/RECORD` & `ScriptCollection-3.3.96.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ScriptCollection/Executables.py,sha256=kXTIX92KLeFuxnYOlsyFs5lkznsxkuoBMVrV3OU7FZU,18064
 ScriptCollection/GeneralUtilities.py,sha256=rRQPyyRNZ1U0UDEuAqKZl3lHj38_4KofM6ON6hXqyRA,34151
 ScriptCollection/ProgramRunnerBase.py,sha256=2kyOuoM3oFjBfLc9Q5t5RTz7Ya2CjUxFtB1rBBDmnjU,1937
 ScriptCollection/ProgramRunnerEpew.py,sha256=nIzY4dG6W-xEpkeoTbozwNZtFSIo-bU_W6t6u1AZKtE,6275
 ScriptCollection/ProgramRunnerPopen.py,sha256=HOs1QVnXiQtwXy1_xvH79bWBdd0i-2tUyyLloQBvMto,3023
-ScriptCollection/ScriptCollectionCore.py,sha256=rR5ASCMiRfeAVO_L1RckujpqgQDSsdEHVDC2YcjdnPg,89376
-ScriptCollection/TasksForCommonProjectStructure.py,sha256=gZUEpmsqWqMi3Jd_6ur0yHJnZwJbelH47CawbXsiMNs,133454
+ScriptCollection/ScriptCollectionCore.py,sha256=gge6WqnQBPQ5HEg-Aq8AKgeU7zL93yezHey5l5n3GH0,90646
+ScriptCollection/TasksForCommonProjectStructure.py,sha256=R641ijodm622j-BTdAFgZNTWJ1vXRN1Y7ZOEPEBIkRw,133998
 ScriptCollection/UpdateCertificates.py,sha256=Go-JJK-YTi7aBB1phlLxypa8GHkmFHBEPB0_TT9G-bw,7918
 ScriptCollection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ScriptCollection-3.3.95.dist-info/METADATA,sha256=XP4pCfbejx3K-6hZsSiFYZ_xULbaoywGYON1SQrRxTo,7795
-ScriptCollection-3.3.95.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ScriptCollection-3.3.95.dist-info/entry_points.txt,sha256=VIuxVCOpX38lSJUwRRENBNgcGKTIBxQyrCfbJVRHP8g,1968
-ScriptCollection-3.3.95.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
-ScriptCollection-3.3.95.dist-info/RECORD,,
+ScriptCollection-3.3.96.dist-info/METADATA,sha256=IpLGAGMOMJAaNRqy-1j-AUnXFMFJshTeICKroaVdbs0,7795
+ScriptCollection-3.3.96.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ScriptCollection-3.3.96.dist-info/entry_points.txt,sha256=VIuxVCOpX38lSJUwRRENBNgcGKTIBxQyrCfbJVRHP8g,1968
+ScriptCollection-3.3.96.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
+ScriptCollection-3.3.96.dist-info/RECORD,,
```

