# Comparing `tmp/customtkinterx-0.2.1.tar.gz` & `tmp/customtkinterx-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkinterx-0.2.1.tar", max compression
+gzip compressed data, was "customtkinterx-0.2.2.tar", max compression
```

## Comparing `customtkinterx-0.2.1.tar` & `customtkinterx-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.2.1/customtkinterx/__base64.py
--rw-r--r--   0        0        0     1012 2023-06-03 04:42:25.299802 customtkinterx-0.2.1/customtkinterx/__init__.py
--rw-r--r--   0        0        0      804 2023-06-03 04:32:03.691398 customtkinterx-0.2.1/customtkinterx/__main__.py
--rw-r--r--   0        0        0     6241 2023-06-03 04:57:04.722519 customtkinterx-0.2.1/customtkinterx/CTkCustom.py
--rw-r--r--   0        0        0     6220 2023-06-03 03:49:13.477694 customtkinterx-0.2.1/customtkinterx/CTkFluentTheme.py
--rw-r--r--   0        0        0     6286 2023-06-03 04:57:04.717519 customtkinterx-0.2.1/customtkinterx/CTkInfoBar.py
--rw-r--r--   0        0        0     1244 2023-06-02 11:00:54.754723 customtkinterx-0.2.1/customtkinterx/CTkListBox.py
--rw-r--r--   0        0        0     3180 2023-06-03 04:57:04.655526 customtkinterx-0.2.1/customtkinterx/CTkMegaMenuBar.py
--rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__init__.py
--rw-r--r--   0        0        0      522 2023-06-03 04:06:01.937274 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16174 2023-06-03 04:13:46.399109 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
--rw-r--r--   0        0        0     5239 2023-06-03 04:13:46.393587 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
--rw-r--r--   0        0        0     9724 2023-06-03 04:13:46.396108 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
--rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/dropdown_menu.py
--rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/menu_bar.py
--rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/title_menu_win.py
--rw-r--r--   0        0        0     6190 2023-06-03 04:57:53.921397 customtkinterx-0.2.1/customtkinterx/CTkMinimalTheme.py
--rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.2.1/customtkinterx/CTkPDFViewer/__init__.py
--rw-r--r--   0        0        0      445 2023-06-03 04:13:46.400109 customtkinterx-0.2.1/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6311 2023-06-03 04:14:21.525818 customtkinterx-0.2.1/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
--rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.2.1/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
--rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.2.1/customtkinterx/CTkTable/__init__.py
--rw-r--r--   0        0        0      427 2023-06-03 04:41:34.919572 customtkinterx-0.2.1/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    11621 2023-06-03 04:41:34.922572 customtkinterx-0.2.1/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
--rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.2.1/customtkinterx/CTkTable/ctktable.py
--rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.2.1/customtkinterx/CTkToolTip/__init__.py
--rw-r--r--   0        0        0      426 2023-06-03 04:22:17.427710 customtkinterx-0.2.1/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10684 2023-06-03 04:26:02.400121 customtkinterx-0.2.1/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
--rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.2.1/customtkinterx/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0        0        0     5598 2023-06-02 14:38:51.493749 customtkinterx-0.2.1/customtkinterx/Fluent.json
--rw-r--r--   0        0        0  1445444 2023-06-03 05:09:33.609641 customtkinterx-0.2.1/customtkinterx/input.png
--rw-r--r--   0        0        0     2418 2023-06-02 22:37:52.229296 customtkinterx-0.2.1/customtkinterx/LaunchMusix.py
--rw-r--r--   0        0        0     5561 2023-06-03 04:47:54.791777 customtkinterx-0.2.1/customtkinterx/Minimal.json
--rw-r--r--   0        0        0      343 2023-06-03 05:14:23.598522 customtkinterx-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3405 2023-06-03 04:59:32.072137 customtkinterx-0.2.1/README.md
--rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 customtkinterx-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.2.2/customtkinterx/__base64.py
+-rw-r--r--   0        0        0     1012 2023-06-03 04:42:25.299802 customtkinterx-0.2.2/customtkinterx/__init__.py
+-rw-r--r--   0        0        0      805 2023-06-03 05:50:39.831676 customtkinterx-0.2.2/customtkinterx/__main__.py
+-rw-r--r--   0        0        0     6409 2023-06-03 05:49:11.439039 customtkinterx-0.2.2/customtkinterx/CTkCustom.py
+-rw-r--r--   0        0        0     6220 2023-06-03 03:49:13.477694 customtkinterx-0.2.2/customtkinterx/CTkFluentTheme.py
+-rw-r--r--   0        0        0     6286 2023-06-03 04:57:04.717519 customtkinterx-0.2.2/customtkinterx/CTkInfoBar.py
+-rw-r--r--   0        0        0     1244 2023-06-02 11:00:54.754723 customtkinterx-0.2.2/customtkinterx/CTkListBox.py
+-rw-r--r--   0        0        0     3180 2023-06-03 04:57:04.655526 customtkinterx-0.2.2/customtkinterx/CTkMegaMenuBar.py
+-rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.2.2/customtkinterx/CTkMenuBar/__init__.py
+-rw-r--r--   0        0        0      522 2023-06-03 04:06:01.937274 customtkinterx-0.2.2/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16174 2023-06-03 04:13:46.399109 customtkinterx-0.2.2/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
+-rw-r--r--   0        0        0     5239 2023-06-03 04:13:46.393587 customtkinterx-0.2.2/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
+-rw-r--r--   0        0        0     9724 2023-06-03 04:13:46.396108 customtkinterx-0.2.2/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
+-rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.2.2/customtkinterx/CTkMenuBar/dropdown_menu.py
+-rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.2.2/customtkinterx/CTkMenuBar/menu_bar.py
+-rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.2.2/customtkinterx/CTkMenuBar/title_menu_win.py
+-rw-r--r--   0        0        0     6190 2023-06-03 04:57:53.921397 customtkinterx-0.2.2/customtkinterx/CTkMinimalTheme.py
+-rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.2.2/customtkinterx/CTkPDFViewer/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-03 04:13:46.400109 customtkinterx-0.2.2/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6312 2023-06-03 05:49:55.800794 customtkinterx-0.2.2/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
+-rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.2.2/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
+-rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.2.2/customtkinterx/CTkTable/__init__.py
+-rw-r--r--   0        0        0      427 2023-06-03 04:41:34.919572 customtkinterx-0.2.2/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    11621 2023-06-03 04:41:34.922572 customtkinterx-0.2.2/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
+-rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.2.2/customtkinterx/CTkTable/ctktable.py
+-rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.2.2/customtkinterx/CTkToolTip/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-03 04:22:17.427710 customtkinterx-0.2.2/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10684 2023-06-03 04:26:02.400121 customtkinterx-0.2.2/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
+-rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.2.2/customtkinterx/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0        0        0     5598 2023-06-02 14:38:51.493749 customtkinterx-0.2.2/customtkinterx/Fluent.json
+-rw-r--r--   0        0        0  1445444 2023-06-03 05:09:33.609641 customtkinterx-0.2.2/customtkinterx/input.png
+-rw-r--r--   0        0        0     2418 2023-06-02 22:37:52.229296 customtkinterx-0.2.2/customtkinterx/LaunchMusix.py
+-rw-r--r--   0        0        0     5563 2023-06-03 05:50:30.149406 customtkinterx-0.2.2/customtkinterx/Minimal.json
+-rw-r--r--   0        0        0      343 2023-06-03 05:17:07.286105 customtkinterx-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3405 2023-06-03 04:59:32.072137 customtkinterx-0.2.2/README.md
+-rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 customtkinterx-0.2.2/PKG-INFO
```

### Comparing `customtkinterx-0.2.1/customtkinterx/__init__.py` & `customtkinterx-0.2.2/customtkinterx/__init__.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/__main__.py` & `customtkinterx-0.2.2/customtkinterx/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from customtkinter import *
 from customtkinterx import *
 
-CTkFluentTheme()
+CTkMinimalTheme()
 
 set_appearance_mode("dark")
 
 root = CTkCustom()
 root.title("CustomTkinterX")
 root.titlebar_title.configure(text="CustomTkinterX")
 root.create_sizegrip()
```

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkCustom.py` & `customtkinterx-0.2.2/customtkinterx/CTkCustom.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
                     self.__transparent_color = "#101010"
                 self.attributes("-transparentcolor", self.__transparent_color)
                 self.configure(fg_color=self.__transparent_color)
             elif platform == "darwin":
                 self.__transparent_color = 'systemTransparent'
                 self.attributes("-transparent", True)
                 self.configure(fg_color=self.__transparent_color)
+            else:
+                self.__transparent_color = '#000001'
 
         self.wm_overrideredirect(True)
 
         if advanced:
             if platform == "win32":
                 from ctypes import windll
                 GWL_EXSTYLE = -20
@@ -83,14 +85,17 @@
             self.__button_close._draw()
 
             self.__button_minimize._text_color = ThemeManager.theme["CTkCustom"]["minimizebutton_text_color"]
             self.__button_minimize._fg_color = ThemeManager.theme["CTkCustom"]["minimizebutton_color"]
             self.__button_minimize._hover_color = ThemeManager.theme["CTkCustom"]["minimizebutton_hover_color"]
             self.__button_minimize._draw()
 
+        if platform == "linux":
+            self.__frame_border.configure(corner_radius=0)
+
         self.x, self.y = 0, 0
 
     def minimize(self):
         try:
             from ctypes import windll
             hwnd = windll.user32.GetParent(self.winfo_id())
             windll.user32.ShowWindow(hwnd, 2)
```

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkFluentTheme.py` & `customtkinterx-0.2.2/customtkinterx/CTkFluentTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkInfoBar.py` & `customtkinterx-0.2.2/customtkinterx/CTkInfoBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkListBox.py` & `customtkinterx-0.2.2/customtkinterx/CTkListBox.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkMegaMenuBar.py` & `customtkinterx-0.2.2/customtkinterx/CTkMegaMenuBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc` & `customtkinterx-0.2.2/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc` & `customtkinterx-0.2.2/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc` & `customtkinterx-0.2.2/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc` & `customtkinterx-0.2.2/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkMenuBar/dropdown_menu.py` & `customtkinterx-0.2.2/customtkinterx/CTkMenuBar/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkMenuBar/menu_bar.py` & `customtkinterx-0.2.2/customtkinterx/CTkMenuBar/menu_bar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkMenuBar/title_menu_win.py` & `customtkinterx-0.2.2/customtkinterx/CTkMenuBar/title_menu_win.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkMinimalTheme.py` & `customtkinterx-0.2.2/customtkinterx/CTkMinimalTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc` & `customtkinterx-0.2.2/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,44 +1,44 @@
 magic:    0xa70d0d0a
-moddate:  0x1dbe7a64 (Sat Jun  3 04:14:21 2023 UTC)
-files sz: 3539
+moddate:  0x23cc7a64 (Sat Jun  3 05:14:11 2023 UTC)
+files sz: 3543
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x970064005a00640164026c015a01640164036c026d035a030100090064
-      0164026c045a046e0b2300650524007203010059006e0477007803590077
+      0x970064005a00640164026c015a010900640164026c025a02640164036c
+      036d045a0401006e0b2300650524007203010059006e0477007803590077
       01640164046c066d075a070100640164026c085a08640164026c095a0964
       0164026c0a5a0a0200470064058400640665016a0b0000000000000000a6
       030000ab0300000000000000005a0c64025300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('\nCTkPDFViewer is a pdf viewer widget for customtkinter.\nAuthor: Akash Bora\nLicense: MIT\n')
                  4 STORE_NAME               0 (__doc__)
    
      7           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
                 10 IMPORT_NAME              1 (customtkinter)
                 12 STORE_NAME               1 (customtkinter)
    
-     8          14 LOAD_CONST               1 (0)
-                16 LOAD_CONST               3 (('Image',))
-                18 IMPORT_NAME              2 (PIL)
-                20 IMPORT_FROM              3 (Image)
-                22 STORE_NAME               3 (Image)
-                24 POP_TOP
-   
-    10          26 NOP
-   
-    11          28 LOAD_CONST               1 (0)
-                30 LOAD_CONST               2 (None)
-                32 IMPORT_NAME              4 (fitz)
-                34 STORE_NAME               4 (fitz)
+     9          14 NOP
+   
+    10          16 LOAD_CONST               1 (0)
+                18 LOAD_CONST               2 (None)
+                20 IMPORT_NAME              2 (fitz)
+                22 STORE_NAME               2 (fitz)
+   
+    11          24 LOAD_CONST               1 (0)
+                26 LOAD_CONST               3 (('Image',))
+                28 IMPORT_NAME              3 (PIL)
+                30 IMPORT_FROM              4 (Image)
+                32 STORE_NAME               4 (Image)
+                34 POP_TOP
                 36 JUMP_FORWARD            11 (to 60)
            >>   38 PUSH_EXC_INFO
    
     12          40 LOAD_NAME                5 (ModuleNotFoundError)
                 42 CHECK_EXC_MATCH
                 44 POP_JUMP_FORWARD_IF_FALSE     3 (to 52)
                 46 POP_TOP
@@ -82,15 +82,15 @@
                108 LOAD_ATTR               11 (CTkScrollableFrame)
                118 PRECALL                  3
                122 CALL                     3
                132 STORE_NAME              12 (CTkPDFViewer)
                134 LOAD_CONST               2 (None)
                136 RETURN_VALUE
    ExceptionTable:
-     28 to 34 -> 38 [0]
+     16 to 34 -> 38 [0]
      38 to 46 -> 54 [1] lasti
      52 to 52 -> 54 [1] lasti
    consts
       '\nCTkPDFViewer is a pdf viewer widget for customtkinter.\nAuthor: Akash Bora\nLicense: MIT\n'
       0
       None
       ('Image',)
@@ -856,15 +856,15 @@
          filename   'D:\\custontkinterx\\customtkinterx\\CTkPDFViewer\\ctk_pdf_viewer.py'
          name       'CTkPDFViewer'
          firstlineno 20
          lnotab
             0x0c050201020102fb040102ff020202fe020302fd020402fc020502fb0c
             1d0603061a
       'CTkPDFViewer'
-   names      ('__doc__', 'customtkinter', 'PIL', 'Image', 'fitz', 'ModuleNotFoundError', 'threading', 'Thread', 'math', 'io', 'os', 'CTkScrollableFrame', 'CTkPDFViewer')
+   names      ('__doc__', 'customtkinter', 'fitz', 'PIL', 'Image', 'ModuleNotFoundError', 'threading', 'Thread', 'math', 'io', 'os', 'CTkScrollableFrame', 'CTkPDFViewer')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\custontkinterx\\customtkinterx\\CTkPDFViewer\\ctk_pdf_viewer.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201040608010c0202010c01080104ff08020c01080108010803
+   lnotab 0x00ff020104060802020108011001080104ff08020c01080108010803
```

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py` & `customtkinterx-0.2.2/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc` & `customtkinterx-0.2.2/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkTable/ctktable.py` & `customtkinterx-0.2.2/customtkinterx/CTkTable/ctktable.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc` & `customtkinterx-0.2.2/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/CTkToolTip/ctk_tooltip.py` & `customtkinterx-0.2.2/customtkinterx/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/Fluent.json` & `customtkinterx-0.2.2/customtkinterx/Fluent.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/input.png` & `customtkinterx-0.2.2/customtkinterx/input.png`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/LaunchMusix.py` & `customtkinterx-0.2.2/customtkinterx/LaunchMusix.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/customtkinterx/Minimal.json` & `customtkinterx-0.2.2/customtkinterx/Minimal.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'CTk'": "{'fg_color': ['#f9fafb', '#161c24']}",*

 * * "'CTkToplevel'": "{'fg_color': ['#f9fafb', '#161c24']}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "CTk": {
         "fg_color": [
-            "#f8fafb",
-            "#151c24"
+            "#f9fafb",
+            "#161c24"
         ]
     },
     "CTkButton": {
         "border_color": [
             "#f3f3f3",
             "#949A9F"
         ],
@@ -392,16 +392,16 @@
         "text_color": [
             "gray10",
             "#DCE4EE"
         ]
     },
     "CTkToplevel": {
         "fg_color": [
-            "#f8fafb",
-            "#151c24"
+            "#f9fafb",
+            "#161c24"
         ]
     },
     "DropdownMenu": {
         "fg_color": [
             "gray90",
             "#1c1c1c"
         ],
```

### Comparing `customtkinterx-0.2.1/README.md` & `customtkinterx-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.1/PKG-INFO` & `customtkinterx-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customtkinterx
-Version: 0.2.1
+Version: 0.2.2
 Summary: extra widgets for customtkinter
 Author: XiangQinxi
 Author-email: XiangQinxi@outlook.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

