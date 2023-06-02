# Comparing `tmp/tktermwidget-0.0.1.tar.gz` & `tmp/tktermwidget-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tktermwidget-0.0.1.tar", last modified: Sun May 28 04:33:13 2023, max compression
+gzip compressed data, was "tktermwidget-0.0.2.tar", last modified: Fri Jun  2 23:38:56 2023, max compression
```

## Comparing `tktermwidget-0.0.1.tar` & `tktermwidget-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:33:13.358174 tktermwidget-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-28 04:32:53.000000 tktermwidget-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-28 04:33:13.354174 tktermwidget-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-28 04:32:53.000000 tktermwidget-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-28 04:32:53.000000 tktermwidget-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 04:33:13.358174 tktermwidget-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-28 04:32:53.000000 tktermwidget-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:33:13.354174 tktermwidget-0.0.1/tktermwidget/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-28 04:32:53.000000 tktermwidget-0.0.1/tktermwidget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-28 04:32:53.000000 tktermwidget-0.0.1/tktermwidget/tkterm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:33:13.354174 tktermwidget-0.0.1/tktermwidget.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-28 04:33:13.000000 tktermwidget-0.0.1/tktermwidget.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-28 04:33:13.000000 tktermwidget-0.0.1/tktermwidget.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 04:33:13.000000 tktermwidget-0.0.1/tktermwidget.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 04:33:13.000000 tktermwidget-0.0.1/tktermwidget.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:38:56.053158 tktermwidget-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-02 23:38:30.000000 tktermwidget-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-02 23:38:56.053158 tktermwidget-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-02 23:38:30.000000 tktermwidget-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-02 23:38:30.000000 tktermwidget-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 23:38:56.053158 tktermwidget-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-02 23:38:30.000000 tktermwidget-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:38:56.053158 tktermwidget-0.0.2/tktermwidget/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 23:38:30.000000 tktermwidget-0.0.2/tktermwidget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-06-02 23:38:30.000000 tktermwidget-0.0.2/tktermwidget/tkterm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 23:38:56.053158 tktermwidget-0.0.2/tktermwidget.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-02 23:38:56.000000 tktermwidget-0.0.2/tktermwidget.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-02 23:38:56.000000 tktermwidget-0.0.2/tktermwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 23:38:56.000000 tktermwidget-0.0.2/tktermwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 23:38:56.000000 tktermwidget-0.0.2/tktermwidget.egg-info/top_level.txt
```

### Comparing `tktermwidget-0.0.1/LICENSE` & `tktermwidget-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tktermwidget-0.0.1/PKG-INFO` & `tktermwidget-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tktermwidget
-Version: 0.0.1
+Version: 0.0.2
 Summary: A terminal emulator for Tkinter
 Home-page: https://github.com/littlewhitecloud/TkTerminal
 Author: littlewhitecloud
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `tkterm`
```

### Comparing `tktermwidget-0.0.1/README.md` & `tktermwidget-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tktermwidget-0.0.1/tktermwidget/tkterm.py` & `tktermwidget-0.0.2/tktermwidget/tkterm.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,51 +26,72 @@
     # Also create the history file
     open(HISTORY_PATH / "history.txt", "w").close()
 
 # Check that the history file exists
 if not (HISTORY_PATH / "history.txt").exists():
     open(HISTORY_PATH / "history.txt", "w").close()
 
+
 class AutoHideScrollbar(Scrollbar):
     """Scrollbar that automatically hides when not needed"""
+
     def __init__(self, master=None, **kwargs):
         Scrollbar.__init__(self, master=master, **kwargs)
 
-    def set(self, l, h):
-        if float(l) <= 0.0 and float(h) >= 1.0:
+    def set(self, length, height):
+        if float(length) <= 0.0 and float(height) >= 1.0:
             self.grid_remove()
         else:
             self.grid()
 
-        Scrollbar.set(self, l, h)
+        Scrollbar.set(self, length, height)
+
 
 class Terminal(Frame):
-    """A terminal widget for tkinter applications"""
+    """A terminal widget for tkinter applications
 
-    def __init__(self, master: Misc) -> None:
+    Args:
+        master (Misc): The parent widget
+        autohide (bool, optional): Whether to autohide the scrollbars. Defaults to True.
+        *args: Arguments for the text widget
+        **kwargs: Keyword arguments for the text widget
+
+    Methods for outside use:
+        None
+
+    Methods for internal use:
+        up (Event) -> str: Goes up in the history
+        down (Event) -> str: Goes down in the history (if the user is at the bottom of the history, it clears the command)
+        left (Event) -> str: Goes left in the command if the index is greater than the length of the directory (so the user can't delete the directory or go left of it)
+        kill (Event) -> str: Kills the current command
+        loop (Event) -> str: Runs the command typed"""
+
+    def __init__(self, master: Misc, autohide: bool = True, *args, **kwargs):
         Frame.__init__(self, master)
 
         # Set row and column weights
         self.rowconfigure(0, weight=1)
         self.columnconfigure(0, weight=1)
 
         # Create text widget and scrollbars
-        self.xscroll = AutoHideScrollbar(self, orient="horizontal")
-        self.yscroll = AutoHideScrollbar(self)
+        scrollbars = Scrollbar if not autohide else AutoHideScrollbar
+        self.xscroll = scrollbars(self, orient="horizontal")
+        self.yscroll = scrollbars(self)
         self.text = Text(
             self,
-            background="#2B2B2B",
-            insertbackground="#DCDCDC",
-            selectbackground="#b4b3b3",
-            relief="flat",
-            foreground="#cccccc",
+            *args,
+            background=kwargs.get("background", "#2B2B2B"),
+            insertbackground=kwargs.get("insertbackground", "#DCDCDC"),
+            selectbackground=kwargs.get("selectbackground", "#b4b3b3"),
+            relief=kwargs.get("relief", "flat"),
+            foreground=kwargs.get("foreground", "#cccccc"),
             xscrollcommand=self.xscroll.set,
             yscrollcommand=self.yscroll.set,
-            wrap="none",
-            font=("Cascadia Code", 9, "normal"),
+            wrap=kwargs.get("wrap", "char"),
+            font=kwargs.get("font", ("Cascadia Code", 9, "normal")),
         )
         self.xscroll.config(command=self.text.xview)
         self.yscroll.config(command=self.text.yview)
 
         # Grid widgets
         self.text.grid(row=0, column=0, sticky="nsew")
         self.xscroll.grid(row=1, column=0, sticky="ew")
@@ -85,36 +106,93 @@
         # Set variables
         self.index = 1
         self.current_process: Popen | None = None
 
         # Bind events
         self.text.bind("<Up>", self.up, add=True)
         self.text.bind("<Down>", self.down, add=True)
+        self.text.bind("<Left>", self.left, add=True)
+        self.text.bind("<BackSpace>", self.left, add=True)
+        self.text.bind("<Control-KeyPress-c>", self.kill, add=True)  # Isn't working
         self.text.bind("<Return>", self.loop, add=True)
 
         # History recorder
         self.history = open(HISTORY_PATH / "history.txt", "r+")
-        self.historys = self.history.readlines()
-        print(self.historys)
+        self.historys = [i.strip() for i in self.history.readlines() if i.strip()]
         self.hi = len(self.historys) - 1
 
+    def up(self, _: Event) -> str:
+        """Go up in the history"""
+        if self.hi >= 0:
+            self.text.delete(f"{self.index}.0", "end-1c")
+            # Insert the directory
+            self.text.insert(
+                "insert",
+                f"{DIR.format(command=getcwd())}",
+            )
+            # Insert the command
+            self.text.insert("insert", self.historys[self.hi].strip())
+            self.hi -= 1
+        return "break"
+
+    def down(self, _: Event) -> str:
+        """Go down in the history"""
+        if self.hi < len(self.historys) - 1:
+            self.text.delete(f"{self.index}.0", "end-1c")
+            # Insert the directory
+            self.text.insert(
+                "insert",
+                f"{DIR.format(command=getcwd())}",
+            )
+            # Insert the command
+            self.text.insert("insert", self.historys[self.hi].strip())
+            self.hi += 1
+        else:
+            # Clear the command
+            self.text.delete(f"{self.index}.0", "end-1c")
+            # Insert the directory
+            self.text.insert(
+                "insert",
+                f"{DIR.format(command=getcwd())}",
+            )
+        return "break"
+
+    def left(self, _: Event) -> str:
+        """Go left in the command if the command is greater than the path"""
+        insert_index = self.text.index("insert")
+        dir_index = f"{insert_index.split('.')[0]}.{len(DIR.format(command=getcwd()))}"
+        if insert_index == dir_index:
+            return "break"
+
+    def kill(self, _: Event) -> str:
+        """Kill the current process"""
+        if self.current_process:
+            self.current_process.kill()
+            self.current_process = None
+        return "break"
+
     def loop(self, _: Event) -> str:
         """Create an input loop"""
         cmd = self.text.get(f"{self.index}.0", "end-1c")
         # Determine command based on system
         cmd = cmd.split("$")[-1]  # Unix
         if SYSTEM == "Windows":
             cmd = cmd.split(">")[-1].strip()
 
         # Record the command
         if cmd != "":
             self.history.write(cmd + "\n")
             self.historys.append(cmd)
             self.hi = len(self.historys) - 1
 
+        # Check that the insert position is at the end
+        if self.text.index("insert") != f"{self.index}.end":
+            self.text.mark_set("insert", f"{self.index}.end")
+            self.text.see("insert")
+
         # If the command is "clear" or "cls", clear the screen
         if cmd in ["clear", "cls"]:
             self.text.delete("1.0", "end")
             self.text.insert(
                 "insert",
                 f"{DIR.format(command=getcwd())}",
             )
@@ -125,74 +203,36 @@
             shell=True,
             stdout=PIPE,
             stderr=PIPE,
             stdin=PIPE,
             text=True,
             cwd=getcwd(),  # Until a solution for changing the working directory is found, this will have to do
             creationflags=CREATE_NEW_CONSOLE,
-        )
+        )  # The following needs to be put in an after so the kill command works and the program doesn't freeze
         # Check if the command was successful
         returncode = self.current_process.wait()
         process = self.current_process
         self.current_process = None
         returnlines = process.stdout.readlines()
         if returncode != 0:
-            returnlines += (
-                process.stderr.readlines()
-            )  # If the command was unsuccessful, it doesn't give stdout
+            returnlines += process.stderr.readlines()  # If the command was unsuccessful, it doesn't give stdout
             # TODO: Get the success message from the command (see #16)
 
         self.text.insert("insert", "\n")
         self.index += 1
         for line in returnlines:
             self.text.insert("insert", line)
             self.index += 1
 
         self.text.insert(
             "insert",
             f"{DIR.format(command=getcwd())}",
         )
         return "break"  # Prevent the default newline character insertion
 
-    def up(self, _: Event) -> str:
-        """Go up in the history"""
-        if self.hi >= 0:
-            self.text.delete(f"{self.index}.0", "end-1c")
-            # Insert the directory
-            self.text.insert(
-                "insert",
-                f"{DIR.format(command=getcwd())}",
-            )
-            # Insert the command
-            self.text.insert("insert", self.historys[self.hi].strip())
-            self.hi -= 1
-        return "break"
-
-    def down(self, _: Event) -> str:
-        """Go down in the history"""
-        if self.hi < len(self.historys) - 1:
-            self.text.delete(f"{self.index}.0", "end-1c")
-            # Insert the directory
-            self.text.insert(
-                "insert",
-                f"{DIR.format(command=getcwd())}",
-            )
-            # Insert the command
-            self.text.insert("insert", self.historys[self.hi].strip())
-            self.hi += 1
-        else:
-            # Clear the command
-            self.text.delete(f"{self.index}.0", "end-1c")
-            # Insert the directory
-            self.text.insert(
-                "insert",
-                f"{DIR.format(command=getcwd())}",
-            )
-        return "break"
-
 
 if __name__ == "__main__":
     from tkinter import Tk
 
     # Create root window
     root = Tk()
```

### Comparing `tktermwidget-0.0.1/tktermwidget.egg-info/PKG-INFO` & `tktermwidget-0.0.2/tktermwidget.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tktermwidget
-Version: 0.0.1
+Version: 0.0.2
 Summary: A terminal emulator for Tkinter
 Home-page: https://github.com/littlewhitecloud/TkTerminal
 Author: littlewhitecloud
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `tkterm`
```

