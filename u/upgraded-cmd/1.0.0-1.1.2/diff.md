# Comparing `tmp/upgraded_cmd-1.0.0.tar.gz` & `tmp/upgraded_cmd-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upgraded_cmd-1.0.0.tar", last modified: Sat Jun  3 18:59:40 2023, max compression
+gzip compressed data, was "upgraded_cmd-1.1.2.tar", last modified: Sat Jun  3 19:57:50 2023, max compression
```

## Comparing `upgraded_cmd-1.0.0.tar` & `upgraded_cmd-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:59:40.407418 upgraded_cmd-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-03 18:59:28.000000 upgraded_cmd-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-03 18:59:40.407418 upgraded_cmd-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 18:59:40.407418 upgraded_cmd-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-03 18:59:28.000000 upgraded_cmd-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:59:40.403418 upgraded_cmd-1.0.0/upgraded_cmd/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-03 18:59:28.000000 upgraded_cmd-1.0.0/upgraded_cmd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:59:40.407418 upgraded_cmd-1.0.0/upgraded_cmd/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-03 18:59:28.000000 upgraded_cmd-1.0.0/upgraded_cmd/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-03 18:59:28.000000 upgraded_cmd-1.0.0/upgraded_cmd/classes/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-06-03 18:59:28.000000 upgraded_cmd-1.0.0/upgraded_cmd/classes/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-03 18:59:28.000000 upgraded_cmd-1.0.0/upgraded_cmd/classes/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-03 18:59:28.000000 upgraded_cmd-1.0.0/upgraded_cmd/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 18:59:40.407418 upgraded_cmd-1.0.0/upgraded_cmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-03 18:59:40.000000 upgraded_cmd-1.0.0/upgraded_cmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-03 18:59:40.000000 upgraded_cmd-1.0.0/upgraded_cmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 18:59:40.000000 upgraded_cmd-1.0.0/upgraded_cmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-03 18:59:40.000000 upgraded_cmd-1.0.0/upgraded_cmd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:50.292365 upgraded_cmd-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-03 19:57:40.000000 upgraded_cmd-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-03 19:57:50.292365 upgraded_cmd-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 19:57:50.292365 upgraded_cmd-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-03 19:57:40.000000 upgraded_cmd-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:50.292365 upgraded_cmd-1.1.2/upgraded_cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-03 19:57:40.000000 upgraded_cmd-1.1.2/upgraded_cmd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:50.292365 upgraded_cmd-1.1.2/upgraded_cmd/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-03 19:57:40.000000 upgraded_cmd-1.1.2/upgraded_cmd/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-03 19:57:40.000000 upgraded_cmd-1.1.2/upgraded_cmd/classes/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-06-03 19:57:40.000000 upgraded_cmd-1.1.2/upgraded_cmd/classes/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-03 19:57:40.000000 upgraded_cmd-1.1.2/upgraded_cmd/classes/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-03 19:57:40.000000 upgraded_cmd-1.1.2/upgraded_cmd/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 19:57:50.292365 upgraded_cmd-1.1.2/upgraded_cmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-03 19:57:50.000000 upgraded_cmd-1.1.2/upgraded_cmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-03 19:57:50.000000 upgraded_cmd-1.1.2/upgraded_cmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 19:57:50.000000 upgraded_cmd-1.1.2/upgraded_cmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-03 19:57:50.000000 upgraded_cmd-1.1.2/upgraded_cmd.egg-info/top_level.txt
```

### Comparing `upgraded_cmd-1.0.0/LICENSE` & `upgraded_cmd-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `upgraded_cmd-1.0.0/upgraded_cmd/classes/cmd.py` & `upgraded_cmd-1.1.2/upgraded_cmd/classes/cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import os
 from upgraded_cmd.classes.entry import Entry, new_command, add_completion
+from upgraded_cmd.constants import SHOW
 
 
 @new_command('help')
 def _(self: Entry, *args):
     """help\nShows all available commands\n\nhelp <command>\nShows <command> description if available"""
     if len(args) > 1:
         return print("Expected at most 1 argument")
@@ -38,17 +39,17 @@
         self.prompt = prompt
 
     async def display_loop(self):
         while self.running:
             self.prompt.display(self.text, self.index)
             await asyncio.sleep(.05)
         if self.text:
-            self.prompt.display_old_line(self.text)
+            self.prompt.display_old_line(self.text + SHOW)
         else:
-            print(self.prompt.pre_display, end='')
+            print(self.prompt.pre_display, end=SHOW)
 
     async def main_loop(self):
         await asyncio.gather(self.display_loop(), self.read_loop())
 
     def run(self):
         asyncio.run(self.main_loop())
```

### Comparing `upgraded_cmd-1.0.0/upgraded_cmd/classes/entry.py` & `upgraded_cmd-1.1.2/upgraded_cmd/classes/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     meta_attr = 'Blue'
 
     def __new__(cls, name, bases, dic: dict):
         commands = {
             name: value for base in bases if hasattr(base, 'commands') for name, value in base.commands.items()
         } | cls.commands | dic.get('commands', {})
         complete = {
-            name: value for base in bases if hasattr(base, 'complete') for name, value in base.commands.items()
+            name: value for base in bases if hasattr(base, 'complete') for name, value in base.complete.items()
         } | cls.complete | dic.get('complete', {})
         cls.commands, cls.complete = {}, {}
         return type.__new__(cls, name, bases, dic | {'commands': commands, 'complete': complete})
 
 
 def new_command(name):
     def decor(func):
@@ -148,19 +148,20 @@
     def k_tab(self):
         self.cycle = self.compute_cycle()
         if not self.cycle:
             return
         text = self.text[:self.index]
         words, new_word = text.split(), not text.split(' ')[-1]
         words += [''] * new_word
+
         if self.cycling_index == -1:
             self.old_word = words[-1]
         self.cycling_index = (self.cycling_index + 2) % (len(self.cycle) + 1) - 1
-        new_words = words[:-1] + [self.old_word if self.cycling_index == -1 else self.cycle[self.cycling_index]]
 
+        new_words = words[:-1] + [self.old_word if self.cycling_index == -1 else self.cycle[self.cycling_index]]
         self.text = ' '.join(new_words)
         self.index = len(self.text)
 
     def k_up(self):
         if not self.history:
             return
         if self.history_index == -1:
```

### Comparing `upgraded_cmd-1.0.0/upgraded_cmd/classes/prompt.py` & `upgraded_cmd-1.1.2/upgraded_cmd/classes/prompt.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,7 +45,20 @@
     def display(self, text: str, index: int):
         BasePrompt.display(self, text, index)
         self.pre_display = self.instr[self.state][1]
         self.state = (self.state + 1) % len(self.prompts)
 
     def get_prompt(self) -> str:
         return self.prompts[self.state] + self.instr[self.state][0]
+
+
+class SimplePrompt(BasePrompt):
+    def __init__(self, prompt):
+        self.old_line_prompt = self.prompt = prompt + (FORMATTER if FORMATTER not in prompt else '')
+        self.instr = self.instructions(self.prompt)
+
+    def display(self, text: str, index: int):
+        BasePrompt.display(self, text, index)
+        self.pre_display = self.instr[1]
+
+    def get_prompt(self) -> str:
+        return self.prompt + self.instr[0]
```

### Comparing `upgraded_cmd-1.0.0/upgraded_cmd/constants.py` & `upgraded_cmd-1.1.2/upgraded_cmd/constants.py`

 * *Files identical despite different names*

