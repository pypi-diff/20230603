# Comparing `tmp/lagrange-2.0.2.tar.gz` & `tmp/lagrange-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lagrange-2.0.2.tar", last modified: Sun Jul 31 19:20:02 2022, max compression
+gzip compressed data, was "lagrange-2.1.0.tar", last modified: Sat Jun  3 15:06:09 2023, max compression
```

## Comparing `lagrange-2.0.2.tar` & `lagrange-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-07-31 19:20:02.667564 lagrange-2.0.2/
--rw-rw-rw-   0        0        0     1091 2022-06-13 22:32:24.000000 lagrange-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     5572 2022-07-31 19:20:02.667564 lagrange-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5043 2022-07-24 05:18:34.000000 lagrange-2.0.2/README.rst
--rw-rw-rw-   0        0        0      975 2022-07-31 18:15:08.000000 lagrange-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-07-31 19:20:02.667564 lagrange-2.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-07-31 19:20:02.657462 lagrange-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2022-07-31 19:20:02.662690 lagrange-2.0.2/src/lagrange/
--rw-rw-rw-   0        0        0      100 2022-06-13 22:32:24.000000 lagrange-2.0.2/src/lagrange/__init__.py
--rw-rw-rw-   0        0        0     9002 2022-07-31 18:18:11.000000 lagrange-2.0.2/src/lagrange/lagrange.py
-drwxrwxrwx   0        0        0        0 2022-07-31 19:20:02.667564 lagrange-2.0.2/src/lagrange.egg-info/
--rw-rw-rw-   0        0        0     5572 2022-07-31 19:20:02.000000 lagrange-2.0.2/src/lagrange.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2022-07-31 19:20:02.000000 lagrange-2.0.2/src/lagrange.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-31 19:20:02.000000 lagrange-2.0.2/src/lagrange.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2022-07-31 19:20:02.000000 lagrange-2.0.2/src/lagrange.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-07-31 19:20:02.000000 lagrange-2.0.2/src/lagrange.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 15:06:09.445938 lagrange-2.1.0/
+-rw-rw-rw-   0        0        0     1091 2022-06-13 22:32:24.000000 lagrange-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5857 2023-06-03 15:06:09.445938 lagrange-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5328 2023-06-03 14:58:22.000000 lagrange-2.1.0/README.rst
+-rw-rw-rw-   0        0        0      976 2023-06-03 15:00:15.000000 lagrange-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 15:06:09.445938 lagrange-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-03 15:06:09.432266 lagrange-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 15:06:09.436432 lagrange-2.1.0/src/lagrange/
+-rw-rw-rw-   0        0        0      100 2022-06-13 22:32:24.000000 lagrange-2.1.0/src/lagrange/__init__.py
+-rw-rw-rw-   0        0        0     9000 2023-06-03 14:51:49.000000 lagrange-2.1.0/src/lagrange/lagrange.py
+drwxrwxrwx   0        0        0        0 2023-06-03 15:06:09.445938 lagrange-2.1.0/src/lagrange.egg-info/
+-rw-rw-rw-   0        0        0     5857 2023-06-03 15:06:09.000000 lagrange-2.1.0/src/lagrange.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-03 15:06:09.000000 lagrange-2.1.0/src/lagrange.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 15:06:09.000000 lagrange-2.1.0/src/lagrange.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      215 2023-06-03 15:06:09.000000 lagrange-2.1.0/src/lagrange.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 15:06:09.000000 lagrange-2.1.0/src/lagrange.egg-info/top_level.txt
```

### Comparing `lagrange-2.0.2/LICENSE` & `lagrange-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lagrange-2.0.2/PKG-INFO` & `lagrange-2.1.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: lagrange
-Version: 2.0.2
-Summary: Pure-Python implementation of Lagrange interpolation over finite fields.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/lapets/lagrange
-Project-URL: Documentation, https://lagrange.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
 ========
 lagrange
 ========
 
 Pure-Python implementation of Lagrange interpolation over finite fields.
 
 |pypi| |readthedocs| |actions| |coveralls|
@@ -42,25 +24,31 @@
 
 Purpose
 -------
 This library provides a pure-Python implementation of the `Lagrange interpolation <https://en.wikipedia.org/wiki/Lagrange_polynomial>`__ algorithm over finite fields.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/lagrange>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/lagrange>`__:
+
+.. code-block:: bash
 
     python -m pip install lagrange
 
-The library can be imported in the usual way::
+The library can be imported in the usual way:
+
+.. code-block:: python
 
     from lagrange import lagrange
 
 Examples
 ^^^^^^^^
-Interpolation can be performed on collections of points represented in a variety of ways::
+Interpolation can be performed on collections of points represented in a variety of ways:
+
+.. code-block:: python
 
     >>> lagrange({1: 15, 2: 9, 3: 3}, 17)
     4
     >>> lagrange([(1, 15), (2, 9), (3, 3)], 17)
     4
     >>> lagrange([15, 9, 3], 17)
     4
@@ -74,62 +62,80 @@
         [119182, 11988467, 6052427, 8694701, 9050123, 3676518,\
          558333, 12198248, 7344866, 10114014, 2239291, 2515398],\
         15485867)
     123
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/lagrange/lagrange.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/lagrange
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/lagrange>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/lagrange>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/lagrange>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

### Comparing `lagrange-2.0.2/pyproject.toml` & `lagrange-2.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lagrange"
-version = "2.0.2"
+version = "2.1.0"
 description = "Pure-Python implementation of Lagrange interpolation over finite fields."
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
     {email = "a@lapets.io"}
 ]
 readme = "README.rst"
@@ -18,29 +18,29 @@
 docs = [
     "toml~=0.10.2",
     "sphinx~=4.2.0",
     "sphinx-rtd-theme~=1.0.0",
     "sphinx-autodoc-typehints~=1.12.0"
 ]
 test = [
-    "pytest~=7.0",
-    "pytest-cov~=3.0"
+    "pytest~=7.2",
+    "pytest-cov~=4.0"
 ]
 lint = [
-    "pylint~=2.14.0"
+    "pylint~=2.17.0"
 ]
 coveralls = [
     "coveralls~=3.3.1"
 ]
 publish = [
-    "build~=0.8",
+    "build~=0.10",
     "twine~=4.0"
 ]
 
 [build-system]
 requires = [
-    "setuptools~=62.0"
+    "setuptools~=67.6"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --ignore=docs --cov=lagrange --cov-report term-missing"
```

### Comparing `lagrange-2.0.2/src/lagrange/lagrange.py` & `lagrange-2.1.0/src/lagrange/lagrange.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Pure-Python implementation of Lagrange interpolation over finite fields.
 """
 from __future__ import annotations
-from functools import reduce
 from typing import Union, Optional, Sequence, Iterable
 import doctest
 import collections.abc
+import functools
 import itertools
 
 def _inv(a: int, prime: int) -> int:
     """
     Compute multiplicative inverse modulo a prime.
     """
     return pow(a, prime - 2, prime)
@@ -225,15 +225,15 @@
     # Field arithmetic helper functions.
     mul = lambda a, b: (a % modulus) * b % modulus # pylint: disable=unnecessary-lambda-assignment
     div = lambda a, b: mul(a, _inv(b, modulus)) # pylint: disable=unnecessary-lambda-assignment
 
     # Compute the value of each unique Lagrange basis polynomial at ``0``,
     # then sum them all up to get the resulting value at ``0``.
     return sum(
-        reduce(
+        functools.reduce(
             mul,
             itertools.chain([values[x]], (
                 # Extrapolate using the fact that *y* = ``1`` if
                 # ``x`` = ``x_known``, and *y* = ``0`` for the other
                 # known values in the domain.
                 div(0 - x_known, x - x_known)
                 for x_known in xs if x_known is not x
```

### Comparing `lagrange-2.0.2/src/lagrange.egg-info/PKG-INFO` & `lagrange-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lagrange
-Version: 2.0.2
+Version: 2.1.0
 Summary: Pure-Python implementation of Lagrange interpolation over finite fields.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/lapets/lagrange
 Project-URL: Documentation, https://lagrange.readthedocs.io
 Requires-Python: >=3.7
@@ -42,25 +42,31 @@
 
 Purpose
 -------
 This library provides a pure-Python implementation of the `Lagrange interpolation <https://en.wikipedia.org/wiki/Lagrange_polynomial>`__ algorithm over finite fields.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/lagrange>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/lagrange>`__:
+
+.. code-block:: bash
 
     python -m pip install lagrange
 
-The library can be imported in the usual way::
+The library can be imported in the usual way:
+
+.. code-block:: python
 
     from lagrange import lagrange
 
 Examples
 ^^^^^^^^
-Interpolation can be performed on collections of points represented in a variety of ways::
+Interpolation can be performed on collections of points represented in a variety of ways:
+
+.. code-block:: python
 
     >>> lagrange({1: 15, 2: 9, 3: 3}, 17)
     4
     >>> lagrange([(1, 15), (2, 9), (3, 3)], 17)
     4
     >>> lagrange([15, 9, 3], 17)
     4
@@ -74,62 +80,80 @@
         [119182, 11988467, 6052427, 8694701, 9050123, 3676518,\
          558333, 12198248, 7344866, 10114014, 2239291, 2515398],\
         15485867)
     123
 
 Development
 -----------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs,lint]
 
 Documentation
 ^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
 
     python -m pip install .[docs]
     cd docs
     sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
 
 Testing and Conventions
 ^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
 
     python -m pip install .[test]
     python -m pytest
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/lagrange/lagrange.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/lagrange
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/lagrange>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/lagrange>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/lagrange>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
 
     python -m pip install .[publish]
 
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
 
     git tag ?.?.?
     git push origin ?.?.?
 
-Remove any old build/distribution files. Then, package the source into a distribution archive::
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
 
     rm -rf build dist src/*.egg-info
     python -m build --sdist --wheel .
 
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
 
     python -m twine upload dist/*
```

