# Comparing `tmp/customtkinterx-0.2.3.tar.gz` & `tmp/customtkinterx-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkinterx-0.2.3.tar", max compression
+gzip compressed data, was "customtkinterx-0.2.4.tar", max compression
```

## Comparing `customtkinterx-0.2.3.tar` & `customtkinterx-0.2.4.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.2.3/customtkinterx/__base64.py
--rw-r--r--   0        0        0     1012 2023-06-03 04:42:25.299802 customtkinterx-0.2.3/customtkinterx/__init__.py
--rw-r--r--   0        0        0      805 2023-06-03 05:50:39.831676 customtkinterx-0.2.3/customtkinterx/__main__.py
--rw-r--r--   0        0        0     6409 2023-06-03 05:49:11.439039 customtkinterx-0.2.3/customtkinterx/CTkCustom.py
--rw-r--r--   0        0        0     6220 2023-06-03 03:49:13.477694 customtkinterx-0.2.3/customtkinterx/CTkFluentTheme.py
--rw-r--r--   0        0        0     6286 2023-06-03 04:57:04.717519 customtkinterx-0.2.3/customtkinterx/CTkInfoBar.py
--rw-r--r--   0        0        0     1244 2023-06-02 11:00:54.754723 customtkinterx-0.2.3/customtkinterx/CTkListBox.py
--rw-r--r--   0        0        0     3180 2023-06-03 04:57:04.655526 customtkinterx-0.2.3/customtkinterx/CTkMegaMenuBar.py
--rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.2.3/customtkinterx/CTkMenuBar/__init__.py
--rw-r--r--   0        0        0      522 2023-06-03 04:06:01.937274 customtkinterx-0.2.3/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16174 2023-06-03 04:13:46.399109 customtkinterx-0.2.3/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
--rw-r--r--   0        0        0     5239 2023-06-03 04:13:46.393587 customtkinterx-0.2.3/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
--rw-r--r--   0        0        0     9724 2023-06-03 04:13:46.396108 customtkinterx-0.2.3/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
--rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.2.3/customtkinterx/CTkMenuBar/dropdown_menu.py
--rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.2.3/customtkinterx/CTkMenuBar/menu_bar.py
--rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.2.3/customtkinterx/CTkMenuBar/title_menu_win.py
--rw-r--r--   0        0        0     6190 2023-06-03 04:57:53.921397 customtkinterx-0.2.3/customtkinterx/CTkMinimalTheme.py
--rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.2.3/customtkinterx/CTkPDFViewer/__init__.py
--rw-r--r--   0        0        0      445 2023-06-03 04:13:46.400109 customtkinterx-0.2.3/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6312 2023-06-03 05:49:55.800794 customtkinterx-0.2.3/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
--rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.2.3/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
--rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.2.3/customtkinterx/CTkTable/__init__.py
--rw-r--r--   0        0        0      427 2023-06-03 04:41:34.919572 customtkinterx-0.2.3/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    11621 2023-06-03 04:41:34.922572 customtkinterx-0.2.3/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
--rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.2.3/customtkinterx/CTkTable/ctktable.py
--rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.2.3/customtkinterx/CTkToolTip/__init__.py
--rw-r--r--   0        0        0      426 2023-06-03 04:22:17.427710 customtkinterx-0.2.3/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10684 2023-06-03 04:26:02.400121 customtkinterx-0.2.3/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
--rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.2.3/customtkinterx/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0        0        0     5598 2023-06-02 14:38:51.493749 customtkinterx-0.2.3/customtkinterx/Fluent.json
--rw-r--r--   0        0        0     2418 2023-06-02 22:37:52.229296 customtkinterx-0.2.3/customtkinterx/LaunchMusix.py
--rw-r--r--   0        0        0     5563 2023-06-03 05:50:30.149406 customtkinterx-0.2.3/customtkinterx/Minimal.json
--rw-r--r--   0        0        0      343 2023-06-03 05:55:04.225658 customtkinterx-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3405 2023-06-03 04:59:32.072137 customtkinterx-0.2.3/README.md
--rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 customtkinterx-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.2.4/customtkinterx/__base64.py
+-rw-r--r--   0        0        0      971 2023-06-03 06:08:32.364752 customtkinterx-0.2.4/customtkinterx/__init__.py
+-rw-r--r--   0        0        0      809 2023-06-03 06:51:26.706174 customtkinterx-0.2.4/customtkinterx/__main__.py
+-rw-r--r--   0        0        0     8210 2023-06-03 06:51:26.711685 customtkinterx-0.2.4/customtkinterx/CTkCustom.py
+-rw-r--r--   0        0        0     6220 2023-06-03 03:49:13.477694 customtkinterx-0.2.4/customtkinterx/CTkFluentTheme.py
+-rw-r--r--   0        0        0     6286 2023-06-03 04:57:04.717519 customtkinterx-0.2.4/customtkinterx/CTkInfoBar.py
+-rw-r--r--   0        0        0     1244 2023-06-02 11:00:54.754723 customtkinterx-0.2.4/customtkinterx/CTkListBox.py
+-rw-r--r--   0        0        0     3180 2023-06-03 04:57:04.655526 customtkinterx-0.2.4/customtkinterx/CTkMegaMenuBar.py
+-rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__init__.py
+-rw-r--r--   0        0        0      522 2023-06-03 04:06:01.937274 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16174 2023-06-03 04:13:46.399109 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
+-rw-r--r--   0        0        0     5239 2023-06-03 04:13:46.393587 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
+-rw-r--r--   0        0        0     9724 2023-06-03 04:13:46.396108 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
+-rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/dropdown_menu.py
+-rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/menu_bar.py
+-rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.2.4/customtkinterx/CTkMenuBar/title_menu_win.py
+-rw-r--r--   0        0        0     6190 2023-06-03 04:57:53.921397 customtkinterx-0.2.4/customtkinterx/CTkMinimalTheme.py
+-rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.2.4/customtkinterx/CTkPDFViewer/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-03 04:13:46.400109 customtkinterx-0.2.4/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6312 2023-06-03 05:49:55.800794 customtkinterx-0.2.4/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
+-rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.2.4/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
+-rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.2.4/customtkinterx/CTkTable/__init__.py
+-rw-r--r--   0        0        0      427 2023-06-03 04:41:34.919572 customtkinterx-0.2.4/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    11621 2023-06-03 04:41:34.922572 customtkinterx-0.2.4/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
+-rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.2.4/customtkinterx/CTkTable/ctktable.py
+-rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.2.4/customtkinterx/CTkToolTip/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-03 04:22:17.427710 customtkinterx-0.2.4/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10684 2023-06-03 04:26:02.400121 customtkinterx-0.2.4/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
+-rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.2.4/customtkinterx/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0        0        0     5598 2023-06-02 14:38:51.493749 customtkinterx-0.2.4/customtkinterx/Fluent.json
+-rw-r--r--   0        0        0     2714 2023-06-03 05:59:19.575174 customtkinterx-0.2.4/customtkinterx/LaunchMusix.py
+-rw-r--r--   0        0        0     5563 2023-06-03 05:50:30.149406 customtkinterx-0.2.4/customtkinterx/Minimal.json
+-rw-r--r--   0        0        0     5435 2023-06-03 06:15:30.726312 customtkinterx-0.2.4/customtkinterx/tk_dragtool.py
+-rw-r--r--   0        0        0      343 2023-06-03 06:54:18.438839 customtkinterx-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3686 2023-06-03 06:54:12.682589 customtkinterx-0.2.4/README.md
+-rw-r--r--   0        0        0     4121 1970-01-01 00:00:00.000000 customtkinterx-0.2.4/PKG-INFO
```

### Comparing `customtkinterx-0.2.3/customtkinterx/__init__.py` & `customtkinterx-0.2.4/customtkinterx/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,9 +12,7 @@
 from customtkinterx.CTkPDFViewer import CTkPDFViewer
 
 # From https://github.com/Akascape/CTkToolTip
 from customtkinterx.CTkToolTip import CTkToolTip
 
 # From https://github.com/Akascape/CTkTable
 from customtkinterx.CTkTable import CTkTable
-
-CTkFluentThemeTempPath = fluent_theme()
```

### Comparing `customtkinterx-0.2.3/customtkinterx/__main__.py` & `customtkinterx-0.2.4/customtkinterx/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 CTkMinimalTheme()
 
 set_appearance_mode("dark")
 
 root = CTkCustom()
 root.title("CustomTkinterX")
 root.titlebar_title.configure(text="CustomTkinterX")
-root.create_sizegrip()
+root.create_sizegrip(True)
 
 CTkButton(root.mainframe, text="Light", command=lambda: set_appearance_mode("light")).pack(fill="x", padx=5, pady=5, ipady=3)
 CTkButton(root.mainframe, text="Dark", command=lambda: set_appearance_mode("dark")).pack(fill="x", padx=5, pady=5, ipady=3)
 
 scrolledframe = CTkScrollableFrame(root.mainframe)
 scrolledframe.pack(fill="both", expand="yes", padx=5, pady=5)
```

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkCustom.py` & `customtkinterx-0.2.4/customtkinterx/CTkCustom.py`

 * *Files 14% similar despite different names*

```diff
@@ -90,33 +90,77 @@
             self.__button_minimize._draw()
 
         if platform == "linux":
             self.__frame_border.configure(corner_radius=0)
 
         self.x, self.y = 0, 0
 
+        self.sg_x = 0
+        self.sg_y = 0
+        self.sg_width = 0
+        self.sg_height = 0
+
     def minimize(self):
         try:
             from ctypes import windll
             hwnd = windll.user32.GetParent(self.winfo_id())
             windll.user32.ShowWindow(hwnd, 2)
         except:
             pass
 
     def bind_move(self, widget):
         widget.bind("<Button-1>", self._click)
         widget.bind("<B1-Motion>", self._move)
 
-    def create_sizegrip(self):
-        if get_appearance_mode() == "Dark":
-            ttk.Style().configure("CTkCustom.TSizegrip", background=ThemeManager.theme["CTkFrame"]["fg_color"][1])
+    from tkinter import Event
+
+    def _sizegrip_click(self, event: Event):
+        from ctypes import Structure, c_ulong, byref, windll
+
+        class _PointAPI(Structure):
+            _fields_ = [("x", c_ulong), ("y", c_ulong)]
+
+        def getpos():
+            # 调用API函数获取当前鼠标位置。返回值以(x,y)形式表示。
+            po = _PointAPI()
+            windll.user32.GetCursorPos(byref(po))
+            return int(po.x), int(po.y)
+
+        self.sg_cx, self.sg_cy = getpos()
+        self.sg_x, self.sg_y = self.winfo_x(), self.winfo_y()
+        self.sg_width = self.winfo_width()
+        self.sg_height = self.winfo_height()
+
+    def _sizegrip_move(self, event: Event):
+        from pyautogui import position
+
+        dx = position()[0] - self.sg_cx
+        dy = position()[1] - self.sg_cy
+        self.geometry(f"{self.sg_width + dx}x{self.sg_height + dy}+{self.sg_x}+{self.sg_y}")
+
+    def create_sizegrip(self, custom: bool = False):
+        from sys import platform
+        if custom:
+            from customtkinterx.tk_dragtool import bind_resize
+            self.sizegrip = CTkButton(self.__frame_border, width=32, height=32, text="⚪")
+            self.sizegrip.configure(cursor="sizing")
+
+            self.sizegrip.bind("<Button-1>", self._sizegrip_click)
+            self.sizegrip.bind("<B1-Motion>", self._sizegrip_move)
+            self.sizegrip._text_color = ThemeManager.theme["CTkLabel"]["text_color"]
+            self.sizegrip._fg_color = self.sizegrip._hover_color = self.__frame_border._fg_color
+            self.sizegrip._draw()
+            self.sizegrip.pack(side="bottom", anchor="se", padx=3, pady=3)
         else:
-            ttk.Style().configure("CTkCustom.TSizegrip", background=ThemeManager.theme["CTkFrame"]["fg_color"][0])
-        self.sizegrip = ttk.Sizegrip(self.__frame_border, style="CTkCustom.TSizegrip")
-        self.sizegrip.pack(side="bottom", anchor="se", padx=5, pady=5, ipady=2)
+            if get_appearance_mode() == "Dark":
+                ttk.Style().configure("CTkCustom.TSizegrip", background=ThemeManager.theme["CTkFrame"]["fg_color"][1])
+            else:
+                ttk.Style().configure("CTkCustom.TSizegrip", background=ThemeManager.theme["CTkFrame"]["fg_color"][0])
+            self.sizegrip = ttk.Sizegrip(self.__frame_border, style="CTkCustom.TSizegrip")
+            self.sizegrip.pack(side="bottom", anchor="se", padx=5, pady=5, ipady=2)
         return self.sizegrip
 
     @property
     def titlebar(self):
         return self.__frame_title
 
     @property
```

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkFluentTheme.py` & `customtkinterx-0.2.4/customtkinterx/CTkFluentTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkInfoBar.py` & `customtkinterx-0.2.4/customtkinterx/CTkInfoBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkListBox.py` & `customtkinterx-0.2.4/customtkinterx/CTkListBox.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkMegaMenuBar.py` & `customtkinterx-0.2.4/customtkinterx/CTkMegaMenuBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc` & `customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc` & `customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc` & `customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc` & `customtkinterx-0.2.4/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkMenuBar/dropdown_menu.py` & `customtkinterx-0.2.4/customtkinterx/CTkMenuBar/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkMenuBar/menu_bar.py` & `customtkinterx-0.2.4/customtkinterx/CTkMenuBar/menu_bar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkMenuBar/title_menu_win.py` & `customtkinterx-0.2.4/customtkinterx/CTkMenuBar/title_menu_win.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkMinimalTheme.py` & `customtkinterx-0.2.4/customtkinterx/CTkMinimalTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc` & `customtkinterx-0.2.4/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py` & `customtkinterx-0.2.4/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc` & `customtkinterx-0.2.4/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkTable/ctktable.py` & `customtkinterx-0.2.4/customtkinterx/CTkTable/ctktable.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc` & `customtkinterx-0.2.4/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/CTkToolTip/ctk_tooltip.py` & `customtkinterx-0.2.4/customtkinterx/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/Fluent.json` & `customtkinterx-0.2.4/customtkinterx/Fluent.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/customtkinterx/LaunchMusix.py` & `customtkinterx-0.2.4/customtkinterx/LaunchMusix.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,15 +32,24 @@
 
     frame_results = CTkScrollableFrame(tk_root.mainframe)
     frame_results.pack(fill="both", expand="yes", padx=5, pady=(2.5, 5))
 
 
     def cloud_search():
         def _search():
-            from cloudmusic import search, getMusic
+            try:
+                from cloudmusic import search, getMusic
+            except ModuleNotFoundError:
+                from os import system
+                from sys import executable
+                from threading import Thread
+
+
+                Thread(target=lambda: system(f"{executable} -m pip install cloudmusic")).start()
+
             results = search(entry_search.get(), 15)
             for index in results:
                 print(index.name)
                 __ = index
 
                 __frame = CTkFrame(frame_results)
                 __frame.setvar()
```

### Comparing `customtkinterx-0.2.3/customtkinterx/Minimal.json` & `customtkinterx-0.2.4/customtkinterx/Minimal.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.3/README.md` & `customtkinterx-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -56,24 +56,42 @@
 }
 ```
 
 ### 添加缩放窗口大小的手柄
 ```python
 CTKCustom.create_sizegrip()
 ```
+自定义手柄，将会使用库`pyautogui`。
+```bash
+python -m pyautogui
+```
+```python
+CTKCustom.create_sizegrip(True)
+```
+
 ```python
 from customtkinter import *
 from customtkinterx import *
 
 root = CTkCustom()
 root.create_sizegrip()
 
 root.mainloop()
 ```
 
+```python
+from customtkinter import *
+from customtkinterx import *
+
+root = CTkCustom()
+root.create_sizegrip(True)
+
+root.mainloop()
+```
+
 ## CTkInfoBar 消息栏
 ### 组件结构
 ```markdown
 | CTkInforBar -> CTkFrame
 |-->> __label_title(title): CTkLabel
 |-->> __label_info(info): CTkLabel
 |-->> __button_close(close): CTkButton
```

### Comparing `customtkinterx-0.2.3/PKG-INFO` & `customtkinterx-0.2.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customtkinterx
-Version: 0.2.3
+Version: 0.2.4
 Summary: extra widgets for customtkinter
 Author: XiangQinxi
 Author-email: XiangQinxi@outlook.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -72,24 +72,42 @@
 }
 ```
 
 ### 添加缩放窗口大小的手柄
 ```python
 CTKCustom.create_sizegrip()
 ```
+自定义手柄，将会使用库`pyautogui`。
+```bash
+python -m pyautogui
+```
+```python
+CTKCustom.create_sizegrip(True)
+```
+
 ```python
 from customtkinter import *
 from customtkinterx import *
 
 root = CTkCustom()
 root.create_sizegrip()
 
 root.mainloop()
 ```
 
+```python
+from customtkinter import *
+from customtkinterx import *
+
+root = CTkCustom()
+root.create_sizegrip(True)
+
+root.mainloop()
+```
+
 ## CTkInfoBar 消息栏
 ### 组件结构
 ```markdown
 | CTkInforBar -> CTkFrame
 |-->> __label_title(title): CTkLabel
 |-->> __label_info(info): CTkLabel
 |-->> __button_close(close): CTkButton
```

