# Comparing `tmp/normcap-0.4.2.tar.gz` & `tmp/normcap-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "normcap-0.4.2.tar", max compression
+gzip compressed data, was "normcap-0.4.3.tar", max compression
```

## Comparing `normcap-0.4.2.tar` & `normcap-0.4.3.tar`

### file list

```diff
@@ -1,65 +1,64 @@
--rw-r--r--   0        0        0    13806 2023-05-21 10:20:44.792297 normcap-0.4.2/CHANGELOG
--rw-r--r--   0        0        0      724 2023-05-21 10:20:44.792297 normcap-0.4.2/LICENSE
--rw-r--r--   0        0        0     6999 2023-05-21 10:20:44.792297 normcap-0.4.2/README.md
--rw-r--r--   0        0        0       46 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/__init__.py
--rw-r--r--   0        0        0      113 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/__main__.py
--rw-r--r--   0        0        0     1659 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/app.py
--rw-r--r--   0        0        0      450 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/clipboard/__init__.py
--rw-r--r--   0        0        0     1440 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/clipboard/linux.py
--rw-r--r--   0        0        0      588 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/clipboard/macos.py
--rw-r--r--   0        0        0      284 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/clipboard/qt.py
--rw-r--r--   0        0        0     5885 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/clipboard/windows.py
--rw-r--r--   0        0        0        0 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/__init__.py
--rw-r--r--   0        0        0     8955 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/constants.py
--rw-r--r--   0        0        0     2356 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/downloader.py
--rw-r--r--   0        0        0     8359 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/language_manager.py
--rw-r--r--   0        0        0     2753 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/loading_indicator.py
--rw-r--r--   0        0        0    10108 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/menu_button.py
--rw-r--r--   0        0        0     3481 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/models.py
--rw-r--r--   0        0        0     3949 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/notifier.py
--rw-r--r--   0        0        0   217598 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/resources.py
--rw-r--r--   0        0        0     3552 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/settings.py
--rw-r--r--   0        0        0     6205 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/system_info.py
--rw-r--r--   0        0        0    20841 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/tray.py
--rw-r--r--   0        0        0     4568 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/update_check.py
--rw-r--r--   0        0        0      758 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/utils.py
--rw-r--r--   0        0        0    11944 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/window.py
--rw-r--r--   0        0        0       93 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/__init__.py
--rw-r--r--   0        0        0     3603 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/enhance.py
--rw-r--r--   0        0        0       46 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/__init__.py
--rw-r--r--   0        0        0      870 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/base_magic.py
--rw-r--r--   0        0        0     1807 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/email_magic.py
--rw-r--r--   0        0        0     2463 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/magic.py
--rw-r--r--   0        0        0     1048 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/multi_line_magic.py
--rw-r--r--   0        0        0     1546 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/paragraph_magic.py
--rw-r--r--   0        0        0      964 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/single_line_magic.py
--rw-r--r--   0        0        0     2699 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/url_magic.py
--rw-r--r--   0        0        0     5121 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/models.py
--rw-r--r--   0        0        0     1535 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/ocr/recognize.py
--rw-r--r--   0        0        0     3321 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/ocr/tesseract.py
--rw-r--r--   0        0        0        0 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/__init__.py
--rw-r--r--   0        0        0    13773 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/normcap.png
--rw-r--r--   0        0        0    24936 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/normcap.svg
--rw-r--r--   0        0        0     9267 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/notification.png
--rw-r--r--   0        0        0    16576 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/notification.svg
--rw-r--r--   0        0        0     9267 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/parse.png
--rw-r--r--   0        0        0    16576 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/parse.svg
--rw-r--r--   0        0        0     2982 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/raw.png
--rw-r--r--   0        0        0    14953 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/raw.svg
--rw-r--r--   0        0        0      528 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/resources.qrc
--rw-r--r--   0        0        0    17968 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/settings.png
--rw-r--r--   0        0        0    13793 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/settings.svg
--rw-r--r--   0        0        0    17311 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/tray.png
--rw-r--r--   0        0        0    16523 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/tray.svg
--rw-r--r--   0        0        0       79 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/tessdata/.keep
--rw-r--r--   0        0        0    11358 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/tessdata/LICENSE.txt
--rw-r--r--   0        0        0     1081 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/tessdata/README.txt
--rw-r--r--   0        0        0     1242 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/screengrab/__init__.py
--rw-r--r--   0        0        0     7202 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/screengrab/dbus_portal.py
--rw-r--r--   0        0        0     1816 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/screengrab/dbus_shell.py
--rw-r--r--   0        0        0      461 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/screengrab/qt.py
--rw-r--r--   0        0        0     5512 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/screengrab/utils.py
--rw-r--r--   0        0        0     7463 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/utils.py
--rw-r--r--   0        0        0     7044 2023-05-21 10:20:45.124303 normcap-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     8174 1970-01-01 00:00:00.000000 normcap-0.4.2/setup.py
--rw-r--r--   0        0        0     8440 1970-01-01 00:00:00.000000 normcap-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    14292 2023-06-03 18:44:49.584327 normcap-0.4.3/CHANGELOG
+-rw-r--r--   0        0        0      724 2023-06-03 18:44:49.584327 normcap-0.4.3/LICENSE
+-rw-r--r--   0        0        0     6999 2023-06-03 18:44:49.584327 normcap-0.4.3/README.md
+-rw-r--r--   0        0        0       46 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/__init__.py
+-rw-r--r--   0        0        0      113 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/__main__.py
+-rw-r--r--   0        0        0     1673 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/app.py
+-rw-r--r--   0        0        0      450 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/clipboard/__init__.py
+-rw-r--r--   0        0        0     1440 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/clipboard/linux.py
+-rw-r--r--   0        0        0      588 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/clipboard/macos.py
+-rw-r--r--   0        0        0      284 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/clipboard/qt.py
+-rw-r--r--   0        0        0     5885 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/clipboard/windows.py
+-rw-r--r--   0        0        0        0 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/gui/__init__.py
+-rw-r--r--   0        0        0     8491 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/gui/constants.py
+-rw-r--r--   0        0        0     2356 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/gui/downloader.py
+-rw-r--r--   0        0        0     8359 2023-06-03 18:44:49.904332 normcap-0.4.3/normcap/gui/language_manager.py
+-rw-r--r--   0        0        0     2753 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/loading_indicator.py
+-rw-r--r--   0        0        0    10108 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/menu_button.py
+-rw-r--r--   0        0        0     3481 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/models.py
+-rw-r--r--   0        0        0     3949 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/notifier.py
+-rw-r--r--   0        0        0   217598 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/resources.py
+-rw-r--r--   0        0        0     3552 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/settings.py
+-rw-r--r--   0        0        0     6205 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/system_info.py
+-rw-r--r--   0        0        0    20934 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/tray.py
+-rw-r--r--   0        0        0     4568 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/update_check.py
+-rw-r--r--   0        0        0      758 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/utils.py
+-rw-r--r--   0        0        0    11944 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/gui/window.py
+-rw-r--r--   0        0        0       93 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/__init__.py
+-rw-r--r--   0        0        0     3603 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/enhance.py
+-rw-r--r--   0        0        0       46 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/__init__.py
+-rw-r--r--   0        0        0      870 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/base_magic.py
+-rw-r--r--   0        0        0     1807 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/email_magic.py
+-rw-r--r--   0        0        0     2463 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/magic.py
+-rw-r--r--   0        0        0     1048 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/multi_line_magic.py
+-rw-r--r--   0        0        0     1546 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/paragraph_magic.py
+-rw-r--r--   0        0        0      964 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/single_line_magic.py
+-rw-r--r--   0        0        0     2699 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/magics/url_magic.py
+-rw-r--r--   0        0        0     5121 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/models.py
+-rw-r--r--   0        0        0     1535 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/recognize.py
+-rw-r--r--   0        0        0     3321 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/ocr/tesseract.py
+-rw-r--r--   0        0        0        0 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/__init__.py
+-rw-r--r--   0        0        0    13773 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/normcap.png
+-rw-r--r--   0        0        0    24936 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/normcap.svg
+-rw-r--r--   0        0        0     9267 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/notification.png
+-rw-r--r--   0        0        0    16576 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/notification.svg
+-rw-r--r--   0        0        0     9267 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/parse.png
+-rw-r--r--   0        0        0    16576 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/parse.svg
+-rw-r--r--   0        0        0     2982 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/raw.png
+-rw-r--r--   0        0        0    14953 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/raw.svg
+-rw-r--r--   0        0        0      528 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/resources.qrc
+-rw-r--r--   0        0        0    17968 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/settings.png
+-rw-r--r--   0        0        0    13793 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/settings.svg
+-rw-r--r--   0        0        0    17311 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/tray.png
+-rw-r--r--   0        0        0    16523 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/icons/tray.svg
+-rw-r--r--   0        0        0       79 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/tessdata/.keep
+-rw-r--r--   0        0        0    11358 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/tessdata/LICENSE.txt
+-rw-r--r--   0        0        0     1081 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/resources/tessdata/README.txt
+-rw-r--r--   0        0        0     1242 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/screengrab/__init__.py
+-rw-r--r--   0        0        0     7298 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/screengrab/dbus_portal.py
+-rw-r--r--   0        0        0     1816 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/screengrab/dbus_shell.py
+-rw-r--r--   0        0        0      461 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/screengrab/qt.py
+-rw-r--r--   0        0        0     5512 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/screengrab/utils.py
+-rw-r--r--   0        0        0     7611 2023-06-03 18:44:49.908332 normcap-0.4.3/normcap/utils.py
+-rw-r--r--   0        0        0     6967 2023-06-03 18:44:49.912332 normcap-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     8440 1970-01-01 00:00:00.000000 normcap-0.4.3/PKG-INFO
```

### Comparing `normcap-0.4.2/CHANGELOG` & `normcap-0.4.3/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## v0.4.3 (2023-06-03)
+
+- All: Add command line flag `--background-mode` to start normcap minimized
+  ([#439](https://github.com/dynobo/normcap/issues/439))
+- macOS: Improve dialog that is shown in case screenshot permissions are missing.
+- Windows: Fix upgrading with `msi`-installer might lead to error on startup.
+  ([#452](https://github.com/dynobo/normcap/issues/452))
+- Windows: Upgrading with `msi`-installer should not remove downloaded languages in
+  future versions anymore.
+
 ## v0.4.2 (2023-05-21)
 
 - Fix quotes in detected text can result in wrong detection.
   ([#446](https://github.com/dynobo/normcap/issues/446))
 - Update AppImage base image from Ubuntu 18.04 (deprected) to 20.04.
 
 ## v0.4.1 (2023-05-01)
```

### Comparing `normcap-0.4.2/LICENSE` & `normcap-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/README.md` & `normcap-0.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 [![Screencast](https://user-images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/assets/normcap.gif)
 
 ## Quickstart
 
 Install a prebuilt release:
 
 - **Windows**:
-  [NormCap-0.4.2-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64-Windows.msi)
+  [NormCap-0.4.3-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-x86_64-Windows.msi)
 - **Linux**:
-  [NormCap-0.4.2-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64.AppImage)
+  [NormCap-0.4.3-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-x86_64.AppImage)
 - **macOS** (x86) ¹:
-  [NormCap-0.4.2-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64-macOS.dmg)
+  [NormCap-0.4.3-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-x86_64-macOS.dmg)
 - **macOS** (M1) ¹·²:
-  [NormCap-0.4.2-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-arm64-macOS.dmg)
+  [NormCap-0.4.3-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-arm64-macOS.dmg)
   \
   <sub>1: On macOS, allow the unsigned application on first start: "System
   Preferences" → "Security & Privacy" → "General" → "Open anyway". You might also need
   to allow NormCap to take screenshots.
   [#135](https://github.com/dynobo/normcap/issues/135)<br> 2: Might be available a bit
   delayed, as it is currently build manually. (Thx,
   [@Takrin](https://github.com/Takrin)!)</sub>
```

#### html2text {}

```diff
@@ -19,22 +19,22 @@
 (https://github.com/dynobo/normcap) | [Documentation](https://dynobo.github.io/
 normcap/) | [FAQs](https://dynobo.github.io/normcap/#faqs) | [Releases](https:/
 /github.com/dynobo/normcap/releases) | [Changelog](https://github.com/dynobo/
 normcap/blob/main/CHANGELOG) [![Screencast](https://user-
 images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-
 cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/
 assets/normcap.gif) ## Quickstart Install a prebuilt release: - **Windows**:
-[NormCap-0.4.2-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/
-download/v0.4.2/NormCap-0.4.2-x86_64-Windows.msi) - **Linux**: [NormCap-0.4.2-
-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.2/
-NormCap-0.4.2-x86_64.AppImage) - **macOS** (x86) Â¹: [NormCap-0.4.2-x86_64-
-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-
-0.4.2-x86_64-macOS.dmg) - **macOS** (M1) Â¹Â·Â²: [NormCap-0.4.2-arm64-
-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-
-0.4.2-arm64-macOS.dmg) \ 1: On macOS, allow the unsigned application on first
+[NormCap-0.4.3-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/
+download/v0.4.3/NormCap-0.4.3-x86_64-Windows.msi) - **Linux**: [NormCap-0.4.3-
+x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.3/
+NormCap-0.4.3-x86_64.AppImage) - **macOS** (x86) Â¹: [NormCap-0.4.3-x86_64-
+macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-
+0.4.3-x86_64-macOS.dmg) - **macOS** (M1) Â¹Â·Â²: [NormCap-0.4.3-arm64-
+macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-
+0.4.3-arm64-macOS.dmg) \ 1: On macOS, allow the unsigned application on first
 start: "System Preferences" â "Security & Privacy" â "General" â "Open
 anyway". You might also need to allow NormCap to take screenshots. [#135]
 (https://github.com/dynobo/normcap/issues/135)
 2: Might be available a bit delayed, as it is currently build manually. (Thx,
 [@Takrin](https://github.com/Takrin)!) Install from repositories: -
 **Windows**: Install from [Microsoft Store](https://apps.microsoft.com/store/
 detail/normcap/XPDLJNB4B6C2ZR). - **Arch / Manjaro**: Install the [`normcap`]
```

### Comparing `normcap-0.4.2/normcap/app.py` & `normcap-0.4.3/normcap/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 
 from normcap import __version__, utils
 from normcap.gui import system_info
 from normcap.gui.tray import SystemTray
 
 
 def _get_args() -> Namespace:
-    """Start main application logic."""
     args = utils.create_argparser().parse_args()
+    if args.background_mode:
+        args.tray = True
     if args.version:
         print(f"NormCap {__version__}")  # noqa: T201
         sys.exit(0)
     return args
 
 
 def _prepare_logging(args: Namespace) -> None:
```

### Comparing `normcap-0.4.2/normcap/clipboard/linux.py` & `normcap-0.4.3/normcap/clipboard/linux.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/clipboard/macos.py` & `normcap-0.4.3/normcap/clipboard/macos.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/clipboard/windows.py` & `normcap-0.4.3/normcap/clipboard/windows.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/gui/constants.py` & `normcap-0.4.3/normcap/gui/constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,135 +31,135 @@
 
 TESSDATA_REPO = "https://github.com/tesseract-ocr/tessdata_fast"
 TESSDATA_BASE_URL = f"{TESSDATA_REPO}/raw/4.1.0/"
 
 LANGUAGES = (
     ("afr", "2.5 MB", "Afrikaans", "Afrikaans"),
     ("amh", "5.2 MB", "Amharic", "አማርኛ"),
-    ("ara", "1.3 MB", "Arabic", "العربية"),  # noqa: RUF001
+    ("ara", "1.3 MB", "Arabic", "العربية"),
     ("asm", "1.9 MB", "Assamese", "অসমীয়া"),
-    ("aze", "3.3 MB", "Azerbaijani", "آذربایجان دیلی"),  # noqa: RUF001
-    ("aze_cyrl", "1.8 MB", "Azerbaijani (cyrillic)", "Азәрбајҹан дили"),  # noqa: RUF001
-    ("bel", "3.5 MB", "Belarusian", "беларуская мова"),  # noqa: RUF001
+    ("aze", "3.3 MB", "Azerbaijani", "آذربایجان دیلی"),
+    ("aze_cyrl", "1.8 MB", "Azerbaijani (cyrillic)", "Азәрбајҹан дили"),
+    ("bel", "3.5 MB", "Belarusian", "беларуская мова"),
     ("ben", "0.8 MB", "Bengali", "বাংলা"),
     ("bod", "1.8 MB", "Tibetan", "བོད་ཡིག"),
     ("bos", "2.3 MB", "Bosnian", "bosanski jezik"),
     ("bre", "6.0 MB", "Breton", "brezhoneg"),
-    ("bul", "1.6 MB", "Bulgarian", "български език"),  # noqa: RUF001
+    ("bul", "1.6 MB", "Bulgarian", "български език"),
     ("cat", "1.0 MB", "Catalan; Valencian", "català"),
     ("ceb", "0.6 MB", "Cebuano", "Sinugbuanong Binisayâ"),
     ("ces", "3.6 MB", "Czech", "čeština; český jazyk"),
     ("chi_sim", "2.3 MB", "Chinese, simplified", "中文; 汉语; 漢語"),
     ("chi_sim_vert", "1.8 MB", "Chinese, simplified (vertical)", "中文; 汉语; 漢語"),
     ("chi_tra", "2.2 MB", "Chinese, traditional", "中文; 汉语; 漢語"),
     ("chi_tra_vert", "1.7 MB", "Chinese, traditional (vertical)", "中文; 汉语; 漢語"),
-    ("chr", "0.3 MB", "Cherokee", "ᏣᎳᎩ ᎦᏬᏂᎯᏍᏗ"),  # noqa: RUF001
+    ("chr", "0.3 MB", "Cherokee", "ᏣᎳᎩ ᎦᏬᏂᎯᏍᏗ"),
     ("cos", "2.1 MB", "Corsican", "corsu"),
     ("cym", "2.1 MB", "Welsh", "Cymraeg"),
     ("dan", "2.4 MB", "Danish", "dansk"),
     ("dan_frak", "1.6 MB", "Danish (fraktur)", "dansk"),
     ("deu", "1.4 MB", "German", "Deutsch"),
     ("deu_frak", "2.0 MB", "German (fraktur)", "Deutsch"),
     ("div", "1.6 MB", "Divehi; Dhivehi; Maldivian", "ދިވެހި"),
     ("dzo", "0.4 MB", "Dzongkha", "རྫོང་ཁ"),
-    ("ell", "1.3 MB", "Greek", "ελληνικά"),  # noqa: RUF001
+    ("ell", "1.3 MB", "Greek", "ελληνικά"),
     ("eng", "3.9 MB", "English", "English"),
     ("enm", "2.9 MB", "Middle English (1100-1500)", ""),
     ("epo", "4.5 MB", "Esperanto", "Esperanto"),
     ("equ", "2.1 MB", "Equations; Math", ""),
     ("est", "4.2 MB", "Estonian", "eesti keel"),
     ("eus", "4.9 MB", "Basque", "euskara; euskera"),
     ("fao", "3.2 MB", "Faroese", "føroyskt"),
-    ("fas", "0.4 MB", "Persian; Farsi", "فارسی"),  # noqa: RUF001
+    ("fas", "0.4 MB", "Persian; Farsi", "فارسی"),
     ("fil", "1.7 MB", "Filipino", "wikang filipino"),
     ("fin", "7.5 MB", "Finnish", "suomen kieli"),
     ("fra", "1.0 MB", "French", "français"),
     ("frk", "6.1 MB", "Frankish", ""),
     ("frm", "1.9 MB", "Middle French (1400-1600)", ""),
     ("fry", "1.8 MB", "Western Frisian", "Frysk"),
     ("gla", "2.9 MB", "Gaelic", "Gàidhlig"),
     ("gle", "1.1 MB", "Irish", "Gaeilge"),
     ("glg", "2.4 MB", "Galician", "galego"),
     ("grc", "2.1 MB", "Ancient Greek (to 1453)", ""),
     ("guj", "1.3 MB", "Gujarati", "ગુજરાતી"),
     ("hat", "1.8 MB", "Haitian", "Kreyòl ayisyen"),
-    ("heb", "0.9 MB", "Hebrew", "עברית"),  # noqa: RUF001
+    ("heb", "0.9 MB", "Hebrew", "עברית"),
     ("hin", "1.0 MB", "Hindi", "हिन्दी; हिंदी"),
     ("hrv", "3.9 MB", "Croatian", "hrvatski jezik"),
     ("hun", "5.0 MB", "Hungarian", "magyar"),
-    ("hye", "3.3 MB", "Armenian", "Հայերեն"),  # noqa: RUF001
+    ("hye", "3.3 MB", "Armenian", "Հայերեն"),
     ("iku", "2.6 MB", "Inuktitut", "ᐃᓄᒃᑎᑐᑦ"),
     ("ind", "1.0 MB", "Indonesian", "Bahasa Indonesia"),
     ("isl", "2.1 MB", "Icelandic", "Íslenska"),
     ("ita", "2.5 MB", "Italian", "italiano"),
     ("ita_old", "3.1 MB", "Italian (old)", ""),
     ("jav", "2.8 MB", "Javanese", "ꦧꦱꦗꦮ"),
     ("jpn", "2.3 MB", "Japanese", "日本語; にほんご"),
     ("jpn_vert", "2.9 MB", "Japanese (vertical)", "日本語; にほんご"),
     ("kan", "3.4 MB", "Kannada", "ಕನ್ನಡ"),
     ("kat", "2.4 MB", "Georgian", "ქართული"),
     ("kat_old", "0.4 MB", "Georgian (old)", "ქართული"),
-    ("kaz", "4.5 MB", "Kazakh", "қазақ тілі"),  # noqa: RUF001
+    ("kaz", "4.5 MB", "Kazakh", "қазақ тілі"),
     ("khm", "1.3 MB", "Khmer", "ខ្មែរ; ខេមរភាសា; ភាសាខ្មែរ"),
-    ("kir", "9.4 MB", "Kirghiz", "Кыргыз тили"),  # noqa: RUF001
+    ("kir", "9.4 MB", "Kirghiz", "Кыргыз тили"),
     ("kmr", "3.4 MB", "Northern Kurdish", ""),
     ("kor", "1.6 MB", "Korean", "한국어"),
     ("kor_vert", "1.0 MB", "Korean (vertical)", "한국어"),
     ("lao", "6.0 MB", "Lao", "ພາສາລາວ"),
     ("lat", "3.0 MB", "Latin", "lingua latina"),
     ("lav", "2.5 MB", "Latvian", "latviešu valoda"),
     ("lit", "3.0 MB", "Lithuanian", "lietuvių kalba"),
     ("ltz", "2.4 MB", "Luxembourgish", "Lëtzebuergesch"),
-    ("mal", "5.0 MB", "Malayalam", "മലയാളം"),  # noqa: RUF001
+    ("mal", "5.0 MB", "Malayalam", "മലയാളം"),
     ("mar", "2.0 MB", "Marathi", "मराठी"),
-    ("mkd", "1.5 MB", "Macedonian", "македонски јазик"),  # noqa: RUF001
+    ("mkd", "1.5 MB", "Macedonian", "македонски јазик"),
     ("mlt", "2.2 MB", "Maltese", "Malti"),
-    ("mon", "2.0 MB", "Mongolian", "Монгол хэл"),  # noqa: RUF001
+    ("mon", "2.0 MB", "Mongolian", "Монгол хэл"),
     ("mri", "0.8 MB", "Maori", "te reo Māori"),
-    ("msa", "1.6 MB", "Malay", "bahasa Melayu; بهاس ملايو\u200e"),  # noqa: RUF001
+    ("msa", "1.6 MB", "Malay", "bahasa Melayu; بهاس ملايو\u200e"),
     ("mya", "4.4 MB", "Burmese", "ဗမာစာ"),
     ("nep", "0.9 MB", "Nepali", "नेपाली"),
     ("nld", "5.7 MB", "Dutch; Flemish", "Nederlands; Vlaams"),
     ("nor", "3.4 MB", "Norwegian", "Norsk"),
     ("oci", "6.0 MB", "Occitan (post 1500)", "lenga d'òc"),
     ("ori", "1.4 MB", "Oriya", "ଓଡ଼ିଆ"),
     ("osd", "10 MB", "Orientation & Script", ""),
-    ("pan", "0.4 MB", "Panjabi; Punjabi", "ਪੰਜਾਬੀ; پنجابی\u200e"),  # noqa: RUF001
+    ("pan", "0.4 MB", "Panjabi; Punjabi", "ਪੰਜਾਬੀ; پنجابی\u200e"),
     ("pol", "4.5 MB", "Polish", "język polski"),
     ("por", "1.8 MB", "Portuguese", "português"),
     ("pus", "1.6 MB", "Pushto; Pashto", "پښتو"),
     ("que", "4.7 MB", "Quechua", "Runa Simi; Kichwa"),
     ("ron", "2.2 MB", "Romanian; Moldavian", "limba română"),
-    ("rus", "3.6 MB", "Russian", "Русский"),  # noqa: RUF001
+    ("rus", "3.6 MB", "Russian", "Русский"),
     ("san", "11 MB", "Sanskrit; Saṁskṛta", "संस्कृतम्"),
-    ("sin", "1.6 MB", "Sinhala; Sinhalese", "සිංහල"),  # noqa: RUF001
+    ("sin", "1.6 MB", "Sinhala; Sinhalese", "සිංහල"),
     ("slk", "4.2 MB", "Slovak", "slovenský jazyk"),
     ("slk_frak", "0.8 MB", "Slovak (fraktur)", "slovenský jazyk"),
     ("slv", "2.8 MB", "Slovenian", "slovenski jezik"),
-    ("snd", "1.6 MB", "Sindhi", "सिन्धी; سنڌي، سندھی\u200e"),  # noqa: RUF001
+    ("snd", "1.6 MB", "Sindhi", "सिन्धी; سنڌي، سندھی\u200e"),
     ("spa", "2.1 MB", "Spanish; Castilian", "español"),
     ("spa_old", "2.7 MB", "Spanish; Castilian (old)", ""),
     ("sqi", "1.7 MB", "Albanian", "Shqip"),
-    ("srp", "2.0 MB", "Serbian", "српски језик"),  # noqa: RUF001
-    ("srp_latn", "3.1 MB", "Serbian (latin)", "српски језик"),  # noqa: RUF001
+    ("srp", "2.0 MB", "Serbian", "српски језик"),
+    ("srp_latn", "3.1 MB", "Serbian (latin)", "српски језик"),
     ("sun", "1.3 MB", "Sundanese", "Basa Sunda"),
     ("swa", "2.0 MB", "Swahili", "Kiswahili"),
     ("swe", "3.9 MB", "Swedish", "svenska"),
     ("syr", "2.1 MB", "Syriac", "ܠܫܢܐ ܣܘܪܝܝܐ"),
     ("tam", "3.0 MB", "Tamil", "தமிழ்"),
-    ("tat", "1.0 MB", "Tatar", "татар теле"),  # noqa: RUF001
+    ("tat", "1.0 MB", "Tatar", "татар теле"),
     ("tel", "2.6 MB", "Telugu", "తెలుగు"),
-    ("tgk", "2.4 MB", "Tajik", "тоҷикӣ; toçikī; تاجیکی\u200e"),  # noqa: RUF001
+    ("tgk", "2.4 MB", "Tajik", "тоҷикӣ; toçikī; تاجیکی\u200e"),
     ("tgl", "7.3 MB", "Tagalog", "Wikang Tagalog"),
     ("tha", "1.0 MB", "Thai", "ไทย"),
     ("tir", "0.3 MB", "Tigrinya", "ትግርኛ"),
     ("ton", "0.9 MB", "Tonga", "faka Tonga"),
     ("tur", "4.3 MB", "Turkish", "Türkçe"),
-    ("uig", "2.6 MB", "Uighur", "ئۇيغۇرچە\u200e"),  # noqa: RUF001
-    ("ukr", "3.6 MB", "Ukrainian", "Українська"),  # noqa: RUF001
-    ("urd", "1.3 MB", "Urdu", "اردو"),  # noqa: RUF001
+    ("uig", "2.6 MB", "Uighur", "ئۇيغۇرچە\u200e"),
+    ("ukr", "3.6 MB", "Ukrainian", "Українська"),
+    ("urd", "1.3 MB", "Urdu", "اردو"),
     ("uzb", "6.1 MB", "Uzbek", "أۇزبېك\u200e"),
-    ("uzb_cyrl", "1.4 MB", "Uzbek (cyrillic)", "Ўзбек"),  # noqa: RUF001
+    ("uzb_cyrl", "1.4 MB", "Uzbek (cyrillic)", "Ўзбек"),
     ("vie", "0.5 MB", "Vietnamese", "Tiếng Việt"),
-    ("yid", "0.5 MB", "Yiddish", "ייִדיש"),  # noqa: RUF001
+    ("yid", "0.5 MB", "Yiddish", "ייִדיש"),
     ("yor", "0.9 MB", "Yoruba", "Yorùbá"),
 )
```

### Comparing `normcap-0.4.2/normcap/gui/downloader.py` & `normcap-0.4.3/normcap/gui/downloader.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/gui/language_manager.py` & `normcap-0.4.3/normcap/gui/language_manager.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/gui/loading_indicator.py` & `normcap-0.4.3/normcap/gui/loading_indicator.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/gui/menu_button.py` & `normcap-0.4.3/normcap/gui/menu_button.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/gui/models.py` & `normcap-0.4.3/normcap/gui/models.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/gui/notifier.py` & `normcap-0.4.3/normcap/gui/notifier.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/gui/resources.py` & `normcap-0.4.3/normcap/gui/resources.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/gui/settings.py` & `normcap-0.4.3/normcap/gui/settings.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/gui/system_info.py` & `normcap-0.4.3/normcap/gui/system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/gui/tray.py` & `normcap-0.4.3/normcap/gui/tray.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,22 +84,25 @@
             CaptureMode.PARSE
             if self.settings.value("mode") == "parse"
             else CaptureMode.RAW
         )
 
         self.screens: list[Screen] = system_info.screens()
 
-        self._ensure_screenshot_permission()
-        self._set_signals()
-        self._update_screenshots(delayed=False)
         self.setContextMenu(QtWidgets.QMenu())
         self._populate_context_menu_entries()
         self.contextMenu().aboutToShow.connect(self._populate_context_menu_entries)
+
+        self._ensure_screenshot_permission()
+        self._set_signals()
         QtCore.QTimer.singleShot(100, self._delayed_init)
 
+        if not args.get("background_mode", False):
+            self._update_screenshots(delayed=False)
+
     @QtCore.Slot()
     def _color_tray_icon(self) -> None:
         if sizes := self.icon().availableSizes():
             pixmap = self.icon().pixmap(sizes[-1])
             mask = pixmap.createMaskFromColor(
                 QtGui.QColor("transparent"), QtCore.Qt.MaskMode.MaskInColor
             )
@@ -306,14 +309,19 @@
                 self._exit_application, reason="notification sent delaying exit"
             )
             QtCore.QTimer.singleShot(5000, delayed_exit)
         else:
             self._exit_application(reason)
 
     def _delayed_init(self) -> None:
+        """Setup things that can be done independent of the first capture.
+
+        By running this async of __init__(),  its runtime of ~30ms doesn't
+        contribute to the delay until the GUI becomes active for the user on startup.
+        """
         self.installed_languages = ocr.tesseract.get_languages(
             tesseract_cmd=system_info.get_tesseract_path(),
             tessdata_path=system_info.get_tessdata_path(),
         )
         self.com.on_languages_changed.emit(self.installed_languages)
         self._add_update_checker()
         self._add_notifier()
@@ -346,28 +354,24 @@
                 screengrab.macos_reset_screenshot_permission()
 
             # Trigger permission request to make the NormCap entry available in settings
             screengrab.macos_request_screenshot_permission()
 
             # Message box to explain what's happening and open the preferences
             app = "NormCap" if system_info.is_prebuild_package() else "Terminal"
-            button = QtWidgets.QMessageBox.critical(
+            QtWidgets.QMessageBox.critical(
                 None,
                 "Error!",
                 (
                     f"{app} is missing permissions for 'Screen Recording'.\n\n"
                     "Grant the permissions via 'Privacy & Security' settings "
                     "and restart NormCap.\n\nClick OK to exit."
                 ),
-                buttons=QtWidgets.QMessageBox.Open | QtWidgets.QMessageBox.Cancel,
+                buttons=QtWidgets.QMessageBox.Ok,
             )
-            if button == QtWidgets.QMessageBox.Open:
-                logger.debug("Open macOS privacy settings")
-                screengrab.macos_open_privacy_settings()
-
             self._exit_application("Screen Recording permissions missing on macOS")
 
     def _set_signals(self) -> None:
         """Set up signals to trigger program logic."""
         self.activated.connect(self._handle_tray_click)
         self.com.on_tray_menu_capture_clicked.connect(self._update_screenshots)
         self.com.on_screenshots_updated.connect(self._show_windows)
```

### Comparing `normcap-0.4.2/normcap/gui/update_check.py` & `normcap-0.4.3/normcap/gui/update_check.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/gui/utils.py` & `normcap-0.4.3/normcap/gui/utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/gui/window.py` & `normcap-0.4.3/normcap/gui/window.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/ocr/enhance.py` & `normcap-0.4.3/normcap/ocr/enhance.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/ocr/magics/base_magic.py` & `normcap-0.4.3/normcap/ocr/magics/base_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/ocr/magics/email_magic.py` & `normcap-0.4.3/normcap/ocr/magics/email_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/ocr/magics/magic.py` & `normcap-0.4.3/normcap/ocr/magics/magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/ocr/magics/multi_line_magic.py` & `normcap-0.4.3/normcap/ocr/magics/multi_line_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/ocr/magics/paragraph_magic.py` & `normcap-0.4.3/normcap/ocr/magics/paragraph_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/ocr/magics/single_line_magic.py` & `normcap-0.4.3/normcap/ocr/magics/single_line_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/ocr/magics/url_magic.py` & `normcap-0.4.3/normcap/ocr/magics/url_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/ocr/models.py` & `normcap-0.4.3/normcap/ocr/models.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/ocr/recognize.py` & `normcap-0.4.3/normcap/ocr/recognize.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/ocr/tesseract.py` & `normcap-0.4.3/normcap/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/icons/normcap.png` & `normcap-0.4.3/normcap/resources/icons/normcap.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/icons/normcap.svg` & `normcap-0.4.3/normcap/resources/icons/normcap.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/icons/notification.png` & `normcap-0.4.3/normcap/resources/icons/notification.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/icons/notification.svg` & `normcap-0.4.3/normcap/resources/icons/notification.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/icons/parse.png` & `normcap-0.4.3/normcap/resources/icons/parse.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/icons/parse.svg` & `normcap-0.4.3/normcap/resources/icons/parse.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/icons/raw.png` & `normcap-0.4.3/normcap/resources/icons/raw.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/icons/raw.svg` & `normcap-0.4.3/normcap/resources/icons/raw.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/icons/resources.qrc` & `normcap-0.4.3/normcap/resources/icons/resources.qrc`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/icons/settings.png` & `normcap-0.4.3/normcap/resources/icons/settings.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/icons/settings.svg` & `normcap-0.4.3/normcap/resources/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/icons/tray.png` & `normcap-0.4.3/normcap/resources/icons/tray.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/icons/tray.svg` & `normcap-0.4.3/normcap/resources/icons/tray.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/tessdata/LICENSE.txt` & `normcap-0.4.3/normcap/resources/tessdata/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/resources/tessdata/README.txt` & `normcap-0.4.3/normcap/resources/tessdata/README.txt`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/screengrab/__init__.py` & `normcap-0.4.3/normcap/screengrab/__init__.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/screengrab/dbus_portal.py` & `normcap-0.4.3/normcap/screengrab/dbus_portal.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,38 +29,40 @@
             "org.freedesktop.portal.Request",  # type: ignore
             connection,
             parent,
         )
 
 
 class OrgFreedesktopPortalScreenshot(QtCore.QObject):
-    on_response = QtCore.Signal(str)
+    on_response = QtCore.Signal(QtDBus.QDBusMessage)
+    on_result = QtCore.Signal(str)
     on_exception = QtCore.Signal(Exception)
 
     def __init__(
         self,
         parent: Optional[QtCore.QObject] = None,
         interactive: bool = False,
         timeout_sec: int = 15,
     ) -> None:
         super().__init__(parent)
         self.interactive = interactive
         self.timeout_timer = self._get_timeout_timer(timeout_sec)
+        self.on_response.connect(self.got_signal)
 
     def grab_full_desktop(self) -> None:
         bus = QtDBus.QDBusConnection.sessionBus()
 
         base = bus.baseService()[1:].replace(".", "_")
 
         random_str = "".join(random.choice("abcdefghi") for _ in range(8))  # noqa: S311
         token = f"normcap_{random_str}"
         object_path = f"/org/freedesktop/portal/desktop/request/{base}/{token}"
 
         request = OrgFreedesktopPortalRequestInterface(object_path, bus, self)
-        request.Response.connect(self.got_signal)
+        request.Response.connect(self.on_response)
 
         interface = QtDBus.QDBusInterface(
             "org.freedesktop.portal.Desktop",
             "/org/freedesktop/portal/desktop",
             "org.freedesktop.portal.Screenshot",
             bus,
             self,
@@ -113,15 +115,15 @@
         #     while not arg.atEnd():
         #         arg.beginMapEntry()
         #         key = arg.asVariant()
         #         value = arg.asVariant()
         #         arg.endMapEntry()
         #     arg.endMap()
         # arg.endArray()
-        self.on_response.emit(uri)
+        self.on_result.emit(uri)
 
 
 def _synchronized_capture(interactive: bool) -> list[QtGui.QImage]:
     loop = QtCore.QEventLoop()
     result = []
     exceptions = []
 
@@ -132,22 +134,22 @@
     def _exception_triggered(uri: Exception) -> None:
         exceptions.append(uri)
         loop.exit()
 
     portal = OrgFreedesktopPortalScreenshot(
         interactive=interactive, timeout_sec=TIMEOUT_SECONDS
     )
-    portal.on_response.connect(_signal_triggered)
+    portal.on_result.connect(_signal_triggered)
     portal.on_exception.connect(_exception_triggered)
 
     portal.timeout_timer.start()
     QtCore.QTimer.singleShot(0, portal.grab_full_desktop)
     loop.exec()
 
-    portal.on_response.disconnect(_signal_triggered)
+    portal.on_result.disconnect(_signal_triggered)
     portal.on_exception.disconnect(_exception_triggered)
 
     for error in exceptions:
         raise error
 
     uri = result[0]
     full_image = QtGui.QImage(urlparse(uri).path)
```

### Comparing `normcap-0.4.2/normcap/screengrab/dbus_shell.py` & `normcap-0.4.3/normcap/screengrab/dbus_shell.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/screengrab/utils.py` & `normcap-0.4.3/normcap/screengrab/utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.2/normcap/utils.py` & `normcap-0.4.3/normcap/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,19 @@
         help="Print NormCap version and exit",
     )
     parser.add_argument(
         "--cli-mode",
         action="store_true",
         help="Print text after detection to stdout and exits immediately",
     )
+    parser.add_argument(
+        "--background-mode",
+        action="store_true",
+        help="Start minimized to tray, without capturing",
+    )
     return parser
 
 
 def set_environ_for_wayland() -> None:
     # QT has 32 as default cursor size on wayland, while it should be 24
     if "XCURSOR_SIZE" not in os.environ:
         logger.debug("Set XCURSOR_SIZE=24")
```

### Comparing `normcap-0.4.2/pyproject.toml` & `normcap-0.4.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "normcap"
-version = "0.4.2"
+version = "0.4.3"
 description = "OCR-powered screen-capture tool to capture information instead of images."
 keywords = ["screenshot", "ocr", "capture", "clipboard"]
 license = "GPLv3"
 authors = ["dynobo <dynobo@mailbox.org>"]
 readme = "README.md"
 homepage = "https://dynobo.github.io/normcap/"
 repository = "https://github.com/dynobo/normcap"
@@ -41,29 +41,29 @@
 "Issues" = "https://github.com/dynobo/normcap/issues"
 
 [tool.poetry.scripts]
 normcap = "normcap.app:main"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-PySide6-Essentials = "6.4.2"
+PySide6-Essentials = "6.5.1"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.1.0"
 briefcase = "0.3.14"
-coverage = { extras = ["toml"], version = "^6.4.2" }
+coverage = { extras = ["toml"], version = ">=6.4.2" }
 coveralls = ">=3.3.1"
 mdformat-gfm = ">=0.3.5"
 mypy = ">=1.3.0"
 pre-commit = ">=3.0.2"
 pydeps = ">=1.11.0"
 pytest = ">=7.2.1"
 pytest-cov = ">=4.0.0"
 pytest-qt = ">=4.2.0"
-pytest-xvfb = "^2.0.0"
+pytest-xvfb = ">=3.0.0"
 rope = ">=1.7.0"
 ruff = ">=0.0.239"
 tbump = ">=6.9.0"
 toml = ">=0.10.2"
 types-toml = ">=0.10.8.1"
 typing-extensions = ">=4.4.0"
 pip-audit = ">=2.5.5"
@@ -156,28 +156,28 @@
 cluster = true
 max_cluster_size = 1
 no_show = true
 
 [tool.briefcase]
 project_name = "NormCap"
 bundle = "eu.dynobo"
-version = "0.4.2"
+version = "0.4.3"
 url = "https://github.com/dynobo/normcap"
 license = "GPLv3"
 author = 'dynobo'
 author_email = "dynobo@mailbox.org"
 
 [tool.briefcase.app.normcap]
 formal_name = "NormCap"
 description = "OCR-powered screen-capture tool to capture information instead of images"
 sources = ["normcap"]
 icon = "bundle/imgs/normcap"
 installer_icon = "bundle/imgs/normcap_install"
 installer_background = "bundle/imgs/normcap_install_bg"
-requires = ["PySide6-Essentials==6.4.2"]
+requires = ["PySide6-Essentials==6.5.1"]
 cleanup_paths = [
   # Globs
   "**/[pP]y[sS]ide6/*[qQ]t*[oO]pen[gG][lL]*",
   "**/*.debug",
   "**/*[lL]abs*",
   "**/*[qQ]t[xX]ml*",
   "**/*[qQ]t*[dD]esigner*",
@@ -196,14 +196,15 @@
   "**/*QtQml*",
   "**/bin/pyside6-*",
   "**/PySide6/[aA]ssistant*",
   "**/PySide6/[dD]esigner*",
   "**/PySide6/[lL]inguist*",
   # Folders
   "**/__pycache__",
+  "**/examples",
   "**/libexec",
   "**/plugins/designer",
   "**/plugins/printsupport",
   "**/plugins/qmltooling",
   "**/plugins/sqldrivers",
   "**/Qt/qml/QtQml",
   "**/Qt/translations",
@@ -248,15 +249,15 @@
 template_branch = "main"
 
 [tool.briefcase.app.normcap.windows]
 
 [tool.tbump]
 
 [tool.tbump.version]
-current = "0.4.2"
+current = "0.4.3"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   ((?P<extra>.+))?
@@ -282,14 +283,10 @@
 src = "README.md"
 search = 'NormCap-{current_version}-'
 
 [[tool.tbump.file]]
 src = "README.md"
 search = 'download/v{current_version}/'
 
-[[tool.tbump.file]]
-src = "bundle/normcap.wxs"
-search = 'ProductVersion = "{current_version}"'
-
 [[tool.tbump.before_commit]]
 name = "check changelog"
 cmd = "grep -q {new_version} CHANGELOG"
```

### Comparing `normcap-0.4.2/setup.py` & `normcap-0.4.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,235 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: normcap
+Version: 0.4.3
+Summary: OCR-powered screen-capture tool to capture information instead of images.
+Home-page: https://dynobo.github.io/normcap/
+License: GPLv3
+Keywords: screenshot,ocr,capture,clipboard
+Author: dynobo
+Author-email: dynobo@mailbox.org
+Requires-Python: >=3.9,<3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Multimedia :: Graphics :: Capture :: Screen Capture
+Classifier: Topic :: Utilities
+Requires-Dist: PySide6-Essentials (==6.5.1)
+Project-URL: FAQs, https://dynobo.github.io/normcap/#faqs
+Project-URL: Issues, https://github.com/dynobo/normcap/issues
+Project-URL: Repository, https://github.com/dynobo/normcap
+Description-Content-Type: text/markdown
 
-packages = \
-['normcap',
- 'normcap.clipboard',
- 'normcap.gui',
- 'normcap.ocr',
- 'normcap.ocr.magics',
- 'normcap.resources',
- 'normcap.screengrab']
-
-package_data = \
-{'': ['*'], 'normcap.resources': ['icons/*', 'tessdata/*']}
-
-install_requires = \
-['PySide6-Essentials==6.4.2']
-
-entry_points = \
-{'console_scripts': ['normcap = normcap.app:main']}
-
-setup_kwargs = {
-    'name': 'normcap',
-    'version': '0.4.2',
-    'description': 'OCR-powered screen-capture tool to capture information instead of images.',
-    'long_description': '<!-- markdownlint-disable MD013 MD026 MD033 -->\n\n# NormCap\n\n**_OCR powered screen-capture tool to capture information instead of images. For Linux,\nmacOS and Windows._**\n\n[![Build](https://img.shields.io/github/actions/workflow/status/dynobo/normcap/python.yaml?branch=main)](https://github.com/dynobo/normcap/releases)\n[![Coverage Status](https://img.shields.io/coverallsCoverage/github/dynobo/normcap?label=Test%20coverage&branch=main)](https://coveralls.io/github/dynobo/normcap)\n[![CodeQL](https://img.shields.io/github/actions/workflow/status/dynobo/normcap/codeql-analysis.yml?branch=main&label=CodeQL)](https://github.com/dynobo/normcap/actions/workflows/codeql-analysis.yml)\n\n[![GitHub](https://img.shields.io/github/downloads/dynobo/normcap/total?label=Github%20downloads&color=blue)](https://github.com/dynobo/normcap/releases)\n[![PyPi](https://img.shields.io/pypi/dm/normcap?label=PyPi%20downloads&color=blue)](https://pypi.org/project/normcap)\n[![Flathub](https://img.shields.io/flathub/downloads/com.github.dynobo.normcap?label=Flathub%20downloads&color=blue)](https://flathub.org/apps/details/com.github.dynobo.normcap)\n[![AUR](https://img.shields.io/aur/votes/normcap?label=AUR%20votes&color=blue)](https://aur.archlinux.org/packages/normcap)\n\n<a href="https://www.buymeacoffee.com/dynobo" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 40px !important;" ></a>\n\n**Links:** [Source Code](https://github.com/dynobo/normcap) |\n[Documentation](https://dynobo.github.io/normcap/) |\n[FAQs](https://dynobo.github.io/normcap/#faqs) |\n[Releases](https://github.com/dynobo/normcap/releases) |\n[Changelog](https://github.com/dynobo/normcap/blob/main/CHANGELOG)\n\n[![Screencast](https://user-images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/assets/normcap.gif)\n\n## Quickstart\n\nInstall a prebuilt release:\n\n- **Windows**:\n  [NormCap-0.4.2-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64-Windows.msi)\n- **Linux**:\n  [NormCap-0.4.2-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64.AppImage)\n- **macOS** (x86) ¹:\n  [NormCap-0.4.2-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64-macOS.dmg)\n- **macOS** (M1) ¹·²:\n  [NormCap-0.4.2-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-arm64-macOS.dmg)\n  \\\n  <sub>1: On macOS, allow the unsigned application on first start: "System\n  Preferences" → "Security & Privacy" → "General" → "Open anyway". You might also need\n  to allow NormCap to take screenshots.\n  [#135](https://github.com/dynobo/normcap/issues/135)<br> 2: Might be available a bit\n  delayed, as it is currently build manually. (Thx,\n  [@Takrin](https://github.com/Takrin)!)</sub>\n\nInstall from repositories:\n\n- **Windows**: Install from\n  [Microsoft Store](https://apps.microsoft.com/store/detail/normcap/XPDLJNB4B6C2ZR).\n- **Arch / Manjaro**: Install the\n  [`normcap`](https://aur.archlinux.org/packages/normcap) package from AUR.\n- **FlatPak (Linux)**: Install\n  [com.github.dynobo.normcap](https://flathub.org/apps/details/com.github.dynobo.normcap)\n  from FlatHub.\n\nIf you experience issues please look at the\n[FAQs](https://dynobo.github.io/normcap/#faqs) or\n[open an issue](https://github.com/dynobo/normcap/issues).\n\n## Python package\n\nAs an _alternative_ to a prebuilt package you can install the\n[NormCap Python package](https://pypi.org/project/normcap/) for **Python >=3.9**:\n\n#### On Linux\n\n```sh\n# Install dependencies (Ubuntu/Debian)\nsudo apt install build-essential tesseract-ocr tesseract-ocr-eng libtesseract-dev libleptonica-dev wl-clipboard\n\n## Install dependencies (Arch)\nsudo pacman -S tesseract tesseract-data-eng wl-clipboard\n\n## Install dependencies (Fedora)\nsudo dnf install tesseract wl-clipboard\n\n## Install dependencies (openSUSE)\nsudo zypper install python3-devel tesseract-ocr tesseract-ocr-devel wl-clipboard\n\n# Install normcap\npip install normcap\n\n# Run\n./normcap\n```\n\n#### On macOS\n\n```sh\n# Install dependencies\nbrew install tesseract tesseract-lang\n\n# Install normcap\npip install normcap\n\n# Run\n./normcap\n```\n\n#### On Windows\n\n1\\. Install `Tesseract 5` by using the\n[installer provided by UB Mannheim](https://github.com/UB-Mannheim/tesseract/wiki).\n\n2\\. Adjust environment variables:\n\n- Create an environment variable `TESSDATA_PREFIX` and set it to Tesseract\'s data\n  folder, e.g.:\n\n  ```cmd\n  setx TESSDATA_PREFIX "C:\\Program Files\\Tesseract-OCR\\tessdata"\n  ```\n\n- Append Tesseract\'s location to the environment variable `Path`, e.g.:\n\n  ```cmd\n  setx Path "%Path%;C:\\Program Files\\Tesseract-OCR"\n  ```\n\n- Make sure to close and reopen your current terminal window to apply the new variables.\n  Test it by running:\n\n  ```cmd\n  tesseract --list-langs\n  ```\n\n3\\. Install and run NormCap:\n\n```bash\n# Install normcap\npip install normcap\n\n# Run\nnormcap\n```\n\n## Why "NormCap"?\n\nSee [XKCD](https://xkcd.com):\n\n[![Comic](https://imgs.xkcd.com/comics/norm_normal_file_format.png)](https://xkcd.com/2116/)\n\n## Development\n\nPrerequisites for setting up a development environment are: **Python >=3.9**,\n**Poetry>=1.3.2** and **Tesseract** (incl. **language data**).\n\n```sh\n# Clone repository\ngit clone https://github.com/dynobo/normcap.git\n\n# Change into project directory\ncd normcap\n\n# Create virtual env and install dependencies\npoetry install\n\n# Register pre-commit hook\npoetry run pre-commit install\n\n# Run NormCap in virtual env\npoetry run python -m normcap\n```\n\n## Credits\n\nThis project uses the following non-standard libraries:\n\n- [pyside6](https://pypi.org/project/PySide6/) _- bindings for Qt UI Framework_\n\nAnd it depends on external software:\n\n- [tesseract](https://github.com/tesseract-ocr/tesseract) - _OCR engine_\n- [wl-clipboard](https://github.com/bugaevc/wl-clipboard) - _Wayland clipboard\n  utilities_\n\nPackaging is done with:\n\n- [briefcase](https://pypi.org/project/briefcase/) _- converting Python projects into_\n  _standalone apps_\n\nThanks to the maintainers of those nice tools!\n\n## Similar open source tools\n\nIf NormCap doesn\'t fit your needs, try those alternatives (no particular order):\n\n- [TextSnatcher](https://github.com/RajSolai/TextSnatcher) (Linux)\n- [GreenShot](https://getgreenshot.org/) (Linux, macOS)\n- [TextShot](https://github.com/ianzhao05/textshot) (Windows)\n- [gImageReader](https://github.com/manisandro/gImageReader) (Linux, Windows)\n- [Capture2Text](https://sourceforge.net/projects/capture2text) (Windows)\n- [Frog](https://github.com/TenderOwl/Frog) (Linux)\n- [Textinator](https://github.com/RhetTbull/textinator) (macOS)\n- [Text-Grab](https://github.com/TheJoeFin/Text-Grab) (Windows)\n- [dpScreenOCR](https://danpla.github.io/dpscreenocr/) (Linux, Windows)\n\n## Certification\n\n![WOMM](https://raw.githubusercontent.com/dynobo/lmdiag/master/badge.png)\n',
-    'author': 'dynobo',
-    'author_email': 'dynobo@mailbox.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://dynobo.github.io/normcap/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<3.12',
-}
+<!-- markdownlint-disable MD013 MD026 MD033 -->
 
+# NormCap
+
+**_OCR powered screen-capture tool to capture information instead of images. For Linux,
+macOS and Windows._**
+
+[![Build](https://img.shields.io/github/actions/workflow/status/dynobo/normcap/python.yaml?branch=main)](https://github.com/dynobo/normcap/releases)
+[![Coverage Status](https://img.shields.io/coverallsCoverage/github/dynobo/normcap?label=Test%20coverage&branch=main)](https://coveralls.io/github/dynobo/normcap)
+[![CodeQL](https://img.shields.io/github/actions/workflow/status/dynobo/normcap/codeql-analysis.yml?branch=main&label=CodeQL)](https://github.com/dynobo/normcap/actions/workflows/codeql-analysis.yml)
+
+[![GitHub](https://img.shields.io/github/downloads/dynobo/normcap/total?label=Github%20downloads&color=blue)](https://github.com/dynobo/normcap/releases)
+[![PyPi](https://img.shields.io/pypi/dm/normcap?label=PyPi%20downloads&color=blue)](https://pypi.org/project/normcap)
+[![Flathub](https://img.shields.io/flathub/downloads/com.github.dynobo.normcap?label=Flathub%20downloads&color=blue)](https://flathub.org/apps/details/com.github.dynobo.normcap)
+[![AUR](https://img.shields.io/aur/votes/normcap?label=AUR%20votes&color=blue)](https://aur.archlinux.org/packages/normcap)
+
+<a href="https://www.buymeacoffee.com/dynobo" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 40px !important;" ></a>
+
+**Links:** [Source Code](https://github.com/dynobo/normcap) |
+[Documentation](https://dynobo.github.io/normcap/) |
+[FAQs](https://dynobo.github.io/normcap/#faqs) |
+[Releases](https://github.com/dynobo/normcap/releases) |
+[Changelog](https://github.com/dynobo/normcap/blob/main/CHANGELOG)
+
+[![Screencast](https://user-images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/assets/normcap.gif)
+
+## Quickstart
+
+Install a prebuilt release:
+
+- **Windows**:
+  [NormCap-0.4.3-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-x86_64-Windows.msi)
+- **Linux**:
+  [NormCap-0.4.3-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-x86_64.AppImage)
+- **macOS** (x86) ¹:
+  [NormCap-0.4.3-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-x86_64-macOS.dmg)
+- **macOS** (M1) ¹·²:
+  [NormCap-0.4.3-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-0.4.3-arm64-macOS.dmg)
+  \
+  <sub>1: On macOS, allow the unsigned application on first start: "System
+  Preferences" → "Security & Privacy" → "General" → "Open anyway". You might also need
+  to allow NormCap to take screenshots.
+  [#135](https://github.com/dynobo/normcap/issues/135)<br> 2: Might be available a bit
+  delayed, as it is currently build manually. (Thx,
+  [@Takrin](https://github.com/Takrin)!)</sub>
+
+Install from repositories:
+
+- **Windows**: Install from
+  [Microsoft Store](https://apps.microsoft.com/store/detail/normcap/XPDLJNB4B6C2ZR).
+- **Arch / Manjaro**: Install the
+  [`normcap`](https://aur.archlinux.org/packages/normcap) package from AUR.
+- **FlatPak (Linux)**: Install
+  [com.github.dynobo.normcap](https://flathub.org/apps/details/com.github.dynobo.normcap)
+  from FlatHub.
+
+If you experience issues please look at the
+[FAQs](https://dynobo.github.io/normcap/#faqs) or
+[open an issue](https://github.com/dynobo/normcap/issues).
+
+## Python package
+
+As an _alternative_ to a prebuilt package you can install the
+[NormCap Python package](https://pypi.org/project/normcap/) for **Python >=3.9**:
+
+#### On Linux
+
+```sh
+# Install dependencies (Ubuntu/Debian)
+sudo apt install build-essential tesseract-ocr tesseract-ocr-eng libtesseract-dev libleptonica-dev wl-clipboard
+
+## Install dependencies (Arch)
+sudo pacman -S tesseract tesseract-data-eng wl-clipboard
+
+## Install dependencies (Fedora)
+sudo dnf install tesseract wl-clipboard
+
+## Install dependencies (openSUSE)
+sudo zypper install python3-devel tesseract-ocr tesseract-ocr-devel wl-clipboard
+
+# Install normcap
+pip install normcap
+
+# Run
+./normcap
+```
+
+#### On macOS
+
+```sh
+# Install dependencies
+brew install tesseract tesseract-lang
+
+# Install normcap
+pip install normcap
+
+# Run
+./normcap
+```
+
+#### On Windows
+
+1\. Install `Tesseract 5` by using the
+[installer provided by UB Mannheim](https://github.com/UB-Mannheim/tesseract/wiki).
+
+2\. Adjust environment variables:
+
+- Create an environment variable `TESSDATA_PREFIX` and set it to Tesseract's data
+  folder, e.g.:
+
+  ```cmd
+  setx TESSDATA_PREFIX "C:\Program Files\Tesseract-OCR\tessdata"
+  ```
+
+- Append Tesseract's location to the environment variable `Path`, e.g.:
+
+  ```cmd
+  setx Path "%Path%;C:\Program Files\Tesseract-OCR"
+  ```
+
+- Make sure to close and reopen your current terminal window to apply the new variables.
+  Test it by running:
+
+  ```cmd
+  tesseract --list-langs
+  ```
+
+3\. Install and run NormCap:
+
+```bash
+# Install normcap
+pip install normcap
+
+# Run
+normcap
+```
+
+## Why "NormCap"?
+
+See [XKCD](https://xkcd.com):
+
+[![Comic](https://imgs.xkcd.com/comics/norm_normal_file_format.png)](https://xkcd.com/2116/)
+
+## Development
+
+Prerequisites for setting up a development environment are: **Python >=3.9**,
+**Poetry>=1.3.2** and **Tesseract** (incl. **language data**).
+
+```sh
+# Clone repository
+git clone https://github.com/dynobo/normcap.git
+
+# Change into project directory
+cd normcap
+
+# Create virtual env and install dependencies
+poetry install
+
+# Register pre-commit hook
+poetry run pre-commit install
+
+# Run NormCap in virtual env
+poetry run python -m normcap
+```
+
+## Credits
+
+This project uses the following non-standard libraries:
+
+- [pyside6](https://pypi.org/project/PySide6/) _- bindings for Qt UI Framework_
+
+And it depends on external software:
+
+- [tesseract](https://github.com/tesseract-ocr/tesseract) - _OCR engine_
+- [wl-clipboard](https://github.com/bugaevc/wl-clipboard) - _Wayland clipboard
+  utilities_
+
+Packaging is done with:
+
+- [briefcase](https://pypi.org/project/briefcase/) _- converting Python projects into_
+  _standalone apps_
+
+Thanks to the maintainers of those nice tools!
+
+## Similar open source tools
+
+If NormCap doesn't fit your needs, try those alternatives (no particular order):
+
+- [TextSnatcher](https://github.com/RajSolai/TextSnatcher) (Linux)
+- [GreenShot](https://getgreenshot.org/) (Linux, macOS)
+- [TextShot](https://github.com/ianzhao05/textshot) (Windows)
+- [gImageReader](https://github.com/manisandro/gImageReader) (Linux, Windows)
+- [Capture2Text](https://sourceforge.net/projects/capture2text) (Windows)
+- [Frog](https://github.com/TenderOwl/Frog) (Linux)
+- [Textinator](https://github.com/RhetTbull/textinator) (macOS)
+- [Text-Grab](https://github.com/TheJoeFin/Text-Grab) (Windows)
+- [dpScreenOCR](https://danpla.github.io/dpscreenocr/) (Linux, Windows)
+
+## Certification
+
+![WOMM](https://raw.githubusercontent.com/dynobo/lmdiag/master/badge.png)
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,107 +1,109 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['normcap',
-'normcap.clipboard', 'normcap.gui', 'normcap.ocr', 'normcap.ocr.magics',
-'normcap.resources', 'normcap.screengrab'] package_data = \ {'': ['*'],
-'normcap.resources': ['icons/*', 'tessdata/*']} install_requires = \ ['PySide6-
-Essentials==6.4.2'] entry_points = \ {'console_scripts': ['normcap =
-normcap.app:main']} setup_kwargs = { 'name': 'normcap', 'version': '0.4.2',
-'description': 'OCR-powered screen-capture tool to capture information instead
-of images.', 'long_description': '\n\n# NormCap\n\n**_OCR powered screen-
-capture tool to capture information instead of images. For Linux,\nmacOS and
-Windows._**\n\n[![Build](https://img.shields.io/github/actions/workflow/status/
-dynobo/normcap/python.yaml?branch=main)](https://github.com/dynobo/normcap/
-releases)\n[![Coverage Status](https://img.shields.io/coverallsCoverage/github/
-dynobo/normcap?label=Test%20coverage&branch=main)](https://coveralls.io/github/
-dynobo/normcap)\n[![CodeQL](https://img.shields.io/github/actions/workflow/
-status/dynobo/normcap/codeql-analysis.yml?branch=main&label=CodeQL)](https://
-github.com/dynobo/normcap/actions/workflows/codeql-analysis.yml)\n\n[![GitHub]
-(https://img.shields.io/github/downloads/dynobo/normcap/
+Metadata-Version: 2.1 Name: normcap Version: 0.4.3 Summary: OCR-powered screen-
+capture tool to capture information instead of images. Home-page: https://
+dynobo.github.io/normcap/ License: GPLv3 Keywords:
+screenshot,ocr,capture,clipboard Author: dynobo Author-email:
+dynobo@mailbox.org Requires-Python: >=3.9,<3.12 Classifier: Development Status
+:: 4 - Beta Classifier: Intended Audience :: End Users/Desktop Classifier:
+License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
+License :: Other/Proprietary License Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
+System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
+Multimedia :: Graphics :: Capture :: Screen Capture Classifier: Topic ::
+Utilities Requires-Dist: PySide6-Essentials (==6.5.1) Project-URL: FAQs, https:
+//dynobo.github.io/normcap/#faqs Project-URL: Issues, https://github.com/
+dynobo/normcap/issues Project-URL: Repository, https://github.com/dynobo/
+normcap Description-Content-Type: text/markdown  # NormCap **_OCR powered
+screen-capture tool to capture information instead of images. For Linux, macOS
+and Windows._** [![Build](https://img.shields.io/github/actions/workflow/
+status/dynobo/normcap/python.yaml?branch=main)](https://github.com/dynobo/
+normcap/releases) [![Coverage Status](https://img.shields.io/coverallsCoverage/
+github/dynobo/normcap?label=Test%20coverage&branch=main)](https://coveralls.io/
+github/dynobo/normcap) [![CodeQL](https://img.shields.io/github/actions/
+workflow/status/dynobo/normcap/codeql-analysis.yml?branch=main&label=CodeQL)]
+(https://github.com/dynobo/normcap/actions/workflows/codeql-analysis.yml) [!
+[GitHub](https://img.shields.io/github/downloads/dynobo/normcap/
 total?label=Github%20downloads&color=blue)](https://github.com/dynobo/normcap/
-releases)\n[![PyPi](https://img.shields.io/pypi/dm/
-normcap?label=PyPi%20downloads&color=blue)](https://pypi.org/project/normcap)\n
+releases) [![PyPi](https://img.shields.io/pypi/dm/
+normcap?label=PyPi%20downloads&color=blue)](https://pypi.org/project/normcap)
 [![Flathub](https://img.shields.io/flathub/downloads/
 com.github.dynobo.normcap?label=Flathub%20downloads&color=blue)](https://
-flathub.org/apps/details/com.github.dynobo.normcap)\n[![AUR](https://
+flathub.org/apps/details/com.github.dynobo.normcap) [![AUR](https://
 img.shields.io/aur/votes/normcap?label=AUR%20votes&color=blue)](https://
-aur.archlinux.org/packages/normcap)\n\n[Buy_Me_A_Coffee]\n\n**Links:** [Source
-Code](https://github.com/dynobo/normcap) |\n[Documentation](https://
-dynobo.github.io/normcap/) |\n[FAQs](https://dynobo.github.io/normcap/#faqs)
-|\n[Releases](https://github.com/dynobo/normcap/releases) |\n[Changelog](https:
-//github.com/dynobo/normcap/blob/main/CHANGELOG)\n\n[![Screencast](https://
-user-images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-
+aur.archlinux.org/packages/normcap) [Buy_Me_A_Coffee] **Links:** [Source Code]
+(https://github.com/dynobo/normcap) | [Documentation](https://dynobo.github.io/
+normcap/) | [FAQs](https://dynobo.github.io/normcap/#faqs) | [Releases](https:/
+/github.com/dynobo/normcap/releases) | [Changelog](https://github.com/dynobo/
+normcap/blob/main/CHANGELOG) [![Screencast](https://user-
+images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-
 cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/
-assets/normcap.gif)\n\n## Quickstart\n\nInstall a prebuilt release:\n\n-
-**Windows**:\n [NormCap-0.4.2-x86_64-Windows.msi](https://github.com/dynobo/
-normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64-Windows.msi)\n-
-**Linux**:\n [NormCap-0.4.2-x86_64.AppImage](https://github.com/dynobo/normcap/
-releases/download/v0.4.2/NormCap-0.4.2-x86_64.AppImage)\n- **macOS** (x86) Â¹:
-\n [NormCap-0.4.2-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/
-download/v0.4.2/NormCap-0.4.2-x86_64-macOS.dmg)\n- **macOS** (M1) Â¹Â·Â²:\n
-[NormCap-0.4.2-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/
-download/v0.4.2/NormCap-0.4.2-arm64-macOS.dmg)\n \\\n 1: On macOS, allow the
-unsigned application on first start: "System\n Preferences" â "Security &
-Privacy" â "General" â "Open anyway". You might also need\n to allow
-NormCap to take screenshots.\n [#135](https://github.com/dynobo/normcap/issues/
-135)
-2: Might be available a bit\n delayed, as it is currently build manually.
-(Thx,\n [@Takrin](https://github.com/Takrin)!)\n\nInstall from repositories:
-\n\n- **Windows**: Install from\n [Microsoft Store](https://apps.microsoft.com/
-store/detail/normcap/XPDLJNB4B6C2ZR).\n- **Arch / Manjaro**: Install the\n
-[`normcap`](https://aur.archlinux.org/packages/normcap) package from AUR.\n-
-**FlatPak (Linux)**: Install\n [com.github.dynobo.normcap](https://flathub.org/
-apps/details/com.github.dynobo.normcap)\n from FlatHub.\n\nIf you experience
-issues please look at the\n[FAQs](https://dynobo.github.io/normcap/#faqs) or\n
-[open an issue](https://github.com/dynobo/normcap/issues).\n\n## Python
-package\n\nAs an _alternative_ to a prebuilt package you can install the\n
-[NormCap Python package](https://pypi.org/project/normcap/) for **Python
->=3.9**:\n\n#### On Linux\n\n```sh\n# Install dependencies (Ubuntu/
-Debian)\nsudo apt install build-essential tesseract-ocr tesseract-ocr-eng
-libtesseract-dev libleptonica-dev wl-clipboard\n\n## Install dependencies
-(Arch)\nsudo pacman -S tesseract tesseract-data-eng wl-clipboard\n\n## Install
-dependencies (Fedora)\nsudo dnf install tesseract wl-clipboard\n\n## Install
-dependencies (openSUSE)\nsudo zypper install python3-devel tesseract-ocr
-tesseract-ocr-devel wl-clipboard\n\n# Install normcap\npip install normcap\n\n#
-Run\n./normcap\n```\n\n#### On macOS\n\n```sh\n# Install dependencies\nbrew
-install tesseract tesseract-lang\n\n# Install normcap\npip install normcap\n\n#
-Run\n./normcap\n```\n\n#### On Windows\n\n1\\. Install `Tesseract 5` by using
-the\n[installer provided by UB Mannheim](https://github.com/UB-Mannheim/
-tesseract/wiki).\n\n2\\. Adjust environment variables:\n\n- Create an
-environment variable `TESSDATA_PREFIX` and set it to Tesseract\'s data\n
-folder, e.g.:\n\n ```cmd\n setx TESSDATA_PREFIX "C:\\Program Files\\Tesseract-
-OCR\\tessdata"\n ```\n\n- Append Tesseract\'s location to the environment
-variable `Path`, e.g.:\n\n ```cmd\n setx Path "%Path%;C:\\Program
-Files\\Tesseract-OCR"\n ```\n\n- Make sure to close and reopen your current
-terminal window to apply the new variables.\n Test it by running:\n\n ```cmd\n
-tesseract --list-langs\n ```\n\n3\\. Install and run NormCap:\n\n```bash\n#
-Install normcap\npip install normcap\n\n# Run\nnormcap\n```\n\n## Why
-"NormCap"?\n\nSee [XKCD](https://xkcd.com):\n\n[![Comic](https://imgs.xkcd.com/
-comics/norm_normal_file_format.png)](https://xkcd.com/2116/)\n\n##
-Development\n\nPrerequisites for setting up a development environment are:
-**Python >=3.9**,\n**Poetry>=1.3.2** and **Tesseract** (incl. **language
-data**).\n\n```sh\n# Clone repository\ngit clone https://github.com/dynobo/
-normcap.git\n\n# Change into project directory\ncd normcap\n\n# Create virtual
-env and install dependencies\npoetry install\n\n# Register pre-commit
-hook\npoetry run pre-commit install\n\n# Run NormCap in virtual env\npoetry run
-python -m normcap\n```\n\n## Credits\n\nThis project uses the following non-
-standard libraries:\n\n- [pyside6](https://pypi.org/project/PySide6/) _-
-bindings for Qt UI Framework_\n\nAnd it depends on external software:\n\n-
-[tesseract](https://github.com/tesseract-ocr/tesseract) - _OCR engine_\n- [wl-
-clipboard](https://github.com/bugaevc/wl-clipboard) - _Wayland clipboard\n
-utilities_\n\nPackaging is done with:\n\n- [briefcase](https://pypi.org/
-project/briefcase/) _- converting Python projects into_\n _standalone
-apps_\n\nThanks to the maintainers of those nice tools!\n\n## Similar open
-source tools\n\nIf NormCap doesn\'t fit your needs, try those alternatives (no
-particular order):\n\n- [TextSnatcher](https://github.com/RajSolai/
-TextSnatcher) (Linux)\n- [GreenShot](https://getgreenshot.org/) (Linux,
-macOS)\n- [TextShot](https://github.com/ianzhao05/textshot) (Windows)\n-
-[gImageReader](https://github.com/manisandro/gImageReader) (Linux, Windows)\n-
-[Capture2Text](https://sourceforge.net/projects/capture2text) (Windows)\n-
-[Frog](https://github.com/TenderOwl/Frog) (Linux)\n- [Textinator](https://
-github.com/RhetTbull/textinator) (macOS)\n- [Text-Grab](https://github.com/
-TheJoeFin/Text-Grab) (Windows)\n- [dpScreenOCR](https://danpla.github.io/
-dpscreenocr/) (Linux, Windows)\n\n## Certification\n\n![WOMM](https://
-raw.githubusercontent.com/dynobo/lmdiag/master/badge.png)\n', 'author':
-'dynobo', 'author_email': 'dynobo@mailbox.org', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://dynobo.github.io/normcap/',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'entry_points': entry_points, 'python_requires':
-'>=3.9,<3.12', } setup(**setup_kwargs)
+assets/normcap.gif) ## Quickstart Install a prebuilt release: - **Windows**:
+[NormCap-0.4.3-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/
+download/v0.4.3/NormCap-0.4.3-x86_64-Windows.msi) - **Linux**: [NormCap-0.4.3-
+x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.3/
+NormCap-0.4.3-x86_64.AppImage) - **macOS** (x86) Â¹: [NormCap-0.4.3-x86_64-
+macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-
+0.4.3-x86_64-macOS.dmg) - **macOS** (M1) Â¹Â·Â²: [NormCap-0.4.3-arm64-
+macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.3/NormCap-
+0.4.3-arm64-macOS.dmg) \ 1: On macOS, allow the unsigned application on first
+start: "System Preferences" â "Security & Privacy" â "General" â "Open
+anyway". You might also need to allow NormCap to take screenshots. [#135]
+(https://github.com/dynobo/normcap/issues/135)
+2: Might be available a bit delayed, as it is currently build manually. (Thx,
+[@Takrin](https://github.com/Takrin)!) Install from repositories: -
+**Windows**: Install from [Microsoft Store](https://apps.microsoft.com/store/
+detail/normcap/XPDLJNB4B6C2ZR). - **Arch / Manjaro**: Install the [`normcap`]
+(https://aur.archlinux.org/packages/normcap) package from AUR. - **FlatPak
+(Linux)**: Install [com.github.dynobo.normcap](https://flathub.org/apps/
+details/com.github.dynobo.normcap) from FlatHub. If you experience issues
+please look at the [FAQs](https://dynobo.github.io/normcap/#faqs) or [open an
+issue](https://github.com/dynobo/normcap/issues). ## Python package As an
+_alternative_ to a prebuilt package you can install the [NormCap Python
+package](https://pypi.org/project/normcap/) for **Python >=3.9**: #### On Linux
+```sh # Install dependencies (Ubuntu/Debian) sudo apt install build-essential
+tesseract-ocr tesseract-ocr-eng libtesseract-dev libleptonica-dev wl-clipboard
+## Install dependencies (Arch) sudo pacman -S tesseract tesseract-data-eng wl-
+clipboard ## Install dependencies (Fedora) sudo dnf install tesseract wl-
+clipboard ## Install dependencies (openSUSE) sudo zypper install python3-devel
+tesseract-ocr tesseract-ocr-devel wl-clipboard # Install normcap pip install
+normcap # Run ./normcap ``` #### On macOS ```sh # Install dependencies brew
+install tesseract tesseract-lang # Install normcap pip install normcap # Run ./
+normcap ``` #### On Windows 1\. Install `Tesseract 5` by using the [installer
+provided by UB Mannheim](https://github.com/UB-Mannheim/tesseract/wiki). 2\.
+Adjust environment variables: - Create an environment variable
+`TESSDATA_PREFIX` and set it to Tesseract's data folder, e.g.: ```cmd setx
+TESSDATA_PREFIX "C:\Program Files\Tesseract-OCR\tessdata" ``` - Append
+Tesseract's location to the environment variable `Path`, e.g.: ```cmd setx Path
+"%Path%;C:\Program Files\Tesseract-OCR" ``` - Make sure to close and reopen
+your current terminal window to apply the new variables. Test it by running:
+```cmd tesseract --list-langs ``` 3\. Install and run NormCap: ```bash #
+Install normcap pip install normcap # Run normcap ``` ## Why "NormCap"? See
+[XKCD](https://xkcd.com): [![Comic](https://imgs.xkcd.com/comics/
+norm_normal_file_format.png)](https://xkcd.com/2116/) ## Development
+Prerequisites for setting up a development environment are: **Python >=3.9**,
+**Poetry>=1.3.2** and **Tesseract** (incl. **language data**). ```sh # Clone
+repository git clone https://github.com/dynobo/normcap.git # Change into
+project directory cd normcap # Create virtual env and install dependencies
+poetry install # Register pre-commit hook poetry run pre-commit install # Run
+NormCap in virtual env poetry run python -m normcap ``` ## Credits This project
+uses the following non-standard libraries: - [pyside6](https://pypi.org/
+project/PySide6/) _- bindings for Qt UI Framework_ And it depends on external
+software: - [tesseract](https://github.com/tesseract-ocr/tesseract) - _OCR
+engine_ - [wl-clipboard](https://github.com/bugaevc/wl-clipboard) - _Wayland
+clipboard utilities_ Packaging is done with: - [briefcase](https://pypi.org/
+project/briefcase/) _- converting Python projects into_ _standalone apps_
+Thanks to the maintainers of those nice tools! ## Similar open source tools If
+NormCap doesn't fit your needs, try those alternatives (no particular order): -
+[TextSnatcher](https://github.com/RajSolai/TextSnatcher) (Linux) - [GreenShot]
+(https://getgreenshot.org/) (Linux, macOS) - [TextShot](https://github.com/
+ianzhao05/textshot) (Windows) - [gImageReader](https://github.com/manisandro/
+gImageReader) (Linux, Windows) - [Capture2Text](https://sourceforge.net/
+projects/capture2text) (Windows) - [Frog](https://github.com/TenderOwl/Frog)
+(Linux) - [Textinator](https://github.com/RhetTbull/textinator) (macOS) -
+[Text-Grab](https://github.com/TheJoeFin/Text-Grab) (Windows) - [dpScreenOCR]
+(https://danpla.github.io/dpscreenocr/) (Linux, Windows) ## Certification !
+[WOMM](https://raw.githubusercontent.com/dynobo/lmdiag/master/badge.png)
```

