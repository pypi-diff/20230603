# Comparing `tmp/egcd-0.4.3.tar.gz` & `tmp/egcd-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egcd-0.4.3.tar", last modified: Mon Aug  1 01:22:06 2022, max compression
+gzip compressed data, was "egcd-0.5.0.tar", last modified: Sat Jun  3 03:44:48 2023, max compression
```

## Comparing `egcd-0.4.3.tar` & `egcd-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-08-01 01:22:06.499834 egcd-0.4.3/
--rw-rw-rw-   0        0        0     1091 2022-06-10 21:06:07.000000 egcd-0.4.3/LICENSE
--rw-rw-rw-   0        0        0     5484 2022-08-01 01:22:06.499772 egcd-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     4928 2022-08-01 01:15:55.000000 egcd-0.4.3/README.rst
--rw-rw-rw-   0        0        0      982 2022-08-01 01:15:30.000000 egcd-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-01 01:22:06.500033 egcd-0.4.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-01 01:22:06.478993 egcd-0.4.3/src/
-drwxrwxrwx   0        0        0        0 2022-08-01 01:22:06.490480 egcd-0.4.3/src/egcd/
--rw-rw-rw-   0        0        0       78 2022-06-10 21:06:07.000000 egcd-0.4.3/src/egcd/__init__.py
--rw-rw-rw-   0        0        0     2106 2022-07-31 18:04:56.000000 egcd-0.4.3/src/egcd/egcd.py
-drwxrwxrwx   0        0        0        0 2022-08-01 01:22:06.498760 egcd-0.4.3/src/egcd.egg-info/
--rw-rw-rw-   0        0        0     5484 2022-08-01 01:22:06.000000 egcd-0.4.3/src/egcd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2022-08-01 01:22:06.000000 egcd-0.4.3/src/egcd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-01 01:22:06.000000 egcd-0.4.3/src/egcd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2022-08-01 01:22:06.000000 egcd-0.4.3/src/egcd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-08-01 01:22:06.000000 egcd-0.4.3/src/egcd.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 03:44:48.453648 egcd-0.5.0/
+-rw-rw-rw-   0        0        0     1091 2022-06-10 21:06:07.000000 egcd-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     5769 2023-06-03 03:44:48.453648 egcd-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5213 2023-06-03 03:38:51.000000 egcd-0.5.0/README.rst
+-rw-rw-rw-   0        0        0      983 2023-06-03 03:40:17.000000 egcd-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 03:44:48.453648 egcd-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-03 03:44:48.438607 egcd-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 03:44:48.443089 egcd-0.5.0/src/egcd/
+-rw-rw-rw-   0        0        0       78 2022-06-10 21:06:07.000000 egcd-0.5.0/src/egcd/__init__.py
+-rw-rw-rw-   0        0        0     2106 2023-06-03 03:43:12.000000 egcd-0.5.0/src/egcd/egcd.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:44:48.452648 egcd-0.5.0/src/egcd.egg-info/
+-rw-rw-rw-   0        0        0     5769 2023-06-03 03:44:48.000000 egcd-0.5.0/src/egcd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-03 03:44:48.000000 egcd-0.5.0/src/egcd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 03:44:48.000000 egcd-0.5.0/src/egcd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2023-06-03 03:44:48.000000 egcd-0.5.0/src/egcd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-03 03:44:48.000000 egcd-0.5.0/src/egcd.egg-info/top_level.txt
```

### Comparing `egcd-0.4.3/LICENSE` & `egcd-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `egcd-0.4.3/PKG-INFO` & `egcd-0.5.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: egcd
-Version: 0.4.3
-Summary: Easy-to-import library with a basic, efficient, pure-Python implementation of the extended Euclidean algorithm.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/lapets/egcd
-Project-URL: Documentation, https://egcd.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
 ====
 egcd
 ====
 
 Easy-to-import library with a basic, efficient, pure-Python implementation of the extended Euclidean algorithm.
 
 |pypi| |readthedocs| |actions| |coveralls|
@@ -38,89 +20,113 @@
 
 .. |coveralls| image:: https://coveralls.io/repos/github/lapets/egcd/badge.svg?branch=main
    :target: https://coveralls.io/github/lapets/egcd?branch=main
    :alt: Coveralls test coverage summary.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/egcd>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/egcd>`__:
+
+.. code-block:: bash
 
     python -m pip install egcd
 
-The library can be imported in the usual way::
+The library can be imported in the usual way:
+
+.. code-block:: python
 
     from egcd import egcd
 
 Examples
 ^^^^^^^^
 
 .. |egcd| replace:: ``egcd``
-.. _egcd: https://egcd.readthedocs.io/en/0.4.3/_source/egcd.html#egcd.egcd.egcd
+.. _egcd: https://egcd.readthedocs.io/en/0.5.0/_source/egcd.html#egcd.egcd.egcd
+
+The function |egcd|_ is an efficient implementation of the `extended Euclidean algorithm <https://en.wikipedia.org/wiki/Extended_Euclidean_algorithm>`__. It accepts two integer inputs ``b`` and ``n``, returning a tuple of the form ``(gcd(b, n), a, m)`` where the three integers in the tuple satisfy the `identity <https://en.wikipedia.org/wiki/B%C3%A9zout%27s_identity>`__ ``(a * b) + (n * m) == gcd(b, n)``:
 
-The function |egcd|_ is an efficient implementation of the `extended Euclidean algorithm <https://en.wikipedia.org/wiki/Extended_Euclidean_algorithm>`__. It accepts two integer inputs ``b`` and ``n``, returning a tuple of the form ``(gcd(b, n), a, m)`` where the three integers in the tuple satisfy the `identity <https://en.wikipedia.org/wiki/B%C3%A9zout%27s_identity>`__ ``(a * b) + (n * m) == gcd(b, n)``::
+.. code-block:: python
 
     >>> egcd(1, 1)
     (1, 0, 1)
     >>> egcd(12, 8)
     (4, 1, -1)
     >>> egcd(23894798501898, 23948178468116)
     (2, 2437250447493, -2431817869532)
     >>> egcd(pow(2, 50), pow(3, 50))
     (1, -260414429242905345185687, 408415383037561)
 
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
 
     python src/egcd/egcd.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/egcd
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/egcd>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/egcd>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/egcd>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `egcd-0.4.3/pyproject.toml` & `egcd-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "egcd"
-version = "0.4.3"
+version = "0.5.0"
 description = """\
     Easy-to-import library with a basic, efficient, pure-Python \
     implementation of the extended Euclidean algorithm.\
     """
 license = {text = "MIT"}
 authors = [
     {name = "Andrei Lapets"},
@@ -20,29 +20,29 @@
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
 addopts = "--doctest-modules --ignore=docs --cov=egcd --cov-report term-missing"
```

### Comparing `egcd-0.4.3/src/egcd/egcd.py` & `egcd-0.5.0/src/egcd/egcd.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,9 +47,9 @@
     (x0, x1, y0, y1) = (1, 0, 0, 1)
     while n != 0:
         (q, b, n) = (b // n, n, b % n)
         (x0, x1) = (x1, x0 - q * x1)
         (y0, y1) = (y1, y0 - q * y1)
     return (b, x0, y0)
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     doctest.testmod() # pragma: no cover
```

### Comparing `egcd-0.4.3/src/egcd.egg-info/PKG-INFO` & `egcd-0.5.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egcd
-Version: 0.4.3
+Version: 0.5.0
 Summary: Easy-to-import library with a basic, efficient, pure-Python implementation of the extended Euclidean algorithm.
 Author: Andrei Lapets
 Author-email: a@lapets.io
 License: MIT
 Project-URL: Repository, https://github.com/lapets/egcd
 Project-URL: Documentation, https://egcd.readthedocs.io
 Requires-Python: >=3.7
@@ -38,89 +38,113 @@
 
 .. |coveralls| image:: https://coveralls.io/repos/github/lapets/egcd/badge.svg?branch=main
    :target: https://coveralls.io/github/lapets/egcd?branch=main
    :alt: Coveralls test coverage summary.
 
 Installation and Usage
 ----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/egcd>`__::
+This library is available as a `package on PyPI <https://pypi.org/project/egcd>`__:
+
+.. code-block:: bash
 
     python -m pip install egcd
 
-The library can be imported in the usual way::
+The library can be imported in the usual way:
+
+.. code-block:: python
 
     from egcd import egcd
 
 Examples
 ^^^^^^^^
 
 .. |egcd| replace:: ``egcd``
-.. _egcd: https://egcd.readthedocs.io/en/0.4.3/_source/egcd.html#egcd.egcd.egcd
+.. _egcd: https://egcd.readthedocs.io/en/0.5.0/_source/egcd.html#egcd.egcd.egcd
+
+The function |egcd|_ is an efficient implementation of the `extended Euclidean algorithm <https://en.wikipedia.org/wiki/Extended_Euclidean_algorithm>`__. It accepts two integer inputs ``b`` and ``n``, returning a tuple of the form ``(gcd(b, n), a, m)`` where the three integers in the tuple satisfy the `identity <https://en.wikipedia.org/wiki/B%C3%A9zout%27s_identity>`__ ``(a * b) + (n * m) == gcd(b, n)``:
 
-The function |egcd|_ is an efficient implementation of the `extended Euclidean algorithm <https://en.wikipedia.org/wiki/Extended_Euclidean_algorithm>`__. It accepts two integer inputs ``b`` and ``n``, returning a tuple of the form ``(gcd(b, n), a, m)`` where the three integers in the tuple satisfy the `identity <https://en.wikipedia.org/wiki/B%C3%A9zout%27s_identity>`__ ``(a * b) + (n * m) == gcd(b, n)``::
+.. code-block:: python
 
     >>> egcd(1, 1)
     (1, 0, 1)
     >>> egcd(12, 8)
     (4, 1, -1)
     >>> egcd(23894798501898, 23948178468116)
     (2, 2437250447493, -2431817869532)
     >>> egcd(pow(2, 50), pow(3, 50))
     (1, -260414429242905345185687, 408415383037561)
 
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
 
     python src/egcd/egcd.py -v
 
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
 
     python -m pip install .[lint]
     python -m pylint src/egcd
 
 Contributions
 ^^^^^^^^^^^^^
 In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/egcd>`__ for this library.
 
 Versioning
 ^^^^^^^^^^
 Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
 
 Publishing
 ^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/egcd>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
+This library can be published as a `package on PyPI <https://pypi.org/project/egcd>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

