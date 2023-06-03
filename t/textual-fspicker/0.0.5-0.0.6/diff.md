# Comparing `tmp/textual_fspicker-0.0.5-py3-none-any.whl.zip` & `tmp/textual_fspicker-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,19 @@
-Zip file size: 16352 bytes, number of entries: 16
--rw-r--r--  2.0 unx      864 b- defN 23-May-23 20:46 textual_fspicker/__init__.py
--rw-r--r--  2.0 unx     3154 b- defN 23-May-23 20:46 textual_fspicker/__main__.py
--rw-r--r--  2.0 unx     4231 b- defN 23-May-23 20:46 textual_fspicker/base_dialog.py
--rw-r--r--  2.0 unx     5621 b- defN 23-May-23 20:46 textual_fspicker/file_dialog.py
+Zip file size: 17169 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      915 b- defN 23-Jun-03 06:49 textual_fspicker/__init__.py
+-rw-r--r--  2.0 unx     3254 b- defN 23-Jun-03 06:49 textual_fspicker/__main__.py
+-rw-r--r--  2.0 unx     4231 b- defN 23-Jun-03 06:39 textual_fspicker/base_dialog.py
+-rw-r--r--  2.0 unx     5682 b- defN 23-Jun-03 06:49 textual_fspicker/file_dialog.py
 -rw-r--r--  2.0 unx     1521 b- defN 23-May-23 20:46 textual_fspicker/file_open.py
 -rw-r--r--  2.0 unx     1570 b- defN 23-May-23 20:46 textual_fspicker/file_save.py
 -rw-r--r--  2.0 unx     1822 b- defN 23-May-21 08:58 textual_fspicker/path_filters.py
+-rw-r--r--  2.0 unx     1369 b- defN 23-Jun-03 06:49 textual_fspicker/path_maker.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-18 20:02 textual_fspicker/py.typed
 -rw-r--r--  2.0 unx     2174 b- defN 23-May-19 09:53 textual_fspicker/safe_tests.py
 -rw-r--r--  2.0 unx     2457 b- defN 23-May-22 20:47 textual_fspicker/select_directory.py
 -rw-r--r--  2.0 unx      389 b- defN 23-May-17 19:18 textual_fspicker/parts/__init__.py
--rw-r--r--  2.0 unx    15053 b- defN 23-May-21 08:58 textual_fspicker/parts/directory_navigation.py
--rw-r--r--  2.0 unx     4235 b- defN 23-May-23 20:47 textual_fspicker-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-23 20:47 textual_fspicker-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-23 20:47 textual_fspicker-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1393 b- defN 23-May-23 20:47 textual_fspicker-0.0.5.dist-info/RECORD
-16 files, 44593 bytes uncompressed, 14028 bytes compressed:  68.5%
+-rw-r--r--  2.0 unx    15134 b- defN 23-Jun-03 06:49 textual_fspicker/parts/directory_navigation.py
+-rw-r--r--  2.0 unx     4235 b- defN 23-Jun-03 06:50 textual_fspicker-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 06:50 textual_fspicker-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-03 06:50 textual_fspicker-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1480 b- defN 23-Jun-03 06:50 textual_fspicker-0.0.6.dist-info/RECORD
+17 files, 46342 bytes uncompressed, 14709 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -15,14 +15,17 @@
 
 Filename: textual_fspicker/file_save.py
 Comment: 
 
 Filename: textual_fspicker/path_filters.py
 Comment: 
 
+Filename: textual_fspicker/path_maker.py
+Comment: 
+
 Filename: textual_fspicker/py.typed
 Comment: 
 
 Filename: textual_fspicker/safe_tests.py
 Comment: 
 
 Filename: textual_fspicker/select_directory.py
@@ -30,20 +33,20 @@
 
 Filename: textual_fspicker/parts/__init__.py
 Comment: 
 
 Filename: textual_fspicker/parts/directory_navigation.py
 Comment: 
 
-Filename: textual_fspicker-0.0.5.dist-info/METADATA
+Filename: textual_fspicker-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: textual_fspicker-0.0.5.dist-info/WHEEL
+Filename: textual_fspicker-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: textual_fspicker-0.0.5.dist-info/top_level.txt
+Filename: textual_fspicker-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: textual_fspicker-0.0.5.dist-info/RECORD
+Filename: textual_fspicker-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## textual_fspicker/__init__.py

```diff
@@ -3,22 +3,23 @@
 ######################################################################
 # Main app information.
 __author__     = "Dave Pearson"
 __copyright__  = "Copyright 2023, Dave Pearson"
 __credits__    = [ "Dave Pearson" ]
 __maintainer__ = "Dave Pearson"
 __email__      = "davep@davep.org"
-__version__    = "0.0.5"
+__version__    = "0.0.6"
 __licence__    = "MIT"
 
 ##############################################################################
 # Local imports.
 from .file_open        import FileOpen
 from .file_save        import FileSave
 from .select_directory import SelectDirectory
 from .path_filters     import Filters
+from .path_maker       import MakePath
 
 ##############################################################################
 # Export the imports.
-__all__ = [ "FileOpen", "FileSave", "SelectDirectory", "Filters" ]
+__all__ = [ "FileOpen", "FileSave", "SelectDirectory", "Filters", "MakePath" ]
 
 ### __init__.py ends here
```

## textual_fspicker/__main__.py

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 ##############################################################################
 # Textual imports.
 from textual            import on
 from textual.app        import App, ComposeResult
 from textual.containers import Center, Horizontal
-from textual.widgets    import Label, Button
+from textual.widgets    import Label, Button, Footer
 
 ##############################################################################
 # Local imports.
 from textual_fspicker import FileOpen, FileSave, Filters, SelectDirectory
 
 ##############################################################################
 class TestApp( App[ None ] ):
@@ -32,22 +32,27 @@
 
     Screen#_default Horizontal Button {
         margin-left: 1;
         margin-right: 1;
     }
     """
 
+    BINDINGS = [
+        ( "d", "toggle_dark", "Light/Dark" )
+    ]
+
     def compose( self ) -> ComposeResult:
         """Compose the layout of the test application."""
         with Horizontal():
             yield Button( "Open a file", id="open" )
             yield Button( "Save a file", id="save" )
             yield Button( "Select a directory", id="directory" )
         with Center():
             yield Label( "Press the button to pick something" )
+        yield Footer()
 
     def show_selected( self, to_show: Path ) -> None:
         """Show the file that was selected by the user.
 
         Args:
             to_show: The file to show.
         """
```

## textual_fspicker/file_dialog.py

```diff
@@ -12,14 +12,15 @@
 from textual.widgets import Button,Input, Select
 
 ##############################################################################
 # Local imports.
 from .base_dialog  import FileSystemPickerScreen
 from .parts        import DirectoryNavigation
 from .path_filters import Filters
+from .path_maker   import MakePath
 
 ##############################################################################
 class FileFilter( Select[ int ] ):
     """The file filter."""
 
 ##############################################################################
 class BaseFileDialog( FileSystemPickerScreen ):
@@ -123,23 +124,24 @@
         """
         event.stop()
         file_name = self.query_one( Input )
 
         # Only even try and process this if there's some input.
         if not file_name.value:
             self._set_error( "A file must be chosen" )
+            return
 
         # If it looks like the user is typing in some sort of home
         # directory path... (does pathlib let me test for this, or at
         # least ask what the home character is? Docs don't mention this;
         # so for now I'm going to hard-code this).
         if file_name.value.startswith( "~" ):
             # ...let's simply expand and go with that.
             try:
-                chosen = Path( file_name.value ).expanduser()
+                chosen = MakePath.of( file_name.value ).expanduser()
             except RuntimeError as error:
                 self._set_error( str( error ) )
                 return
         else:
             # It's not a home directory path, so let's combine with the
             # location of the directory navigator widget.
             chosen = (
```

## textual_fspicker/parts/directory_navigation.py

```diff
@@ -25,14 +25,15 @@
 from textual.widgets.option_list import Option
 from textual.worker              import get_current_worker
 
 ##############################################################################
 # Local imports.
 from ..safe_tests   import is_dir, is_file, is_symlink
 from ..path_filters import Filter
+from ..path_maker   import MakePath
 
 ##############################################################################
 class DirectoryEntryStyling( NamedTuple ):
     """Styling for directory entries."""
 
     hidden: Style
     """Styling for hidden entries."""
@@ -173,23 +174,23 @@
     DEFAULT_CSS = """
     DirectoryNavigation > .directory-navigation--hidden {
         color: $text-muted;
         text-style: italic;
     }
 
     DirectoryNavigation > .directory-navigation--name {
-        color: $text;
+        /*color: $text;*/
     }
 
     DirectoryNavigation > .directory-navigation--size {
-        color: $text;
+        /*color: $text;*/
     }
 
     DirectoryNavigation > .directory-navigation--time {
-        color: $text;
+        /*color: $text;*/
     }
     """
     """Default styling for the widget."""
 
     @dataclass
     class _BaseMessage( Message ):
         """Base class for directory navigation messages."""
@@ -200,27 +201,27 @@
     class Changed( _BaseMessage ):
         """Message sent when the current directory has changed."""
 
     @dataclass
     class _PathMessage( _BaseMessage ):
         """Base class for messages relating to a location in the filesystem."""
 
-        path: Path = Path()
+        path: Path = MakePath.of()
         """The path to the entry that was selected."""
 
     class Highlighted( _PathMessage ):
         """Message sent when an entry in the display is highlighted."""
 
     class Selected( _PathMessage ):
         """Message sent when an entry in the filesystem is selected."""
 
     class PermissionError( _PathMessage ):
         """Message sent when there's a permission problem with a path."""
 
-    _location: var[ Path ] = var[ Path ]( Path( "." ).absolute(), init=False )
+    _location: var[ Path ] = var[ Path ]( MakePath.of( "." ).absolute(), init=False )
     """The current location for the directory."""
 
     file_filter: var[ Filter | None ] = var[ Optional[ Filter ] ]( None )
     """The active file filter."""
 
     show_files: var[ bool ] = var( True )
     """Should files be shown and be selectable?"""
@@ -235,25 +236,25 @@
         """Initialise the directory navigation widget.
 
         Args:
             location: The starting location.
         """
         super().__init__()
         self._mounted                       = False
-        self.location                       = Path( "~" if location is None else location ).expanduser().absolute()
+        self.location                       = MakePath.of( "~" if location is None else location ).expanduser().absolute()
         self._entries: list[DirectoryEntry] = []
 
     @property
     def location( self ) -> Path:
         """The current location of the navigation widget."""
         return self._location
 
     @location.setter
     def location( self, new_location: Path | str ) -> None:
-        new_location = Path( new_location ).expanduser().absolute()
+        new_location = MakePath.of( new_location ).expanduser().absolute()
         if self._mounted:
             self._location = new_location
         else:
             self._initial_location = new_location
 
     def on_mount( self ) -> None:
         """Populate the widget once the DOM is ready."""
@@ -265,15 +266,15 @@
         if self.highlighted is None:
             self.highlighted = 0
 
     @property
     def is_root( self ) -> bool:
         """Are we at the root of the filesystem?"""
         # TODO: Worry about portability.
-        return self._location == Path( self._location.root )
+        return self._location == MakePath.of( self._location.root )
 
     @staticmethod
     def is_hidden( path: Path ) -> bool:
         """Does the given path appear to be hidden?
 
         Args:
             path: The path to test.
@@ -313,16 +314,16 @@
 
     @property
     def _styles( self ) -> DirectoryEntryStyling:
         """The styles to use for a directory entry."""
         return DirectoryEntryStyling(
             self.get_component_rich_style( "directory-navigation--hidden" ),
             self.get_component_rich_style( "directory-navigation--name", partial=True ),
-            self.get_component_rich_style( "directory-navigation--size", partial=True  ),
-            self.get_component_rich_style( "directory-navigation--time", partial=True  ),
+            self.get_component_rich_style( "directory-navigation--size", partial=True ),
+            self.get_component_rich_style( "directory-navigation--time", partial=True ),
         )
 
     def _repopulate_display( self ) -> None:
         """Repopulate the display of directories."""
         styles = self._styles
         with self.app.batch_update():
             self.clear_options()
```

## Comparing `textual_fspicker-0.0.5.dist-info/METADATA` & `textual_fspicker-0.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-fspicker
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple Textual filesystem picker dialog library.
 Home-page: https://github.com/davep/textual-fspicker
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
```

## Comparing `textual_fspicker-0.0.5.dist-info/RECORD` & `textual_fspicker-0.0.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-textual_fspicker/__init__.py,sha256=woJe61X2hsH2WcxTiV1GWghIMTfeuDze2IEPsu7Acgw,864
-textual_fspicker/__main__.py,sha256=zukQlivMgmarTkIjIm46sZOhCGcPPcaMy6lq8ZoF_kA,3154
+textual_fspicker/__init__.py,sha256=gGYXuCpn6zfg2Y4rFvVyu0BXnCBLsArJTQLgx9tvPaE,915
+textual_fspicker/__main__.py,sha256=IYU475b7ao-qLClpqYeRRMrjfQksNRaMTp-luNh7mr8,3254
 textual_fspicker/base_dialog.py,sha256=qDbghAxRYU1K8723w1YarQfPwIVkzs8BO5xcBmXK1ZA,4231
-textual_fspicker/file_dialog.py,sha256=MFgdmOGgSL8h4Z3RyaA02AIPKk58AkVHEVxBQaXdynU,5621
+textual_fspicker/file_dialog.py,sha256=0Jugxeqjc312D379Ag0xA11BU-tgA8ygiAi2tchhK3w,5682
 textual_fspicker/file_open.py,sha256=eMXpA1xOmYoOPSMEcefVsk_lc2xH7Nn-x-mEJhhdblY,1521
 textual_fspicker/file_save.py,sha256=WIE9rRUvb_UCntMw47Hjmbqnq2xr8u1oE7VPGJ3I7H8,1570
 textual_fspicker/path_filters.py,sha256=XpPrynKVI_p8Tf6tUuhEmU5lxAaf3TQlsjKsRwXC5nk,1822
+textual_fspicker/path_maker.py,sha256=1wYOQ9EQKYu8kZBqH7kYv-qwdUwIpkybvwkDaZkc6zw,1369
 textual_fspicker/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 textual_fspicker/safe_tests.py,sha256=U3gpqVRr7qcv7mqF-I_sFojtr9Pv5JyqFzAxGG7qofA,2174
 textual_fspicker/select_directory.py,sha256=vE1MYCL-_QqTyPiveJrxl90oEwjQB14lfSsHteUEBNM,2457
 textual_fspicker/parts/__init__.py,sha256=vjP1jzd5ty4IhwUZnVFkOjzctZn22EbwWDHh_16x-GM,389
-textual_fspicker/parts/directory_navigation.py,sha256=6jg6mBcBbVsH7DcimhsF2XKpwXqWBaVb4f2xx5G9mm0,15053
-textual_fspicker-0.0.5.dist-info/METADATA,sha256=wrIXnKgsbJ6gnjhedQ1CRpdABcnvZ7F-hsQZ58pFQbo,4235
-textual_fspicker-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-textual_fspicker-0.0.5.dist-info/top_level.txt,sha256=htFx3DXug_utI8h7tIJmd3FSxg6-fjXfcf4_Rd6ohLQ,17
-textual_fspicker-0.0.5.dist-info/RECORD,,
+textual_fspicker/parts/directory_navigation.py,sha256=qP_KCRFnOe4o6BsdrXnMZMizZN_WqkwljpzfgDsk5ck,15134
+textual_fspicker-0.0.6.dist-info/METADATA,sha256=GCxia7iJhcT2KAbT6dJX_nGtIZUcX8GdiRA4w1rZ5UQ,4235
+textual_fspicker-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+textual_fspicker-0.0.6.dist-info/top_level.txt,sha256=htFx3DXug_utI8h7tIJmd3FSxg6-fjXfcf4_Rd6ohLQ,17
+textual_fspicker-0.0.6.dist-info/RECORD,,
```

