# Comparing `tmp/elm-messenger-0.2.5.tar.gz` & `tmp/elm-messenger-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.2.5.tar", last modified: Thu Jun  1 03:52:17 2023, max compression
+gzip compressed data, was "elm-messenger-0.2.6.tar", last modified: Sat Jun  3 16:15:26 2023, max compression
```

## Comparing `elm-messenger-0.2.5.tar` & `elm-messenger-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-06-01 03:52:17.280542 elm-messenger-0.2.5/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.2.5/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)     7374 2023-06-01 03:52:17.280542 elm-messenger-0.2.5/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)     7109 2023-05-31 16:29:21.000000 elm-messenger-0.2.5/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-06-01 03:52:17.277209 elm-messenger-0.2.5/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)     7374 2023-06-01 03:52:17.000000 elm-messenger-0.2.5/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2023-06-01 03:52:17.000000 elm-messenger-0.2.5/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-06-01 03:52:17.000000 elm-messenger-0.2.5/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-06-01 03:52:17.000000 elm-messenger-0.2.5/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       16 2023-06-01 03:52:17.000000 elm-messenger-0.2.5/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-06-01 03:52:17.000000 elm-messenger-0.2.5/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-06-01 03:52:17.280542 elm-messenger-0.2.5/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.2.5/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.2.5/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)    19438 2023-06-01 03:45:19.000000 elm-messenger-0.2.5/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      771 2023-05-27 16:23:18.000000 elm-messenger-0.2.5/messengercli/patcher.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.2.5/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      418 2023-06-01 03:52:17.280542 elm-messenger-0.2.5/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.2.5/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-06-03 16:15:26.254666 elm-messenger-0.2.6/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.2.6/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     7374 2023-06-03 16:15:26.254666 elm-messenger-0.2.6/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     7109 2023-05-31 16:29:21.000000 elm-messenger-0.2.6/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-06-03 16:15:26.254666 elm-messenger-0.2.6/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     7374 2023-06-03 16:15:26.000000 elm-messenger-0.2.6/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2023-06-03 16:15:26.000000 elm-messenger-0.2.6/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-06-03 16:15:26.000000 elm-messenger-0.2.6/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-06-03 16:15:26.000000 elm-messenger-0.2.6/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       16 2023-06-03 16:15:26.000000 elm-messenger-0.2.6/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-06-03 16:15:26.000000 elm-messenger-0.2.6/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-06-03 16:15:26.254666 elm-messenger-0.2.6/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.2.6/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.2.6/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)    20016 2023-06-03 16:12:48.000000 elm-messenger-0.2.6/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      798 2023-06-03 16:04:50.000000 elm-messenger-0.2.6/messengercli/patcher.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.2.6/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      418 2023-06-03 16:15:26.258000 elm-messenger-0.2.6/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.2.6/setup.py
```

### Comparing `elm-messenger-0.2.5/PKG-INFO` & `elm-messenger-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elm-messenger
-Version: 0.2.5
+Version: 0.2.6
 Summary: The Messenger game framework toolkit for Elm
 Author: linsyking
 Author-email: linsy_king@sjtu.edu.cn
 License: MIT License
 Keywords: cli
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `elm-messenger-0.2.5/Readme.md` & `elm-messenger-0.2.6/Readme.md`

 * *Files identical despite different names*

### Comparing `elm-messenger-0.2.5/elm_messenger.egg-info/PKG-INFO` & `elm-messenger-0.2.6/elm_messenger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elm-messenger
-Version: 0.2.5
+Version: 0.2.6
 Summary: The Messenger game framework toolkit for Elm
 Author: linsyking
 Author-email: linsy_king@sjtu.edu.cn
 License: MIT License
 Keywords: cli
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `elm-messenger-0.2.5/messengercli/messenger.py` & `elm-messenger-0.2.6/messengercli/messenger.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import shutil
 import json
 from .updater import Updater
 from .patcher import patch
 
 app = typer.Typer(add_completion=False, help="Messenger CLI")
-API_VERSION = "0.2.5"
+API_VERSION = "0.2.6"
 
 
 class Messenger:
     config = None
 
     def __init__(self) -> None:
         """
@@ -26,15 +26,15 @@
         if os.path.exists("messenger.json"):
             with open("messenger.json", "r") as f:
                 self.config = json.load(f)
             if "version" not in self.config:
                 raise Exception("Messenger API version not found in the config file.")
             if self.config["version"] != API_VERSION:
                 raise Exception(
-                    f"Messenger API version not matched. I'm using v{API_VERSION}. You can edit messenger.json manually to upgrade."
+                    f"Messenger API version not matched. I'm using v{API_VERSION}. You can edit messenger.json manually to upgrade/downgrade."
                 )
         else:
             raise Exception(
                 "messenger.json not found. Are you in the project initialized by the Messenger? Try `messenger init <your-project-name>`."
             )
         if not os.path.exists(".messenger"):
             print("Messenger files not found. Initializing...")
@@ -388,14 +388,24 @@
                     f"{l}G.getLayerT <| {l}.initLayer (addCommonData nullCommonData env) layerInitData"
                     for l in layers
                 ]
             )
         )
 
 
+def check_name(name: str):
+    """
+    Check if the the first character of the name is Capital
+    """
+    if name[0].islower():
+        return name[0].capitalize() + name[1:]
+    else:
+        return name
+
+
 @app.command()
 def init(
     name: str,
     template_repo=typer.Option(
         "https://github.com/linsyking/messenger-templates",
         "--template-repo",
         "-t",
@@ -447,14 +457,15 @@
 @app.command()
 def component(
     name: str,
     dir=typer.Option(
         "", "--dir", "-d", help="Component module to create component in."
     ),
 ):
+    name = check_name(name)
     msg = Messenger()
     input(f"You are going to create a component named {name}, continue?")
     msg.add_component(name, dir)
     msg.format()
     print("Done!")
 
 
@@ -483,14 +494,15 @@
         msg.update_sceneproto_layers(sceneprotolayer)
     msg.format()
     print("Done!")
 
 
 @app.command()
 def scene(name: str):
+    name = check_name(name)
     msg = Messenger()
     input(f"You are going to create a scene named {name}, continue?")
     msg.add_scene(name)
     msg.update_scenes()
     msg.format()
     print("Done!")
 
@@ -499,59 +511,68 @@
 def layer(
     scene: str,
     layer: str,
     has_component: bool = typer.Option(
         False, "--with-component", "-c", help="Use components in this layer"
     ),
 ):
+    scene = check_name(scene)
+    layer = check_name(layer)
     msg = Messenger()
     input(
         f"You are going to create a layer named {layer} under scene {scene}, continue?"
     )
     msg.add_layer(scene, layer, has_component)
     msg.update_layers(scene)
     msg.format()
     print("Done!")
 
 
 @app.command()
 def sceneproto(sceneproto: str):
+    sceneproto = check_name(sceneproto)
     msg = Messenger()
     input(f"You are going to create a sceneproto named {sceneproto}, continue?")
     msg.add_sceneproto(sceneproto)
     msg.format()
     print("Done!")
 
 
 @app.command()
 def level(sceneproto: str, level: str):
+    sceneproto = check_name(sceneproto)
+    level = check_name(level)
     msg = Messenger()
     input(
         f"You are going to create a level named {level} under sceneproto {sceneproto}, continue?"
     )
     msg.add_level(sceneproto, level)
     msg.update_scenes()
     msg.format()
     print("Done!")
 
 
 @app.command()
 def protolayer(sceneproto: str, layer: str):
+    sceneproto = check_name(sceneproto)
+    layer = check_name(layer)
     msg = Messenger()
     input(
         f"You are going to create a layer named {layer} under sceneproto {sceneproto}, continue?"
     )
     msg.add_sceneproto_layer(sceneproto, layer)
     msg.update_sceneproto_layers(sceneproto)
     msg.format()
     print("Done!")
 
 
 @app.command()
 def gamecomponent(sceneproto: str, gc: str):
+    sceneproto = check_name(sceneproto)
+    gc = check_name(gc)
     msg = Messenger()
     input(
         f"You are going to create a game component named {gc} under sceneproto {sceneproto}, continue?"
     )
     msg.add_gamecomponent(sceneproto, gc)
     msg.format()
     print("Done!")
```

### Comparing `elm-messenger-0.2.5/messengercli/patcher.py` & `elm-messenger-0.2.6/messengercli/patcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from git import Repo
 import os
 
 def patch():
     repo = Repo(".messenger")
     oldsha = repo.head.commit.hexsha
     print(f"Current commit: {oldsha}")
-    remote = repo.remote()
     print(f"Pulling...")
-    remote.pull()
+    os.chdir(".messenger")
+    os.system("git pull")
+    os.chdir("..")
     newsha = repo.head.commit.hexsha
     print(f"Current commit: {newsha}")
     if newsha == oldsha:
         print("No update found.")
         return
     else:
         # Create patch
```

### Comparing `elm-messenger-0.2.5/messengercli/updater.py` & `elm-messenger-0.2.6/messengercli/updater.py`

 * *Files identical despite different names*

