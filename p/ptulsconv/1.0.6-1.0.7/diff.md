# Comparing `tmp/ptulsconv-1.0.6.tar.gz` & `tmp/ptulsconv-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptulsconv-1.0.6.tar", last modified: Tue Feb 28 18:55:03 2023, max compression
+gzip compressed data, was "ptulsconv-1.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ptulsconv-1.0.6.tar` & `ptulsconv-1.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1068 2023-02-28 18:54:45.736191 ptulsconv-1.0.6/LICENSE
--rw-r--r--   0        0        0     1241 2023-02-28 18:54:45.736191 ptulsconv-1.0.6/README.md
--rw-r--r--   0        0        0      222 2023-02-28 18:54:45.820192 ptulsconv-1.0.6/ptulsconv/__init__.py
--rw-r--r--   0        0        0     3929 2023-02-28 18:54:45.820192 ptulsconv-1.0.6/ptulsconv/__main__.py
--rw-r--r--   0        0        0     4130 2023-02-28 18:54:45.820192 ptulsconv-1.0.6/ptulsconv/broadcast_timecode.py
--rw-r--r--   0        0        0     8579 2023-02-28 18:54:45.820192 ptulsconv-1.0.6/ptulsconv/commands.py
--rw-r--r--   0        0        0       67 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/docparser/__init__.py
--rw-r--r--   0        0        0     4539 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/docparser/adr_entity.py
--rw-r--r--   0        0        0     5622 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/docparser/doc_entity.py
--rw-r--r--   0        0        0       34 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/docparser/generic_entity.py
--rw-r--r--   0        0        0     9996 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/docparser/pt_doc_parser.py
--rw-r--r--   0        0        0     8007 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/docparser/tag_compiler.py
--rw-r--r--   0        0        0     2922 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/docparser/tag_mapping.py
--rw-r--r--   0        0        0     2842 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/docparser/tagged_string_parser_visitor.py
--rw-r--r--   0        0        0      756 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/footage.py
--rw-r--r--   0        0        0      462 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/movie_export.py
--rw-r--r--   0        0        0    11941 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/pdf/__init__.py
--rw-r--r--   0        0        0     2075 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/pdf/continuity.py
--rw-r--r--   0        0        0    10181 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/pdf/line_count.py
--rw-r--r--   0        0        0       90 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/pdf/recordist_log.py
--rw-r--r--   0        0        0     5668 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/pdf/summary_log.py
--rw-r--r--   0        0        0    10063 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/pdf/supervisor_1pg.py
--rw-r--r--   0        0        0     2954 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/pdf/talent_sides.py
--rw-r--r--   0        0        0     2186 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/reporting.py
--rw-r--r--   0        0        0     2616 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/validations.py
--rw-r--r--   0        0        0     5494 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/xml/common.py
--rw-r--r--   0        0        0     3275 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/xslt/AvidMarkers.xsl
--rw-r--r--   0        0        0     1529 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/ptulsconv/xslt/SRT.xsl
--rw-r--r--   0        0        0     1225 2023-02-28 18:54:45.824192 ptulsconv-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     2396 1970-01-01 00:00:00.000000 ptulsconv-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-03 02:45:27.925497 ptulsconv-1.0.7/LICENSE
+-rw-r--r--   0        0        0     1241 2023-06-03 02:45:27.925497 ptulsconv-1.0.7/README.md
+-rw-r--r--   0        0        0      216 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/__init__.py
+-rw-r--r--   0        0        0     3930 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/__main__.py
+-rw-r--r--   0        0        0     4130 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/broadcast_timecode.py
+-rw-r--r--   0        0        0     8579 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/commands.py
+-rw-r--r--   0        0        0       67 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/__init__.py
+-rw-r--r--   0        0        0     4539 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/adr_entity.py
+-rw-r--r--   0        0        0     5622 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/doc_entity.py
+-rw-r--r--   0        0        0       34 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/generic_entity.py
+-rw-r--r--   0        0        0     9996 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/pt_doc_parser.py
+-rw-r--r--   0        0        0     8007 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/tag_compiler.py
+-rw-r--r--   0        0        0     2922 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/tag_mapping.py
+-rw-r--r--   0        0        0     2842 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/docparser/tagged_string_parser_visitor.py
+-rw-r--r--   0        0        0      756 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/footage.py
+-rw-r--r--   0        0        0      462 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/movie_export.py
+-rw-r--r--   0        0        0    11941 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/pdf/__init__.py
+-rw-r--r--   0        0        0     2075 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/pdf/continuity.py
+-rw-r--r--   0        0        0    10181 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/pdf/line_count.py
+-rw-r--r--   0        0        0       90 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/pdf/recordist_log.py
+-rw-r--r--   0        0        0     5668 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/pdf/summary_log.py
+-rw-r--r--   0        0        0    10063 2023-06-03 02:45:28.033499 ptulsconv-1.0.7/ptulsconv/pdf/supervisor_1pg.py
+-rw-r--r--   0        0        0     2954 2023-06-03 02:45:28.037499 ptulsconv-1.0.7/ptulsconv/pdf/talent_sides.py
+-rw-r--r--   0        0        0     2186 2023-06-03 02:45:28.037499 ptulsconv-1.0.7/ptulsconv/reporting.py
+-rw-r--r--   0        0        0     2616 2023-06-03 02:45:28.037499 ptulsconv-1.0.7/ptulsconv/validations.py
+-rw-r--r--   0        0        0     5494 2023-06-03 02:45:28.037499 ptulsconv-1.0.7/ptulsconv/xml/common.py
+-rw-r--r--   0        0        0     3275 2023-06-03 02:45:28.037499 ptulsconv-1.0.7/ptulsconv/xslt/AvidMarkers.xsl
+-rw-r--r--   0        0        0     1529 2023-06-03 02:45:28.037499 ptulsconv-1.0.7/ptulsconv/xslt/SRT.xsl
+-rw-r--r--   0        0        0     1347 2023-06-03 02:45:28.037499 ptulsconv-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2396 1970-01-01 00:00:00.000000 ptulsconv-1.0.7/PKG-INFO
```

### Comparing `ptulsconv-1.0.6/LICENSE` & `ptulsconv-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/README.md` & `ptulsconv-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/__main__.py` & `ptulsconv-1.0.7/ptulsconv/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from optparse import OptionParser, OptionGroup
 import datetime
 import sys
 
-from ptulsconv import __name__, __version__, __author__,__copyright__
+from ptulsconv import __name__, __version__, __author__, __copyright__
 from ptulsconv.commands import convert
 from ptulsconv.reporting import print_status_style, print_banner_style, print_section_header_style, print_fatal_error
 
 
 def dump_field_map(output=sys.stdout):
     from ptulsconv.docparser.tag_mapping import TagMapping
     from ptulsconv.docparser.adr_entity import ADRLine, GenericEvent
```

### Comparing `ptulsconv-1.0.6/ptulsconv/broadcast_timecode.py` & `ptulsconv-1.0.7/ptulsconv/broadcast_timecode.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/commands.py` & `ptulsconv-1.0.7/ptulsconv/commands.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/docparser/adr_entity.py` & `ptulsconv-1.0.7/ptulsconv/docparser/adr_entity.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/docparser/doc_entity.py` & `ptulsconv-1.0.7/ptulsconv/docparser/doc_entity.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/docparser/pt_doc_parser.py` & `ptulsconv-1.0.7/ptulsconv/docparser/pt_doc_parser.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/docparser/tag_compiler.py` & `ptulsconv-1.0.7/ptulsconv/docparser/tag_compiler.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/docparser/tag_mapping.py` & `ptulsconv-1.0.7/ptulsconv/docparser/tag_mapping.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/docparser/tagged_string_parser_visitor.py` & `ptulsconv-1.0.7/ptulsconv/docparser/tagged_string_parser_visitor.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/footage.py` & `ptulsconv-1.0.7/ptulsconv/footage.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/pdf/__init__.py` & `ptulsconv-1.0.7/ptulsconv/pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/pdf/continuity.py` & `ptulsconv-1.0.7/ptulsconv/pdf/continuity.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/pdf/line_count.py` & `ptulsconv-1.0.7/ptulsconv/pdf/line_count.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/pdf/summary_log.py` & `ptulsconv-1.0.7/ptulsconv/pdf/summary_log.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/pdf/supervisor_1pg.py` & `ptulsconv-1.0.7/ptulsconv/pdf/supervisor_1pg.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/pdf/talent_sides.py` & `ptulsconv-1.0.7/ptulsconv/pdf/talent_sides.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/reporting.py` & `ptulsconv-1.0.7/ptulsconv/reporting.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/validations.py` & `ptulsconv-1.0.7/ptulsconv/validations.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/xml/common.py` & `ptulsconv-1.0.7/ptulsconv/xml/common.py`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/xslt/AvidMarkers.xsl` & `ptulsconv-1.0.7/ptulsconv/xslt/AvidMarkers.xsl`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/ptulsconv/xslt/SRT.xsl` & `ptulsconv-1.0.7/ptulsconv/xslt/SRT.xsl`

 * *Files identical despite different names*

### Comparing `ptulsconv-1.0.6/pyproject.toml` & `ptulsconv-1.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,20 @@
 
 [project.optional-dependencies]
 doc = [
     "Sphinx ~= 5.3.0",
     "sphinx-rtd-theme >= 1.1.1"
 ]
 
+[tool.flit.module]
+name = "ptulsconv"
+
 [project.scripts]
-flit = "ptulsconv.__main__:main"
+ptulsconv = "ptulsconv.__main__:main"
 
+[project.entry_points.console_scripts]
+ptulsconv = 'ptulsconv.__main__:main'
 
 [project.urls]
 Source = 'https://github.com/iluvcapra/ptulsconv'
 Issues = 'https://github.com/iluvcapra/ptulsconv/issues'
-Documentation = 'https://ptulsconv.readthedocs.io/'
+Documentation = 'https://ptulsconv.readthedocs.io/'
```

### Comparing `ptulsconv-1.0.6/PKG-INFO` & `ptulsconv-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptulsconv
-Version: 1.0.6
+Version: 1.0.7
 Summary: Parse and convert Pro Tools text exports
 Keywords: text-processing,parsers,film,broadcast,editing,editorial
 Author-email: Jamie Hardt <jamiehardt@me.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia
```

