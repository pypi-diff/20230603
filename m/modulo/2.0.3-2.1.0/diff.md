# Comparing `tmp/modulo-2.0.3.tar.gz` & `tmp/modulo-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modulo-2.0.3.tar", last modified: Sun Jul 31 19:16:27 2022, max compression
+gzip compressed data, was "modulo-2.1.0.tar", last modified: Sat Jun  3 03:58:41 2023, max compression
```

## Comparing `modulo-2.0.3.tar` & `modulo-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-07-31 19:16:27.214900 modulo-2.0.3/
--rw-rw-rw-   0        0        0     1091 2022-06-15 03:05:21.000000 modulo-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     8029 2022-07-31 19:16:27.214900 modulo-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7479 2022-07-24 05:04:20.000000 modulo-2.0.3/README.rst
--rw-rw-rw-   0        0        0     1016 2022-07-31 18:08:00.000000 modulo-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-07-31 19:16:27.214900 modulo-2.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-07-31 19:16:27.197627 modulo-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2022-07-31 19:16:27.213891 modulo-2.0.3/src/modulo/
--rw-rw-rw-   0        0        0       98 2022-06-15 03:05:21.000000 modulo-2.0.3/src/modulo/__init__.py
--rw-rw-rw-   0        0        0    37922 2022-07-31 18:14:12.000000 modulo-2.0.3/src/modulo/modulo.py
-drwxrwxrwx   0        0        0        0 2022-07-31 19:16:27.214900 modulo-2.0.3/src/modulo.egg-info/
--rw-rw-rw-   0        0        0     8029 2022-07-31 19:16:26.000000 modulo-2.0.3/src/modulo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2022-07-31 19:16:27.000000 modulo-2.0.3/src/modulo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-31 19:16:26.000000 modulo-2.0.3/src/modulo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      191 2022-07-31 19:16:27.000000 modulo-2.0.3/src/modulo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-07-31 19:16:27.000000 modulo-2.0.3/src/modulo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 03:58:41.474760 modulo-2.1.0/
+-rw-rw-rw-   0        0        0     1091 2022-06-15 03:05:21.000000 modulo-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     8539 2023-06-03 03:58:41.474760 modulo-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7989 2023-06-03 03:54:07.000000 modulo-2.1.0/README.rst
+-rw-rw-rw-   0        0        0     1017 2023-06-03 03:55:58.000000 modulo-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 03:58:41.474760 modulo-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-03 03:58:41.462254 modulo-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 03:58:41.464256 modulo-2.1.0/src/modulo/
+-rw-rw-rw-   0        0        0       98 2022-06-15 03:05:21.000000 modulo-2.1.0/src/modulo/__init__.py
+-rw-rw-rw-   0        0        0    37922 2023-06-03 03:51:33.000000 modulo-2.1.0/src/modulo/modulo.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:58:41.473760 modulo-2.1.0/src/modulo.egg-info/
+-rw-rw-rw-   0        0        0     8539 2023-06-03 03:58:41.000000 modulo-2.1.0/src/modulo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-03 03:58:41.000000 modulo-2.1.0/src/modulo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 03:58:41.000000 modulo-2.1.0/src/modulo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2023-06-03 03:58:41.000000 modulo-2.1.0/src/modulo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-03 03:58:41.000000 modulo-2.1.0/src/modulo.egg-info/top_level.txt
```

### Comparing `modulo-2.0.3/LICENSE` & `modulo-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modulo-2.0.3/PKG-INFO` & `modulo-2.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modulo
-Version: 2.0.3
+Version: 2.1.0
 Summary: Pure-Python library for working with modular arithmetic, congruence classes, and finite fields.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/lapets/modulo
 Project-URL: Documentation, https://modulo-lib.readthedocs.io
 Requires-Python: >=3.7
@@ -42,163 +42,205 @@
 
 Purpose
 -------
 The library allows users to work with congruence classes (including finite field elements) as objects, with support for many common operations.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/modulo>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/modulo>`__:
+
+.. code-block:: bash
 
     python -m pip install modulo
 
-The library can be imported in the usual way::
+The library can be imported in the usual way:
+
+.. code-block:: python
 
     from modulo import modulo
 
 Examples
 ^^^^^^^^
-This library makes it possible to work with `congruence classes <https://en.wikipedia.org/wiki/Congruence_relation>`__ (and sets of congruence classes such as finite fields) as objects. A congruence class is defined using a representative integer and a modulus::
+This library makes it possible to work with `congruence classes <https://en.wikipedia.org/wiki/Congruence_relation>`__ (and sets of congruence classes such as finite fields) as objects. A congruence class is defined using a representative integer and a modulus:
+
+.. code-block:: python
 
     >>> from modulo import modulo
     >>> modulo(3, 7)
     modulo(3, 7)
 
-Built-in operators can be used to perform modular addition, modular subtraction, and modular negation of congruence classes::
+Built-in operators can be used to perform modular addition, modular subtraction, and modular negation of congruence classes:
+
+.. code-block:: python
 
     >>> modulo(3, 7) + modulo(5, 7)
     modulo(1, 7)
     >>> modulo(1, 7) - modulo(4, 7)
     modulo(4, 7)
     >>> -modulo(5, 7)
     modulo(2, 7)
 
-Modular multiplication, division, inversion, and exponentiation are also supported (when they are defined)::
+Modular multiplication, division, inversion, and exponentiation are also supported (when they are defined):
+
+.. code-block:: python
 
     >>> modulo(3, 7) * modulo(5, 7)
     modulo(1, 7)
     >>> modulo(1, 7) // modulo(3, 7)
     modulo(5, 7)
     >>> modulo(5, 7) ** 2
     modulo(4, 7)
     >>> modulo(5, 7) ** (-1)
     modulo(3, 7)
 
-Individual congruence classes can be compared with one another according to their least nonnegative residues (and, thus, can also be sorted)::
+Individual congruence classes can be compared with one another according to their least nonnegative residues (and, thus, can also be sorted):
+
+.. code-block:: python
 
     >>> mod(2, 7) < mod(3, 7)
     True
     >>> list(sorted([mod(2, 3), mod(1, 3), mod(0, 3)]))
     [modulo(0, 3), modulo(1, 3), modulo(2, 3)]
 
-The membership operation is supported between integers and congruence classes::
+The membership operation is supported between integers and congruence classes:
+
+.. code-block:: python
 
     >>> 3 in mod(3, 7)
     True
     >>> 10 in mod(3, 7)
     True
     >>> 4 in mod(3, 7)
     False
 
 .. |len| replace:: ``len``
 .. _len: https://docs.python.org/3/library/functions.html#len
 
-A set of congruence classes such as a finite field can also be defined. The built-in length function |len|_ and the membership operator are supported::
+A set of congruence classes such as a finite field can also be defined. The built-in length function |len|_ and the membership operator are supported:
+
+.. code-block:: python
 
     >>> len(modulo(7))
     7
     >>> modulo(3, 7) in modulo(7)
     True
 
 .. |int| replace:: ``int``
 .. _int: https://docs.python.org/3/library/functions.html#int
 
-The built-in |int|_ function can be used to retrieve the least nonnegative residue of a congruence class and the built-in |len|_ function can be used to retrieve the modulus of a congruence class or set of congruence classes (this is the recommended approach)::
+The built-in |int|_ function can be used to retrieve the least nonnegative residue of a congruence class and the built-in |len|_ function can be used to retrieve the modulus of a congruence class or set of congruence classes (this is the recommended approach):
+
+.. code-block:: python
 
     >>> c = modulo(3, 7)
     >>> int(c)
     3
     >>> len(c)
     7
 
-Congruence classes and sets of congruence classes are also hashable (making it possible to use them as dictionary keys and as set members) and iterable::
+Congruence classes and sets of congruence classes are also hashable (making it possible to use them as dictionary keys and as set members) and iterable:
+
+.. code-block:: python
 
     >>> len({mod(0, 3), mod(1, 3), mod(2, 3)})
     3
     >>> list(mod(4))
     [modulo(0, 4), modulo(1, 4), modulo(2, 4), modulo(3, 4)]
     >>> from itertools import islice
     >>> list(islice(mod(3, 7), 5))
     [3, 10, 17, 24, 31]
 
-The `Chinese remainder theorem <https://en.wikipedia.org/wiki/Chinese_remainder_theorem>`__ can be applied to construct the intersection of two congruence classes as a congruence class (when it is possible to do so)::
+The `Chinese remainder theorem <https://en.wikipedia.org/wiki/Chinese_remainder_theorem>`__ can be applied to construct the intersection of two congruence classes as a congruence class (when it is possible to do so):
+
+.. code-block:: python
 
     >>> mod(23, 100) & mod(31, 49)
     modulo(423, 4900)
     >>> mod(2, 10) & mod(4, 20) is None
     True
 
-Some familiar forms of notation for referring to congruence classes (and sets thereof) are also supported::
+Some familiar forms of notation for referring to congruence classes (and sets thereof) are also supported:
+
+.. code-block:: python
 
     >>> Z/(23*Z)
     modulo(23)
     >>> 23*Z
     modulo(0, 23)
     >>> 17 + 23*Z
     modulo(17, 23)
 
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
 
     python src/modulo/modulo.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/modulo
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/modulo>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/modulo>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/modulo>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `modulo-2.0.3/README.rst` & `modulo-2.1.0/src/modulo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: modulo
+Version: 2.1.0
+Summary: Pure-Python library for working with modular arithmetic, congruence classes, and finite fields.
+Author: Andrei Lapets
+Author-email: a@lapets.io
+License: MIT
+Project-URL: Repository, https://github.com/lapets/modulo
+Project-URL: Documentation, https://modulo-lib.readthedocs.io
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
 ======
 modulo
 ======
 
 Pure-Python library for working with modular arithmetic, congruence classes, and finite fields.
 
 |pypi| |readthedocs| |actions| |coveralls|
@@ -24,163 +42,205 @@
 
 Purpose
 -------
 The library allows users to work with congruence classes (including finite field elements) as objects, with support for many common operations.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/modulo>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/modulo>`__:
+
+.. code-block:: bash
 
     python -m pip install modulo
 
-The library can be imported in the usual way::
+The library can be imported in the usual way:
+
+.. code-block:: python
 
     from modulo import modulo
 
 Examples
 ^^^^^^^^
-This library makes it possible to work with `congruence classes <https://en.wikipedia.org/wiki/Congruence_relation>`__ (and sets of congruence classes such as finite fields) as objects. A congruence class is defined using a representative integer and a modulus::
+This library makes it possible to work with `congruence classes <https://en.wikipedia.org/wiki/Congruence_relation>`__ (and sets of congruence classes such as finite fields) as objects. A congruence class is defined using a representative integer and a modulus:
+
+.. code-block:: python
 
     >>> from modulo import modulo
     >>> modulo(3, 7)
     modulo(3, 7)
 
-Built-in operators can be used to perform modular addition, modular subtraction, and modular negation of congruence classes::
+Built-in operators can be used to perform modular addition, modular subtraction, and modular negation of congruence classes:
+
+.. code-block:: python
 
     >>> modulo(3, 7) + modulo(5, 7)
     modulo(1, 7)
     >>> modulo(1, 7) - modulo(4, 7)
     modulo(4, 7)
     >>> -modulo(5, 7)
     modulo(2, 7)
 
-Modular multiplication, division, inversion, and exponentiation are also supported (when they are defined)::
+Modular multiplication, division, inversion, and exponentiation are also supported (when they are defined):
+
+.. code-block:: python
 
     >>> modulo(3, 7) * modulo(5, 7)
     modulo(1, 7)
     >>> modulo(1, 7) // modulo(3, 7)
     modulo(5, 7)
     >>> modulo(5, 7) ** 2
     modulo(4, 7)
     >>> modulo(5, 7) ** (-1)
     modulo(3, 7)
 
-Individual congruence classes can be compared with one another according to their least nonnegative residues (and, thus, can also be sorted)::
+Individual congruence classes can be compared with one another according to their least nonnegative residues (and, thus, can also be sorted):
+
+.. code-block:: python
 
     >>> mod(2, 7) < mod(3, 7)
     True
     >>> list(sorted([mod(2, 3), mod(1, 3), mod(0, 3)]))
     [modulo(0, 3), modulo(1, 3), modulo(2, 3)]
 
-The membership operation is supported between integers and congruence classes::
+The membership operation is supported between integers and congruence classes:
+
+.. code-block:: python
 
     >>> 3 in mod(3, 7)
     True
     >>> 10 in mod(3, 7)
     True
     >>> 4 in mod(3, 7)
     False
 
 .. |len| replace:: ``len``
 .. _len: https://docs.python.org/3/library/functions.html#len
 
-A set of congruence classes such as a finite field can also be defined. The built-in length function |len|_ and the membership operator are supported::
+A set of congruence classes such as a finite field can also be defined. The built-in length function |len|_ and the membership operator are supported:
+
+.. code-block:: python
 
     >>> len(modulo(7))
     7
     >>> modulo(3, 7) in modulo(7)
     True
 
 .. |int| replace:: ``int``
 .. _int: https://docs.python.org/3/library/functions.html#int
 
-The built-in |int|_ function can be used to retrieve the least nonnegative residue of a congruence class and the built-in |len|_ function can be used to retrieve the modulus of a congruence class or set of congruence classes (this is the recommended approach)::
+The built-in |int|_ function can be used to retrieve the least nonnegative residue of a congruence class and the built-in |len|_ function can be used to retrieve the modulus of a congruence class or set of congruence classes (this is the recommended approach):
+
+.. code-block:: python
 
     >>> c = modulo(3, 7)
     >>> int(c)
     3
     >>> len(c)
     7
 
-Congruence classes and sets of congruence classes are also hashable (making it possible to use them as dictionary keys and as set members) and iterable::
+Congruence classes and sets of congruence classes are also hashable (making it possible to use them as dictionary keys and as set members) and iterable:
+
+.. code-block:: python
 
     >>> len({mod(0, 3), mod(1, 3), mod(2, 3)})
     3
     >>> list(mod(4))
     [modulo(0, 4), modulo(1, 4), modulo(2, 4), modulo(3, 4)]
     >>> from itertools import islice
     >>> list(islice(mod(3, 7), 5))
     [3, 10, 17, 24, 31]
 
-The `Chinese remainder theorem <https://en.wikipedia.org/wiki/Chinese_remainder_theorem>`__ can be applied to construct the intersection of two congruence classes as a congruence class (when it is possible to do so)::
+The `Chinese remainder theorem <https://en.wikipedia.org/wiki/Chinese_remainder_theorem>`__ can be applied to construct the intersection of two congruence classes as a congruence class (when it is possible to do so):
+
+.. code-block:: python
 
     >>> mod(23, 100) & mod(31, 49)
     modulo(423, 4900)
     >>> mod(2, 10) & mod(4, 20) is None
     True
 
-Some familiar forms of notation for referring to congruence classes (and sets thereof) are also supported::
+Some familiar forms of notation for referring to congruence classes (and sets thereof) are also supported:
+
+.. code-block:: python
 
     >>> Z/(23*Z)
     modulo(23)
     >>> 23*Z
     modulo(0, 23)
     >>> 17 + 23*Z
     modulo(17, 23)
 
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
 
     python src/modulo/modulo.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/modulo
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/modulo>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/modulo>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/modulo>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `modulo-2.0.3/pyproject.toml` & `modulo-2.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 [project]
 name = "modulo"
-version = "2.0.3"
+version = "2.1.0"
 description = """\
     Pure-Python library for working with modular arithmetic, \
     congruence classes, and finite fields.\
     """
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
     {email = "a@lapets.io"}
 ]
 readme = "README.rst"
 requires-python = ">=3.7"
 dependencies = [
-    "egcd~=0.4"
+    "egcd~=0.5"
 ]
 
 [project.urls]
 Repository = "https://github.com/lapets/modulo"
 Documentation = "https://modulo-lib.readthedocs.io"
 
 [project.optional-dependencies]
 docs = [
     "toml~=0.10.2",
     "sphinx~=4.2.0",
     "sphinx-rtd-theme~=1.0.0"
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
 addopts = "--doctest-modules --ignore=docs --cov=modulo --cov-report term-missing"
```

### Comparing `modulo-2.0.3/src/modulo/modulo.py` & `modulo-2.1.0/src/modulo/modulo.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from egcd import egcd
 
 class _symbol(type): # pylint: disable=invalid-name # Private/internal class.
     """
     Metaclass to enable the use of a class as a mathematical symbol within
     expressions.
     """
-    def __new__(cls, clsname, bases, attrs):
-        return super(_symbol, cls).__new__(cls, clsname, bases, attrs)
+    def __new__(mcs, clsname, bases, attrs):
+        return super(_symbol, mcs).__new__(mcs, clsname, bases, attrs)
 
     def __rmul__(cls: _symbol, other: int) -> modulo:
         """
         Enable use of the :obj:`modulo` class and its synonyms as a
         mathematical symbol, enabling construction of congruence class
         instances via a concise and familiar notation.
```

### Comparing `modulo-2.0.3/src/modulo.egg-info/PKG-INFO` & `modulo-2.1.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: modulo
-Version: 2.0.3
-Summary: Pure-Python library for working with modular arithmetic, congruence classes, and finite fields.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/lapets/modulo
-Project-URL: Documentation, https://modulo-lib.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
 ======
 modulo
 ======
 
 Pure-Python library for working with modular arithmetic, congruence classes, and finite fields.
 
 |pypi| |readthedocs| |actions| |coveralls|
@@ -42,163 +24,205 @@
 
 Purpose
 -------
 The library allows users to work with congruence classes (including finite field elements) as objects, with support for many common operations.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/modulo>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/modulo>`__:
+
+.. code-block:: bash
 
     python -m pip install modulo
 
-The library can be imported in the usual way::
+The library can be imported in the usual way:
+
+.. code-block:: python
 
     from modulo import modulo
 
 Examples
 ^^^^^^^^
-This library makes it possible to work with `congruence classes <https://en.wikipedia.org/wiki/Congruence_relation>`__ (and sets of congruence classes such as finite fields) as objects. A congruence class is defined using a representative integer and a modulus::
+This library makes it possible to work with `congruence classes <https://en.wikipedia.org/wiki/Congruence_relation>`__ (and sets of congruence classes such as finite fields) as objects. A congruence class is defined using a representative integer and a modulus:
+
+.. code-block:: python
 
     >>> from modulo import modulo
     >>> modulo(3, 7)
     modulo(3, 7)
 
-Built-in operators can be used to perform modular addition, modular subtraction, and modular negation of congruence classes::
+Built-in operators can be used to perform modular addition, modular subtraction, and modular negation of congruence classes:
+
+.. code-block:: python
 
     >>> modulo(3, 7) + modulo(5, 7)
     modulo(1, 7)
     >>> modulo(1, 7) - modulo(4, 7)
     modulo(4, 7)
     >>> -modulo(5, 7)
     modulo(2, 7)
 
-Modular multiplication, division, inversion, and exponentiation are also supported (when they are defined)::
+Modular multiplication, division, inversion, and exponentiation are also supported (when they are defined):
+
+.. code-block:: python
 
     >>> modulo(3, 7) * modulo(5, 7)
     modulo(1, 7)
     >>> modulo(1, 7) // modulo(3, 7)
     modulo(5, 7)
     >>> modulo(5, 7) ** 2
     modulo(4, 7)
     >>> modulo(5, 7) ** (-1)
     modulo(3, 7)
 
-Individual congruence classes can be compared with one another according to their least nonnegative residues (and, thus, can also be sorted)::
+Individual congruence classes can be compared with one another according to their least nonnegative residues (and, thus, can also be sorted):
+
+.. code-block:: python
 
     >>> mod(2, 7) < mod(3, 7)
     True
     >>> list(sorted([mod(2, 3), mod(1, 3), mod(0, 3)]))
     [modulo(0, 3), modulo(1, 3), modulo(2, 3)]
 
-The membership operation is supported between integers and congruence classes::
+The membership operation is supported between integers and congruence classes:
+
+.. code-block:: python
 
     >>> 3 in mod(3, 7)
     True
     >>> 10 in mod(3, 7)
     True
     >>> 4 in mod(3, 7)
     False
 
 .. |len| replace:: ``len``
 .. _len: https://docs.python.org/3/library/functions.html#len
 
-A set of congruence classes such as a finite field can also be defined. The built-in length function |len|_ and the membership operator are supported::
+A set of congruence classes such as a finite field can also be defined. The built-in length function |len|_ and the membership operator are supported:
+
+.. code-block:: python
 
     >>> len(modulo(7))
     7
     >>> modulo(3, 7) in modulo(7)
     True
 
 .. |int| replace:: ``int``
 .. _int: https://docs.python.org/3/library/functions.html#int
 
-The built-in |int|_ function can be used to retrieve the least nonnegative residue of a congruence class and the built-in |len|_ function can be used to retrieve the modulus of a congruence class or set of congruence classes (this is the recommended approach)::
+The built-in |int|_ function can be used to retrieve the least nonnegative residue of a congruence class and the built-in |len|_ function can be used to retrieve the modulus of a congruence class or set of congruence classes (this is the recommended approach):
+
+.. code-block:: python
 
     >>> c = modulo(3, 7)
     >>> int(c)
     3
     >>> len(c)
     7
 
-Congruence classes and sets of congruence classes are also hashable (making it possible to use them as dictionary keys and as set members) and iterable::
+Congruence classes and sets of congruence classes are also hashable (making it possible to use them as dictionary keys and as set members) and iterable:
+
+.. code-block:: python
 
     >>> len({mod(0, 3), mod(1, 3), mod(2, 3)})
     3
     >>> list(mod(4))
     [modulo(0, 4), modulo(1, 4), modulo(2, 4), modulo(3, 4)]
     >>> from itertools import islice
     >>> list(islice(mod(3, 7), 5))
     [3, 10, 17, 24, 31]
 
-The `Chinese remainder theorem <https://en.wikipedia.org/wiki/Chinese_remainder_theorem>`__ can be applied to construct the intersection of two congruence classes as a congruence class (when it is possible to do so)::
+The `Chinese remainder theorem <https://en.wikipedia.org/wiki/Chinese_remainder_theorem>`__ can be applied to construct the intersection of two congruence classes as a congruence class (when it is possible to do so):
+
+.. code-block:: python
 
     >>> mod(23, 100) & mod(31, 49)
     modulo(423, 4900)
     >>> mod(2, 10) & mod(4, 20) is None
     True
 
-Some familiar forms of notation for referring to congruence classes (and sets thereof) are also supported::
+Some familiar forms of notation for referring to congruence classes (and sets thereof) are also supported:
+
+.. code-block:: python
 
     >>> Z/(23*Z)
     modulo(23)
     >>> 23*Z
     modulo(0, 23)
     >>> 17 + 23*Z
     modulo(17, 23)
 
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
 
     python src/modulo/modulo.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/modulo
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/modulo>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/modulo>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/modulo>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

