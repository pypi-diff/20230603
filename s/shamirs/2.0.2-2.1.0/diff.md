# Comparing `tmp/shamirs-2.0.2.tar.gz` & `tmp/shamirs-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shamirs-2.0.2.tar", last modified: Sun Jul 31 19:22:39 2022, max compression
+gzip compressed data, was "shamirs-2.1.0.tar", last modified: Sat Jun  3 17:52:20 2023, max compression
```

## Comparing `shamirs-2.0.2.tar` & `shamirs-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-07-31 19:22:39.490382 shamirs-2.0.2/
--rw-rw-rw-   0        0        0     1091 2022-06-17 22:55:54.000000 shamirs-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     6239 2022-07-31 19:22:39.490382 shamirs-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5716 2022-07-24 05:57:50.000000 shamirs-2.0.2/README.rst
--rw-rw-rw-   0        0        0     1035 2022-07-31 18:23:19.000000 shamirs-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-07-31 19:22:39.490382 shamirs-2.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-07-31 19:22:39.483275 shamirs-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2022-07-31 19:22:39.483860 shamirs-2.0.2/src/shamirs/
--rw-rw-rw-   0        0        0      113 2022-06-18 03:00:05.000000 shamirs-2.0.2/src/shamirs/__init__.py
--rw-rw-rw-   0        0        0    19110 2022-07-31 18:24:22.000000 shamirs-2.0.2/src/shamirs/shamirs.py
-drwxrwxrwx   0        0        0        0 2022-07-31 19:22:39.490382 shamirs-2.0.2/src/shamirs.egg-info/
--rw-rw-rw-   0        0        0     6239 2022-07-31 19:22:39.000000 shamirs-2.0.2/src/shamirs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2022-07-31 19:22:39.000000 shamirs-2.0.2/src/shamirs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-31 19:22:39.000000 shamirs-2.0.2/src/shamirs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      228 2022-07-31 19:22:39.000000 shamirs-2.0.2/src/shamirs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-07-31 19:22:39.000000 shamirs-2.0.2/src/shamirs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 17:52:20.888195 shamirs-2.1.0/
+-rw-rw-rw-   0        0        0     1091 2022-06-17 22:55:54.000000 shamirs-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     6549 2023-06-03 17:52:20.888195 shamirs-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6026 2023-06-03 17:46:20.000000 shamirs-2.1.0/README.rst
+-rw-rw-rw-   0        0        0     1036 2023-06-03 17:47:32.000000 shamirs-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 17:52:20.888195 shamirs-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-03 17:52:20.877692 shamirs-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 17:52:20.878693 shamirs-2.1.0/src/shamirs/
+-rw-rw-rw-   0        0        0      113 2022-06-18 03:00:05.000000 shamirs-2.1.0/src/shamirs/__init__.py
+-rw-rw-rw-   0        0        0    19939 2023-06-03 17:40:08.000000 shamirs-2.1.0/src/shamirs/shamirs.py
+drwxrwxrwx   0        0        0        0 2023-06-03 17:52:20.888195 shamirs-2.1.0/src/shamirs.egg-info/
+-rw-rw-rw-   0        0        0     6549 2023-06-03 17:52:20.000000 shamirs-2.1.0/src/shamirs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-06-03 17:52:20.000000 shamirs-2.1.0/src/shamirs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 17:52:20.000000 shamirs-2.1.0/src/shamirs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      229 2023-06-03 17:52:20.000000 shamirs-2.1.0/src/shamirs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-03 17:52:20.000000 shamirs-2.1.0/src/shamirs.egg-info/top_level.txt
```

### Comparing `shamirs-2.0.2/LICENSE` & `shamirs-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shamirs-2.0.2/PKG-INFO` & `shamirs-2.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shamirs
-Version: 2.0.2
+Version: 2.1.0
 Summary: Minimal pure-Python implementation of Shamir's Secret Sharing scheme.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/lapets/shamirs
 Project-URL: Documentation, https://shamirs.readthedocs.io
 Requires-Python: >=3.7
@@ -46,98 +46,124 @@
 .. |secrets_token_bytes| replace:: ``secrets.token_bytes``
 .. _secrets_token_bytes: https://docs.python.org/3/library/secrets.html#secrets.token_bytes
 
 This library provides functions and data structures for computing secret shares given an integer input value and for reassembling an integer from its corresponding secret shares via Lagrange interpolation over finite fields (according to `Shamir's Secret Sharing scheme <https://en.wikipedia.org/wiki/Shamir%27s_Secret_Sharing>`__). The built-in |secrets_token_bytes|_ function and rejection sampling are used to generate random coefficients. The `lagrange <https://pypi.org/project/lagrange>`__ library is used for Lagrange interpolation.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/shamirs>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/shamirs>`__:
+
+.. code-block:: bash
 
     python -m pip install shamirs
 
-The library can be imported in the usual way::
+The library can be imported in the usual way:
+
+.. code-block:: python
 
     import shamirs
 
 Examples
 ^^^^^^^^
-The library provides functions for transforming a nonnegative integer value into a number of secret shares and for reassembling those shares back into the value they represent::
+The library provides functions for transforming a nonnegative integer value into a number of secret shares and for reassembling those shares back into the value they represent:
+
+.. code-block:: python
 
     >>> ss = shamirs.shares(123, quantity=3)
     >>> len(ss)
     3
     >>> shamirs.interpolate(ss)
     123
     >>> ss = shamirs.shares(456, quantity=20, modulus=15485867, threshold=10)
     >>> shamirs.interpolate(ss[5:15], threshold=10)
     456
 
-Addition of shares and multiplication of shares by a scalar are both supported::
+Addition of shares and multiplication of shares by a scalar are both supported:
+
+.. code-block:: python
 
     >>> (r, s, t) = shamirs.shares(123, 3)
     >>> (u, v, w) = shamirs.shares(456, 3)
     >>> shamirs.interpolate([r + u, s + v, t + w])
     579
     >>> (r, s, t) = shamirs.shares(123, 3)
     >>> r = r * 2
     >>> s = s * 2
     >>> t = t * 2
     >>> shamirs.interpolate([r, s, t])
     246
 
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
     python -m pytest -W ignore::UserWarning
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/shamirs/shamirs.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/shamirs
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/shamirs>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 1.0.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/shamirs>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/shamirs>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `shamirs-2.0.2/README.rst` & `shamirs-2.1.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -28,98 +28,124 @@
 .. |secrets_token_bytes| replace:: ``secrets.token_bytes``
 .. _secrets_token_bytes: https://docs.python.org/3/library/secrets.html#secrets.token_bytes
 
 This library provides functions and data structures for computing secret shares given an integer input value and for reassembling an integer from its corresponding secret shares via Lagrange interpolation over finite fields (according to `Shamir's Secret Sharing scheme <https://en.wikipedia.org/wiki/Shamir%27s_Secret_Sharing>`__). The built-in |secrets_token_bytes|_ function and rejection sampling are used to generate random coefficients. The `lagrange <https://pypi.org/project/lagrange>`__ library is used for Lagrange interpolation.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/shamirs>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/shamirs>`__:
+
+.. code-block:: bash
 
     python -m pip install shamirs
 
-The library can be imported in the usual way::
+The library can be imported in the usual way:
+
+.. code-block:: python
 
     import shamirs
 
 Examples
 ^^^^^^^^
-The library provides functions for transforming a nonnegative integer value into a number of secret shares and for reassembling those shares back into the value they represent::
+The library provides functions for transforming a nonnegative integer value into a number of secret shares and for reassembling those shares back into the value they represent:
+
+.. code-block:: python
 
     >>> ss = shamirs.shares(123, quantity=3)
     >>> len(ss)
     3
     >>> shamirs.interpolate(ss)
     123
     >>> ss = shamirs.shares(456, quantity=20, modulus=15485867, threshold=10)
     >>> shamirs.interpolate(ss[5:15], threshold=10)
     456
 
-Addition of shares and multiplication of shares by a scalar are both supported::
+Addition of shares and multiplication of shares by a scalar are both supported:
+
+.. code-block:: python
 
     >>> (r, s, t) = shamirs.shares(123, 3)
     >>> (u, v, w) = shamirs.shares(456, 3)
     >>> shamirs.interpolate([r + u, s + v, t + w])
     579
     >>> (r, s, t) = shamirs.shares(123, 3)
     >>> r = r * 2
     >>> s = s * 2
     >>> t = t * 2
     >>> shamirs.interpolate([r, s, t])
     246
 
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
     python -m pytest -W ignore::UserWarning
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/shamirs/shamirs.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/shamirs
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/shamirs>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 1.0.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/shamirs>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/shamirs>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `shamirs-2.0.2/pyproject.toml` & `shamirs-2.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 [project]
 name = "shamirs"
-version = "2.0.2"
+version = "2.1.0"
 description = """\
     Minimal pure-Python implementation of Shamir's Secret \
     Sharing scheme.\
     """
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
     {email = "a@lapets.io"}
 ]
 readme = "README.rst"
 requires-python = ">=3.7"
 dependencies = [
-    "lagrange~=2.0"
+    "lagrange~=2.1"
 ]
 
 [project.urls]
 Repository = "https://github.com/lapets/shamirs"
 Documentation = "https://shamirs.readthedocs.io"
 
 [project.optional-dependencies]
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
 addopts = "--doctest-modules --ignore=docs --cov=shamirs --cov-report term-missing"
```

### Comparing `shamirs-2.0.2/src/shamirs/shamirs.py` & `shamirs-2.1.0/src/shamirs/shamirs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 Minimal pure-Python implementation of
 `Shamir's Secret Sharing scheme <https://en.wikipedia.org/wiki/Shamir%27s_Secret_Sharing>`__.
 """
 from __future__ import annotations
 import doctest
 import warnings
-from typing import Union, Optional, Sequence
-from collections.abc import Iterable
+from typing import Union, Optional, Sequence, Iterable
 import base64
 import secrets
 import lagrange
 
-MODULUS_DEFAULT = (2 ** 127) - 1
+_MODULUS_DEFAULT = (2 ** 127) - 1
 """
 Default prime modulus (equivalent to ``(2 ** 127) - 1``) that is used for
 creating secret shares if a prime modulus is not specified explicitly.
 """
 
 def _randint(bound: int) -> int:
     """
@@ -49,15 +48,15 @@
     bound on the size of the value.
 
     >>> share(4294967296, 123)
     Traceback (most recent call last):
       ...
     ValueError: index must be an integer that can be represented using at most 32 bits
     """
-    def __init__(self: share, index: int, value: int, modulus: Optional[int] = MODULUS_DEFAULT):
+    def __init__(self: share, index: int, value: int, modulus: Optional[int] = _MODULUS_DEFAULT):
         """
         Create a share instance according to the supplied parameters.
         """
         if index > 4294967295:
             raise ValueError(
                 'index must be an integer that can be represented using at most 32 bits'
             )
@@ -344,15 +343,15 @@
         share(123, 456, 1021)
         """
         return str(self)
 
 def shares(
         value: int,
         quantity: int,
-        modulus: Optional[int] = MODULUS_DEFAULT,
+        modulus: Optional[int] = _MODULUS_DEFAULT,
         threshold: Optional[int] = None
     ) -> Sequence[share]:
     """
     Transforms an integer value into the specified number of secret shares, with
     recovery of the original value possible using the returned sequence of secret
     shares (via the :obj:`interpolate` function).
 
@@ -452,15 +451,15 @@
     threshold = threshold or quantity
     if threshold > quantity:
         warnings.warn(
             'quantity of shares should be at least the threshold to be reconstructable'
         )
 
     # Add the base coefficient.
-    coefficients = [value] + [_randint(modulus - 1) for _ in range(1, threshold - 1)]
+    coefficients = [value] + [_randint(modulus - 1) for _ in range(1, threshold)]
 
     # Compute each share value such that ``shares[i] = f(i)`` if the polynomial
     # is ``f``.
     shares_ = [
         sum(
             c_j * i ** j % modulus
             for j, c_j in enumerate(coefficients)
@@ -503,21 +502,39 @@
     was shared with twenty parties such that at least twelve of them
     must collaborate to reconstruct the value.
 
     >>> interpolate(shares(123, 20, 1223, 12)[:12], 12) # Use first twelve shares.
     123
     >>> interpolate(shares(123, 20, 1223, 12)[20-12:], 12) # Use last twelve shares.
     123
-    >>> interpolate(shares(123, 20, 1223, 12)[:15], 12)  # Use first fifteen shares.
+    >>> interpolate(shares(123, 20, 1223, 12)[:15], 12) # Use first fifteen shares.
     123
-    >>> interpolate(shares(123, 20, 1223, 12)[:11], 12)  # Try using only eleven shares.
+    >>> interpolate(shares(123, 20, 1223, 12)[:11], 12) # Try using only eleven shares.
     Traceback (most recent call last):
       ...
     ValueError: not enough points for a unique interpolation
 
+    Any attempt to interpolate using a threshold value that is smaller than the
+    threshold value originally specified when the shares were created yields an
+    arbitrary output. However, no confirmation is performed (at the time of
+    interpolation) that interpolation is being performed with the correct threshold
+    value.
+
+    >>> 123 != interpolate(shares(123, 20, 2**31 - 1, 12)[:11], 11) # Try using smaller threshold.
+    True
+    >>> 123 != interpolate(shares(123, 20, 2**31 - 1, 2)[:1], 1) # Try using smaller threshold.
+    True
+
+    Any attempt to interpolate using a threshold value that is larger than the
+    threshold value originally specified when the shares were created returns
+    the original secret-shared value.
+
+    >>> interpolate(shares(123, 20, 2**31 - 1, 12)[:13], 13) # Try using larger threshold.
+    123
+
     Invocations with invalid parameter values raise exceptions.
 
     >>> interpolate([1, 2, 3])
     Traceback (most recent call last):
       ...
     TypeError: input must contain share objects
     >>> interpolate(shares(123, 3, 1223) + shares(123, 3, 1021))
```

### Comparing `shamirs-2.0.2/src/shamirs.egg-info/PKG-INFO` & `shamirs-2.1.0/src/shamirs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shamirs
-Version: 2.0.2
+Version: 2.1.0
 Summary: Minimal pure-Python implementation of Shamir's Secret Sharing scheme.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/lapets/shamirs
 Project-URL: Documentation, https://shamirs.readthedocs.io
 Requires-Python: >=3.7
@@ -46,98 +46,124 @@
 .. |secrets_token_bytes| replace:: ``secrets.token_bytes``
 .. _secrets_token_bytes: https://docs.python.org/3/library/secrets.html#secrets.token_bytes
 
 This library provides functions and data structures for computing secret shares given an integer input value and for reassembling an integer from its corresponding secret shares via Lagrange interpolation over finite fields (according to `Shamir's Secret Sharing scheme <https://en.wikipedia.org/wiki/Shamir%27s_Secret_Sharing>`__). The built-in |secrets_token_bytes|_ function and rejection sampling are used to generate random coefficients. The `lagrange <https://pypi.org/project/lagrange>`__ library is used for Lagrange interpolation.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/shamirs>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/shamirs>`__:
+
+.. code-block:: bash
 
     python -m pip install shamirs
 
-The library can be imported in the usual way::
+The library can be imported in the usual way:
+
+.. code-block:: python
 
     import shamirs
 
 Examples
 ^^^^^^^^
-The library provides functions for transforming a nonnegative integer value into a number of secret shares and for reassembling those shares back into the value they represent::
+The library provides functions for transforming a nonnegative integer value into a number of secret shares and for reassembling those shares back into the value they represent:
+
+.. code-block:: python
 
     >>> ss = shamirs.shares(123, quantity=3)
     >>> len(ss)
     3
     >>> shamirs.interpolate(ss)
     123
     >>> ss = shamirs.shares(456, quantity=20, modulus=15485867, threshold=10)
     >>> shamirs.interpolate(ss[5:15], threshold=10)
     456
 
-Addition of shares and multiplication of shares by a scalar are both supported::
+Addition of shares and multiplication of shares by a scalar are both supported:
+
+.. code-block:: python
 
     >>> (r, s, t) = shamirs.shares(123, 3)
     >>> (u, v, w) = shamirs.shares(456, 3)
     >>> shamirs.interpolate([r + u, s + v, t + w])
     579
     >>> (r, s, t) = shamirs.shares(123, 3)
     >>> r = r * 2
     >>> s = s * 2
     >>> t = t * 2
     >>> shamirs.interpolate([r, s, t])
     246
 
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
     python -m pytest -W ignore::UserWarning
 
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
 
     python src/shamirs/shamirs.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/shamirs
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/shamirs>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 1.0.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/shamirs>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/shamirs>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

