# Comparing `tmp/rico-0.0.6.tar.gz` & `tmp/rico-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rico-0.0.6.tar", last modified: Sun May 28 13:40:17 2023, max compression
+gzip compressed data, was "rico-0.1.0.tar", last modified: Sat Jun  3 18:31:56 2023, max compression
```

## Comparing `rico-0.0.6.tar` & `rico-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-05-28 13:39:52.898590 rico-0.0.6/LICENSE
--rw-r--r--   0        0        0      715 2023-05-28 13:39:52.898590 rico-0.0.6/README.md
--rw-r--r--   0        0        0     2818 2023-05-28 13:40:17.066776 rico-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      454 2023-05-28 13:39:52.898590 rico-0.0.6/src/rico/__init__.py
--rw-r--r--   0        0        0     2166 2023-05-28 13:39:52.898590 rico-0.0.6/src/rico/_config.py
--rw-r--r--   0        0        0    14582 2023-05-28 13:39:52.898590 rico-0.0.6/src/rico/_content.py
--rw-r--r--   0        0        0     7012 2023-05-28 13:39:52.898590 rico-0.0.6/src/rico/_html.py
--rw-r--r--   0        0        0      340 2023-05-28 13:39:52.898590 rico-0.0.6/src/rico/_version.py
--rw-r--r--   0        0        0       18 2023-05-28 13:39:52.898590 rico-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     1476 2023-05-28 13:39:52.898590 rico-0.0.6/tests/test__config.py
--rw-r--r--   0        0        0    17176 2023-05-28 13:39:52.898590 rico-0.0.6/tests/test__content.py
--rw-r--r--   0        0        0     9491 2023-05-28 13:39:52.898590 rico-0.0.6/tests/test__html.py
--rw-r--r--   0        0        0      730 2023-05-28 13:39:52.898590 rico-0.0.6/tests/test__version.py
--rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 rico-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-03 18:30:57.625474 rico-0.1.0/LICENSE
+-rw-r--r--   0        0        0      706 2023-06-03 18:30:57.625474 rico-0.1.0/README.md
+-rw-r--r--   0        0        0     2870 2023-06-03 18:31:56.350493 rico-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      585 2023-06-03 18:30:57.625474 rico-0.1.0/src/rico/__init__.py
+-rw-r--r--   0        0        0     4384 2023-06-03 18:30:57.625474 rico-0.1.0/src/rico/_config.py
+-rw-r--r--   0        0        0     5751 2023-06-03 18:30:57.625474 rico-0.1.0/src/rico/_container.py
+-rw-r--r--   0        0        0    14615 2023-06-03 18:30:57.625474 rico-0.1.0/src/rico/_content.py
+-rw-r--r--   0        0        0     7012 2023-06-03 18:30:57.625474 rico-0.1.0/src/rico/_html.py
+-rw-r--r--   0        0        0      340 2023-06-03 18:30:57.625474 rico-0.1.0/src/rico/_version.py
+-rw-r--r--   0        0        0       18 2023-06-03 18:30:57.625474 rico-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1476 2023-06-03 18:30:57.625474 rico-0.1.0/tests/test__config.py
+-rw-r--r--   0        0        0    10237 2023-06-03 18:30:57.625474 rico-0.1.0/tests/test__container.py
+-rw-r--r--   0        0        0    17190 2023-06-03 18:30:57.625474 rico-0.1.0/tests/test__content.py
+-rw-r--r--   0        0        0     9491 2023-06-03 18:30:57.625474 rico-0.1.0/tests/test__html.py
+-rw-r--r--   0        0        0      730 2023-06-03 18:30:57.625474 rico-0.1.0/tests/test__version.py
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 rico-0.1.0/PKG-INFO
```

### Comparing `rico-0.0.6/LICENSE` & `rico-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rico-0.0.6/README.md` & `rico-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-# rico
-Rich content to HTML as easy as Doc([df, plot]).
-
-<br>
-
 [![CI](https://github.com/e10v/rico/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/e10v/rico/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/github/e10v/rico/coverage.svg?branch=main)](https://codecov.io/gh/e10v/rico)
 [![License](https://img.shields.io/github/license/e10v/rico)](https://github.com/e10v/rico/blob/main/LICENSE)
 [![Version](https://img.shields.io/pypi/v/rico.svg)](https://pypi.org/project/rico/)
 [![Package Status](https://img.shields.io/pypi/status/rico.svg)](https://pypi.org/project/rico/)
-[![PyPI Python Versions](https://img.shields.io/pypi/pyversions/rico.svg)](https://pypi.python.org/pypi/rico/)
+[![PyPI Python Versions](https://img.shields.io/pypi/pyversions/rico.svg)](https://pypi.org/project/rico/)
+
+# rico
+
+Rich content to HTML as easy as `Doc(df, plot)`.
```

### Comparing `rico-0.0.6/pyproject.toml` & `rico-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 [project]
 name = "rico"
 dynamic = []
-description = "Rich content to HTML as easy as Doc([df, plot])."
+description = "Rich content to HTML as easy as Doc(df, plot)."
 authors = [
     { name = "Evgeny Ivanov", email = "ivanov.evgeny.n@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Text Processing",
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: HTML",
     "Topic :: Text Processing :: Markup :: Markdown",
 ]
-version = "0.0.6"
+version = "0.1.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 source = "https://github.com/e10v/rico"
+"release notes" = "https://github.com/e10v/rico/releases"
 
 [project.optional-dependencies]
 altair = [
     "altair>=4.2",
     "vl-convert-python>=0.8",
 ]
 markdown = [
```

### Comparing `rico-0.0.6/src/rico/_content.py` & `rico-0.1.0/src/rico/_content.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     Attributes:
         container (Element): The container element.
     """
     container: ET.Element
 
     def __init__(self, class_: str | None = None):
-        """Initialize base content.
+        """Create base content.
 
         Args:
             class_: The container element's class attribute.
         """
         attrib = {"class": class_} if class_ is not None else {}
         self.container = ET.Element("div", attrib=attrib)
 
@@ -96,15 +96,15 @@
         tag: str,
         text: str | None = None,
         tail: str | None = None,
         attrib: dict[str, Any] = {},
         class_: str | None = None,
         **extra: Any,
     ):
-        """Initialize content using tag parameters.
+        """Create content using tag parameters.
 
         Args:
             tag: The content element's tag.
             text: Text before first subelement.
             tail: Text after the end tag.
             attrib: The tag's attributes.
             extra: Extra attributes.
@@ -125,15 +125,15 @@
     def __init__(
         self,
         obj: Any,
         mono: bool = False,
         wrap: bool = False,
         class_: str | None = None,
     ):
-        """Initialize content from a text.
+        """Create content from a text.
 
         The default tag is <p> unless the text contains a line break.
         Then the <pre> tag is used.
 
         The `mono` and `wrap` parameters rely on Bootstrap CSS.
 
         Args:
@@ -162,15 +162,15 @@
 
 class Code(ContentBase):
     """A Code content definition.
 
     Creates content elements from a code and appends them to the container.
     """
     def __init__(self, text: str, class_: str | None = None):
-        """Initialize content from a code.
+        """Create content from a code.
 
         Args:
             text: The code.
             class_: The container class attribute.
         """
         super().__init__(class_)
         pre = ET.Element("pre")
@@ -187,15 +187,15 @@
     """
     def __init__(
         self,
         text: str,
         strip_dataframe_borders: bool = False,
         class_: str | None = None,
     ):
-        """Initialize content from an HTML text.
+        """Create content from an HTML text.
 
         Args:
             text: The HTML text.
             strip_dataframe_borders: Delete borders attributes from dataframes.
             class_: The container class attribute.
         """
         super().__init__(class_)
@@ -217,15 +217,15 @@
     """
     def __init__(
         self,
         text: str,
         class_: str | None = None,
         **kwargs: Any,
     ):
-        """Initialize content from a markdown text.
+        """Create content from a markdown text.
 
         Args:
             text: The markdown text.
             class_: The container class attribute.
             **kwargs: Keyword arguments passed to the `markdown.markdown` function.
 
         Raises:
@@ -242,29 +242,26 @@
     """An Image content definition.
 
     Creates content elements using an image data and appends them to the container.
     """
     def __init__(
         self,
         data: bytes | str,
-        format: str | None = None,  # noqa: A002
+        format: str,  # noqa: A002
         class_: str | None = None,
     ):
-        """Initialize content using image data.
+        """Create content using image data.
 
         Args:
             data: The image data.
             format: The image format.
             class_: The container class attribute.
         """
         super().__init__(class_)
 
-        if format is None:
-            format = rico._config.get_config("image_format")  # noqa: A001
-
         if format == "svg":
             if isinstance(data, bytes):
                 data = data.decode()
 
             for element in rico._html.parse_html(data):
                 self.container.append(element)
         else:
@@ -292,29 +289,29 @@
     def __init__(
         self,
         obj: Any,
         format: Literal["svg", "png"] | None = None,  # noqa: A002
         class_: str | None = None,
         **kwargs: Any,
     ):
-        """Initialize content from a chart object.
+        """Create content from a chart object.
 
         Args:
             obj: The chart object.
             format: The image format.
             class_: The container class attribute.
             **kwargs: Keyword arguments passed to a function
                 which converts object to an image.
 
         Raises:
             TypeError: Chart type is not supported
                 or required extra package is not installed.
         """
         if format is None:
-            format = rico._config.get_config("chart_format")  # noqa: A001
+            format = rico._config.get_config("image_format")  # noqa: A001
 
         if plt is not None and isinstance(obj, plt.Axes):
             obj = obj.figure
 
         if plt is not None and isinstance(obj, plt.Figure):  # type: ignore
             stream = io.StringIO() if format == "svg" else io.BytesIO()
             obj.savefig(stream, format=format, **kwargs)
@@ -345,15 +342,15 @@
     """An arbitrary content definition.
 
     Creates content elements from arbitrary objects and appends them to the container.
 
     Automatically determines the content type.
     """
     def __init__(self, *objects: Any, class_: str | None = None):
-        """Initialize content from arbitrary objects.
+        """Create content from arbitrary objects.
 
         Args:
             *objects: The objects which are used to create a content.
             class_: The container class attribute.
         """
         super().__init__(class_=class_)
         for obj in objects:
@@ -383,20 +380,20 @@
     script: ET.Element
     footer: bool = False
 
     def __init__(
         self,
         text: str | None = None,
         src: str | None = None,
-        inline: bool = False,
+        inline: bool | None = None,
         defer: bool = False,
         attrib: dict[str, Any] = {},
         **extra: Any,
     ):
-        """Initialize script.
+        """Create script.
 
         Either `text` or `src` should be used.
 
         Args:
             text: The script text.
             src: The script source link.
             inline: If True, load script inline, downdload it from source link
@@ -406,14 +403,17 @@
             attrib: The script attributes.
             **extra: Extra attributes.
 
         Raises:
             ValueError: Both text and src are not None.
             ValueError: Both text and src are None.
         """
+        if inline is None:
+            inline = rico._config.get_config("inline_scripts")
+
         if text is not None and src is not None:
             raise ValueError("Either `text` or `src` should be None.")
 
         if text is None and src is None:
             raise ValueError("Either `text` or `src` should be not None.")
 
         if inline and src is not None:
@@ -441,19 +441,19 @@
     """
     style: ET.Element
 
     def __init__(
         self,
         text: str | None = None,
         src: str | None = None,
-        inline: bool = False,
+        inline: bool | None = None,
         attrib: dict[str, Any] = {},
         **extra: Any,
     ):
-        """Initialize stylesheet.
+        """Create stylesheet.
 
         Either `text` or `src` should be used.
 
         Args:
             text: The stylesheet text.
             src: The stylesheet source link.
             inline: If True, load stylesheet inline, downdload it from source link
@@ -461,14 +461,17 @@
             attrib: The stylesheet attributes.
             **extra: Extra attributes.
 
         Raises:
             ValueError: Both text and src are not None.
             ValueError: Both text and src are None.
         """
+        if inline is None:
+            inline = rico._config.get_config("inline_scripts")
+
         if text is not None and src is not None:
             raise ValueError("Either `text` or `src` should be None.")
 
         if text is None and src is None:
             raise ValueError("Either `text` or `src` should be not None.")
 
         if inline and src is not None:
```

### Comparing `rico-0.0.6/src/rico/_html.py` & `rico-0.1.0/src/rico/_html.py`

 * *Files identical despite different names*

### Comparing `rico-0.0.6/tests/test__config.py` & `rico-0.1.0/tests/test__config.py`

 * *Files identical despite different names*

### Comparing `rico-0.0.6/tests/test__content.py` & `rico-0.1.0/tests/test__content.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
     'width="16" height="16" fill="currentColor" class="bi bi-dash">'
     '<path d="M4 8a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7A.5.5 0 0 1 4 8z"/>'
     "</svg>"
 )
 
 @pytest.mark.parametrize("data", [svg_data, svg_data.encode()], ids=["str", "bytes"])
 def test_image_svg(data: str | bytes):
-    content = rico._content.Image(data, class_="row")
+    content = rico._content.Image(data, format="svg", class_="row")
 
     div = content.container
     assert isinstance(div, ET.Element)
     assert div.tag == "div"
     assert div.attrib == {"class": "row"}
     assert div.text is None
     assert div.tail is None
```

### Comparing `rico-0.0.6/tests/test__html.py` & `rico-0.1.0/tests/test__html.py`

 * *Files identical despite different names*

### Comparing `rico-0.0.6/tests/test__version.py` & `rico-0.1.0/tests/test__version.py`

 * *Files identical despite different names*

### Comparing `rico-0.0.6/PKG-INFO` & `rico-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: rico
-Version: 0.0.6
-Summary: Rich content to HTML as easy as Doc([df, plot]).
+Version: 0.1.0
+Summary: Rich content to HTML as easy as Doc(df, plot).
 Author-Email: Evgeny Ivanov <ivanov.evgeny.n@gmail.com>
 License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Project-URL: Source, https://github.com/e10v/rico
+Project-URL: Release notes, https://github.com/e10v/rico/releases
 Requires-Python: >=3.10
 Provides-Extra: altair
 Provides-Extra: markdown
 Provides-Extra: pyplot
 Provides-Extra: seaborn
 Provides-Extra: complete
 Requires-Dist: altair>=4.2; extra == "altair"
 Requires-Dist: vl-convert-python>=0.8; extra == "altair"
 Requires-Dist: markdown>=3.3; extra == "markdown"
 Requires-Dist: matplotlib>=3.5; extra == "pyplot"
 Requires-Dist: seaborn>=0.12; extra == "seaborn"
 Requires-Dist: rico[altair,markdown,pyplot,seaborn]; extra == "complete"
 Description-Content-Type: text/markdown
 
-# rico
-Rich content to HTML as easy as Doc([df, plot]).
-
-<br>
-
 [![CI](https://github.com/e10v/rico/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/e10v/rico/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/github/e10v/rico/coverage.svg?branch=main)](https://codecov.io/gh/e10v/rico)
 [![License](https://img.shields.io/github/license/e10v/rico)](https://github.com/e10v/rico/blob/main/LICENSE)
 [![Version](https://img.shields.io/pypi/v/rico.svg)](https://pypi.org/project/rico/)
 [![Package Status](https://img.shields.io/pypi/status/rico.svg)](https://pypi.org/project/rico/)
-[![PyPI Python Versions](https://img.shields.io/pypi/pyversions/rico.svg)](https://pypi.python.org/pypi/rico/)
+[![PyPI Python Versions](https://img.shields.io/pypi/pyversions/rico.svg)](https://pypi.org/project/rico/)
+
+# rico
+
+Rich content to HTML as easy as `Doc(df, plot)`.
```

