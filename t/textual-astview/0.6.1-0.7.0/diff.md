# Comparing `tmp/textual-astview-0.6.1.tar.gz` & `tmp/textual-astview-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual-astview-0.6.1.tar", last modified: Sat Apr 29 07:35:35 2023, max compression
+gzip compressed data, was "textual-astview-0.7.0.tar", last modified: Sat Jun  3 07:40:23 2023, max compression
```

## Comparing `textual-astview-0.6.1.tar` & `textual-astview-0.7.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:35:35.347220 textual-astview-0.6.1/
--rw-r--r--   0 davep      (501) staff       (20)     1087 2023-04-27 21:09:18.000000 textual-astview-0.6.1/LICENCE
--rw-r--r--   0 davep      (501) staff       (20)     6207 2023-04-29 07:35:35.347269 textual-astview-0.6.1/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)     4828 2023-04-27 21:09:18.000000 textual-astview-0.6.1/README.md
--rw-r--r--   0 davep      (501) staff       (20)      124 2023-04-27 21:09:18.000000 textual-astview-0.6.1/pyproject.toml
--rw-r--r--   0 davep      (501) staff       (20)     1580 2023-04-29 07:35:35.347486 textual-astview-0.6.1/setup.cfg
--rw-r--r--   0 davep      (501) staff       (20)      345 2023-04-27 21:09:18.000000 textual-astview-0.6.1/setup.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:35:35.345494 textual-astview-0.6.1/textual_astview/
--rw-r--r--   0 davep      (501) staff       (20)      934 2023-04-29 07:35:10.000000 textual-astview-0.6.1/textual_astview/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)      352 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/__main__.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:35:35.346379 textual-astview-0.6.1/textual_astview/app/
--rw-r--r--   0 davep      (501) staff       (20)       88 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/app/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     3676 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/app/astare.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:35:35.346607 textual-astview-0.6.1/textual_astview/app/screens/
--rw-r--r--   0 davep      (501) staff       (20)      342 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/app/screens/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)    10012 2023-04-29 07:35:10.000000 textual-astview-0.6.1/textual_astview/app/screens/main.py
--rw-r--r--   0 davep      (501) staff       (20)        0 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/py.typed
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:35:35.347116 textual-astview-0.6.1/textual_astview/widgets/
--rw-r--r--   0 davep      (501) staff       (20)       72 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/widgets/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     7226 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/widgets/astview.py
--rw-r--r--   0 davep      (501) staff       (20)     1770 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/widgets/node_info.py
--rw-r--r--   0 davep      (501) staff       (20)     7847 2023-04-27 21:09:18.000000 textual-astview-0.6.1/textual_astview/widgets/source.py
--rw-r--r--   0 davep      (501) staff       (20)     3790 2023-04-28 08:00:33.000000 textual-astview-0.6.1/textual_astview/widgets/source_info.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-04-29 07:35:35.346143 textual-astview-0.6.1/textual_astview.egg-info/
--rw-r--r--   0 davep      (501) staff       (20)     6207 2023-04-29 07:35:35.000000 textual-astview-0.6.1/textual_astview.egg-info/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      687 2023-04-29 07:35:35.000000 textual-astview-0.6.1/textual_astview.egg-info/SOURCES.txt
--rw-r--r--   0 davep      (501) staff       (20)        1 2023-04-29 07:35:35.000000 textual-astview-0.6.1/textual_astview.egg-info/dependency_links.txt
--rw-r--r--   0 davep      (501) staff       (20)       59 2023-04-29 07:35:35.000000 textual-astview-0.6.1/textual_astview.egg-info/entry_points.txt
--rw-r--r--   0 davep      (501) staff       (20)       16 2023-04-29 07:35:35.000000 textual-astview-0.6.1/textual_astview.egg-info/requires.txt
--rw-r--r--   0 davep      (501) staff       (20)       16 2023-04-29 07:35:35.000000 textual-astview-0.6.1/textual_astview.egg-info/top_level.txt
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-03 07:40:23.476415 textual-astview-0.7.0/
+-rw-r--r--   0 davep      (501) staff       (20)     1087 2023-04-27 21:09:18.000000 textual-astview-0.7.0/LICENCE
+-rw-r--r--   0 davep      (501) staff       (20)     6342 2023-06-03 07:40:23.476487 textual-astview-0.7.0/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)     4963 2023-06-03 07:39:48.000000 textual-astview-0.7.0/README.md
+-rw-r--r--   0 davep      (501) staff       (20)      124 2023-04-27 21:09:18.000000 textual-astview-0.7.0/pyproject.toml
+-rw-r--r--   0 davep      (501) staff       (20)     1600 2023-06-03 07:40:23.476730 textual-astview-0.7.0/setup.cfg
+-rw-r--r--   0 davep      (501) staff       (20)      345 2023-04-27 21:09:18.000000 textual-astview-0.7.0/setup.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-03 07:40:23.473872 textual-astview-0.7.0/textual_astview/
+-rw-r--r--   0 davep      (501) staff       (20)      934 2023-06-03 07:39:48.000000 textual-astview-0.7.0/textual_astview/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)      352 2023-04-27 21:09:18.000000 textual-astview-0.7.0/textual_astview/__main__.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-03 07:40:23.475088 textual-astview-0.7.0/textual_astview/app/
+-rw-r--r--   0 davep      (501) staff       (20)       88 2023-04-27 21:09:18.000000 textual-astview-0.7.0/textual_astview/app/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     3624 2023-06-03 07:39:48.000000 textual-astview-0.7.0/textual_astview/app/astare.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-03 07:40:23.475461 textual-astview-0.7.0/textual_astview/app/screens/
+-rw-r--r--   0 davep      (501) staff       (20)      342 2023-04-27 21:09:18.000000 textual-astview-0.7.0/textual_astview/app/screens/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     7822 2023-06-03 07:39:48.000000 textual-astview-0.7.0/textual_astview/app/screens/main.py
+-rw-r--r--   0 davep      (501) staff       (20)        0 2023-04-27 21:09:18.000000 textual-astview-0.7.0/textual_astview/py.typed
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-03 07:40:23.476198 textual-astview-0.7.0/textual_astview/widgets/
+-rw-r--r--   0 davep      (501) staff       (20)       72 2023-04-27 21:09:18.000000 textual-astview-0.7.0/textual_astview/widgets/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     7774 2023-06-03 07:39:48.000000 textual-astview-0.7.0/textual_astview/widgets/astview.py
+-rw-r--r--   0 davep      (501) staff       (20)     1770 2023-04-27 21:09:18.000000 textual-astview-0.7.0/textual_astview/widgets/node_info.py
+-rw-r--r--   0 davep      (501) staff       (20)     7847 2023-04-27 21:09:18.000000 textual-astview-0.7.0/textual_astview/widgets/source.py
+-rw-r--r--   0 davep      (501) staff       (20)     3790 2023-04-28 08:00:33.000000 textual-astview-0.7.0/textual_astview/widgets/source_info.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2023-06-03 07:40:23.474653 textual-astview-0.7.0/textual_astview.egg-info/
+-rw-r--r--   0 davep      (501) staff       (20)     6342 2023-06-03 07:40:23.000000 textual-astview-0.7.0/textual_astview.egg-info/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      687 2023-06-03 07:40:23.000000 textual-astview-0.7.0/textual_astview.egg-info/SOURCES.txt
+-rw-r--r--   0 davep      (501) staff       (20)        1 2023-06-03 07:40:23.000000 textual-astview-0.7.0/textual_astview.egg-info/dependency_links.txt
+-rw-r--r--   0 davep      (501) staff       (20)       59 2023-06-03 07:40:23.000000 textual-astview-0.7.0/textual_astview.egg-info/entry_points.txt
+-rw-r--r--   0 davep      (501) staff       (20)       33 2023-06-03 07:40:23.000000 textual-astview-0.7.0/textual_astview.egg-info/requires.txt
+-rw-r--r--   0 davep      (501) staff       (20)       16 2023-06-03 07:40:23.000000 textual-astview-0.7.0/textual_astview.egg-info/top_level.txt
```

### Comparing `textual-astview-0.6.1/LICENCE` & `textual-astview-0.7.0/LICENCE`

 * *Files identical despite different names*

### Comparing `textual-astview-0.6.1/PKG-INFO` & `textual-astview-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-astview
-Version: 0.6.1
+Version: 0.7.0
 Summary: An AST viewing widget library plus app, built for and with Textual.
 Home-page: https://github.com/davep/textual-astview
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
@@ -140,11 +140,13 @@
       position.
 - [X] Add support for setting the [source style](https://pygments.org/styles/).
 - [X] Add a dark/light mode toggle to `astare`.
 - [ ] Better handle really long "paths" in `NodeInfo`.
 - [X] In `astare` allow resizing of the panes.
 - [ ] Look at making the rainbow highlight in the source more of an "onion"
       style (try and use indentation columns to show the layers too).
+- [ ] Add more muted labels to the tree, but perhaps place them behind a
+      verbosity switch so the tree doesn't get too cluttered.
 - [ ] Keep on having fun hacking on it.
 - [ ] Other stuff. I'm sure there's other stuff.
 
 [//]: # (README.md ends here)
```

### Comparing `textual-astview-0.6.1/README.md` & `textual-astview-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -108,11 +108,13 @@
       position.
 - [X] Add support for setting the [source style](https://pygments.org/styles/).
 - [X] Add a dark/light mode toggle to `astare`.
 - [ ] Better handle really long "paths" in `NodeInfo`.
 - [X] In `astare` allow resizing of the panes.
 - [ ] Look at making the rainbow highlight in the source more of an "onion"
       style (try and use indentation columns to show the layers too).
+- [ ] Add more muted labels to the tree, but perhaps place them behind a
+      verbosity switch so the tree doesn't get too cluttered.
 - [ ] Keep on having fun hacking on it.
 - [ ] Other stuff. I'm sure there's other stuff.
 
 [//]: # (README.md ends here)
```

### Comparing `textual-astview-0.6.1/setup.cfg` & `textual-astview-0.7.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 	Issues = https://github.com/davep/textual-astview/issues
 	Discussions = https://github.com/davep/textual-astview/discussions
 
 [options]
 packages = find:
 platforms = any
 include_package_data = True
-install_requires = textual==0.22.3
+install_requires = 
+	textual>=0.27.0
+	textual-fspicker
 python_requires = >=3.8
 
 [options.package_data]
 textual_astview = py.typed
 
 [options.entry_points]
 console_scripts =
```

### Comparing `textual-astview-0.6.1/textual_astview/__init__.py` & `textual-astview-0.7.0/textual_astview/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ######################################################################
 # Main app information.
 __author__     = "Dave Pearson"
 __copyright__  = "Copyright 2022-2023, Dave Pearson"
 __credits__    = [ "Dave Pearson" ]
 __maintainer__ = "Dave Pearson"
 __email__      = "davep@davep.org"
-__version__    = "0.6.1"
+__version__    = "0.7.0"
 __licence__    = "MIT"
 
 ##############################################################################
 # Import the widgets to make them easier to get at.
 from .widgets.astview     import ASTView, ASTNode
 from .widgets.node_info   import NodeInfo
 from .widgets.source_info import SourceInfo
```

### Comparing `textual-astview-0.6.1/textual_astview/app/astare.py` & `textual-astview-0.7.0/textual_astview/app/astare.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,18 +101,16 @@
         action  = "version",
         version = f"%(prog)s {__version__} (Textual v{version( 'textual' )})"
     )
 
     # The remainder is the file to explore.
     parser.add_argument(
         "file",
-        help    = "The file to explore",
-        nargs   = "?",
-        type    = py_file,
-        default = "."
+        help = "The file to explore",
+        type = py_file
     )
 
     # Return the arguments.
     return parser.parse_args()
 
 ##############################################################################
 def main() -> None:
```

### Comparing `textual-astview-0.6.1/textual_astview/app/screens/main.py` & `textual-astview-0.7.0/textual_astview/app/screens/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,48 +10,31 @@
 ##############################################################################
 # Textual imports.
 from textual.app        import ComposeResult
 from textual.binding    import Binding
 from textual.screen     import Screen
 from textual.reactive   import reactive
 from textual.timer      import Timer
-from textual.widgets    import Header, Footer, Tree, DirectoryTree
+from textual.widgets    import Header, Footer, Tree
 from textual.containers import Horizontal, Vertical
 from textual.css.query  import NoMatches
 
 ##############################################################################
+# Other imports.
+from textual_fspicker import FileOpen, Filters
+
+##############################################################################
 # Local imports.
 from textual_astview import ASTView, ASTNode, NodeInfo, Source, __version__
 
 ##############################################################################
 class MainDisplay( Screen ):
     """The main display of the app."""
 
     DEFAULT_CSS = """
-    DirectoryTree {
-        border: solid $primary-background-lighten-2;
-        display: none;
-    }
-
-    DirectoryTree.visible {
-        display: block;
-    }
-
-    DirectiryTree.initial {
-        width: 100%;
-    }
-
-    DirectoryTree.insert {
-        width: 20%;
-    }
-
-    DirectoryTree:focus-within {
-        border: double $primary-lighten-2;
-    }
-
     Vertical {
         width: 1fr;
     }
 
     ASTView {
         border: solid $primary-background-lighten-2;
         width: 10fr;
@@ -91,50 +74,30 @@
         Args:
             cli_args: The command line arguments.
         """
         super().__init__( *args, **kwargs )
         self._args                       = cli_args
         self._refresh: Optional[ Timer ] = None
 
-    def ast_pane( self ) -> ASTView:
-        """Make an ASTView pane.
-
-        Returns:
-            An ASTView pane for viewing the AST.
-        """
-        return ASTView( self._args.file, id="ast-view" )
-
-    def source_pane( self ) -> Source:
-        """Make a Source pane.
-
-        Returns:
-            A source pane for viewing the code.
-        """
-        return Source(
-            self._args.file,
-            dark_theme  = self._args.dark_theme,
-            light_theme = self._args.light_theme
-        )
-
     def compose( self ) -> ComposeResult:
         """Compose the main app screen.
 
         Returns:
             The result of composing the screen.
         """
-
-        if self._args.file.is_file():
-            body = [
-                DirectoryTree( str( self._args.file.parent ), classes="insert" ), self.ast_pane(), self.source_pane()
-            ]
-        else:
-            body = [ DirectoryTree( str( self._args.file ), classes="visible initial" ) ]
-
         yield Header()
-        yield Vertical( Horizontal( *body ), NodeInfo() )
+        with Vertical():
+            with Horizontal():
+                yield ASTView( self._args.file, id="ast-view" )
+                yield Source(
+                    self._args.file,
+                    dark_theme  = self._args.dark_theme,
+                    light_theme = self._args.light_theme
+                )
+            yield NodeInfo()
         yield Footer()
 
     def _init_tree( self ) -> None:
         """Set up the tree view when (re)loaded."""
         view = self.query_one( ASTView )
         view.root.expand()
         if view.root.children:
@@ -142,18 +105,15 @@
             if view.root.children[ 0 ].children:
                 view.root.children[ 0 ].children[ 0 ].expand()
         view.focus()
         self.highlight_node( view.root )
 
     def on_mount( self ) -> None:
         """Sort the screen once the DOM is mounted."""
-        if self.query( ASTView ):
-            self._init_tree()
-        else:
-            self.query_one( DirectoryTree ).focus()
+        self._init_tree()
 
     def highlight_node( self, node: ASTNode ) -> None:
         """Update the display to highlight the given node.
 
         Args:
             node: The node to highlight.
         """
@@ -223,20 +183,31 @@
         self.app.dark = not self.app.dark
         try:
             self.query_one( Source ).dark = self.app.dark
             self.highlight_node( cast( ASTNode, self.query_one( ASTView ).cursor_node ) )
         except NoMatches:
             pass
 
+    async def open_file( self, new_file: Path ) -> None:
+        """Open a new file for viewing.
+
+        Args:
+            new_file: The new file to view.
+        """
+        self._args.file = new_file
+        self.query_one( ASTView ).reset( new_file )
+        self.query_one( Source ).show_file( self._args.file )
+        self._init_tree()
+
     def action_open_new( self ) -> None:
         """Open a new file for viewing."""
-        opener = self.query_one( DirectoryTree )
-        opener.toggle_class( "visible" )
-        if "visible" in opener.classes:
-            opener.focus()
+        self.app.push_screen( FileOpen( self._args.file.parent if self._args.file else ".", filters=Filters(
+            ( "Python Source", lambda p: p.suffix.lower() == ".py" ),
+            ( "Any",           lambda _: True )
+        ), must_exist=True ), callback=self.open_file )
 
     def watch_ast_width( self ) -> None:
         """React to the AST view width being changed by the user."""
         self.query_one( ASTView ).styles.width = f"{self.ast_width}fr"
         self.query_one( Source ).styles.width = f"{10 + ( 10 - self.ast_width )}fr"
 
     def action_shrink_left( self ) -> None:
@@ -245,43 +216,8 @@
             self.ast_width -= 1
 
     def action_shrink_right( self ) -> None:
         """Shrink the right pane in the display."""
         if self.ast_width < 18:
             self.ast_width += 1
 
-    async def on_directory_tree_file_selected( self, event: DirectoryTree.FileSelected ) -> None:
-        """React to a file being selected in the directory tree.
-
-        Args:
-            event: The file selection event.
-        """
-        self._args.file = Path( event.path )
-
-        # Currently there's no good way to 100% empty out a Textual Tree and
-        # populate it again from scratch. You can clear everything under the
-        # root node, which would almost work, but then there's no public
-        # method of setting a new label or data. Se we need to do a rebuild
-        # dance instead. First, if there's already an ASTView in the DOM...
-        if self.query( ASTView ):
-            # ...remove it...
-            await self.query_one( ASTView ).remove()
-            # ...and then add a fresh one, splicing it into the display
-            # before the source view.
-            await self.mount( self.ast_pane(), before="Source" )
-        else:
-            # There's no ASTView. This means we've dome from just showing
-            # just the directory tree and nothing else. In that case we need
-            # to spin up and splice in an ASTView...
-            await self.mount( self.ast_pane(), after="DirectoryTree" )
-            # ...and then also a Source view.
-            await self.mount( self.source_pane(), after="ASTView" )
-            # Finally: the DirectiryTree will have been in its initial "fill
-            # the display" state; so swap out that class and put it into
-            # "insert me on the left when called upon" state.
-            self.query_one( DirectoryTree ).toggle_class( "initial", "insert" )
-
-        self.query_one( Source ).show_file( self._args.file )
-        self.query_one( DirectoryTree ).set_class( False, "visible" )
-        self._init_tree()
-
 ### main.py ends here
```

### Comparing `textual-astview-0.6.1/textual_astview/widgets/astview.py` & `textual-astview-0.7.0/textual_astview/widgets/astview.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 ##############################################################################
 # Rich imports.
 from rich.text import Text
 
 ##############################################################################
 # Textual imports.
+from textual              import on
+from textual.events       import Mount
 from textual.widgets      import Tree
 from textual.widgets.tree import TreeNode
 from textual.binding      import Binding
 
 ##############################################################################
 ASTNode = TreeNode[ Any ]
 
@@ -61,28 +63,52 @@
             `name_defs` to turn this off.
         """
 
         # Remember some key stuff
         self._name_defs   = name_defs
         self._module_path = module
 
+        self._parse( module )
+
+        # Now that we've configured things, get the Tree to do its own
+        # thing.
+        kwargs[ "label" ] = module.name
+        kwargs[ "data" ]  = self._module_path
+        super().__init__( *args, **kwargs )
+
+    @on( Mount )
+    def _populate_tree( self ) -> None:
+        """Populate the tree with the module's AST."""
+        self.add( self._module, self.root )
+        self.select_node( self.root )
+
+    def _parse( self, module: Path ) -> None:
+        """Parse the module.
+
+        Args:
+            module: The module to parse.
+        """
         # Get the AST parsed in. I *suppose* it would make sense to try and
         # do this in an async way, perhaps? But for now anyway let's just
         # parse in the whole blasted thing up front. I've never found the
         # AST parser to be noticeably slow.
         try:
             self._module: Optional[ ast.Module ] = ast.parse( module.read_text() )
         except SyntaxError:
             self._module = None
 
-        # Now that we've configured things, get the Tree to do its own
-        # thing.
-        kwargs[ "label" ] = module.name
-        kwargs[ "data" ]  = self._module_path
-        super().__init__( *args, **kwargs )
+    def reset( self, module: Path ) -> None:
+        """Reset the display to show a new module.
+
+        Args:
+            module: The new module to show.
+        """
+        self._parse( module )
+        super().reset( module.name, module )
+        self._populate_tree()
 
     @property
     def module_path( self ) -> Path:
         """Path: The path for the module being shown."""
         return self._module_path
 
     @singledispatchmethod
@@ -201,18 +227,13 @@
                 if self.maybe_add( value := getattr( item, field ) ):
                     self.add( value, self.base_node( field, node ) )
         else:
             # It's a AST item with no fields, so don't allow expanding as
             # there's nothing to expand.
             node.allow_expand = False
 
-    def on_mount( self ) -> None:
-        """Populate the view once we're mounted."""
-        self.add( self._module, self.root )
-        self.select_node( self.root )
-
     def action_toggle_all( self ) -> None:
         """Toggle all the nodes from the selected node down."""
         if self.cursor_node is not None:
             self.cursor_node.toggle_all()
 
 ### astview.py ends here
```

### Comparing `textual-astview-0.6.1/textual_astview/widgets/node_info.py` & `textual-astview-0.7.0/textual_astview/widgets/node_info.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.6.1/textual_astview/widgets/source.py` & `textual-astview-0.7.0/textual_astview/widgets/source.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.6.1/textual_astview/widgets/source_info.py` & `textual-astview-0.7.0/textual_astview/widgets/source_info.py`

 * *Files identical despite different names*

### Comparing `textual-astview-0.6.1/textual_astview.egg-info/PKG-INFO` & `textual-astview-0.7.0/textual_astview.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-astview
-Version: 0.6.1
+Version: 0.7.0
 Summary: An AST viewing widget library plus app, built for and with Textual.
 Home-page: https://github.com/davep/textual-astview
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
@@ -140,11 +140,13 @@
       position.
 - [X] Add support for setting the [source style](https://pygments.org/styles/).
 - [X] Add a dark/light mode toggle to `astare`.
 - [ ] Better handle really long "paths" in `NodeInfo`.
 - [X] In `astare` allow resizing of the panes.
 - [ ] Look at making the rainbow highlight in the source more of an "onion"
       style (try and use indentation columns to show the layers too).
+- [ ] Add more muted labels to the tree, but perhaps place them behind a
+      verbosity switch so the tree doesn't get too cluttered.
 - [ ] Keep on having fun hacking on it.
 - [ ] Other stuff. I'm sure there's other stuff.
 
 [//]: # (README.md ends here)
```

### Comparing `textual-astview-0.6.1/textual_astview.egg-info/SOURCES.txt` & `textual-astview-0.7.0/textual_astview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

