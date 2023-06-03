# Comparing `tmp/waveformtools-2023.5.19.tar.gz` & `tmp/waveformtools-2023.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveformtools-2023.5.19.tar", last modified: Fri May 19 07:14:07 2023, max compression
+gzip compressed data, was "waveformtools-2023.6.3.tar", last modified: Sat Jun  3 11:00:01 2023, max compression
```

## Comparing `waveformtools-2023.5.19.tar` & `waveformtools-2023.6.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:14:07.263553 waveformtools-2023.5.19/
--rwxrwxrwx   0 root         (0) root         (0)     1075 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8708 2023-05-19 07:14:07.263553 waveformtools-2023.5.19/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      106 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/README
--rwxrwxrwx   0 root         (0) root         (0)     8052 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 07:14:07.263553 waveformtools-2023.5.19/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1396 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:14:07.262554 waveformtools-2023.5.19/waveformtools/
--rw-rw-rw-   0 root         (0) root         (0)     5480 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/BMS.py
--rw-rw-rw-   0 root         (0) root         (0)     9130 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/CoM.py
--rwxrwxrwx   0 root         (0) root         (0)     1284 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10875 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/compare.py
--rw-rw-rw-   0 root         (0) root         (0)    54107 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/dataIO.py
--rw-rw-rw-   0 root         (0) root         (0)     1698 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/diagnostics.py
--rw-rw-rw-   0 root         (0) root         (0)    25348 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/differentiate.py
--rw-rw-rw-   0 root         (0) root         (0)     9106 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/extrapolate.py
--rw-rw-rw-   0 root         (0) root         (0)    14069 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/grids.py
--rw-rw-rw-   0 root         (0) root         (0)    10952 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/integrate.py
--rw-rw-rw-   0 root         (0) root         (0)     7204 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/legacy.py
--rw-rw-rw-   0 root         (0) root         (0)    53835 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/simulations.py
--rw-rw-rw-   0 root         (0) root         (0)     6476 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/spherical.py
--rw-rw-rw-   0 root         (0) root         (0)    12491 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/transforms.py
--rw-rw-rw-   0 root         (0) root         (0)   124986 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/waveforms.py
--rw-rw-rw-   0 root         (0) root         (0)   110367 2023-05-19 07:13:32.000000 waveformtools-2023.5.19/waveformtools/waveformtools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 07:14:07.263553 waveformtools-2023.5.19/waveformtools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8708 2023-05-19 07:14:07.000000 waveformtools-2023.5.19/waveformtools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-19 07:14:07.000000 waveformtools-2023.5.19/waveformtools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 07:14:07.000000 waveformtools-2023.5.19/waveformtools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-19 07:14:07.000000 waveformtools-2023.5.19/waveformtools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-19 07:14:07.000000 waveformtools-2023.5.19/waveformtools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:00:01.870920 waveformtools-2023.6.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1075 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-06-03 11:00:01.869918 waveformtools-2023.6.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      106 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/README
+-rwxrwxrwx   0 root         (0) root         (0)     8103 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 11:00:01.870920 waveformtools-2023.6.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1396 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:00:01.868916 waveformtools-2023.6.3/waveformtools/
+-rw-rw-rw-   0 root         (0) root         (0)     5392 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/BMS.py
+-rw-rw-rw-   0 root         (0) root         (0)     8709 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/CoM.py
+-rwxrwxrwx   0 root         (0) root         (0)     1306 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11540 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)    53234 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/dataIO.py
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/diagnostics.py
+-rw-rw-rw-   0 root         (0) root         (0)    27426 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/differentiate.py
+-rw-rw-rw-   0 root         (0) root         (0)     9304 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/extrapolate.py
+-rw-rw-rw-   0 root         (0) root         (0)    13790 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/grids.py
+-rw-rw-rw-   0 root         (0) root         (0)    11033 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)    29963 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)    56776 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/simulations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6443 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/spherical.py
+-rw-rw-rw-   0 root         (0) root         (0)    12205 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/transforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    65808 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/waveforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    91309 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/waveformtools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:00:01.869918 waveformtools-2023.6.3/waveformtools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-06-03 11:00:01.000000 waveformtools-2023.6.3/waveformtools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-03 11:00:01.000000 waveformtools-2023.6.3/waveformtools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 11:00:01.000000 waveformtools-2023.6.3/waveformtools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-03 11:00:01.000000 waveformtools-2023.6.3/waveformtools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-03 11:00:01.000000 waveformtools-2023.6.3/waveformtools.egg-info/top_level.txt
```

### Comparing `waveformtools-2023.5.19/LICENSE` & `waveformtools-2023.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.5.19/PKG-INFO` & `waveformtools-2023.6.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: waveformtools
-Version: 2023.5.19
-Summary:  Tools for working with numerical relativity and waveforms data 
-Home-page: https://gitlab.com/vaishakp/waveformtools
-Author: Vaishak Prasad
-Author-email: Vaishak Prasad <vaishakprasad@gmail.com>
-Project-URL: Homepage, https://gitlab.com/vaishakp/waveformtools
-Project-URL: Bug Tracker, https://gitlab.com/vaishakp/waveformtools/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-Provides-Extra: EXT
-License-File: LICENSE
-
 [[Project landing page]](https://sites.google.com/view/waveformtools/home)
 [![pipeline status](https://gitlab.com/vaishakp/waveformtools/badges/main/pipeline.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main)
 [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/waveformtools/badge/?version=latest)](https://waveformtools.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://badge.fury.io/py/waveformtools.svg)](https://badge.fury.io/py/waveformtools)
 # Waveformtools 
@@ -125,68 +108,58 @@
 
 * Standard packages (come with full anaconda installation)
     * [`numpy`](http://www.numpy.org/)
     * [`scipy`](http://scipy.org/)
     * [`statistics`](https://docs.python.org/3/library/statistics.html)
     * [`matplotlib`](http://matplotlib.org/)
     * [`h5py`](http://www.h5py.org/)
-* The pyCBC module
-    * [`pyCBC`](https://pycbc.org/).
-* Third party modules
     * [`termcolor`](https://pypi.org/project/termcolor/)
+    * 
+* Optional dependencies (labelled [EXT])
+    * For use with PyCBC data analysis packages.
+        * [`pyCBC`](https://pycbc.org/)
+        * [`lalsuite`](https://git.ligo.org/lscsoft/lalsuite)
+        * [`ligo-common`](https://git.ligo.org/lscsoft/ligo-common)
+    * [`gmpy2`](https://gmpy2.readthedocs.io/en/latest/)
 
 
 ## Recommended method
 
-I recommend installing this module using anaconda with python 3. 
-
-* First, clone this repository:
-
-```sh
-git clone https://gitlab.com/vaishakp/waveformtools.git
-
-```
-
-* Second, create an environment with dependencies resolved, and activate it.
+I recommend installing this module through pypi:
 ```sh
-conda create env -f docs/environment.yml
-conda activate wftools
+pip install waveformtools
 ```
+## Alternate method
 
+Manual install directly from gitlab:
 
-* Third, add the path to the $PYTHONPATH variable
-
-```sh
-PYTHONPATH="/path/to/this/cloned/repo":$PYTHONPATH
-export PYTHONPATH
-```
+```pip install git+https://gitlab.com/vaishakp/waveformtools@main```
 
-* Alternatively, steps 1-2 can be replaced by a manual environment creation and conda package installation.
+Or from a clone:
 
-
-## Manual method
-
-This is not recommended. One can also install this using the pip commands on this git repository:
+* First, clone this repository:
 
 ```sh
-pip install git+https://gitlab.com/vaishakp/waveformtools.git
+git clone https://gitlab.com/vaishakp/waveformtools.git
+
 ```
-or by running python setup file on the cloned repository:
+* Second, run python setup from the `waveformtools` directory:
+```sh
+cd waveformtools
+python setup.py install --prefix="<path to your preferred installation dir>"
+``` 
 
+## Manually setup conda environment
 
+* To create an environment with automatic dependency resolution and activate it, run
 ```sh
-python setyp.py install
+conda create env -f docs/environment.yml
+conda activate wftools
 ```
 
-This is not recommended because of various reasons:
-
-* The commands are better run on user privelages, and using virtual environments, so as to 
-    * not cause system version conflicts 
-    * Avoid dependency issues
-
 
 # Using this code
 ```
 >>> from waveformtools.waveforms import modes_array
 >>> fdir = "<path to data dir>"
 >>> fname = 'ExtrapStrain_RIT-BBH-0001-n100.h5'
 >>> wf1 = modes_array(label='RIT001', spin_weight=-2)
@@ -238,12 +211,17 @@
 
 # Documentation
 
 The documentation for this module is available at [Link to the Documentation](https://waveformtools.readthedocs.io/en/latest/). This was built automatically using Read the Docs.
 
 In some case where the repo has run out of gitlab CI minutes, the documentation is not automatically built. In such cases, we request the user to access the documentation through the `index.html` file in `docs` directory.
 
+
+# Bug tracker
+If you run into any issues while using this package, please report the issue on the [issue tracker](https://gitlab.com/vaishakp/waveformtools/-/issues).
+
+ 
 # Acknowledgements
 
 This project has been hosted, as you can see, on gitlab. Several gitlab tools are used in the deployment of the code, its testing, version control.
 
 The work of this was developed in aiding my PhD work at Inter-University Centre for Astronomy and Astrophysics (IUCAA, Pune, India)](https://www.iucaa.in/). The PhD is in part supported by the [Shyama Prasad Nukherjee Fellowship](https://csirhrdg.res.in/Home/Index/1/Default/2006/59) awarded to me by the [Council of Scientific and Industrial Research (CSIR, India)](https://csirhrdg.res.in/). Resources of the [Inter-University Centre for Astronomy and Astrophysics (IUCAA, Pune, India)](https://www.iucaa.in/) were are used in part.
```

### Comparing `waveformtools-2023.5.19/README.md` & `waveformtools-2023.6.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: waveformtools
+Version: 2023.6.3
+Summary:  Tools for working with numerical relativity and waveforms data 
+Home-page: https://gitlab.com/vaishakp/waveformtools
+Author: Vaishak Prasad
+Author-email: Vaishak Prasad <vaishakprasad@gmail.com>
+Project-URL: Homepage, https://gitlab.com/vaishakp/waveformtools
+Project-URL: Bug Tracker, https://gitlab.com/vaishakp/waveformtools/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+Provides-Extra: EXT
+License-File: LICENSE
+
 [[Project landing page]](https://sites.google.com/view/waveformtools/home)
 [![pipeline status](https://gitlab.com/vaishakp/waveformtools/badges/main/pipeline.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main)
 [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://gitlab.com/vaishakp/waveformtools/commits/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/waveformtools/badge/?version=latest)](https://waveformtools.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://badge.fury.io/py/waveformtools.svg)](https://badge.fury.io/py/waveformtools)
 # Waveformtools 
@@ -108,68 +125,58 @@
 
 * Standard packages (come with full anaconda installation)
     * [`numpy`](http://www.numpy.org/)
     * [`scipy`](http://scipy.org/)
     * [`statistics`](https://docs.python.org/3/library/statistics.html)
     * [`matplotlib`](http://matplotlib.org/)
     * [`h5py`](http://www.h5py.org/)
-* The pyCBC module
-    * [`pyCBC`](https://pycbc.org/).
-* Third party modules
     * [`termcolor`](https://pypi.org/project/termcolor/)
+    * 
+* Optional dependencies (labelled [EXT])
+    * For use with PyCBC data analysis packages.
+        * [`pyCBC`](https://pycbc.org/)
+        * [`lalsuite`](https://git.ligo.org/lscsoft/lalsuite)
+        * [`ligo-common`](https://git.ligo.org/lscsoft/ligo-common)
+    * [`gmpy2`](https://gmpy2.readthedocs.io/en/latest/)
 
 
 ## Recommended method
 
-I recommend installing this module using anaconda with python 3. 
-
-* First, clone this repository:
-
-```sh
-git clone https://gitlab.com/vaishakp/waveformtools.git
-
-```
-
-* Second, create an environment with dependencies resolved, and activate it.
+I recommend installing this module through pypi:
 ```sh
-conda create env -f docs/environment.yml
-conda activate wftools
+pip install waveformtools
 ```
+## Alternate method
 
+Manual install directly from gitlab:
 
-* Third, add the path to the $PYTHONPATH variable
-
-```sh
-PYTHONPATH="/path/to/this/cloned/repo":$PYTHONPATH
-export PYTHONPATH
-```
+```pip install git+https://gitlab.com/vaishakp/waveformtools@main```
 
-* Alternatively, steps 1-2 can be replaced by a manual environment creation and conda package installation.
+Or from a clone:
 
-
-## Manual method
-
-This is not recommended. One can also install this using the pip commands on this git repository:
+* First, clone this repository:
 
 ```sh
-pip install git+https://gitlab.com/vaishakp/waveformtools.git
+git clone https://gitlab.com/vaishakp/waveformtools.git
+
 ```
-or by running python setup file on the cloned repository:
+* Second, run python setup from the `waveformtools` directory:
+```sh
+cd waveformtools
+python setup.py install --prefix="<path to your preferred installation dir>"
+``` 
 
+## Manually setup conda environment
 
+* To create an environment with automatic dependency resolution and activate it, run
 ```sh
-python setyp.py install
+conda create env -f docs/environment.yml
+conda activate wftools
 ```
 
-This is not recommended because of various reasons:
-
-* The commands are better run on user privelages, and using virtual environments, so as to 
-    * not cause system version conflicts 
-    * Avoid dependency issues
-
 
 # Using this code
 ```
 >>> from waveformtools.waveforms import modes_array
 >>> fdir = "<path to data dir>"
 >>> fname = 'ExtrapStrain_RIT-BBH-0001-n100.h5'
 >>> wf1 = modes_array(label='RIT001', spin_weight=-2)
@@ -221,12 +228,17 @@
 
 # Documentation
 
 The documentation for this module is available at [Link to the Documentation](https://waveformtools.readthedocs.io/en/latest/). This was built automatically using Read the Docs.
 
 In some case where the repo has run out of gitlab CI minutes, the documentation is not automatically built. In such cases, we request the user to access the documentation through the `index.html` file in `docs` directory.
 
+
+# Bug tracker
+If you run into any issues while using this package, please report the issue on the [issue tracker](https://gitlab.com/vaishakp/waveformtools/-/issues).
+
+ 
 # Acknowledgements
 
 This project has been hosted, as you can see, on gitlab. Several gitlab tools are used in the deployment of the code, its testing, version control.
 
 The work of this was developed in aiding my PhD work at Inter-University Centre for Astronomy and Astrophysics (IUCAA, Pune, India)](https://www.iucaa.in/). The PhD is in part supported by the [Shyama Prasad Nukherjee Fellowship](https://csirhrdg.res.in/Home/Index/1/Default/2006/59) awarded to me by the [Council of Scientific and Industrial Research (CSIR, India)](https://csirhrdg.res.in/). Resources of the [Inter-University Centre for Astronomy and Astrophysics (IUCAA, Pune, India)](https://www.iucaa.in/) were are used in part.
```

### Comparing `waveformtools-2023.5.19/pyproject.toml` & `waveformtools-2023.6.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.black]
-line-length = 125
+line-length = 80
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.'MESSAGES CONTROL']
-max-line-length = 125
+max-line-length = 120
 disable= "W0311"
 
 [tool.flake8]
-max-line-length = 125
+max-line-length = 120
 ignore = ['E203']
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
```

### Comparing `waveformtools-2023.5.19/setup.py` & `waveformtools-2023.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # requiremnts directly from toml
 # mreq, oreq = get_requirements()
 
 
 
 setuptools.setup(
     name="waveformtools",
- 	version="2023.05.19",
+ 	version="2023.06.03",
     author="Vaishak Prasad",
     author_email="vaishakprasad@gmail.com",
     description="Functions for handling waveform and numerical relativity data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/vaishakp/waveformtools",
     packages=setuptools.find_packages(),
```

### Comparing `waveformtools-2023.5.19/waveformtools/BMS.py` & `waveformtools-2023.6.3/waveformtools/BMS.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,40 +12,42 @@
 def compute_conformal_k(vec_v, theta, phi, spin_phase=0):
     """Compute the conformal factor for the boost transformation
             :math:`k = \\exp(-2i \\lambda) \\gamma^3
             (1 - \\mathbf{v} \\cdot \\mathbf{r})^3`
 
     Parameters
     ----------
-    vec_v: list
-                    The velocity vector.
+    vec_v : list
+            The velocity vector.
 
-    theta: float
-                    The polar angle :math:`\\theta' in radians.
+    theta : float
+            The polar angle :math:`\\theta' in radians.
 
-    phi: float
-                            The azimuthal angle :math:`\\phi' in radians.
+    phi : float
+          The azimuthal angle :math:`\\phi' in radians.
 
-    spin_phase: float, optional
-                             The spin phase :math:`\\lambda'. Defaults to 0.
+    spin_phase : float, optional
+                 The spin phase :math:`\\lambda'. Defaults to 0.
 
     Returns
     -------
-    conformal_k:	float
-                    The conformal factor for the
-                    boost transformation as defined above.
+    conformal_k : float
+                  The conformal factor for the
+                  boost transformation as defined above.
     """
 
     # unpack the velocity vector
     vel_x, vel_y, vel_z = vec_v
 
     # magnitude of velocity
     mag_v = np.sqrt(vel_x**2 + vel_y**2 + vel_z**2)
     # compute the dot product
-    v_dot_r = np.sin(theta) * (vel_x * np.cos(phi) + vel_y * np.sin(phi)) + vel_z * np.cos(theta)
+    v_dot_r = np.sin(theta) * (
+        vel_x * np.cos(phi) + vel_y * np.sin(phi)
+    ) + vel_z * np.cos(theta)
 
     # Lorentz factor
     gamma = 1.0 / np.sqrt(1 - mag_v**2)
 
     # spin_phase
     spin_factor = np.exp(-2 * 1j * spin_phase)
 
@@ -60,33 +62,29 @@
     :math:`\\alpha(\\theta, \\phi)` given its modes. This method
     just multiplies the alpha modes with their corresponding spherical
     harmonic basis functions and returns the summed result.
 
 
     Parameters
     ----------
-
-    supertransl_alpha_modes:	dict
-                                A dictionary of lists, each sublist
-                                containing the set of super-translation
-                                modes corresponding to a particular
-                                :math:`\\ell'.
-    theta:		float
-                            The polar angle :math:`\\theta'.
-    phi:	float
-                    The azimuthal angle :math:`\\phi'.
+    supertransl_alpha_modes : dict
+                              A dictionary of lists, each sublist
+                              containing the set of super-translation
+                              modes corresponding to a particular
+                              :math:`\\ell'.
+    theta : float
+            The polar angle :math:`\\theta'.
+    phi : float
+          The azimuthal angle :math:`\\phi'.
 
     Returns
     --------
-
-    supertransl_alpha_sphere:		func
-                                    A function on the sphere
-                                    (arguments :math:`\\theta', math:`\\phi').
-
-
+    supertransl_alpha_sphere : func
+                               A function on the sphere
+                               (arguments :math:`\\theta', math:`\\phi').
     """
 
     # For partial evaluation of functions
     # from functools import partial
     message(supertransl_alpha_modes.keys())
     # Find the extreme ell values.
     keys_list = sorted(list(supertransl_alpha_modes.keys()))
@@ -106,57 +104,55 @@
     theta = np.pi / 2
     phi = 0.0
     for item in keys_list:
         ell = int(item[1])
         for m_index in range(2 * ell + 1):
             emm = m_index - ell
             message("ell is", ell, type(ell), "emm is ", emm)
-            supertransl_alpha_sphere += supertransl_alpha_modes[item][m_index] * Yslm(spin_weight, ell, emm, theta, phi)
+            supertransl_alpha_sphere += supertransl_alpha_modes[item][
+                m_index
+            ] * Yslm(spin_weight, ell, emm, theta, phi)
 
     return supertransl_alpha_sphere
 
 
 def boost_waveform(unboosted_waveform, conformal_factor):
     """Boost the waveform given the unboosted waveform and the boost conformal factor.
 
     Parameters
     ----------
-
-    non_boosted_waveform:	list
-                            A list with a single floating point number
-                            or a numpy array of the unboosted waveform.
-                            The waveform can have angular as well as
-                            time dimentions.
-
-                            The nesting order should be that, given the
-                            list `non_boosted_waveform', each item in the
-                            list refers to an array defined on the sphere
-                            at a particular time or frequency. The subitem
-                            will have dimensions [ntheta, nphi].
-
-
-
-    conformal_factor:		float/array
-                            The conformal factor for the Lorentz transformation.
-                            It may be a single floating point number or an array
-                            on a spherical grid. The array will be of dimensions
-                            [ntheta, nphi]
-
-    gridinfo:		class instance
-                    The class instance that contains the properties
-                    of the spherical grid.
+    non_boosted_waveform : list
+                           A list with a single floating point number
+                           or a numpy array of the unboosted waveform.
+                           The waveform can have angular as well as
+                           time dimentions.
+
+                           The nesting order should be that, given the
+                           list `non_boosted_waveform', each item in the
+                           list refers to an array defined on the sphere
+                           at a particular time or frequency. The subitem
+                           will have dimensions [ntheta, nphi].
+    conformal_factor : float/array
+                       The conformal factor for the Lorentz transformation.
+                       It may be a single floating point number or an array
+                       on a spherical grid. The array will be of dimensions
+                       [ntheta, nphi]
+
+    gridinfo : class instance
+               The class instance that contains the properties
+               of the spherical grid.
 
     """
 
     # Find out if the unboosted waveform is a single number or defined on a spherical grid.
     # onepoint = isinstance(unboosted_waveform[0], float)
 
     # if not onepoint:
     # Get the spherical grid shape.
-    # 	ntheta, nphi = np.array(unboosted_waveform[0]).shape
+    #   ntheta, nphi = np.array(unboosted_waveform[0]).shape
 
     # Compute the meshgrid for theta and phi.
     # theta, phi = gridinfo.meshgrid
 
     # A list to store the boosted waveform.
     boosted_waveform = []
```

### Comparing `waveformtools-2023.5.19/waveformtools/CoM.py` & `waveformtools-2023.6.3/waveformtools/CoM.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,45 +8,55 @@
 
 
 def X_com_moments(time_axis, Xcom, order):
     """Compute the nth order temporal moment of the COM coordinates.
 
     Parameters
     ----------
-
-    time_axis:		1d array
-                                    The time axis.
-    Xcom:		list
-                            A list of three 1d arrays, each a 1d array containing the
-                            time series of the x, y and z co-ordinates in that order.
-    order:		int
-                            The order of the moment.
+    time_axis : 1d array
+                The time axis.
+    Xcom : list of arrays
+           A list of three 1d arrays, each a 1d array containing the
+           time series of the x, y and z co-ordinates in that order.
+    order : int
+            The order of the moment.
 
     Returns
     -------
-
-    moments:	list
-                            A list containing three real numbers, one each for the moment
-                            of x, y and z locations.
+    moments : list
+              A list containing three real numbers, one each for the moment
+              of x, y and z locations.
 
     """
     # Initial and final times
     time_i = time_axis[0]
     time_f = time_axis[-1]
 
     duration_t = time_f - time_i
     # Split the data
     x_all, y_all, z_all = Xcom
 
     # Interpolate
     from scipy.interpolate import interp1d
 
-    x_all_int_fun = interp1d(time_axis, np.power(time_axis, order) * x_all / duration_t, kind="quadratic")
-    y_all_int_fun = interp1d(time_axis, np.power(time_axis, order) * y_all / duration_t, kind="quadratic")
-    z_all_int_fun = interp1d(time_axis, np.power(time_axis, order) * z_all / duration_t, kind="quadratic")
+    x_all_int_fun = interp1d(
+        time_axis,
+        np.power(time_axis, order) * x_all / duration_t,
+        kind="quadratic",
+    )
+    y_all_int_fun = interp1d(
+        time_axis,
+        np.power(time_axis, order) * y_all / duration_t,
+        kind="quadratic",
+    )
+    z_all_int_fun = interp1d(
+        time_axis,
+        np.power(time_axis, order) * z_all / duration_t,
+        kind="quadratic",
+    )
 
     int_funcs = [x_all_int_fun, y_all_int_fun, z_all_int_fun]
 
     # Integrate
     from scipy.integrate import quad
 
     moments = {}
@@ -64,109 +74,107 @@
 
 def compute_com_alpha(time_i, time_f, Xcom_0, Xcom_1):
     """Computes the CoM correction alpha parameter: the mean displacement of the system,
     of the COM correction as defined in Woodford et al. 2019 (Phys. Rev. D 100, 124010).
 
     Parameters
     ----------
-
-    time_i:	float
-                            initial time
-    time_f:	float
-                            final time
-    Xcom_0:	list
-                            A list containing the zeroth order moments of the COM.
-    Xcom_1:	list
-                            A list containing the first order moments of the COM.
+    time_i : float
+             initial time
+    time_f : float
+             final time
+    Xcom_0 : list
+             A list containing the zeroth order moments of the COM.
+    Xcom_1 : list
+             A list containing the first order moments of the COM.
 
     Returns
     -------
-
-    com_alpha:		list
-                                    The list containig the alpha parameter vector
+    com_alpha : list
+                The list containig the alpha parameter vector
 
     """
 
     com_alpha = (
-        4 * (time_f**2 + time_f * time_i + time_i**2) * np.array(Xcom_0) - 6 * (time_f + time_i) * np.array(Xcom_1)
+        4 * (time_f**2 + time_f * time_i + time_i**2) * np.array(Xcom_0)
+        - 6 * (time_f + time_i) * np.array(Xcom_1)
     ) / (time_f - time_i) ** 2
 
     return com_alpha
 
 
 def compute_com_beta(time_i, time_f, Xcom_0, Xcom_1):
     """Computes the CoM beta parameter: the mean drift of the system,
     of the COM correction as defined in Woodford et al. 2019 (Phys. Rev. D 100, 124010).
 
     Parameters
     ----------
-
-    time_i:	 float
-                             initial time
-    time_f:	float
-                            final time
-    Xcom_0:	list
-                            A list containing the zeroth order moments of the COM.
-    Xcom_1:	list
-                            A list containing the first order moments of the COM.
+    time_i : float
+             initial time
+    time_f : float
+             final time
+    Xcom_0 : list
+             A list containing the zeroth order moments of the COM.
+    Xcom_1 : list
+             A list containing the first order moments of the COM.
 
     Returns
     -------
-
-    com_beta:		list
-                            The list containig the alpha parameter vector
+    com_beta : list
+                The list containig the alpha parameter vector
 
     """
 
-    com_beta = (12 * (Xcom_1) - 6 * (time_f + time_i) * Xcom_0) / (time_f - time_i) ** 2
+    com_beta = (12 * (Xcom_1) - 6 * (time_f + time_i) * Xcom_0) / (
+        time_f - time_i
+    ) ** 2
 
     return com_beta
 
 
 def compute_conformal_k(vec_v, info, spin_phase=0):
     """Compute the conformal factor for the boost transformation
             :math:`k = \\exp(-2i \\lambda) \\gamma^3 (1 - \\mathbf{v} \\cdot \\mathbf{r})^3
 
-    Inputs
-    ------
+    Parameters
+    ----------
+    vec_v : list
+            A list of 2d arrays containing
+            the velocity vector in the form
+            [vec_x, vec_y, vec_z].
+
+    spin_phase : float, optional
+                 The spin phase :math:`\\lambda'. Defaults to 0.
+    info : class instance
+           An instance of the class `grids.sp_grid`
+           that contains information about the
+           spherical grid being used for the
+           transformations.
 
-    vec_v:		list
-                            A list of 2d arrays containing
-                            the velocity vector in the form
-                            [vec_x, vec_y, vec_z].
-
-    spin_phase:	float, optional
-                                    The spin phase :math:`\\lambda'. Defaults to 0.
-
-    info:		class instance
-                            An instance of the class `grids.sp_grid`
-                            that contains information about the
-                            spherical grid being used for the
-                            transformations.
     Returns
     --------
-
-    conformal_k:	2d array
-                                    The conformal factor for the boost transformation
-                                    as defined above.
-
+    conformal_k : 2d array
+                  The conformal factor for the boost transformation
+                  as defined above.
 
     """
 
     # unpack the velocity vector
     vel_x, vel_y, vel_z = vec_v
 
     # magnitude of velocity
     mag_v = np.sqrt(vel_x**2 + vel_y**2 + vel_z**2)
 
     # Compute the 2d co-ordinate axis on the sphere
     theta, phi = info.meshgrid
 
     # compute the dot product
-    v_dot_r = np.sin(theta) * (vel_x * np.cos(phi) + vel_y * np.sin(phi)) + vel_z * np.cos(theta)
+    v_dot_r = np.sin(theta) * (
+        vel_x * np.cos(phi) + vel_y * np.sin(phi)
+    ) + vel_z * np.cos(theta)
 
     # Lorentz factor
     gamma = 1.0 / np.sqrt(1 - mag_v**2)
 
     # spin_phase
     spin_factor = np.exp(-2 * 1j * spin_phase)
 
@@ -179,28 +187,26 @@
 def compute_translation_alpha_modes(time_axis, com_alpha, com_beta):
     """Compute the translation scalar :math:`\\alpha` in its spherical harmonic
     components given the mean motion of the centre of mass. These are basically
     the quantities in Eq. (4-5d) in the reference Woodford et al. 2019.
 
     Parameters
     ----------
-
-    time_axis:		1d array
-                                    The 1D array containing the time axis of the simulation.
-    alpha:		1d array
-                            The 1D array containing the mean co-ordinate displacement of the COM of the system.
-    beta:		1d array
-                            The 1D array containing the mean co-ordinate velocity of the COM.
+    time_axis : 1d array
+                The 1D array containing the time axis of the simulation.
+    alpha : 1d array
+            The 1D array containing the mean co-ordinate displacement of the COM of the system.
+    beta : 1d array
+           The 1D array containing the mean co-ordinate velocity of the COM.
 
     Returns
     -------
-
-    alpha_modes :   modes_array
-                    A `waveforms.modes_array` object containing the SH
-                    decomposition of the 'Alpha' supertranslation variable.
+    alpha_modes : modes_array
+                  A `waveforms.modes_array` object containing the SH
+                  decomposition of the 'Alpha' supertranslation variable.
 
     """
 
     # Define the total displacement
     delta_t = 0
     delta_x = com_alpha[0] + com_beta[0] * time_axis
     delta_y = com_alpha[1] + com_beta[1] * time_axis
@@ -227,64 +233,64 @@
     alpha_modes.set_mode_data(ell_value=1, emm_value=-1, data=Alpha_1m1)
     # l1m0
     alpha_modes.set_mode_data(ell_value=1, emm_value=0, data=Alpha_10)
     # l1m1
     alpha_modes.set_mode_data(ell_value=1, emm_value=1, data=Alpha_11)
 
     # Combine into one list
-    # modes	   = { 'l0' : [Alpha_00], 'l1' : [Alpha_1m1, Alpha_10, Alpha_11]}
+    # modes    = { 'l0' : [Alpha_00], 'l1' : [Alpha_1m1, Alpha_10, Alpha_11]}
     modes_list = [[0, [0]], [1, [-1, 0, 1]]]
     alpha_modes.modes_list = modes_list
     alpha_modes.time_axis = time_axis
     alpha_modes.ell_max = 1
     alpha_modes.spin_weight = -1
     return alpha_modes
 
 
 def boost_waveform(unboosted_waveform, conformal_factor):
     """Boost the waveform given the unboosted waveform and the boost conformal factor.
 
     Parameters
     ----------
+    unboosted_waveform : spherical_array
+                         A class instance of `spherical array`.
 
-    unboosted_waveform:		spherical_array
-                                                            A class instance of `spherical array`.
-
-    conformal_factor:		2d array
-                            The conformal factor for the Lorentz transformation.
-                            It may be a single floating point number or an array
-                            on a spherical grid. The array will be of dimensions
-                            [ntheta, nphi].
-
-    gridinfo:		class instance
-                    The class instance that contains the properties of the spherical grid.
+    conformal_factor : 2d array
+                       The conformal factor for the Lorentz transformation.
+                       It may be a single floating point number or an array
+                       on a spherical grid. The array will be of dimensions
+                       [ntheta, nphi].
 
+    gridinfo : class instance
+               The class instance that contains the properties of the spherical grid.
 
     Returns
     -------
-
-    boosted_waveform:	  sp_array
-                                              The class instance `sp_array` that
-                                              contains the boosted waveform.
+    boosted_waveform : sp_array
+                       The class instance `sp_array` that
+                       contains the boosted waveform.
     """
 
     from waveforms import spherical_array
 
     # Compute the meshgrid for theta and phi.
     # theta, phi = unboosted_waveform.gridinfo.meshgrid
-    # 	= unboosted_waveform.gridinfo.phi
+    #   = unboosted_waveform.gridinfo.phi
     # A list to store the boosted waveform.
     boosted_waveform_data = []
 
     for item in unboosted_waveform.data:
         # Compute the boosted waveform on the spherical grid on all the elements.
 
         # conformal_k_on_sphere = compute_conformal_k(vec_v, theta, phi)
         boosted_waveform_item = conformal_factor * item
 
         boosted_waveform_data.append(boosted_waveform_item)
 
     # Construct a 2d waveform array object
-    boosted_waveform = spherical_array(gridinfo=unboosted_waveform.gridinfo, data=np.array(boosted_waveform_data))
+    boosted_waveform = spherical_array(
+        gridinfo=unboosted_waveform.gridinfo,
+        data=np.array(boosted_waveform_data),
+    )
     boosted_waveform.label = "boosted"
 
     return boosted_waveform
```

### Comparing `waveformtools-2023.5.19/waveformtools/__init__.py` & `waveformtools-2023.6.3/waveformtools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     # print(package_directory)
     # Open the file
     vers = "-1"
     try:
         with open(package_directory + "/../public/version", "r") as vers_file:
             vers = vers_file.readlines()[0]
     except Exception as excep:
-        print("This is not a git repo! please use the version attribute instead!")
+        print(
+            "This is not a git repo! please use the version attribute instead!"
+        )
     # with open(package_directory + "/../public/date.txt", "r") as vers_file:
     # vers = vers_file.read()[:10]
 
     return vers
 
 
-__version__ = "2023.05.19"
+__version__ = "2023.06.03"
```

### Comparing `waveformtools-2023.5.19/waveformtools/compare.py` & `waveformtools-2023.6.3/waveformtools/compare.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,29 +23,37 @@
 # plt.rcParams.update({"axes.labelweight" : "bold"})
 plt.rcParams.update({"font.style": "normal"})
 plt.rcParams.update({"legend.markerscale": 9})
 
 # from waveformtools.waveforms import modes_array
 
 
-def plot_modes(wf1, nmodes=3, save_fig=False, xlim=[-1200, 100], ylim="auto", nstop=1, plot22=False):
+def plot_modes(
+    wf1,
+    nmodes=3,
+    save_fig=False,
+    xlim=[-1200, 100],
+    ylim="auto",
+    nstop=1,
+    plot22=False,
+):
     """Plot the first `nmodes` dominant modes of
     the input waveforms
 
     Parameters
     ----------
-    wf:           modes_array
-                              The list of `modes_array` waveforms
-                              to plot.
-    nmodes:     int
-                            The number of modes to plot.
+    wf : modes_array
+         The list of `modes_array` waveforms
+         to plot.
+    nmodes : int
+             The number of modes to plot.
     xlim : list
            [xmin, xmax] limits to plot.
-    tol:    float
-                    The tolerance to detect the modes.
+    tol : float
+          The tolerance to detect the modes.
 
     Returns
     -------
     Plots.
     """
 
     from waveformtools.waveformtools import xtract_cphase
@@ -97,28 +105,50 @@
         for emm in emm_list:
             mode_values = wf1.mode(ell, emm)
             mode_amp = np.absolute(mode_values)
             max_mode_value = np.amax(mode_values)
 
             mode_phase = xtract_cphase(mode_values.real, mode_values.imag)
 
-            ax1.scatter(wf1.time_axis[:], mode_amp[:], label=rf"$\ell${ell}$m${emm}", s=1, alpha=0.2 * abs(emm) % 1)
-            ax2.scatter(wf1.time_axis[:], abs(mode_phase[:]), label=rf"$\ell${ell}$m${emm}", s=1)
+            ax1.scatter(
+                wf1.time_axis[:],
+                mode_amp[:],
+                label=rf"$\ell${ell}$m${emm}",
+                s=1,
+                alpha=0.2 * abs(emm) % 1,
+            )
+            ax2.scatter(
+                wf1.time_axis[:],
+                abs(mode_phase[:]),
+                label=rf"$\ell${ell}$m${emm}",
+                s=1,
+            )
 
     if plot22:
         ell = 2
         emm = 2
         mode_values = wf1.mode(ell, emm)
         mode_amp = np.absolute(mode_values)
         max_mode_value = np.amax(mode_values)
 
         mode_phase = xtract_cphase(mode_values.real, mode_values.imag)
 
-        ax1.scatter(wf1.time_axis[:], mode_amp[:], label=rf"$\ell${ell}$m${emm}", s=1, alpha=0.2 * abs(emm) % 1)
-        ax2.scatter(wf1.time_axis[:], abs(mode_phase[:]), label=rf"$\ell${ell}$m${emm}", s=1)
+        ax1.scatter(
+            wf1.time_axis[:],
+            mode_amp[:],
+            label=rf"$\ell${ell}$m${emm}",
+            s=1,
+            alpha=0.2 * abs(emm) % 1,
+        )
+        ax2.scatter(
+            wf1.time_axis[:],
+            abs(mode_phase[:]),
+            label=rf"$\ell${ell}$m${emm}",
+            s=1,
+        )
 
     ax1.grid(which="both")
     ax2.grid(which="both")
     ax1.legend()
     ax2.legend()
     plt.tight_layout()
     ax1.set_xlabel("t/M")
@@ -143,28 +173,34 @@
         fig1.savefig(f"{wf1.label}_waveform_amp_modes.pdf")
         fig2.savefig(f"{wf1.label}_waveform_phase_modes.pdf")
 
     plt.show()
 
 
 def plot_mode_differences(
-    waveforms, nmodes=3, save_fig=False, xlabel="t/M", ylabel=r"r\Psi_{4}^{(\ell m)}", labels=None, xlim=[-1000, 100]
+    waveforms,
+    nmodes=3,
+    save_fig=False,
+    xlabel="t/M",
+    ylabel=r"r\Psi_{4}^{(\ell m)}",
+    labels=None,
+    xlim=[-1000, 100],
 ):
     """Plot the fractional difference of the first `nmodes`
     dominant modes of the input waveforms.
 
     Parameters
     ----------
-    waveforms:    modes_array
-                              The list of `modes_array` waveforms
-                              to plot.
-    nmodes:     int
-                            The number of modes to plot.
-    tol:    float
-                    The tolerance to detect the modes.
+    waveforms : modes_array
+                The list of `modes_array` waveforms
+                to plot.
+    nmodes : int
+             The number of modes to plot.
+    tol : float
+          The tolerance to detect the modes.
 
     Returns
     -------
     Plots.
     """
 
     # For phase computation.
@@ -270,56 +306,78 @@
             mode_phase_resam0 = mode_phase_int_fun0(new_time_axis)
 
             for index, wfx in enumerate(waveforms[1:]):
                 label = wfx.label  # labels[index+1]
 
                 mode_valuesx = wfx.mode(ell, emm)
                 mode_ampx = np.absolute(mode_valuesx)
-                mode_phasex = xtract_cphase(mode_valuesx.real, mode_valuesx.imag)
+                mode_phasex = xtract_cphase(
+                    mode_valuesx.real, mode_valuesx.imag
+                )
 
                 mode_amp_int_funx = interp1d(wfx.time_axis, mode_ampx)
                 mode_amp_resamx = mode_amp_int_funx(new_time_axis)
 
                 mode_phase_int_funx = interp1d(wfx.time_axis, mode_phasex)
                 mode_phase_resamx = mode_phase_int_funx(new_time_axis)
 
                 start_ind = int((-new_time_axis[0] - start_time) / new_delta_t)
 
                 # message(start_ind)
                 # Remove the man phase shift
                 mean_phase_shift = np.mean(
-                    mode_phase_resamx[start_ind : start_ind + dindex] - mode_phase_resam0[start_ind : start_ind + dindex]
+                    mode_phase_resamx[start_ind : start_ind + dindex]
+                    - mode_phase_resam0[start_ind : start_ind + dindex]
                 )
 
                 # mean_phase_shift = np.mean(
                 #   mode_phase_resamx - mode_phase_resam0
                 # )
 
                 # message(mean_phase_shift)
-                delta_mode_ampx = (mode_amp_resamx - mode_amp_resam0) / mode_amp_resam0
-                delta_mode_phasex = (mode_phase_resamx - mode_phase_resam0 - mean_phase_shift) / mode_phase_resam0
+                delta_mode_ampx = (
+                    mode_amp_resamx - mode_amp_resam0
+                ) / mode_amp_resam0
+                delta_mode_phasex = (
+                    mode_phase_resamx - mode_phase_resam0 - mean_phase_shift
+                ) / mode_phase_resam0
 
-                rms_amp_diff = np.sqrt(np.sum(delta_mode_ampx**2) / (len(delta_mode_ampx)))
-                rms_phase_diff = np.sqrt(np.sum(delta_mode_phasex**2) / (len(delta_mode_phasex)))
+                rms_amp_diff = np.sqrt(
+                    np.sum(delta_mode_ampx**2) / (len(delta_mode_ampx))
+                )
+                rms_phase_diff = np.sqrt(
+                    np.sum(delta_mode_phasex**2) / (len(delta_mode_phasex))
+                )
                 max_phase_diff = np.amax(np.absolute(delta_mode_phasex))
                 max_phase_diff_loc = np.argmax(np.absolute(delta_mode_phasex))
                 max_phase_diff_time = new_time_axis[max_phase_diff_loc]
                 cumulative_diff.update(
-                    {f"l{ell}m{emm}": [rms_amp_diff, rms_phase_diff, [max_phase_diff, max_phase_diff_time]]}
+                    {
+                        f"l{ell}m{emm}": [
+                            rms_amp_diff,
+                            rms_phase_diff,
+                            [max_phase_diff, max_phase_diff_time],
+                        ]
+                    }
                 )
                 max_mode_value = np.amax(mode_values)
 
             ax1.scatter(
                 new_time_axis[:],
                 abs(delta_mode_ampx[:]),
                 label=rf"{label} $\ell${ell}$m${emm}",
                 s=1,
                 alpha=0.2 * abs(emm) % 1,
             )
-            ax2.scatter(new_time_axis[:], abs(delta_mode_phasex[:]), label=rf"{label} $\ell${ell}$m${emm}", s=1)
+            ax2.scatter(
+                new_time_axis[:],
+                abs(delta_mode_phasex[:]),
+                label=rf"{label} $\ell${ell}$m${emm}",
+                s=1,
+            )
 
     ax1.grid(which="both")
     ax2.grid(which="both")
     ax1.legend()
     ax2.legend()
     plt.tight_layout()
     ax1.set_xlabel(xlabel)
```

### Comparing `waveformtools-2023.5.19/waveformtools/dataIO.py` & `waveformtools-2023.6.3/waveformtools/dataIO.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,119 +11,129 @@
 import sys
 
 import h5py
 import numpy as np
 from scipy.interpolate import InterpolatedUnivariateSpline as interp
 from scipy.interpolate import interp1d
 
-from waveformtools.waveformtools import interp_resam_wfs, message, xtract_camp_phase
+from waveformtools.waveformtools import (
+    cleandata,
+    interp_resam_wfs,
+    message,
+    xtract_camp_phase,
+)
 
 ##########################
 # RIT data
 ##########################
 
 
 def _key_gen(ell, emm, extras=None):
-    """Generates strings to be used as keys for
-    managing h5 datasets.
+	"""Generates strings to be used as keys for
+	managing h5 datasets.
 
     Parameters
     ----------
-    ell:	int
-                                    The polar angular mode number
-                                    :math:`\\ell`.
+    ell : int
+          The polar angular mode number
+          :math:`\\ell`.
     emm : int
-                      The aximuthal angular mode number
-                      :math:`m`.
-    extras: str
-                            Any extra string to be appended
-                            to the end of the key.
+          The aximuthal angular mode number
+          :math:`m`.
+    extras : str
+             Any extra string to be appended
+             to the end of the key.
 
     Returns
     -------
-    key:	 str
-                                     A string key.
+    key : str
+          A key string.
     """
 
-    key = f"l{ell}_m{emm}"
+	key = f"l{ell}_m{emm}"
 
-    if extras is not None:
-        key += f"_{extras}"
-        # message('adding rext')
+	if extras is not None:
+		key += f"_{extras}"
+		# message('adding rext')
 
-    return key
+	return key
 
 
 def get_ell_max_from_keys(all_keys):
-    """Get ell max from a list of keys.
+	"""Get ell max from a list of keys.
 
     Parameters
     ----------
-    all_keys :	list
-                    A list of strings string containing the modes keys.
+    all_keys : list
+               A list of strings string containing the modes keys.
     Returns
     -------
     ell_max : int
-                      The maximum available ell.
+              The maximum available ell.
     """
 
-    # available mode numbers
-    all_ell_modes = set({})
+	# available mode numbers
+	all_ell_modes = set({})
 
-    # Get mode numbers
-    for item in all_keys:
-        this_match = re.search("\_l\d\_", item)
-
-        if this_match is None:
-            # message(f'Skipped file {item}')
-            continue
+	# Get mode numbers
+	for item in all_keys:
+		this_match = re.search("\_l\d\_", item)
+
+		if this_match is None:
+			# message(f'Skipped file {item}')
+			continue
 
         # message('Match found', this_match.string)
         s1, s2 = this_match.span()
         this_ell = int(this_match.string[s1 + 2 : s2 - 1])
         # message(this_ell)
 
-        all_ell_modes.add(this_ell)
+		all_ell_modes.add(this_ell)
 
-    ell_max = max(all_ell_modes)
-    return ell_max
+	ell_max = max(all_ell_modes)
+	return ell_max
 
 
 def get_ell_max_from_file(data_dir, var_type="Psi4", file_name="*.h5"):
     """Get the largest available mode number from available data in files.
 
     Parameters
     ----------
-    data_dir :	string
-                            A string containing the directory path where the mode files can be found.
-    var_type: string, optional
-                    A string that denotes the variable that is being loaded. Options are Psi4 and strain.
-                    The former is the default.
+    data_dir : string
+               A string containing the directory path where the mode files can be found.
+    var_type : string, optional
+               A string that denotes the variable
+               that is being loaded. Options are Psi4
+               and strain. The former is the default.
     file_name : string, optional
-                      The h5 file that contains the modes data. It defaults to the only file in the directory.
-                      If there are multiple files, it throws an error.
+                The h5 file that contains the modes data.
+                It defaults to the only file in the directory.
+                If there are multiple files, it throws an error.
+
     Returns
     -------
     ell_max : int
-                      The maximum available ell.
+              The maximum available ell.
     keys_list : list
-                            A list of data access keys.
+                A list of data access keys.
 
     Notes
     -----
     Reads in various ASCII dat files for RIT Psi4, h5 files for RIT strain and gen strain.
     """
 
     if var_type == "Psi4":
         import os
 
         # Get files
         all_fnames = os.listdir(data_dir)
         # Get only files
-        all_fnames = [item for item in all_fnames if os.path.isfile(f"{data_dir}/{item}")]
+        all_fnames = [
+            item for item in all_fnames if os.path.isfile(f"{data_dir}/{item}")
+        ]
 
     elif var_type == "Strain":
         # import h5py
         message("Fetching all keys from H5 file", message_verbosity=2)
         data_file = h5py.File(f"{data_dir}/{file_name}")
         all_fnames = list(data_file.keys())
         data_file.close()
@@ -137,262 +147,267 @@
 
     ell_max = get_ell_max_from_keys(all_fnames)
 
     return ell_max, all_fnames
 
 
 def _get_modes_list_from_keys(keys_list, r_ext):
-    """Get the modes list from the keys list
-    of an hdf file.
+	"""Get the modes list from the keys list
+	of an hdf file.
 
     Parameters
     ----------
-    keys_list:		list
-                                    The list containing all the keys
-    r_ext:		float
-                            The extraction radius of the data.
+    keys_list : list
+                The list containing all the keys
+    r_ext : float
+            The extraction radius of the data.
 
     Returns
     -------
-    modes_list: list
-                                    The list of modes.
+    modes_list : list
+                 The list of modes.
     """
 
-    # Sort the keys to ensure a nice
-    # modes list structure.
-    keys_list_orig = sorted(keys_list)
+	# Sort the keys to ensure a nice
+	# modes list structure.
+	keys_list_orig = sorted(keys_list)
 
-    if r_ext != -1:
-        keys_list = [item for item in keys_list_orig if f"r{r_ext}" in item]
+	if r_ext != -1:
+		keys_list = [item for item in keys_list_orig if f"r{r_ext}" in item]
 
         if keys_list == []:
-            message("Got an empty list. Searching for r_ext value in key string")
+            message(
+                "Got an empty list. Searching for r_ext value in key string"
+            )
             keys_list = [item for item in keys_list_orig if f"{r_ext}" in item]
 
-    # message('List of keys received', keys_list)
-    # The list of modes.
-    modes_list = []
-
-    # Initialize the emm modes sublist.
-    emm_modes_for_ell = []
-
-    # Present ell value to
-    # initialize the mode concatenation.
-    ell_old = 0
+	# message('List of keys received', keys_list)
+	# The list of modes.
+	modes_list = []
+
+	# Initialize the emm modes sublist.
+	emm_modes_for_ell = []
+
+	# Present ell value to
+	# initialize the mode concatenation.
+	ell_old = 0
+
+	for key in keys_list:
+		# message(key)
+		# Get the ell value
+		ell_value, emm_value = _get_ell_emm_from_key(key)
+
+		if ell_value != ell_old:
+			# If the ell value has changed,
+			# update the modes list before moving
+			# onto the next ell value.
+			modes_list.append([ell_old, emm_modes_for_ell])
+			# The present ell value is the old
+			# ell value.
+			ell_old = ell_value
+
+			# Reset the ell_mode list.
+			emm_modes_for_ell = []
 
-    for key in keys_list:
-        # message(key)
-        # Get the ell value
-        ell_value, emm_value = _get_ell_emm_from_key(key)
-
-        if ell_value != ell_old:
-            # If the ell value has changed,
-            # update the modes list before moving
-            # onto the next ell value.
-            modes_list.append([ell_old, emm_modes_for_ell])
-            # The present ell value is the old
-            # ell value.
-            ell_old = ell_value
-
-            # Reset the ell_mode list.
-            emm_modes_for_ell = []
-
-        # Update it with the new emm mode.
-        emm_modes_for_ell.append(emm_value)
+		# Update it with the new emm mode.
+		emm_modes_for_ell.append(emm_value)
 
-    modes_list.append([ell_value, emm_modes_for_ell])
+	modes_list.append([ell_value, emm_modes_for_ell])
 
-    return modes_list
+	return modes_list
 
 
 def _get_ell_emm_from_key(key):
-    """Get the :math:`\\ell` and :math:`m` values
-    from a given key string of an hdf file.
+	"""Get the :math:`\\ell` and :math:`m` values
+	from a given key string of an hdf file.
 
     Parameters
     ----------
-    key:	str
-                    The input key string
+    key : str
+          The input key string
 
     Returns
     -------
-    ell_value:		int
-                                    The :math:`\\ell` value
-    emm_value:		int
-                                    The :math:`m` value.
+    ell_value : int
+                The :math:`\\ell` value
+    emm_value : int
+                The :math:`m` value.
 
     Notes
     -----
-
     Assumes that the input string has :math:`\\ell` and :math:`m` values
     in the form `l{int}m{int}`.
 
-    """
+	"""
 
-    import re
+	import re
 
     str_match = re.search("l\d*", key)
     ell_str_start = str_match.start()
     ell_str_end = str_match.end()
     ell_value = int(key[ell_str_start + 1 : ell_str_end])
 
     str_match = re.search("m-*\d*", key)
     emm_str_start = str_match.start()
     emm_str_end = str_match.end()
     emm_value = int(key[emm_str_start + 1 : emm_str_end])
 
-    return ell_value, emm_value
+	return ell_value, emm_value
 
 
 def get_iteration_numbers_from_keys(keys_list):
-    """Get the iteration number from keys.
+	"""Get the iteration number from keys.
 
     Parameters
     ----------
-    keys_list: list
-                       The list of keys.
+    keys_list : list
+                The list of keys.
 
     Returns
     -------
-    iteration_numbers: list
-                                            The list containing the iteration
-                                            numbers.
+    iteration_numbers : list
+                        The list containing the iteration
+                        numbers.
     """
     import re
 
-    iteration_numbers = []
+	iteration_numbers = []
 
     for key in keys_list:
         str_match = re.search(" it=\d* ", key)
         it_str_start = str_match.start()
         it_str_end = str_match.end()
         it_value = int(key[it_str_start + 4 : it_str_end])
         iteration_numbers.append(it_value)
 
-    return iteration_numbers
+	return iteration_numbers
 
 
 def construct_mode_list(ell_max, spin_weight):
-    """
-    Construct a modes list in the form [[ell1, [emm1, emm2, ...], [ell2, [emm..]],..]
+    """Construct a modes list in the form
+    [[ell1, [emm1, emm2, ...], [ell2, [emm..]],..]
     given the :math:`\\ell_{max}.`
 
     Parameters
     ----------
     spin_weight : int
-                            The spin weight of the modes.
+                  The spin weight of the modes.
     ell_max : int
-                      The :math:`\\ell_{max}` of the modes list.
+              The :math:`\\ell_{max}` of the modes list.
 
     Returns
     -------
-
     modes_list : list
-                             A list containg the mode indices lists.
+                 A list containg the mode indices lists.
 
-    Notes
-    -----
-    The modes list is the form which the `waveform` object understands.
-    """
+	Notes
+	-----
+	The modes list is the form which the `waveform` object understands.
+	"""
 
-    # The modes list.
-    modes_list = []
+	# The modes list.
+	modes_list = []
 
-    for ell_index in range(abs(spin_weight), ell_max + 1):
-        # Append all emm modes for each ell mode.
-        modes_list.append([ell_index, list(range(-ell_index, ell_index + 1))])
+	for ell_index in range(abs(spin_weight), ell_max + 1):
+		# Append all emm modes for each ell mode.
+		modes_list.append([ell_index, list(range(-ell_index, ell_index + 1))])
 
-    return modes_list
+	return modes_list
 
 
 def sort_keys(modes_keys_list):
     """Sort the keys in a list based on
-            its iteration number
+    its iteration number
 
     Parameters
     ----------
-    modes_keys_list: str
-                                     The list of keys.
+    modes_keys_list : str
+                      The list of keys.
 
     Returns
     -------
-    sorted_modes_keys_list: str
-                                                    The sorted list.
+    sorted_modes_keys_list : str
+                             The sorted list.
     """
 
-    iteration_numbers = get_iteration_numbers_from_keys(modes_keys_list)
+	iteration_numbers = get_iteration_numbers_from_keys(modes_keys_list)
 
-    sargs = np.argsort(iteration_numbers)
+	sargs = np.argsort(iteration_numbers)
 
-    sorted_modes_keys_list = np.array(modes_keys_list)[sargs]
+	sorted_modes_keys_list = np.array(modes_keys_list)[sargs]
 
-    return sorted_modes_keys_list
+	return sorted_modes_keys_list
 
 
 def load_RIT_Psi4_data_from_disk(
-    wfa=None,
-    data_dir="./",
-    label="RIT_rPsi4inf",
-    ell_max=None,
-    modes_list=None,
-    save_as_ma=False,
-    spin_weight=-2,
-    resam_type="finest",
-    interp_kind="cubic",
-    crop=False,
-    centre=False,
+	wfa=None,
+	data_dir="./",
+	label="RIT_rPsi4inf",
+	ell_max=None,
+	modes_list=None,
+	save_as_ma=False,
+	spin_weight=-2,
+	resam_type="finest",
+	interp_kind="cubic",
+	crop=False,
+	centre=False,
 ):
     """Load the Psi4 waveforms from the RIT catalogue
     from ASCII files from disk.
 
     Parameters
     ----------
-    wfa  :	waveforms
-                    An instance of the waveforms class. Updates this instance if provided, else creates a new instance.
-    data_dir :	string
-                    A string containing the directory path where the mode files can be found.
+    wfa : waveforms
+          An instance of the waveforms class. Updates this instance
+          if provided, else creates a new instance.
+    data_dir : string
+               A string containing the directory path where
+               the mode files can be found.
     label : string, optional
-                    The label of the modes_array object.
+            The label of the modes_array object.
     ell_max : int, optional
-                            The maximum mode number to load. If not specified,
-                            then all available modes are loaded.
+              The maximum mode number to load. If not specified,
+              then all available modes are loaded.
     save_as_ma : bool, optional
-                             Save to disk again as a modes_array h5 file?
+                 Save to disk again as a modes_array h5 file?
     spin_weight : int, optional
-                              The spin weight of the object. Used for filtering modes.
-                              Defaults to -2.
+                  The spin weight of the object. Used for filtering modes.
+                  Defaults to -2.
     resam_type : string, float, optional
-                             The type of resampling to do. Options are finest and coarsest, and user input float.
+                 The type of resampling to do. Options are the
+                 `finest` and `coarsest`, or user input float.
     interp_kind : string, optional
-                              The interpolation type to use. Default is cubic.
+                  The interpolation type to use. Default is cubic.
 
     Returns
     -------
-
     rit_modes_array : modes_array
-                                            A modes_array instance containing the loaded modes.
+                      A modes_array instance containing the loaded modes.
 
     Notes
     -----
-    It seems like the time axis of individual modes are identical to each other. Hence, one need not worry about
+    It seems like the time axis of individual modes are
+    identical to each other. Hence, one need not worry about
     choosing the time domain. This may change in future.
     """
     message("Loading RIT Psi4 type data.", message_verbosity=1)
     from waveformtools.waveforms import modes_array
 
     if not wfa:
-        wfa = modes_array(label=label, data_dir=data_dir, modes_list=wf_modes_list)
+        wfa = modes_array(label=label, data_dir=data_dir, modes_list=modes_list)
 
     if modes_list is None:
         # Max available mode l.
         if ell_max is None:
             ell_max, _ = get_ell_max_from_file(data_dir)
 
         # Construct a modes list
-        wf_modes_list = construct_mode_list(ell_max=ell_max, spin_weight=spin_weight)
+        wf_modes_list = construct_mode_list(
+            ell_max=ell_max, spin_weight=spin_weight
+        )
 
         message("The modes list is", wf_modes_list, message_verbosity=2)
 
     else:
         ell_max = max([item[0] for item in modes_list])
         wf_modes_list = modes_list
 
@@ -402,15 +417,17 @@
     # For interpolation
     from scipy.interpolate import interp1d
 
     # Alias of the modes_array
     # label = 'q1a0_a'
     # Create a modes array
     # Enforce only l>2 modes.
-    wf_modes_list = [item for item in wf_modes_list if item[0] >= abs(spin_weight)]
+    wf_modes_list = [
+        item for item in wf_modes_list if item[0] >= abs(spin_weight)
+    ]
 
     # tend = []
     # tstart = []
 
     ##########################################
     # Read in the data
     #########################################
@@ -451,15 +468,17 @@
                     message("Resampling at the coarsest timestep", m_dt)
 
                 if isinstance(resam_type, float):
                     m_dt = resam_type
                     message("Resampling at user defined timestep", m_dt)
 
                 # New (resampled) time axis
-                time_axis = np.arange(wf_psi4_time[0], wf_psi4_time[-1] + m_dt, m_dt)
+                time_axis = np.arange(
+                    wf_psi4_time[0], wf_psi4_time[-1] + m_dt, m_dt
+                )
 
                 # Length of data.
                 data_len = len(time_axis)
 
                 # Create a modes array object
                 wfa.create_modes_array(ell_max=ell_max, data_len=data_len)
 
@@ -478,122 +497,128 @@
             ##############################
 
             Yphase = wf_psi4_file[:, 4]
             Yphase_interp_fun = interp1d(wf_psi4_time, Yphase, kind=interp_kind)
 
             # Resample
 
-            Yphase_resam = Yphase_interp_fun(time_axis)
-
-            ###########################
-            # Load the amplitude data
-            ###########################
-            Yamp = wf_psi4_file[:, 3]
-            Yamp_interp_fun = interp1d(wf_psi4_time, Yamp, kind=interp_kind)
-
-            # Resample
-            Yamp_resam = Yamp_interp_fun(time_axis)
-            wfmode = Yamp_resam * np.exp(1j * Yphase_resam)
-
-            ###################################
-            # Load the modes data
-            ###################################
-
-            wfa.set_mode_data(ell, emm, wfmode)
+			Yphase_resam = Yphase_interp_fun(time_axis)
 
-    wfa.actions += "->load_modes"
-
-    if crop is not False or centre is True:
-        # Trim or recenter
-        if crop is True or centre is True:
-            wfa.trim(trim_upto_time=0)
-            wfa.centered = True
-            wfa.actions += "->recenter"
-
-        elif isinstance(crop, float):
-            wfa.trim(trim_upto_time=crop)
-            wfa.actions += "->crop"
-
-        if save_as_ma is True:
-            # Save the modes array as waveforms hdf file
-            wfa.save_modes(out_file_name="{label}_resam.h5")
-            wfa.actions += "->save_as_wfh5"
-    return wfa
+			###########################
+			# Load the amplitude data
+			###########################
+			Yamp = wf_psi4_file[:, 3]
+			Yamp_interp_fun = interp1d(wf_psi4_time, Yamp, kind=interp_kind)
+
+			# Resample
+			Yamp_resam = Yamp_interp_fun(time_axis)
+			wfmode = Yamp_resam * np.exp(1j * Yphase_resam)
+
+			###################################
+			# Load the modes data
+			###################################
+
+			wfa.set_mode_data(ell, emm, wfmode)
+
+	wfa.actions += "->load_modes"
+
+	if crop is not False or centre is True:
+		# Trim or recenter
+		if crop is True or centre is True:
+			wfa.trim(trim_upto_time=0)
+			wfa.centered = True
+			wfa.actions += "->recenter"
+
+		elif isinstance(crop, float):
+			wfa.trim(trim_upto_time=crop)
+			wfa.actions += "->crop"
+
+		if save_as_ma is True:
+			# Save the modes array as waveforms hdf file
+			wfa.save_modes(out_file_name="{label}_resam.h5")
+			wfa.actions += "->save_as_wfh5"
+	return wfa
 
 
 def load_RIT_Strain_data_from_disk(
-    wfa=None,
-    data_dir="./",
-    file_name="*",
-    label="RIT_strain",
-    spin_weight=-2,
-    ell_max="auto",
-    resam_type="auto",
-    interp_kind="cubic",
-    save_as_ma=False,
-    modes_list=None,
-    crop=False,
-    centre=True,
-    r_ext_factor=1,
-    debug=False,
+	wfa=None,
+	data_dir="./",
+	file_name="*",
+	label="RIT_strain",
+	spin_weight=-2,
+	ell_max="auto",
+	resam_type="auto",
+	interp_kind="cubic",
+	save_as_ma=False,
+	modes_list=None,
+	crop=False,
+	centre=True,
+	r_ext_factor=1,
+	debug=False,
 ):
     """Load the RIT or strain waveforms from the RIT/ MAYA catalogue data,
     from hdf5 files from disk.
 
     Parameters
     ----------
-    wfa  : waveforms
-               An instance of the waveforms class. Creates a new one if not provided.
-    data_dir :	string
-                    A string containing the directory path where the mode files can be found.
+    wfa : modes_array
+          An instance of the waveforms class. Creates a new one if not provided.
+    data_dir : string
+               A string containing the directory path where the mode files can be found.
     label : string, optional
-                    The label of the modes_array object.
+            The label of the modes_array object.
     ell_max : int, optional
-                            The maximum mode number to load. If not specified,
-                            then all available modes are loaded.
+              The maximum mode number to load. If not specified,
+              then all available modes are loaded.
     save_as_ma : bool, optional
-                             Save to disk again as a modes_array h5 file?
+                 Save to disk again as a modes_array h5 file?
     spin_weight : int, optional
-                              The spin weight of the object. Used for filtering modes.
-                              Defaults to -2.
+                  The spin weight of the object. Used for filtering modes.
+                  Defaults to -2.
     resam_type : string, float, optional
-                             The type of resampling to do. Options are finest and coarsest, and user input float.
+                 The type of resampling to do. Options are the `finest` and `coarsest`,
+                 and user input float.
     interp_kind : string, optional
-                              The interpolation type to use. Default is cubic.
+                  The interpolation type to use. Default is cubic.
 
     Returns
     -------
-
     rit_modes_array : modes_array
-                                            A modes_array instance containing the loaded modes.
+                      A modes_array instance containing the loaded modes.
 
     Notes
     -----
-    It seems like the time axis of individual modes are identical to each other. Hence, one need not worry about
-    choosing the time domain. This may change in future.
+    It seems like the time axis of individual modes are identical
+    to each other. Hence, one need not worry about choosing
+    the time domain. This may change in future.
     """
     message("Loading RIT strain data.", message_verbosity=1)
 
     from functools import partial
 
     # Initialize the interpolator
     if isinstance(interp_kind, int):
-        message("Interpolating using InterpolatedUnivariateSpline", message_verbosity=2)
+        message(
+            "Interpolating using InterpolatedUnivariateSpline",
+            message_verbosity=2,
+        )
         interpolator = partial(interp, k=interp_kind)
 
     elif isinstance(interp_kind, str):
         from scipy.interpolate import interp1d
 
         message("Interpolating using interp1d", message_verbosity=2)
         interpolator = partial(interp1d, kind=interp_kind)
 
     from waveformtools.waveforms import modes_array
 
     # Max available mode l.
-    ell_max_act, keys_list = get_ell_max_from_file(data_dir=data_dir, var_type="Strain", file_name=file_name)
+    ell_max_act, keys_list = get_ell_max_from_file(
+        data_dir=data_dir, var_type="Strain", file_name=file_name
+    )
 
     ####################################
     # Set variables with priorities
     # Note: rework this in dictionaries
     ####################################
 
     if ell_max == "auto":
@@ -616,15 +641,17 @@
     message("Chosen ell max", ell_max, "Available ell_max", ell_max_act)
 
     if not wfa:
         # Create a modes array
         wfa = modes_array(label=label, ell_max=ell_max, modes_list=modes_list)
     # wfa = modes_array(label=label, data_dir=data_dir, modes_list=modes_list)
     if debug is True:
-        wf_nl = modes_array(label=label + "_nl", ell_max=ell_max, modes_list=modes_list)
+        wf_nl = modes_array(
+            label=label + "_nl", ell_max=ell_max, modes_list=modes_list
+        )
 
     if not data_dir:
         data_dir = wfa.data_dir
     else:
         wfa.data_dir = data_dir
 
     if not file_name:
@@ -633,19 +660,21 @@
         wfa.file_name = file_name
 
     if not ell_max:
         ell_max = wfa.ell_max
     else:
         wfa.ell_max = ell_max
 
-    # ell_max		 = 12
+    # ell_max        = 12
     if not modes_list:
         if not wfa.modes_list:
             message("Constructing the modes list")
-            modes_list = construct_mode_list(ell_max=ell_max, spin_weight=wfa.spin_weight)
+            modes_list = construct_mode_list(
+                ell_max=ell_max, spin_weight=wfa.spin_weight
+            )
         else:
             modes_list = wfa.modes_list
     else:
         wfa.modes_list = modes_list
 
     # For interpolation
     from scipy.interpolate import interp1d
@@ -670,15 +699,19 @@
         # dt_auto = time_axis[1]-time_axis[0]
         from scipy.stats import mode
 
         dt_auto = mode(np.diff(time_axis))[0][0]
 
     except Exception as excep:
         dt_auto = None
-        message("NRTimes not present. Will compute dt auto from mode time axis")
+        message(
+            "NRTimes not present. Will compute dt auto from mode time axis",
+            excep,
+            message_verbosity=2,
+        )
 
     message("Reading in modes...")
     for ell, emm_list in modes_list:
         for emm in emm_list:
             this_amp_key = f"amp_l{ell}_m{emm}"
             this_phase_key = f"phase_l{ell}_m{emm}"
 
@@ -710,194 +743,220 @@
                 max_dt = round(max(np.diff(time_axis)), 2)
                 message(f"Default dt is {dt_auto}", message_verbosity=2)
 
                 if resam_type == "auto":
                     # Choose finest available timestep
                     # for upto 3 decimal digits.
                     m_dt = dt_auto
-                    message("Sampling at the default timestep", m_dt, message_verbosity=2)
+                    message(
+                        "Sampling at the default timestep",
+                        m_dt,
+                        message_verbosity=2,
+                    )
 
                 elif resam_type == "finest":
                     m_dt = min_dt
-                    message("Sampling at the finest available timestep", m_dt, message_verbosity=2)
+                    message(
+                        "Sampling at the finest available timestep",
+                        m_dt,
+                        message_verbosity=2,
+                    )
 
                 elif resam_type == "coarsest":
                     m_dt = max_dt
-                    message("Sampling at the coarsest available timestep", m_dt, message_verbosity=2)
+                    message(
+                        "Sampling at the coarsest available timestep",
+                        m_dt,
+                        message_verbosity=2,
+                    )
 
                 elif isinstance(resam_type, float):
                     m_dt = resam_type
-                    message("Resampling at user defined timestep", m_dt, message_verbosity=2)
+                    message(
+                        "Resampling at user defined timestep",
+                        m_dt,
+                        message_verbosity=2,
+                    )
 
-                    # New (resampled) time axis
-                    time_axis = np.arange(time_axis[0], time_axis[-1], m_dt)
+					# New (resampled) time axis
+					time_axis = np.arange(time_axis[0], time_axis[-1], m_dt)
 
                 else:
-                    raise NotImplementedError(f"Unknown resampling parameter {resam_type}")
+                    raise NotImplementedError(
+                        f"Unknown resampling parameter {resam_type}"
+                    )
 
-                # Length of data.
-                data_len = len(time_axis)
+				# Length of data.
+				data_len = len(time_axis)
 
-                # Create a modes array object
-                wfa.create_modes_array(ell_max=ell_max, data_len=data_len)
+				# Create a modes array object
+				wfa.create_modes_array(ell_max=ell_max, data_len=data_len)
 
-                # Assign to it the time axis
-                wfa.time_axis = time_axis
-                # message(wfa.time_axis)
-            # message(wfa.time_axis - wf_psi4_time)
-            # continue
-            ###################################
-            # Uniform sampling
-            ###################################
-            # message('Wfa time axis', wfa.time_axis)
+				# Assign to it the time axis
+				wfa.time_axis = time_axis
+				# message(wfa.time_axis)
+			# message(wfa.time_axis - wf_psi4_time)
+			# continue
+			###################################
+			# Uniform sampling
+			###################################
+			# message('Wfa time axis', wfa.time_axis)
 
-            Yphase_interp_fun = interpolator(Tphase, Yphase)
-            # Yphase_interp_fun = interpolator(Tphase, Yphase, k=3)
+			Yphase_interp_fun = interpolator(Tphase, Yphase)
+			# Yphase_interp_fun = interpolator(Tphase, Yphase, k=3)
 
-            # Resample
+			# Resample
 
-            Yphase_resam = Yphase_interp_fun(time_axis)
+			Yphase_resam = Yphase_interp_fun(time_axis)
 
-            ###########################
-            # Load the amplitude data
-            ###########################
-            Tamp = data_file[this_amp_key]["X"][...]
+			###########################
+			# Load the amplitude data
+			###########################
+			Tamp = data_file[this_amp_key]["X"][...]
 
-            Yamp = data_file[this_amp_key]["Y"][...]
+			Yamp = data_file[this_amp_key]["Y"][...]
 
-            Yamp_interp_fun = interpolator(Tamp, Yamp)
-            # Yamp_interp_fun = interpolator(Tamp, Yamp, k=3)
+			Yamp_interp_fun = interpolator(Tamp, Yamp)
+			# Yamp_interp_fun = interpolator(Tamp, Yamp, k=3)
 
-            # wf_c = Yamp*np.exp(1j*Yphase)
+			# wf_c = Yamp*np.exp(1j*Yphase)
 
-            # Resample
+			# Resample
 
-            Yamp_resam = Yamp_interp_fun(time_axis)
+			Yamp_resam = Yamp_interp_fun(time_axis)
 
-            wfmode = Yamp_resam * np.exp(1j * Yphase_resam)
+			wfmode = Yamp_resam * np.exp(1j * Yphase_resam)
 
             # if not (Tphase==Tamp).all():
-            # 	 raise ValueError('The time axis of the amps and phase are different!')
+            #    raise ValueError('The time axis of the amps and phase are different!')
 
-            # wfmode = interp_resam_wfs(wf_c, Tphase, time_axis, k=4)
+			# wfmode = interp_resam_wfs(wf_c, Tphase, time_axis, k=4)
 
-            ###################################
-            # Load the modes data
-            ###################################
+			###################################
+			# Load the modes data
+			###################################
 
-            wfa.set_mode_data(ell, emm, r_ext_factor * wfmode)
+			wfa.set_mode_data(ell, emm, r_ext_factor * wfmode)
 
-    data_file.close()
+	data_file.close()
 
-    #####################
-    # Finishing touches
-    #####################
-    wfa.actions += "->load_modes"
-
-    # Trim or recenter
-    if centre is True:
-        wfa.trim(trim_upto_time=0)
-        wfa.actions += "->center"
-
-    if isinstance(crop, float):
-        wfa.trim(trim_upto_time=crop)
-        wfa.actions += "->crop"
+	#####################
+	# Finishing touches
+	#####################
+	wfa.actions += "->load_modes"
 
-    if save_as_ma is True:
-        # Save the modes array as waveforms hdf file
-        wfa.save_modes(out_file_name=f"{label}_resam.h5")
-        wfa.actions += "->save_as_wfh5"
+	# Trim or recenter
+	if centre is True:
+		wfa.trim(trim_upto_time=0)
+		wfa.actions += "->center"
 
-    if debug is True:
-        return wfa, wf_nl
-    else:
-        return wfa
+	if isinstance(crop, float):
+		wfa.trim(trim_upto_time=crop)
+		wfa.actions += "->crop"
+
+	if save_as_ma is True:
+		# Save the modes array as waveforms hdf file
+		wfa.save_modes(out_file_name=f"{label}_resam.h5")
+		wfa.actions += "->save_as_wfh5"
+
+	if debug is True:
+		return wfa, wf_nl
+	else:
+		return wfa
 
 
 #################################################################
 # Generic data type
 #################################################################
 
 
 def load_gen_data_from_disk(
-    wfa=None,
-    label="generic waveform",
-    data_dir="./",
-    file_name="*.h5",
-    r_ext=None,
-    ell_max=8,
-    pre_key=None,
-    modes_list=None,
-    crop=False,
-    centre=True,
-    key_ex=None,
-    r_ext_factor=1,
-    *args,
-    **kwargs,
+	wfa=None,
+	label="generic waveform",
+	data_dir="./",
+	file_name="*.h5",
+	r_ext=None,
+	ell_max=8,
+	pre_key=None,
+	modes_list=None,
+	crop=False,
+	centre=True,
+	key_ex=None,
+	r_ext_factor=1,
+	*args,
+	**kwargs,
 ):
     """Load the RIT strain waveforms from the RIT catalogue,
     from hdf5 files from disk.
 
     Parameters
     ----------
-    data_dir :	string
-                    A string containing the directory path where the mode files can be found.
+    data_dir : string
+               A string containing the directory path
+               where the mode files can be found.
     label : string, optional
-                    The label of the modes_array object.
+            The label of the modes_array object.
     ell_max : int, optional
-                            The maximum mode number to load. If not specified,
-                            then all available modes are loaded.
+              The maximum mode number to load. If not specified,
+              then all available modes are loaded.
     save_as_ma : bool, optional
-                             Save to disk again as a modes_array h5 file?
+                 Save to disk again as a modes_array h5 file?
     spin_weight : int, optional
-                              The spin weight of the object. Used for filtering modes.
-                              Defaults to -2.
+                  The spin weight of the object. Used for filtering modes.
+                  Defaults to -2.
     resam_type : string, float, optional
-                             The type of resampling to do. Options are finest and coarsest, and user input float.
+                 The type of resampling to do. Options are the `finest` and `coarsest`,
+                 and user input float.
     interp_kind : string, optional
-                              The interpolation type to use. Default is cubic.
+                  The interpolation type to use. Default is cubic.
 
     Returns
     -------
 
     rit_modes_array : modes_array
-                                            A modes_array instance containing the loaded modes.
+                      A modes_array instance containing the loaded modes.
 
     Notes
     -----
-    It seems like the time axis of individual modes are identical to each other. Hence, one need not worry about
-    choosing the time domain. This may change in future.
+    It seems like the time axis of individual modes are identical to each other.
+    Hence, one need not worry about choosing the time domain. This may change
+    in future.
 
     """
     message("Loading generic data.", message_verbosity=1)
     from waveformtools.waveforms import modes_array
 
     # Max available mode l.
     if not wfa:
         # Create a modes array
-        wfa = modes_array(label=label, data_dir=data_dir, modes_list=modes_list, ell_max=ell_max)
+        wfa = modes_array(
+            label=label,
+            data_dir=data_dir,
+            modes_list=modes_list,
+            ell_max=ell_max,
+        )
 
     # if not data_dir:
-    # 	data_dir = wfa.data_dir
+    #   data_dir = wfa.data_dir
     # else:
-    # 	wfa.data_dir = data_dir
+    #   wfa.data_dir = data_dir
 
     # if not file_name:
-    # 	file_name = wfa.file_name
+    #   file_name = wfa.file_name
     # else:
-    # 	wfa.file_name = file_name
+    #   wfa.file_name = file_name
 
     # if not ell_max:
-    # 	ell_max = wfa.ell_max
+    #   ell_max = wfa.ell_max
     # else:
-    # 	wfa.ell_max = ell_max
+    #   wfa.ell_max = ell_max
 
     # if not label:
-    # 	label = wfa.label
-    # ell_max		 = 12
+    #   label = wfa.label
+    # ell_max        = 12
     # Max available mode l.
 
     full_path = f"{data_dir}/{file_name}"
     message(f"Loading data from {full_path}")
     # Enforce only l>2 modes.
     # wf_modes_list = [item for item in wf_modes_list if item[0]>=abs(spin_weight)]
 
@@ -917,15 +976,17 @@
             metadata_bytes = bytes(np.void(wfile["metadata"])).decode()
             metadata = json.loads(metadata_bytes)
             # Import the metadata.
             for key, val in metadata.items():
                 if val is not None:
                     wfa.__dict__.update({key: val})
             message("Metadata loaded", message_verbosity=2)
-            message("Waveform meta data:", wfa.get_metadata(), message_verbosity=1)
+            message(
+                "Waveform meta data:", wfa.get_metadata(), message_verbosity=1
+            )
 
         except Exception as ex:
             # If no metadata found, pass empty dict for updation.
             message("No metadata found!", ex)
             metadata = {}
             pass
         # message(wfa.file_name)
@@ -937,15 +998,17 @@
         # message(wfa.get_metadata())
         # Check and filter for particular key string pattern
 
         if key_ex is not None:
             # Filter the keys according to key_ex if specified.
             message("Filtering as per", key_ex)
             wfa.key_ex = key_ex
-            modes_keys_list = [item for item in modes_keys_list if key_ex in item]
+            modes_keys_list = [
+                item for item in modes_keys_list if key_ex in item
+            ]
             # message(modes_keys_list)
 
         else:
             message("key_ex is not specified. Proceeding without filtering..")
 
         modes_keys_list = sorted(modes_keys_list)
 
@@ -1013,40 +1076,50 @@
 
             for emm_index, emm_value in enumerate(emm_list):
                 # For every (ell, emm) mode.
 
                 # Find the key corresponding to the mode
                 try:
                     key = str(
-                        [item for item in modes_keys_list if re.search(f"l{ell_value}_m{emm_value}_r{r_ext}", item)][0]
+                        [
+                            item
+                            for item in modes_keys_list
+                            if re.search(
+                                f"l{ell_value}_m{emm_value}_r{r_ext}", item
+                            )
+                        ][0]
                     )
                     # message('The loaded key is ', key, type(key))
                     # message('The loaded key is ', key, type(key))
                     # if key=='l0_m0_r500.00':
                     # message('Its alright')
                 except Exception as ex:
-                    message(f"Waveform dataset for l{ell_value}, m{emm_value} not found", ex)
+                    message(
+                        f"Waveform dataset for l{ell_value}, m{emm_value} not found",
+                        ex,
+                    )
                     sys.exit(0)
 
                 # Get the data
                 data = np.array(wfile[key])
 
                 # set the time and data axis
-                time_axis = data[:, 0]
-                data_re = data[:, 1]
-                data_im = data[:, 2]
+                time_axis, data_re = cleandata([data[:, 0], data[:, 1]])
+                time_axis, data_im = cleandata([data[:, 0], data[:, 2]])
 
                 # create flag
                 if not cflag:
                     if wfa.modes_data.all() == np.array(None):
                         if crop:
                             # Crop the beginning portion.
                             # delta_t = time_axis[1] - time_axis[0]
                             # shift = int(wfa.r_ext / delta_t)
-                            raise NotImplementedError("Not implemented! Please contact the developers!")
+                            raise NotImplementedError(
+                                "Not implemented! Please contact the developers!"
+                            )
 
                         else:
                             shift = 0
                         data_len = len(time_axis) - shift
                         wfa.data_len = data_len
                         # Delete the attribute
                         # del self.modes_data
@@ -1058,15 +1131,19 @@
                         cflag = 1
 
                         # set the time axis.
                         # wfa.time_axis = time_axis[shift:]
                         wfa._time_axis = time_axis
 
                 # wfa.set_mode_data(ell_value, emm_value, r_ext_factor*(data_re[shift:] + 1j * data_im[shift:]))
-                wfa.set_mode_data(ell_value, emm_value, r_ext_factor * (data_re + 1j * data_im))
+                wfa.set_mode_data(
+                    ell_value,
+                    emm_value,
+                    r_ext_factor * (data_re + 1j * data_im),
+                )
 
         ##############################
         # Recenter axis
         ##############################
         # Trim or recenter
         if centre:
             crop_time = 0
@@ -1075,74 +1152,74 @@
 
             wfa.trim(trim_upto_time=crop_time)
 
         # maxloc = np.argmax(np.absolute(self.mode(2, 2)))
         # maxtime = time_axis[shift + maxloc]
 
         # if wfa.maxtime is None:
-        # 	 wfa.maxtime = maxtime
+        #    wfa.maxtime = maxtime
         # message("Max time is", maxtime)
 
         # if centre:
-        # 	 wfa.time_axis = time_axis[shift:] - maxtime
+        #    wfa.time_axis = time_axis[shift:] - maxtime
         # message(wfa.file_name)
         return wfa
 
 
 ########################################################################################################################
 # SpEC
 ########################################################################################################################
 
 
 def load_SpEC_data_from_disk(
-    wfa=None,
-    label="SXS Strain",
-    data_dir="./",
-    file_name="rhOverM_Extrapolated_N5_CoM_Mem.h5",
-    extrap_order=4,
-    r_ext=None,
-    ell_max=None,
-    centre=True,
-    modes_list=None,
-    save_as_ma="False",
-    resam_type="auto",
-    interp_kind="cubic",
-    compression_opts=0,
-    r_ext_factor=1,
-    debug=False,
+	wfa=None,
+	label="SXS Strain",
+	data_dir="./",
+	file_name="rhOverM_Extrapolated_N5_CoM_Mem.h5",
+	extrap_order=4,
+	r_ext=None,
+	ell_max=None,
+	centre=True,
+	modes_list=None,
+	save_as_ma="False",
+	resam_type="auto",
+	interp_kind="cubic",
+	compression_opts=0,
+	r_ext_factor=1,
+	debug=False,
 ):
     """Load the SpEC waveform to modes_array,from hdf5 files from disk.
 
     Parameters
     ----------
     wfa : modes_array, optional
-              The modes array to which to store the loaded waveform to. A new modes array will be returned
-              if not provided.
-    data_dir :	string
-                    A string containing the directory path where the mode files can be found.
+          The modes array to which to store the loaded waveform to.
+          A new modes array will be returned if not provided.
+    data_dir : string
+               A string containing the directory path
+               where the mode files can be found.
     file_name : string
-                    The name of the file containing the waveform data.
+                The name of the file containing the waveform data.
     label : string, optional
-                    The label of the modes_array object.
+            The label of the modes_array object.
     ell_max : int, optional
-                            The maximum mode number to load. If not specified,
-                            then all available modes are loaded.
+              The maximum mode number to load. If not specified,
+              then all available modes are loaded.
     save_as_ma : bool, optional
-                             Save to disk again as a modes_array h5 file?
+                 Save to disk again as a modes_array h5 file?
     resam_type : string, float, optional
-                             The type of resampling to do. Options are finest and coarsest, and user input float.
+                 The type of resampling to do. Options are
+                 the `fines`t and `coarsest`, and user input float.
     interp_kind : string, optional
-                              The interpolation type to use. Default is cubic.
+                  The interpolation type to use. Default is cubic.
 
     Returns
     -------
-
     modes_array : modes_array
-                              A modes_array instance containing the loaded modes.
-
+                  A modes_array instance containing the loaded modes.
 
     """
     message("Loading SpEC data.", message_verbosity=1)
 
     from waveformtools.waveforms import modes_array
 
     # Load SXS waveforms to modes_array.
@@ -1186,15 +1263,17 @@
     message("Chosen ell max", ell_max, "Available ell_max", ell_max_act)
 
     if not wfa:
         # Create a modes array
         wfa = modes_array(label=label, ell_max=ell_max, modes_list=modes_list)
     # wfa = modes_array(label=label, data_dir=data_dir, modes_list=modes_list)
     if debug is True:
-        wf_nl = modes_array(label=label + "_nl", ell_max=ell_max, modes_list=modes_list)
+        wf_nl = modes_array(
+            label=label + "_nl", ell_max=ell_max, modes_list=modes_list
+        )
 
     wfa.extrap_order = extrap_order
     message(f"Using extrap order {extrap_order}")
 
     if not data_dir:
         data_dir = wfa.data_dir
     else:
@@ -1206,20 +1285,22 @@
         wfa.file_name = file_name
 
     if not ell_max:
         ell_max = wfa.ell_max
     else:
         wfa.ell_max = ell_max
 
-    # ell_max		 = 12
+    # ell_max        = 12
     if not modes_list:
         if not wfa.modes_list:
             message("Constructing the modes list")
             # sys.exit(0)
-            modes_list = construct_mode_list(ell_max=ell_max, spin_weight=wfa.spin_weight)
+            modes_list = construct_mode_list(
+                ell_max=ell_max, spin_weight=wfa.spin_weight
+            )
         else:
             modes_list = wfa.modes_list
     else:
         wfa.modes_list = modes_list
 
     # Filter
     modes_list = [item for item in modes_list if item[0] >= 2]
@@ -1287,124 +1368,130 @@
                     m_dt = dt_auto
                     message("Resampling at the default timestep", m_dt)
 
                 message("Chosen resampling fineness:", resam_type)
                 # New (resampled) time axis
                 time_axis = np.arange(time_axis[0], time_axis[-1], m_dt)
 
-                # Length of data.
-                data_len = len(time_axis)
-                # message(data_len)
-
-                wfa.create_modes_array(ell_max=ell_max, data_len=data_len)
-                # message(wfa.mode(0,0).shape)
-                wfa.time_axis = time_axis
-
-            # Interpolate and resamplea
-            # Note
-            # Interpolating in amplitude and phase is better
-            # and has lower interpolation errors
-            # but is slower due to unwrapping of phases.
-
-            wf_int = interp_resam_wfs(wf_data_c, wf_time, time_axis, kind="cubic", k=None)
-
-            # amp_int = interp_resam_wfs(wf_amp, wf_time, time_axis)
-            # phase_int = interp_resam_wfs(wf_phase, wf_time, time_axis)
-
-            # re_int = interp1d(wf_time, wf_data_re)
-            # message(wf_time[0], wf_time[-1], time_axis[0], time_axis[-1])
-            # re_dat = re_int(time_axis)
-
-            # im_int = interp1d(wf_time, wf_data_im)
-            # im_dat = im_int(time_axis)
-
-            # wfa.set_mode_data(ell, emm, data=re_dat + 1j * im_dat)
-            wfa.set_mode_data(ell, emm, data=wf_int)
-
-    if debug is True:
-        for ell, emm_list in modes_list:
-            for emm in emm_list:
-                this_key = f"Y_l{ell}_m{emm}.dat"
-
-                # Input waveform from disk
-                wf_data = wf_file[this_key]
-                wf_time = wf_data[:, 0]
-                wf_data_re = wf_data[:, 1]
-                wf_data_im = wf_data[:, 2]
+				# Length of data.
+				data_len = len(time_axis)
+				# message(data_len)
+
+				wfa.create_modes_array(ell_max=ell_max, data_len=data_len)
+				# message(wfa.mode(0,0).shape)
+				wfa.time_axis = time_axis
+
+			# Interpolate and resamplea
+			# Note
+			# Interpolating in amplitude and phase is better
+			# and has lower interpolation errors
+			# but is slower due to unwrapping of phases.
+
+            wf_int = interp_resam_wfs(
+                wf_data_c, wf_time, time_axis, kind="cubic", k=None
+            )
+
+			# amp_int = interp_resam_wfs(wf_amp, wf_time, time_axis)
+			# phase_int = interp_resam_wfs(wf_phase, wf_time, time_axis)
+
+			# re_int = interp1d(wf_time, wf_data_re)
+			# message(wf_time[0], wf_time[-1], time_axis[0], time_axis[-1])
+			# re_dat = re_int(time_axis)
+
+			# im_int = interp1d(wf_time, wf_data_im)
+			# im_dat = im_int(time_axis)
+
+			# wfa.set_mode_data(ell, emm, data=re_dat + 1j * im_dat)
+			wfa.set_mode_data(ell, emm, data=wf_int)
+
+	if debug is True:
+		for ell, emm_list in modes_list:
+			for emm in emm_list:
+				this_key = f"Y_l{ell}_m{emm}.dat"
+
+				# Input waveform from disk
+				wf_data = wf_file[this_key]
+				wf_time = wf_data[:, 0]
+				wf_data_re = wf_data[:, 1]
+				wf_data_im = wf_data[:, 2]
 
                 if wf_nl.modes_data.all() == np.array(None):
-                    wf_nl.create_modes_array(ell_max=ell_max, data_len=len(wf_time))
+                    wf_nl.create_modes_array(
+                        ell_max=ell_max, data_len=len(wf_time)
+                    )
                     wf_nl.time_axis = wf_time
                     wf_nl.data_len = len(wf_time)
 
-                wf_nl.set_mode_data(ell, emm, data=wf_data_re + 1j * wf_data_im)
+				wf_nl.set_mode_data(ell, emm, data=wf_data_re + 1j * wf_data_im)
 
-    if centre:
-        wfa.trim(trim_upto_time=0)
+	if centre:
+		wfa.trim(trim_upto_time=0)
 
     if save_as_ma is True:
         # Save the modes array as waveforms hdf file
-        wfa.save_modes(out_file_name=f"{label}_resam.h5", compression_opts=compression_opts)
-
-    wf_f0.close()
-
-    if debug is True:
-        return wfa, wf_nl
-    else:
-        return wfa
+        wfa.save_modes(
+            out_file_name=f"{label}_resam.h5", compression_opts=compression_opts
+        )
+
+	wf_f0.close()
+
+	if debug is True:
+		return wfa, wf_nl
+	else:
+		return wfa
 
 
 ########################################################################################################################
 # SpECTRE
 ########################################################################################################################
 
 
 def load_SpECTRE_data_from_disk(
-    wfa=None,
-    label="SpECTRE Strain",
-    data_dir="./",
-    file_name="rhOverM_Extrapolated_N5_CoM_Mem.h5",
-    r_ext=None,
-    ell_max=12,
-    centre=True,
-    modes_list=None,
-    r_ext_factor=1,
-    save_as_ma="False",
-    resam_type="auto",
-    kind="cubic",
-    compression_opts=0,
+	wfa=None,
+	label="SpECTRE Strain",
+	data_dir="./",
+	file_name="rhOverM_Extrapolated_N5_CoM_Mem.h5",
+	r_ext=None,
+	ell_max=12,
+	centre=True,
+	modes_list=None,
+	r_ext_factor=1,
+	save_as_ma="False",
+	resam_type="auto",
+	kind="cubic",
+	compression_opts=0,
 ):
     """Load the SpECTRE or SpEC CCE waveform to modes_array,from hdf5 files from disk.
 
     Parameters
     ----------
     wfa : modes_array, optional
-              The modes array to which to store the loaded waveform to. A new modes array will be returned
-              if not provided.
-    data_dir :	string
-                    A string containing the directory path where the mode files can be found.
+          The modes array to which to store the loaded waveform to.
+          A new modes array will be returned if not provided.
+    data_dir : string
+               A string containing the directory path where the mode files can be found.
     file_name : string
-                    The name of the file containing the waveform data.
+                The name of the file containing the waveform data.
     label : string, optional
-                    The label of the modes_array object.
+            The label of the modes_array object.
     ell_max : int, optional
-                            The maximum mode number to load. If not specified,
-                            then all available modes are loaded.
+              The maximum mode number to load. If not specified,
+              then all available modes are loaded.
     save_as_ma : bool, optional
-                             Save to disk again as a modes_array h5 file?
+                 Save to disk again as a modes_array h5 file?
     resam_type : string, float, optional
-                             The type of resampling to do. Options are finest and coarsest, and user input float.
+                 The type of resampling to do. Options are
+                 the `finest` and `coarsest`, and user input float.
     interp_kind : string, optional
-                              The interpolation type to use. Default is cubic.
+                  The interpolation type to use. Default is cubic.
 
     Returns
     -------
-
     modes_array : modes_array
-                              A modes_array instance containing the loaded modes.
+                  A modes_array instance containing the loaded modes.
 
 
     """
     spin_weight = -2
     message("Loading SpECTRE data.", message_verbosity=1)
     from waveformtools.waveforms import modes_array
 
@@ -1412,15 +1499,18 @@
     # Spectra infinty
 
     full_path = f"{data_dir}/{file_name}"
 
     try:
         import scri
     except Exception as ex:
-        message("scri module is required for reading in SXS waveforms. Please install and try again", ex)
+        message(
+            "scri module is required for reading in SXS waveforms. Please install and try again",
+            ex,
+        )
         sys.exit(0)
 
     wf_file = scri.rpxmb.load(full_path)[0].to_inertial_frame()
     ell_max_act = wf_file.ell_max
     # Add readinf ell max from file
 
     if ell_max is None:
@@ -1449,20 +1539,22 @@
         wfa.file_name = file_name
 
     if not ell_max:
         ell_max = wfa.ell_max
     else:
         wfa.ell_max = ell_max
 
-    # ell_max		 = 12
+    # ell_max        = 12
     if not modes_list:
         if not wfa.modes_list:
             message("Constructing the modes list")
             # sys.exit(0)
-            modes_list = construct_mode_list(ell_max=ell_max, spin_weight=spin_weight)
+            modes_list = construct_mode_list(
+                ell_max=ell_max, spin_weight=spin_weight
+            )
         else:
             modes_list = wfa.modes_list
     else:
         wfa.modes_list = modes_list
 
     # flag = None
 
@@ -1490,113 +1582,132 @@
 
                 # min_dt = round(min(np.diff(time_axis)), 2)
                 # max_dt = round(max(np.diff(time_axis)), 2)
 
                 min_dt = min(np.diff(time_axis))
                 max_dt = max(np.diff(time_axis))
 
-                message(f"Min dt {min_dt} and Max dt {max_dt}", message_verbosity=2)
+                message(
+                    f"Min dt {min_dt} and Max dt {max_dt}", message_verbosity=2
+                )
 
                 if resam_type == "finest":
                     # Choose finest available timestep
                     # for upto 3 decimal digits.
                     m_dt = min_dt
-                    message("Resampling at the finest timestep", m_dt, message_verbosity=1)
+                    message(
+                        "Resampling at the finest timestep",
+                        m_dt,
+                        message_verbosity=1,
+                    )
                 if resam_type == "coarsest":
                     m_dt = max_dt
-                    message("Resampling at the coarsest timestep", m_dt, message_verbosity=1)
+                    message(
+                        "Resampling at the coarsest timestep",
+                        m_dt,
+                        message_verbosity=1,
+                    )
 
                 if isinstance(resam_type, float):
                     m_dt = resam_type
-                    message("Resampling at user defined timestep", m_dt, message_verbosity=1)
+                    message(
+                        "Resampling at user defined timestep",
+                        m_dt,
+                        message_verbosity=1,
+                    )
 
                 if resam_type == "auto":
                     # Choose finest available timestep
                     # for upto 3 decimal digits.
                     m_dt = dt_auto
-                    message("Resampling at the default timestep", m_dt, message_verbosity=1)
+                    message(
+                        "Resampling at the default timestep",
+                        m_dt,
+                        message_verbosity=1,
+                    )
 
-                # New (resampled) time axis
-                time_axis = np.arange(time_axis[0], time_axis[-1], m_dt)
+				# New (resampled) time axis
+				time_axis = np.arange(time_axis[0], time_axis[-1], m_dt)
 
-                # Length of data.
-                data_len = len(time_axis)
-                # message(data_len)
+				# Length of data.
+				data_len = len(time_axis)
+				# message(data_len)
 
-                wfa.create_modes_array(ell_max=ell_max, data_len=data_len)
-                # message(wfa.mode(0,0).shape)
-                wfa.time_axis = time_axis
+				wfa.create_modes_array(ell_max=ell_max, data_len=data_len)
+				# message(wfa.mode(0,0).shape)
+				wfa.time_axis = time_axis
 
-            re_int = interp1d(wf_time, wf_data_re, kind=kind)
-            # message(wf_time[0], wf_time[-1], time_axis[0], time_axis[-1])
-            re_dat = re_int(time_axis)
+			re_int = interp1d(wf_time, wf_data_re, kind=kind)
+			# message(wf_time[0], wf_time[-1], time_axis[0], time_axis[-1])
+			re_dat = re_int(time_axis)
 
-            im_int = interp1d(wf_time, wf_data_im, kind=kind)
-            im_dat = im_int(time_axis)
+			im_int = interp1d(wf_time, wf_data_im, kind=kind)
+			im_dat = im_int(time_axis)
 
-            wfa.set_mode_data(ell, emm, data=re_dat + 1j * im_dat)
+			wfa.set_mode_data(ell, emm, data=re_dat + 1j * im_dat)
 
-    if centre:
-        wfa.trim(trim_upto_time=0)
+	if centre:
+		wfa.trim(trim_upto_time=0)
 
     if save_as_ma is True:
         # Save the modes array as waveforms hdf file
-        wfa.save_modes(out_file_name=f"{label}_resam.h5", compression_opts=compression_opts)
+        wfa.save_modes(
+            out_file_name=f"{label}_resam.h5", compression_opts=compression_opts
+        )
 
-    return wfa
+	return wfa
 
 
 ########################################################################################################################
 # Output
 ########################################################################################################################
 
 
 def save_modes_data_to_gen(
-    wfa,
-    ell_max=None,
-    pre_key=None,
-    key_format=None,
-    modes_to_save=None,
-    out_file_name="mp_new_modes.h5",
-    r_ext_factor=None,
-    compression_opts=0,
-    r_ext=None,
+	wfa,
+	ell_max=None,
+	pre_key=None,
+	key_format=None,
+	modes_to_save=None,
+	out_file_name="mp_new_modes.h5",
+	r_ext_factor=None,
+	compression_opts=0,
+	r_ext=None,
 ):
     """Save the waveform mode data to an hdf file.
 
     Parameters
     ----------
-    pre_key:	str, optional
-                                                    A string containing the key of the group in
-                                                    the HDF file in which the modes` dataset exists.
-                                                    It defaults to `None`.
-    mode_numbers:	list
-                                                                    The mode numbers to load from the file.
-                                                                    Each item in the list is a list that
-                                                                    contains two integrer numbers, one for
-                                                                    the mode index :math:`\\ell` and the
-                                                                    other for the mode index :math:`m`.
+    pre_key : str, optional
+              A string containing the key of the group in
+              the HDF file in which the modes` dataset exists.
+              It defaults to `None`.
+    mode_numbers : list
+                   The mode numbers to load from the file.
+                   Each item in the list is a list that
+                   contains two integrer numbers, one for
+                   the mode index :math:`\\ell` and the
+                   other for the mode index :math:`m`.
 
     Returns
     -------
-    waveform_obj:	3d array
-                                                                    Sets the three dimensional array `waveform.modes` that contains
-                                                                    the required :math:`\\ell, m` modes.
+    waveform_obj : 3d array
+                   Sets the three dimensional array `waveform.modes`
+                   that contains the required :math:`\\ell, m` modes.
 
     Examples
     --------
     >>> from waveformtools.waveforms import modes_array
     >>> wf = modes_array()
     >>> wf.data_dir = './'
     >>> wf.filename = 'data_file.h5'
     >>> wf.modes_list = [[2, 2], [3, 3]]
     >>> wf.load_gen_data()
     """
-
-    from waveformtools.waveforms import modes_array
+    # from waveformtools.waveforms import modes_array
 
     #############################
     # I/O assignments.
     #############################
 
     wfa.out_file_name = wfa.label + "_" + out_file_name
     wfa.out_file_name = wfa.out_file_name.replace(" ", "_")
@@ -1624,26 +1735,28 @@
 
         else:
             modes_to_save = wfa.modes_list
 
     ##########################
     # Create the modes file.
     ##########################
-    message(wfa.label)
+    message("Saving waveform", wfa.label, message_verbosity=2)
     with h5py.File(full_path, "w") as wfile:
         # Create the metadata dataset.
         metadata = wfa.get_metadata()
 
         message(metadata, message_verbosity=1)
 
         metadata_bytes = json.dumps(metadata).encode()
 
         # dt = h5py.special_dtype(vlen=str)
         # metadata=np.asarray([metadata_bytes], dtype=dt)
-        wfile.create_dataset("metadata", data=metadata_bytes, compression_opts=compression_opts)
+        wfile.create_dataset(
+            "metadata", data=metadata_bytes, compression_opts=compression_opts
+        )
 
         # Load the modes listed in mode_numbers list
         for item in modes_to_save:
             # For every ell mode list in modes_list
 
             ell_value, emm_list = item
 
@@ -1651,15 +1764,17 @@
                 # For every (ell, emm) mode.
 
                 data = wfa.mode(ell_value, emm_value)
                 # set the time and data axis
                 data_re = data.real
                 data_im = data.imag
 
-                save_data = np.transpose(np.array([wfa.time_axis, data_re, data_im]))
+                save_data = np.transpose(
+                    np.array([wfa.time_axis, data_re, data_im])
+                )
                 # Make the key
                 key = _key_gen(ell_value, emm_value, extras=f"r{r_ext:.2f}")
                 # message('Processing key', key)
                 # Create data set
                 wfile.create_dataset(key, data=save_data)
 
     return 1
```

### Comparing `waveformtools-2023.5.19/waveformtools/diagnostics.py` & `waveformtools-2023.6.3/waveformtools/diagnostics.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import numpy as np
 
 
 class method_info:
     """The methods for integration ,differential to be passed on
     for operations."""
 
-    def __init__(self, int_method="MP", diff_method="SH", ell_max=8, degree=8, reg=True):
+    def __init__(
+        self, int_method="MP", diff_method="SH", ell_max=8, degree=8, reg=True
+    ):
         self.int_method = int_method
         self.diff_method = diff_method
         self.ell_max = ell_max
         self.reg = reg
         self.degree = degree
```

### Comparing `waveformtools-2023.5.19/waveformtools/differentiate.py` & `waveformtools-2023.6.3/waveformtools/differentiate.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,36 +17,39 @@
     """Compute the derivative of the y data w.r.t the x data
     using the specified method. x_data can be non-uniformly sampled
     in which case the derivative will be computed by resampling.
 
     Parameters
     ----------
     x_data, y_data : 1d array
-                     The x and y data. x_data is assumed
-                     to be sorted.
+                                     The x and y data. x_data is assumed
+                                     to be sorted.
     method : str
-             The method to use for differentiation.
-             Presently supported values are
-             'CS' : Chebyshev
-             'FS' : Fourier
-             'FD' : Finite difference
+                     The method to use for differentiation.
+                     Presently supported values are
+                     'SP' : Spline
+                     'CS' : Chebyshev
+                     'FS' : Fourier
+                     'FD' : Finite difference
     degree : int
-            The algorithm degree to use for differentiating. This
-            is applicable when dealing with the 'CS'
-            method, which is the number of basis functions
-            to use and 'FD' method, which is the number
-            of points on either side to use.
+                    The algorithm degree to use for differentiating. This
+                    is applicable when dealing with the 'CS'
+                    method, which is the number of basis functions
+                    to use and 'FD' method, which is the number
+                    of points on either side to use.
 
     Returns
     -------
     dydx : 1d array
-           The first order derivative of y w.r.t. x.
+               The first order derivative of y w.r.t. x.
     """
 
-    if method == "CS":
+    if method == "SP":
+        dydx = spline_differential(x_data, y_data, k=degree)
+    elif method == "CS":
         dydx = Chebyshev_differential(x_data, y_data, order=1, degree=degree)
     else:
         delta_x_all = np.diff(x_data)
 
         if (delta_x_all - delta_x_all[0] < 1e-14).all():
             message("No interpolation required.")
             interp = False
@@ -61,15 +64,19 @@
             x_uniform = np.linspace(x_data[0], x_data[-1], 2 * len(x_data))
             y_uniform = interp1d(x_data, y_data, kind="cubic")(x_uniform)
 
         delta_x = np.diff(x_uniform)[0]
 
         if method == "FS":
             dydx_new, _, x_new, _ = Fourier_differential(
-                delta_x=delta_x, udata_x=y_uniform, order=1, zero_mode=0, taper=False
+                delta_x=delta_x,
+                udata_x=y_uniform,
+                order=1,
+                zero_mode=0,
+                taper=False,
             )
 
         elif method == "FD":
             if degree == 1:
                 dydx_new = differentiate(y_uniform, delta_x)
             elif degree == 2:
                 dydx_new = differentiate2(y_uniform, delta_x)
@@ -88,84 +95,121 @@
             dydx = interp1d(x_uniform, dydx_new, kind="cubic")(x_data)
         else:
             dydx = dydx_new
 
     return dydx
 
 
+#######################################################
+# Spline differentiation
+########################################################
+
+
+def spline_differential(x_data, y_data, k=5):
+    """Spline differentiation
+
+        Parameters
+        ----------
+    x_data, y_data : 1d array
+                     The x and y data. x_data is assumed
+                     to be sorted.
+
+        k : int
+                The interpolation order
+
+        Returns
+        -------
+    dydx : 1d array
+           The first order derivative of y w.r.t. x.
+    """
+
+    from scipy.interpolate import InterpolatedUnivariateSpline as interpolator
+
+    interp = interpolator(x_data, y_data, k=k)
+
+    dydx = interp.derivative()(x_data)
+
+    return dydx
+
+
 ########################################################
 # Chebyshev differentiation
 ########################################################
 
 
 def Chebyshev_differential(x_data, y_data, order=1, degree=8):
     """Differentiate a function using the Chebyshev expansion.
 
 
     Parameters
     ----------
 
 
-    x_data:	1d array
-                            The x data.
-    y_data:	1d array
-                    The y data.
+    x_data: 1d array
+                                                    The x data.
+    y_data: 1d array
+                                    The y data.
 
-    order:	int
-                    The number of times to differentiate.
+    order:  int
+                                    The number of times to differentiate.
 
-    degree:	int
-                            The number of basis functions to use.
+    degree: int
+                                                    The number of basis functions to use.
 
 
     Returns
     -------
 
-    dydx_data:	1d array
-                            The differentiated data.
+    dydx_data:  1d array
+                                                    The differentiated data.
 
     """
 
     # Find the basis coefficients.
     from numpy.polynomial.chebyshev import chebder, chebfit, chebval
 
     # L2errs = []
     # p_res = 1e21
     # for deg_index in range(degree):
-    # 	cheb_coeffs, result = chebfit(x_data, y_data, deg=deg_index, full=True)
-    # 	res = result[0][0]
+    #   cheb_coeffs, result = chebfit(x_data, y_data, deg=deg_index, full=True)
+    #   res = result[0][0]
     # if res%2==0:
-    # 	L2errs.append(res)
+    #   L2errs.append(res)
     # print(x_data, y_data)
     cheb_coeffs, result = chebfit(x_data, y_data, deg=degree, full=True)
 
+    message("Result", result, result[0], message_verbosity=1)
     res = result[0][0]
 
     # L2errs = [(a + b)  for a, b in zip(L2errs[::2], L2errs[1::2])]
 
     # best_deg = 2*np.argmin(L2errs)+2
     # if best_deg<degree:
     # plt.plot(L2errs)
     # plt.show()
 
-    # 	print(f'Optimizing degree to {best_deg}')
-    # 	degree=best_deg
-    # 	cheb_coeffs, result = chebfit(x_data, y_data, deg=degree, full=True)
+    #   print(f'Optimizing degree to {best_deg}')
+    #   degree=best_deg
+    #   cheb_coeffs, result = chebfit(x_data, y_data, deg=degree, full=True)
 
-    # 	res = result[0][0]
+    #   res = result[0][0]
     if res >= 1e-3:
         if res <= 1e-1 and res >= 1e-3:
             message(f"Residue warning {res}")
         elif res > 1e-1:
             import traceback
 
             traceback.print_stack()
             y_fit_data = chebval(x_data, cheb_coeffs)
-            plt.scatter(x_data, y_data, label="Input", s=3, c="magenta", marker="o")
-            plt.scatter(x_data, y_fit_data, label="fit", s=3, c="blue", marker="X")
+            plt.scatter(
+                x_data, y_data, label="Input", s=3, c="magenta", marker="o"
+            )
+            plt.scatter(
+                x_data, y_fit_data, label="fit", s=3, c="blue", marker="X"
+            )
             plt.grid()
             plt.legend()
             plt.show()
 
             message(f"Residue warning {res}: Bad fit!")
 
     # compute the derivative
@@ -178,57 +222,65 @@
 
 
 ########################################################
 # Fourier differentiation
 ########################################################
 
 
-def Fourier_differential(delta_x, udata_x=None, utilde_conven=None, omega0=np.inf, order=1, zero_mode=0, taper=True):
+def Fourier_differential(
+    delta_x,
+    udata_x=None,
+    utilde_conven=None,
+    omega0=np.inf,
+    order=1,
+    zero_mode=0,
+    taper=True,
+):
     """Fixed frequency differentiation, the inverse of the
     Fixed frequency integration as presented in Reisswig et al.
     This function takes in a function and returns its nth order
     derivative differential taken in the frequency domain.
 
 
     Parameters
     ----------
-    xaxis:	1d array
-            The co-ordinate space axis.
-    udata_x:	1d array
-                The data to be differentiated,
-                expressed in coordinate space.
-    omega0:	float, optional
-            The cutoff angular frequency in the integration.
-            Must be lower than the starting angular frequency
-            of the input waveform.
-    order:	int, optional
-            The number of times to differentiate
-            the integrand in time.
-    zero_mode:	float, optional
-                The zero mode amplitude of the FFT required.
-    taper:	bool
-            Whether or not to taper the real co-ordinate space data.
+    xaxis:  1d array
+                    The co-ordinate space axis.
+    udata_x:    1d array
+                            The data to be differentiated,
+                            expressed in coordinate space.
+    omega0: float, optional
+                    The cutoff angular frequency in the integration.
+                    Must be lower than the starting angular frequency
+                    of the input waveform.
+    order:  int, optional
+                    The number of times to differentiate
+                    the integrand in time.
+    zero_mode:  float, optional
+                            The zero mode amplitude of the FFT required.
+    taper:  bool
+                    Whether or not to taper the real co-ordinate space data.
 
     Returns
     -------
-    udata_differentiated:	1d array
-                            The input waveform in time-space, integrated
-                            in frequency space using FFI.
-
-    utilde_differentiated:	1d array
-                            The FFT of the frixed frequency
-                            differentiated array in good conventions.
-
-
-    new_x_axis:	1d array
-                The new x-axis, assuming the
-                data may have been changed in length
+    udata_differentiated:   1d array
+                                                    The input waveform in time-space, integrated
+                                                    in frequency space using FFI.
+
+    utilde_differentiated:  1d array
+                                                    The FFT of the frixed frequency
+                                                    differentiated array in good conventions.
+
+
+    new_x_axis: 1d array
+                            The new x-axis, assuming the
+                            data may have been changed in length
 
-    freq_axis:	1d array
-                The frequency axis of the FFT of data.
+    freq_axis:  1d array
+                            The frequency axis of the FFT of data.
 
     Notes
     -----
 
     The returned differentiated function of a real udata_x
     in real co-ordinate space is a complex number
     due to the numerical inaccuracies. Take
@@ -314,24 +366,24 @@
 
 def differentiate(data, delta_t):
     """Central difference derivative calculator. Forward/ backward Euler near the boundaries.
 
     Parameters
     ----------
 
-    data:	1d array
-                    The 1d data.
-    delta_t:	float
-                            The time step in units of t/M.
+    data:   1d array
+                                    The 1d data.
+    delta_t:    float
+                                                    The time step in units of t/M.
 
     Returns
     -------
 
-    dAdt:	1d array
-                    The derivative.
+    dAdt:   1d array
+                                    The derivative.
 
     """
 
     # A list to hold the derivatives.
     dAdt = []
 
     # Near boundaries: For n=0
@@ -354,24 +406,24 @@
 def differentiate2(data, delta_t):
     """Five point difference derivative calculator.  Not accurate near the boundaries.
 
 
     Parameters
     ----------
 
-    data:	1d array
-                    The 1d data.
-    delta_t:	float
-                            The time step in t/M.
+    data:   1d array
+                                    The 1d data.
+    delta_t:    float
+                                                    The time step in t/M.
 
     Returns
     -------
 
-    dAdt:	1d array
-                    The derivative.
+    dAdt:   1d array
+                                    The derivative.
 
     """
 
     # Number of points on right side.
     order = 2
 
     # The five point derivative stencil.
@@ -409,24 +461,24 @@
 def differentiate3(data, delta_t):
     """Seven point difference derivative calculator. Not accurate near the boundaries.
 
 
     Parameters
     ----------
 
-    data:	1d array
-                    The 1d data.
-    delta_t:	float
-                            The time step in t/M.
+    data:   1d array
+                                    The 1d data.
+    delta_t:    float
+                                                    The time step in t/M.
 
     Returns
     -------
 
-    dAdt:	1d array
-                    The derivative.
+    dAdt:   1d array
+                                    The derivative.
 
     """
 
     # The number of points on one direction.
     order = 3
     # The seven point stencil.
     coeffs = np.array([-1, 9, -45, 0, 45, -9, 1])
@@ -475,24 +527,24 @@
 def differentiate4(data, delta_t):
     """Nine point difference derivative calculator. Not accurate near the boundaries.
 
 
     Parameters
     ----------
 
-    data:	1d array
-                    The 1d data.
-    delta_t:	float
-                            The time step in t/M.
+    data:   1d array
+                                    The 1d data.
+    delta_t:    float
+                                                    The time step in t/M.
 
     Returns
     -------
 
-    dAdt:	1d array
-                    The derivative.
+    dAdt:   1d array
+                                    The derivative.
 
     """
 
     # The number of points on one side.
     order = 4
     # THe stencil.
     coeffs = np.array([3, -32, 168, -672, 0, 672, -168, 32, 3])
@@ -557,24 +609,24 @@
 def differentiate5(data, delta_t):
     """Eleven point difference derivative calculator. Not accurate near the boundaries.
 
 
     Parameters
     ----------
 
-    data:	1d array
-                    The 1d data.
-    delta_t:	float
-                            The time step in t/M.
+    data:   1d array
+                                    The 1d data.
+    delta_t:    float
+                                                    The time step in t/M.
 
     Returns
     -------
 
-    dAdt:	1d array
-                    The derivative of the data.
+    dAdt:   1d array
+                                    The derivative of the data.
 
     """
 
     # The number of points on one side.
     order = 5
     # The stencil.
     coeffs = np.array([-2, 25, -150, 600, -2100, 0, 2100, -600, 150, -25, 2])
@@ -653,24 +705,24 @@
 def differentiate5_vec_nonumba(data, delta_t):
     """Eleven point difference derivative calculator. Not accurate near the boundaries.
 
 
     Parameters
     ----------
 
-    data:	1d array
-                    The 1d data.
-    delta_t:	float
-                            The time step in t/M.
+    data:   1d array
+                                    The 1d data.
+    delta_t:    float
+                                                    The time step in t/M.
 
     Returns
     -------
 
-    dAdt:	1d array
-                    The derivative of the data.
+    dAdt:   1d array
+                                    The derivative of the data.
 
     """
 
     # import pdb
     # pdb.set_trace()
 
     data = np.transpose(data, (2, 0, 1))
@@ -743,15 +795,17 @@
     # der_data = np.append(der_data, [der4], axis=aax)
     der_data[4] = der4
     for index in range(order, len(data) - order):
         # For the interior points.
         data_subarray = data[index - order : index + order + 1]
         # der_data = np.append(der_data, [np.tensordot(coeffs, data_subarray, axes=((0), (0)))
         # / (divide * delta_t)], axis=aax)
-        der_data[index] = np.tensordot(coeffs, data_subarray, axes=((0), (0))) / (divide * delta_t)
+        der_data[index] = np.tensordot(
+            coeffs, data_subarray, axes=((0), (0))
+        ) / (divide * delta_t)
 
     # der_data = np.append(der_data, [derNm5], axis=aax)
     der_data[-5] = derNm5
     # der_data = np.append(der_data, [derNm4], axis=aax)
     der_data[-4] = derNm4
     # der_data = np.append(der_data, [derNm3], axis=aax)
     der_data[-3] = derNm3
@@ -768,24 +822,24 @@
 def differentiate5_vec_numba(data, delta_t):
     """Eleven point difference derivative calculator. Not accurate near the boundaries.
 
 
     Parameters
     ----------
 
-    data:	1d array
-                    The 1d data.
-    delta_t:	float
-                            The time step in t/M.
+    data:   1d array
+                                    The 1d data.
+    delta_t:    float
+                                                    The time step in t/M.
 
     Returns
     -------
 
-    dAdt:	1d array
-                    The derivative of the data.
+    dAdt:   1d array
+                                    The derivative of the data.
 
     """
 
     # import pdb
     # pdb.set_trace()
 
     s1, s2, s3 = data.shape
@@ -877,15 +931,17 @@
     for index in range(order, len(data) - order):
         # For the interior points.
         data_subarray = data[index - order : index + order + 1]
         # der_data = np.append(der_data, [np.tensordot(coeffs, data_subarray, axes=((0), (0)))
         # / (divide * delta_t)], axis=aax)
         # der_data[index] = np.tensordot(coeffs, data_subarray, axes=((0), (0))) / (divide * delta_t)
         for inner_index, val in enumerate(coeffs):
-            der_data[index] += val * data_subarray[inner_index] / (divide * delta_t)
+            der_data[index] += (
+                val * data_subarray[inner_index] / (divide * delta_t)
+            )
 
     # der_data = np.append(der_data, [derNm5], axis=aax)
     # der_data[-5] = derNm5
     # der_data = np.append(der_data, [derNm4], axis=aax)
     # der_data[-4] = derNm4
     # der_data = np.append(der_data, [derNm3], axis=aax)
     # der_data[-3] = derNm3
@@ -899,41 +955,47 @@
 
 
 ######################################################################################
 # Complex Amplitude-Phase differentiation
 ######################################################################################
 
 
-def differentiate_cwaveform(time_axis, waveform):
+def differentiate_cwaveform(time_axis, waveform, method="SP", degree=5):
     """Differentiate a given waveform by differentiating the Amplitude-Phase form.
 
     Parameters
     ----------
+    time_axis:  1d array
+                The time axis of the waveform.
 
-    time_axis:	1d array
-                            The time axis of the waveform.
-
-    waveform:	1d array
-                            The complex 1d array of the waveform timeseries.
+    waveform:   1d array
+                The complex 1d array of the waveform timeseries.
 
 
     Returns
     -------
-
-    differentiated_waveform:	1d array
-                                                            The waveform differentiated in time.
+    differentiated_waveform:    1d array
+                                The waveform differentiated in time.
 
     """
 
     # Get the amplitude and phase of the complex 1d waveform.
     from waveformtools.waveformtools import xtract_camp_phase
 
-    waveform_amp, waveform_phase = xtract_camp_phase(waveform.real, waveform.imag)
+    waveform_amp, waveform_phase = xtract_camp_phase(
+        waveform.real, waveform.imag
+    )
 
     # Differentiate the waveform.
 
-    Amplitude_dot = Chebyshev_differential(time_axis, waveform_amp, degree=25)
-    Phase_dot = Chebyshev_differential(time_axis, waveform_phase, degree=25)
-
-    differentiated_waveform = (Amplitude_dot + waveform_amp * 1j * Phase_dot) * np.exp(1j * waveform_phase)
+    Amplitude_dot = derivative(
+        time_axis, waveform_amp, method=method, degree=degree
+    )
+    Phase_dot = derivative(
+        time_axis, waveform_phase, method=method, degree=degree
+    )
+
+    differentiated_waveform = (
+        Amplitude_dot + waveform_amp * 1j * Phase_dot
+    ) * np.exp(1j * waveform_phase)
 
     return differentiated_waveform
```

### Comparing `waveformtools-2023.5.19/waveformtools/extrapolate.py` & `waveformtools-2023.6.3/waveformtools/extrapolate.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,279 +9,283 @@
 
 ###############################################
 # Basic utilities
 ###############################################
 
 
 def r_to_ra_conversion(coord_radius, mass=1, spin=0):
-    """Convert the isotropic co-ordinate radius parameter `r` in the ETK simulations
-            into the approximate areal radius.
+    """Convert the isotropic co-ordinate radius parameter `r`
+    in the ETK simulations into the approximate areal radius.
 
     Parameters
     ----------
-
-    coord_radius:	float
-                                    The coordinate radius in the Einstein toolkit
-
-    mass:	float, optional
-                    The sum of the quasi-local horizon (Christodolou) masses of the black holes.
-                    Defaults to 1.
-
-    spin:	float, optional
-                    The magnitude of the spin of the system, as approximated by a single Kerr black hole
-                    far away from the system. Defaults to 0.
-
+    coord_radius : float
+                   The coordinate radius in the Einstein toolkit
+    mass : float, optional
+           The sum of the quasi-local (Christodolou) horizon masses
+           of the black holes. Defaults to 1.
+    spin : float, optional
+           The magnitude of the spin of the system, as approximated
+           by a single Kerr black hole far away from the system.
+           Defaults to 0.
 
     Returns
     -------
-
-    areal_radius:	float
-                                    The appriximate areal radius of the sphere.
+    areal_radius : float
+                   The appriximate areal radius of the sphere.
 
 
     Notes
     -----
-
-    Assumes that the system interoir to the sphere at co-ordinate radius `r_coord` is well approximated by a
-    Kerr black hole.
-
-
+    Assumes that the system interoir to the sphere at co-ordinate radius `r_coord`
+    is well approximated by a deformed Kerr black hole.
 
     References
     ----------
 
-    Nakano et al., (2015),	Phys. Rev. D 91, 104022, in-text below Eq.[30].
+    Nakano et al., (2015),  Phys. Rev. D 91, 104022, in-text below Eq.[30].
     """
 
-    areal_radius = coord_radius * (1 + (mass + spin) / (2 * coord_radius)) * (1 + (mass - spin) / (2 * coord_radius))
+    areal_radius = (
+        coord_radius
+        * (1 + (mass + spin) / (2 * coord_radius))
+        * (1 + (mass - spin) / (2 * coord_radius))
+    )
 
     return areal_radius
 
 
 ############################################################################
 # Perturbative extraction
 ############################################################################
 
 
-def waveextract_to_inf_perturbative_twop5_order(rPsi4_rlm, delta_t, areal_radius=500, mass=1, spin=0, ell=2, emm=2):
+def waveextract_to_inf_perturbative_twop5_order(
+    rPsi4_rlm,
+    delta_t,
+    areal_radius=500,
+    mass=1,
+    spin=0,
+    ell=2,
+    emm=2,
+    degree=24,
+    method="CS",
+):
     """Extract a numerical waveform to null infinity using perturbative techniques. This is :
             * accurate to second order in :math:`1/r`.
             * accurate to first order in Kerr mass and spin.
             * corrects for spheroidal harmonics
 
-
-
     Parameters
     ----------
-
-    rPsi4_rlm:	1d array
-                            The extracted Weyl scalar :math:`r\\Psi_{4\\ell m}` data array
-
-    delta_t:	float
-                            The time stepping.
-
-
-    areal_radius:	1d array
-                                    The areal radius of the extraction sphere.
-
-
-    mass:	float
-                    The total horizon mass of the system.
-
-    spin:	float, optional
-                    The effective spin of the spacetime. Defaults to 0.
-
-    ell:	int
-                    The polar quantum number :math:`\\ell`.
-
-    emm:	int
-                    The azimuthal quantum number :math:`m`.
+    rPsi4_rlm : 1d array
+                The extracted Weyl scalar :math:`r\\Psi_{4\\ell m}` data array
+    delta_t : float
+              The time stepping.
+    areal_radius : 1d array
+                   The areal radius of the extraction sphere.
+    mass : float
+           The total horizon mass of the system.
+    spin : float, optional
+           The effective spin of the spacetime. Defaults to 0.
+    ell : int
+          The polar quantum number :math:`\\ell`.
+    emm : int
+          The azimuthal quantum number :math:`m`.
+    method : str
+             The method to use for differentiation.
+    degree : int
+             The degree to use for dfferentiation.
 
     Returns
     -------
-
-    rPsi4_inflm:	1d array
-                            The waveform extracted to null infninity :math:`\\mathcal{I}^+`
-
+    rPsi4_inflm : 1d array
+                  The waveform extracted to
+                  null infninity :math:`\\mathcal{I}^+`
 
     References
     ----------
-
-    This implements the definition in Nakano et al., (2015),  Phys. Rev. D 91, 104022 Eq.[29].
-
-
+    This implements the definition in Nakano et al., (2015),
+    Phys. Rev. D 91, 104022 Eq.[29].
     """
 
     from waveformtools.differentiate import differentiate_cwaveform
     from waveformtools.integrate import fixed_frequency_integrator
 
     # Timeaxis
 
     timeaxis = np.arange(0, len(rPsi4_rlm) * delta_t, delta_t)
     # Assigning the terms. Each set of subterms in a pair of paranthesis is a term.
     term_1_prefac = 1 - 2 * mass / areal_radius
     subterm_1_1 = rPsi4_rlm
     subterm_1_2_prefac = (ell - 1) * (ell + 2) / (2 * areal_radius)
-    subterm_1_2, _ = fixed_frequency_integrator(rPsi4_rlm, delta_t, omega0=0.015)  # Integral_rPsi4_rlm
-    subterm_1_3_prefac = (ell - 1) * (ell + 2) * (ell**2 + ell - 4) / (8 * areal_radius**2)
-    subterm_1_3, _ = fixed_frequency_integrator(rPsi4_rlm, delta_t, order=2, omega0=0.015)  # Double_integral_rPsi4_rlm
-
-    term_1 = term_1_prefac * (subterm_1_1 + subterm_1_2_prefac * subterm_1_2 + subterm_1_3_prefac * subterm_1_3)
+    subterm_1_2, _ = fixed_frequency_integrator(
+        rPsi4_rlm, delta_t, omega0=0.015
+    )  # Integral_rPsi4_rlm
+    subterm_1_3_prefac = (
+        (ell - 1) * (ell + 2) * (ell**2 + ell - 4) / (8 * areal_radius**2)
+    )
+    subterm_1_3, _ = fixed_frequency_integrator(
+        rPsi4_rlm, delta_t, order=2, omega0=0.015
+    )  # Double_integral_rPsi4_rlm
+
+    term_1 = term_1_prefac * (
+        subterm_1_1
+        + subterm_1_2_prefac * subterm_1_2
+        + subterm_1_3_prefac * subterm_1_3
+    )
 
     term_2_prefac = (2 * 1j * spin / (ell + 1) ** 2) * np.sqrt(
-        (ell + 3) * (ell - 1) * (ell + emm + 1) * (ell - emm + 1) / ((2 * ell + 1) * (2 * ell + 3))
+        (ell + 3)
+        * (ell - 1)
+        * (ell + emm + 1)
+        * (ell - emm + 1)
+        / ((2 * ell + 1) * (2 * ell + 3))
     )
-    subterm_2_1 = differentiate_cwaveform(timeaxis, rPsi4_rlm)  # Differential of waveform
+    subterm_2_1 = differentiate_cwaveform(
+        timeaxis, rPsi4_rlm, method=method, degree=degree
+    )  # Differential of waveform
     subterm_2_2_prefac = -ell * (ell + 3) / areal_radius
     subterm_2_2 = subterm_1_1
 
     term_2 = term_2_prefac * (subterm_2_1 + subterm_2_2_prefac * subterm_2_2)
 
     term_3_prefac = (-2 * 1j * spin / ell**2) * np.sqrt(
-        ((ell + 2) * (ell - 2) * (ell + emm) * (ell - emm)) / ((2 * ell - 1) * (2 * ell + 1))
+        ((ell + 2) * (ell - 2) * (ell + emm) * (ell - emm))
+        / ((2 * ell - 1) * (2 * ell + 1))
     )
     subterm_3_1 = subterm_2_1
     subterm_3_2_prefac = -(ell - 2) * (ell + 1) / areal_radius
     subterm_3_2 = subterm_1_1
 
     term_3 = term_3_prefac * (subterm_3_1 + subterm_3_2_prefac * subterm_3_2)
 
     rPsi4_inflm = term_1 + term_2 + term_3
 
     return rPsi4_inflm
 
 
-def waveextract_to_inf_perturbative_two_order(rPsi4_rlm, delta_t, areal_radius=500, mass=1, ell=2):
+def waveextract_to_inf_perturbative_two_order(
+    rPsi4_rlm, delta_t, areal_radius=500, mass=1, ell=2
+):
     """Extract a numerical waveform to null infinity using perturbative techniques. This is :
             * accurate to second order in :math:`1/r`.
             * accurate to first order in Kerr mass and spin.
             * corrects for spheroidal harmonics
 
-
-
     Parameters
     ----------
-
-    rPsi4_rlm:	1d array
-                            The extracted Weyl scalar :math:`r\\Psi_{4\\ell m}` data array.
-
-    delta_t:	float
-                            The time stepping.
-
-    areal_radius:	1d array
-                                    The areal radius of the extraction sphere.
-
-
-    mass:	float
-                    The total horizon mass of the system.
-
-    spin:	float, optional
-                    The effective spin of the spacetime. Defaults to 0.
-
-    ell:	int
-                    The polar quantum number :math:`\\ell`.
-
-    emm:	int
-                    The azimuthal quantum number :math:`m`.
+    rPsi4_rlm : 1d array
+                The extracted Weyl scalar :math:`r\\Psi_{4\\ell m}` data array.
+    delta_t : float
+              The time stepping.
+    areal_radius : 1d array
+                   The areal radius of the extraction sphere.
+    mass : float
+           The total horizon mass of the system.
+
+    spin : float, optional
+           The effective spin of the spacetime. Defaults to 0.
+    ell : int
+          The polar quantum number :math:`\\ell`.
+    emm : int
+          The azimuthal quantum number :math:`m`.
 
     Returns
     -------
-
-    rPsi4_inflm:	1d array
-                            The waveform extracted to null infninity :math:`\\mathcal{I}^+`
-
+    rPsi4_inflm : 1d array
+                  The waveform extracted to
+                  null infninity :math:`\\mathcal{I}^+`
 
     References
     ----------
-
-    This implements the definition in Nakano et al., (2015),  Phys. Rev. D 91, 104022 Eq.[29].
-
-
+    This implements the definition in Nakano et al., (2015),
+    Phys. Rev. D 91, 104022 Eq.[29].
     """
 
     from integrate import fixed_frequency_integrator
 
     # Assigning the terms. Each set of subterms in a pair of paranthesis is a term.
     term_1 = rPsi4_rlm
 
     term_2_prefac = -(ell - 1) * (ell + 2) / (2 * areal_radius)
-    subterm_2_1, _ = fixed_frequency_integrator(rPsi4_rlm, delta_t, omega0=0.015)  # Integral_rPsi4_rlm
+    subterm_2_1, _ = fixed_frequency_integrator(
+        rPsi4_rlm, delta_t, omega0=0.015
+    )  # Integral_rPsi4_rlm
     term_2 = term_2_prefac * subterm_2_1
 
-    term_3_prefac = (ell - 1) * (ell + 2) * (ell**2 + ell - 4) / (8 * areal_radius**2)
-    subterm_3_1, _ = fixed_frequency_integrator(rPsi4_rlm, delta_t, order=2, omega0=0.015)  # Double_Integral_rPsi4_rlm
+    term_3_prefac = (
+        (ell - 1) * (ell + 2) * (ell**2 + ell - 4) / (8 * areal_radius**2)
+    )
+    subterm_3_1, _ = fixed_frequency_integrator(
+        rPsi4_rlm, delta_t, order=2, omega0=0.015
+    )  # Double_Integral_rPsi4_rlm
     term_3 = term_3_prefac * subterm_3_1
 
     term_4_prefac = -3 * mass / (2 * areal_radius**2)
     subterm_4_1 = subterm_2_1
     term_4 = term_4_prefac * subterm_4_1
 
     rPsi4_inflm = term_1 + term_2 + term_3 + term_4
 
     return rPsi4_inflm
 
 
-def waveextract_to_inf_perturbative_one_order(u_ret, rPsi4_rlm, areal_radius=500, ell=2):
+def waveextract_to_inf_perturbative_one_order(
+    u_ret, rPsi4_rlm, areal_radius=500, ell=2
+):
     """Extract a numerical waveform to null infinity using perturbative techniques. This is :
             * accurate to second order in :math:`1/r`.
             * accurate to first order in Kerr mass and spin.
             * corrects for spheroidal harmonics
 
-
-
     Parameters
     ----------
-
-    u_ret:	1d array
-                    The retarted time array at the location r = areal_radius.
-
-    rPsi4_rlm:	1d array
-                            The extracted Weyl scalar :math:`r\\Psi_{4\\ell m}` data array
-
-    areal_radius:	1d array
-                                    The areal radius of the extraction sphere.
-
-
-    mass:	float
-                    The total horizon mass of the system.
-
-    ell:	int
-                    The polar quantum number :math:`\\ell`.
-
-    emm:	int
-                    The azimuthal quantum number :math:`m`.
+    u_ret : 1d array
+            The retarted time array at the location r = areal_radius.
+    rPsi4_rlm : 1d array
+                The extracted Weyl scalar :math:`r\\Psi_{4\\ell m}` data array
+    areal_radius : 1d array
+                   The areal radius of the extraction sphere.
+    mass : float
+           The total horizon mass of the system.
+    ell : int
+          The polar quantum number :math:`\\ell`.
+    emm : int
+          The azimuthal quantum number :math:`m`.
 
     Returns
     -------
-
-    rPsi4_inflm:	1d array
-                            The waveform extracted to null infninity :math:`\\mathcal{I}^+`
-
+    rPsi4_inflm : 1d array
+                  The waveform extracted to
+                  null infninity :math:`\\mathcal{I}^+`
 
     References
     ----------
-
-    This implements the definition in Nakano et al., (2015),  Phys. Rev. D 91, 104022 Eq.[29].
-
-
+    This implements the definition in
+    Nakano et al., (2015),  Phys. Rev. D 91, 104022 Eq.[29].
     """
 
     # Get the amplitude and phase
     A_lm, _ = waveformtools.xtract_camp_phase(rPsi4_rlm.real, rPsi4_rlm.imag)
 
     # Get the time stepping
     delta_t = u_ret[1] - u_ret[0]
 
     # Get the waveform instantaneous frequency
-    omega_lm = waveformtools.get_waveform_angular_frequency(rPsi4_rlm, delta_t=delta_t, timeaxis=u_ret)
+    omega_lm = waveformtools.get_waveform_angular_frequency(
+        rPsi4_rlm, delta_t=delta_t, timeaxis=u_ret
+    )
 
     # Assigning the terms. Each set of subterms in a pair of paranthesis is a term.
 
     # The amplitude correction factor
-    A_lm_correction = 0.5 * np.power(((ell * (ell + 1) / (2 * omega_lm * areal_radius))), 2)
+    A_lm_correction = 0.5 * np.power(
+        ((ell * (ell + 1) / (2 * omega_lm * areal_radius))), 2
+    )
 
     # The phase correction factor.
     sin_Phase_correction = ell * (ell + 1) / (2 * omega_lm * areal_radius)
     cos_Phase_correction = np.sqrt(1 - np.power(sin_Phase_correction, 2))
     Phase_correction = cos_Phase_correction + 1j * sin_Phase_correction
 
     # The extrapolated waveform
```

### Comparing `waveformtools-2023.5.19/waveformtools/grids.py` & `waveformtools-2023.6.3/waveformtools/grids.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,65 +8,64 @@
 gl_grid : grid info
           Stores a Gauss-Legendre type grid on a spherical surface.
 """
 
 import numpy as np
 
 # from numba import jit, njit
-
 # import numba as nb
-
 # from numba.experimental import jitclass
 
 
 class spherical_grid:
     """A class to store the coordinate grid on a sphere.
 
     Attributes
     ----------
-    ntheta: int
-                            The number of angular points in the :math:`\\theta`
-                            direction, including ghost zones.
-    nphi:   int
-                    The number of angular points in the :math:`\\phi`
-                    direction, including ghost zones.
-    nghosts:    int
-                            The number of ghost zones at the end of
-                            each direction.
-    meshgrid:   tuple of 2d array
-                            The 2d array containing the meshgrid of
-                            (:math:`\\theta, \\phi`) angular points.
-    theta_1d:   1d array
-                            The 1d array of angular points
-                            along the :math:`\\theta` axis.
-    phi_1d: 1d array
-                            The 1d array of angular points
-                            along the :math:`\\phi` axis.
-    dtheta: float
-                            The angular step size in the :math:`\\theta`
-                            direction.
-    dphi:   float
-                    The angular step size inthe :math:`\\phi`
-                    direction.
-    npix_act:   int
-                            The total number of gridpoints on the sphere,
-                            excluding the ghost points.
-    meshgrid:
-                            Get the 2d angular grid.
+    ntheta : int
+             The number of angular points in the :math:`\\theta`
+             direction, including ghost zones.
+    nphi : int
+           The number of angular points in the :math:`\\phi`
+           direction, including ghost zones.
+    nghosts : int
+              The number of ghost zones at the end of
+              each direction.
+    meshgrid : tuple of 2d array
+               The 2d array containing the meshgrid of
+               (:math:`\\theta, \\phi`) angular points.
+    theta_1d : 1d array
+               The 1d array of angular points
+               along the :math:`\\theta` axis.
+    phi_1d : 1d array
+             The 1d array of angular points
+             along the :math:`\\phi` axis.
+    dtheta : float
+             The angular step size in the :math:`\\theta`
+             direction.
+    dphi : float
+           The angular step size in the :math:`\\phi`
+           direction.
+    npix_act : int
+               The total number of gridpoints on the sphere,
+               excluding the ghost points.
+    meshgrid : 2darray (2)
+               Get the 2d angular grid.
 
     Methods
     -------
-    theta_1d:
-                            Get the :math:`\\theta` axis.
-    phi_1d:
-                            Get the :math:`\\phi` axis.
-
+    theta_1d :
+               Get the :math:`\\theta` axis.
+    phi_1d :
+               Get the :math:`\\phi` axis.
     """
 
-    def __init__(self, nphi=80, ntheta=41, nphimax=124, nthetamax=66, nghosts=2):
+    def __init__(
+        self, nphi=80, ntheta=41, nphimax=124, nthetamax=66, nghosts=2
+    ):
         # Number of gridpoints along phi direction including ghost points.
         self.nphi = nphi
         # Number of gridpoints along theta direction including ghost points.
         self.ntheta = ntheta
         # Total length of phi array used by ETK.
         self.nphimax = nphimax
         # Total length of theta array used by ETK.
@@ -130,72 +129,71 @@
         the coordinate index. The coordinate index
         ranges from (0, ntheta). The actual indices
         without the ghost and extra zones
         is (nghosts, ntheta-nghosts).
 
         Parameters
         -----------
-
-        theta_index:    int/ 1d array
-                                        The theta coordinate index or axis.
+        theta_index : int or 1d array
+                      The theta coordinate index or axis.
 
         Returns
         -------
-
-        theta_1d:   float
-                                The coordinate(s) :math:`\\theta` on the sphere.
-
+        theta_1d : float
+                   The coordinate(s) :math:`\\theta` on the sphere.
         """
 
         if not theta_index:
             theta_index = np.arange(self.nghosts, self.ntheta - self.nghosts)
 
-        return (theta_index - self.nghosts + 0.5) * np.pi / (self.ntheta - 2 * self.nghosts)
+        return (
+            (theta_index - self.nghosts + 0.5)
+            * np.pi
+            / (self.ntheta - 2 * self.nghosts)
+        )
 
     def phi_1d(self, phi_index=None):
         """Returns the coordinate value theta
         given the coordinate index. The coordinate
         index lies in (0, nphi). The actual indices
         without the ghost and extra zones
         is (nghosts, nphi-nghosts).
 
         Parameters
         -----------
-
-        phi_1d: int / 1d array
-                                The phi coordinate index or axis.
+        phi_1d : int / 1d array
+                 The phi coordinate index or axis.
 
         Returns
         -------
-
-        phi_1d: float or 1d array
-                                The coordinate(s) :math:`\\phi` on the sphere.
-
+        phi_1d : float or 1d array
+                 The coordinate(s) :math:`\\phi` on the sphere.
         """
 
         if not phi_index:
             phi_index = np.arange(self.nghosts, self.nphi - self.nghosts)
 
-        return (phi_index - self.nghosts) * 2 * np.pi / (self.nphi - 2 * self.nghosts)
+        return (
+            (phi_index - self.nghosts)
+            * 2
+            * np.pi
+            / (self.nphi - 2 * self.nghosts)
+        )
 
     @property
     def meshgrid(self):
         """The (:math:`\\theta, \\phi)`: coordinate meshes.
-                Excludes the ghost zones.
-
+        Excludes the ghost zones.
 
         Returns
         -------
-
-        theta:  2d array
-                        The :math:`\\theta` coordinate matrix for vectorization.
-
-        phi:    2d array
-                        The :math:`\\phi` coordinate matrix for vectorization.
-
+        theta : 2d array
+                The :math:`\\theta` coordinate matrix for vectorization.
+        phi : 2d array
+              The :math:`\\phi` coordinate matrix for vectorization.
         """
 
         theta, phi = np.meshgrid(self.theta_1d(), self.phi_1d())
 
         # theta = np.zeros((self.ntheta_act, self.nphi_act))
         # phi   = np.zeros((self.ntheta_act, self.nphi_act))
 
@@ -208,61 +206,60 @@
 
 
 class gl_grid:
     """A class to store the coordinate grid on a sphere.
 
     Attributes
     ----------
-    ntheta: int
-                The number of angular points in the :math:`\\theta`
-                direction, including ghost zones.
-    nphi:   int
-            The number of angular points in the :math:`\\phi`
-            direction, including ghost zones.
-    nghosts:    int
-                The number of ghost zones at the end of
-                each direction.
-    meshgrid:   tuple of 2d array
-                The 2d array containing the meshgrid of
-                (:math:`\\theta, \\phi`) angular points.
-    theta_1d:   1d array
-                The 1d array of angular points
-                along the :math:`\\theta` axis.
-    phi_1d: 1d array
-                The 1d array of angular points
-                along the :math:`\\phi` axis.
-    dtheta: float
-                The angular step size in the :math:`\\theta`
-                direction.
-    dphi:   float
-            The angular step size inthe :math:`\\phi`
-            direction.
-    npix_act:   int
-                The total number of gridpoints on the sphere,
-                excluding the ghost points.
-    meshgrid:
-                Get the 2d angular grid.
+    ntheta : int
+             The number of angular points in the :math:`\\theta`
+             direction, including ghost zones.
+    nphi : int
+           The number of angular points in the :math:`\\phi`
+           direction, including ghost zones.
+    nghosts : int
+              The number of ghost zones at the end of
+              each direction.
+    meshgrid : tuple of 2d array
+               The 2d array containing the meshgrid of
+               (:math:`\\theta, \\phi`) angular points.
+    theta_1d : 1d array
+               The 1d array of angular points
+               along the :math:`\\theta` axis.
+    phi_1d : 1d array
+             The 1d array of angular points
+             along the :math:`\\phi` axis.
+    dtheta : float
+             The angular step size in the :math:`\\theta`
+             direction.
+    dphi : float
+           The angular step size inthe :math:`\\phi`
+           direction.
+    npix_act : int
+               The total number of gridpoints on the sphere,
+               excluding the ghost points.
+    meshgrid :
+               Get the 2d angular grid.
 
     Methods
     -------
-    theta_1d:
-                Get the :math:`\\theta` axis.
-    phi_1d:
-                Get the :math:`\\phi` axis.
+    theta_1d :
+               Get the :math:`\\theta` axis.
+    phi_1d :
+             Get the :math:`\\phi` axis.
 
     Notes
     -----
-
     The total number of points on the sphere is assumed to be :math:`(L+1)^2`
 
     :math:`N_\theta = L+1`
 
     :math:`N_\phi = 2(L+1)`
 
-    This integrates out spherical harmonics of degree L exactly,
+    This integrates out spherical harmonics of degree `L` exactly,
     given a regular function on the sphere.
     """
 
     def __init__(self, nphi=None, ntheta=None, L=47, nghosts=2):
         # Number of gridpoints along phi direction including ghost points.
         self._nphi = nphi
         # Number of gridpoints along theta direction including ghost points.
@@ -294,15 +291,17 @@
                 raise ValueError("Please specify L or angular points!")
             else:
                 self.L = self.ntheta - 1
                 assert nphi % 2 == 0
 
         from scipy.special import roots_legendre
 
-        cpoints, self._weights, self._sum_of_weights = roots_legendre(L + 1, mu=True)
+        cpoints, self._weights, self._sum_of_weights = roots_legendre(
+            L + 1, mu=True
+        )
 
         # xpoints = (np.pi-np.arccos(cpoints))
         xpoints = np.arccos(cpoints[::-1])
         self._theta_1d = xpoints
 
         dphi = 2 * np.pi / self._nphi_act
 
@@ -405,61 +404,53 @@
     def theta_1d(self):
         """Returns the coordinate values theta given the coordinate index.
         The coordinate index ranges from (0, ntheta). The actual indices
         without the ghost and extra zones is (nghosts, ntheta-nghosts).
 
         Parameters
         -----------
-
-        theta_index:    int/ 1d array
-                        The theta coordinate index or axis.
+        theta_index : int/ 1d array
+                      The theta coordinate index or axis.
 
         Returns
         -------
-
-        theta_1d:   float
-                    The coordinate(s) :math:`\\theta` on the sphere.
-
+        theta_1d : float
+                   The coordinate(s) :math:`\\theta` on the sphere.
         """
 
         return self._theta_1d
 
     @property
     def phi_1d(self):
         """Returns the coordinate values phi given the coordinate index.
         The coordinate index lies in (0, nphi). The actual indices without
         the ghost and extra zones is (nghosts, nphi-nghosts).
 
         Parameters
         -----------
-
-        phi_1d: int / 1d array
-                    The phi coordinate index or axis.
+        phi_1d : int / 1d array
+                 The phi coordinate index or axis.
 
         Returns
         -------
-
-        phi_1d: float or 1d array
-                    The coordinate(s) :math:`\\phi` on the sphere.
-
+        phi_1d : float or 1d array
+                 The coordinate(s) :math:`\\phi` on the sphere.
         """
 
         return self._phi_1d
 
     @property
     def meshgrid(self):
         """The (:math:`\\theta, \\phi)`: coordinate meshes.
-            Excludes the ghost zones.
+        Excludes the ghost zones.
 
 
         Returns
         -------
-
-        theta:  2d array
+        theta : 2d array
                 The :math:`\\theta` coordinate matrix for vectorization.
 
-        phi:    2d array
-                The :math:`\\phi` coordinate matrix for vectorization.
-
+        phi : 2d array
+              The :math:`\\phi` coordinate matrix for vectorization.
         """
 
         return self._meshgrid
```

### Comparing `waveformtools-2023.5.19/waveformtools/integrate.py` & `waveformtools-2023.6.3/waveformtools/integrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,63 +9,64 @@
 from waveformtools.waveformtools import message
 
 ##################################################
 # Fixed frequency integration
 ##################################################
 
 
-def fixed_frequency_integrator(udata_time, delta_t, utilde_conven=None, omega0=0, order=1, zero_mode=0):
+def fixed_frequency_integrator(
+    udata_time, delta_t, utilde_conven=None, omega0=0, order=1, zero_mode=0
+):
     """Fixed frequency integrator as presented in Reisswig et. al.
 
 
     Parameters
     ----------
-    udata_time:	1d array
-                            The input data in time.
-    delta_t:	float
-                            The time stepping.
-
-    utilde_conven:		1d array, optional
-                                            The conventional FFT of the samples udata_time.
-    omega0:	float, optional
-            The cutoff angular frequency in the integration.
-            Must be lower than the starting angular frequency
-            of the input waveform. All frequencies whose absolute
-            value is below this value will be neglected.
-            The default cutoff-value is 0.
-
-    order:		int, optional
-                The number of times to integrate
-                the integrand in time. Defaults to 1.
-
-    zero_mode:	float, optional
-                            The zero mode amplitude of the FFT required.
-                            Defaults to 0 i.e. the zero mode is removed.
+    udata_time : 1d array
+                 The input data in time.
+    delta_t : float
+              The time stepping.
+
+    utilde_conven : 1d array, optional
+                    The conventional FFT of the samples udata_time.
+    omega0 : float, optional
+             The cutoff angular frequency in the integration.
+             Must be lower than the starting angular frequency
+             of the input waveform. All frequencies whose absolute
+             value is below this value will be neglected.
+             The default cutoff-value is 0.
+
+    order : int, optional
+            The number of times to integrate
+            the integrand in time. Defaults to 1.
+
+    zero_mode : float, optional
+                The zero mode amplitude of the FFT required.
+                Defaults to 0 i.e. the zero mode is removed.
 
     Returns
     -------
+    u_integ_n_time : 1d array
+                     The input waveform in time-space,
+                     integrated in frequency space using FFI.
 
-    u_integ_n_time:	1d array
-                                            The input waveform in time-space, integrated in frequency space using FFI.
-
-    u_integ_integ_n:	1d array
-                                            The integrated u samples in Fourier space.
-
+    u_integ_integ_n : 1d array
+                      The integrated u samples in Fourier space.
     """
 
     if not utilde_conven:
         # Compute the FFT of data
         from numpy.fft import ifft
 
         from waveformtools.transforms import compute_fft, unset_fft_conven
 
         # from waveformtools import taper
         # udata_x_re = taper(u_time.real, delta_t=delta_t)
         # udata_x_im = taper(u_time.imag, delta_t=delta_t)
-        # udata_x	   = np.array(udata_x_re) + 1j * np.array(udata_x_im)
+        # udata_x      = np.array(udata_x_re) + 1j * np.array(udata_x_im)
         # x_axis = udata_x_re.sample_times
         # udata_x = np.array(udata_x)
         freq_axis, utilde_conven = compute_fft(udata_time, delta_t)
 
         # Find the length of the input data.
         Nlen = len(udata_time)
 
@@ -126,18 +127,18 @@
 
 def TwoDIntegral(func, info, method="DH"):
     """Integrate a function over a sphere.
 
     Parameters
     ----------
     func : function
-            The function to be integrated
+           The function to be integrated
     NTheta, NPhi : int
-             The number of grid points in the theta and phi directions.
-             Note that NTheta must be even.
+                   The number of grid points in the theta and phi directions.
+                   Note that NTheta must be even.
     ht, hp : float
              The grid spacings.
     method : string
              The method to use for the integration. Options are DH (Driscoll Healy), SP (Simpson's), MP (Midpoint).
 
     Returns
     -------
@@ -171,19 +172,19 @@
     """Evaulate the 2D surface integral using the midpoint rule.
 
     Parameters
     ----------
     func : ndarray
            The data to be integrated
     info : surface_grid_info
-            An instance of the surface grid info class containing information about the grid.
+           An instance of the surface grid info class containing information about the grid.
     Returns
     -------
      integ : float
-            The function f integrated over the sphere.
+             The function f integrated over the sphere.
     """
 
     ht = info.dtheta
     hp = info.dphi
 
     theta_grid, _ = info.meshgrid
 
@@ -296,31 +297,46 @@
     assert NTheta % 2 == 0
     assert NPhi % 2 == 0
 
     Px = int(NTheta / 2)
     Py = int(NPhi / 2)
 
     # Around corners
-    integrand_sum += func[0, 0] + func[NTheta - 1, 0] + func[0, NPhi - 1] + func[NTheta - 1, NPhi - 1]
+    integrand_sum += (
+        func[0, 0]
+        + func[NTheta - 1, 0]
+        + func[0, NPhi - 1]
+        + func[NTheta - 1, NPhi - 1]
+    )
 
     # Arount edges
     for index_phi in range(1, Py):
-        integrand_sum += 4 * func[0, 2 * index_phi - 1] + 4 * func[NTheta - 1, 2 * index_phi - 1]
+        integrand_sum += (
+            4 * func[0, 2 * index_phi - 1]
+            + 4 * func[NTheta - 1, 2 * index_phi - 1]
+        )
 
     # for (iy = 1; iy <= py-1; iy++)
     for index_phi in range(1, Py - 1):
-        integrand_sum += 2 * func[0, 2 * index_phi] + 2 * func[NTheta - 1, 2 * index_phi]
+        integrand_sum += (
+            2 * func[0, 2 * index_phi] + 2 * func[NTheta - 1, 2 * index_phi]
+        )
 
     # for (ix = 1; ix <= px; ix++)
     for index_theta in range(1, Px):
-        integrand_sum += 4 * func[2 * index_theta - 1, 0] + 4 * func[2 * index_theta - 1, NPhi - 1]
+        integrand_sum += (
+            4 * func[2 * index_theta - 1, 0]
+            + 4 * func[2 * index_theta - 1, NPhi - 1]
+        )
 
     # for (ix = 1; ix <= px-1; ix++)
     for index_theta in range(1, Px - 1):
-        integrand_sum += 2 * func[2 * index_theta, 0] + 2 * func[2 * index_theta, NPhi - 1]
+        integrand_sum += (
+            2 * func[2 * index_theta, 0] + 2 * func[2 * index_theta, NPhi - 1]
+        )
 
     # In the Interiors
     # for (iy = 1; iy <= py; iy++)
     for index_phi in range(1, Py):
         # for (ix = 1; ix <= px; ix++)
         for index_theta in range(1, Px):
             integrand_sum += 16 * func[2 * index_theta - 1, 2 * index_phi - 1]
@@ -350,18 +366,18 @@
     """Evaulate the 2D surface integral using the Gauss-Legendre rule.
 
     Parameters
     ----------
     func : ndarray
            The data to be integrated
     info : surface_grid_info
-            An instance of the surface grid info class containing information about the grid.
+           An instance of the surface grid info class containing information about the grid.
     Returns
     -------
-     integ : float
+    integ : float
             The function f integrated over the sphere.
     """
 
     # NTheta = info.ntheta_act
     # NPhi  = info.nphi_act
 
     # NTheta, NPhi = func.shape
```

### Comparing `waveformtools-2023.5.19/waveformtools/simulations.py` & `waveformtools-2023.6.3/waveformtools/simulations.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,113 +13,84 @@
 
 
 class sim:
     """A data container for simulation data.
 
     Arrtibutes
     ----------
-
-    ROOTDIR:	string
-                            Root directory as a string containing the simulation folders.
-
-    WAVDIR:	string
-                            Root directory as a string containing the simulation directies containing the wavefom data.
-
-    data_dir:	string
-                            The path of the folder containing data relative to the simulation direcory.
-
-    strain_dir:	string
-                                    The path of the folder containing the waveform data relative to the strain directory.
-
-    aliases:	a list of strings
-                            The names/aliases for the simulations.
-
-    multipoles:	dict of lists
-                                    The multipole moments of the simulation as a dictionary.
-                                    Each entry is a list of width 4 with axis 0 the timeaxis of multipoles.
-
-    mass1:	dict of floats
-                    The BH1 horizon mass.
-
-    mass2:	dict of floats)
-                    The BH2 horizon mass.
-
-    mass3:	dict of floats
-                    The BH3 horizon mass.
-
-    delta_t:	dict of floats
-                            The time stepping in simulation units (delta_t/M).
-
-    timeaxis:	dict of 1d arrays
-                            The timeaxis of the simulations.
-
-    distance:	dict of 1d arrays
-                            The distances of simulations.
-
-    merger_ind:	dict of ints
-                                    The merger index/ common horizon formation index of simulations.
-
-    dinit:	dict of floats
-                    The initial distances.
-
-    multipoles:	dict of lists
-                                    The two sets of  mass multipoles of the three horizons. Axis 0 is usuall the time array.
-
-    mass_multipoles:	dict of lists
-                                            The mass multipoles upto (ell=8).
-
-    spin_multipoles:	dict of lists
-                                            The spin multipoles upto (l=8).
-
-    data_length:	dict of float
-                                    The data length of the multipole simulation data loaded.
-
-    dist_data_length:	dict of ints
-                                            The data length of distances of simulations.
-
-    merger_distance:	dict of floats
-                                            The distance between the blackholes at the merger index.
-
-    true_merger_dist:	dict of floats
-                                            The true merger distance (non-normalized).
-
-    sampling_f:	dict of floats
-                                    The sampling frequency of simulations (1/delta_t).
-
-    merger_time:	dict of floats
-                                    The cctk_time stamp at merger.
-
-    massratio:	dict of floats
-                            The massratio of the simulations.
-
-    chirpmass:	dict of floats
-                            The chirpmass of the simulations.
-
-    totalmass:	dict of floats
-                            The total mass of the simulations.
-
-    log_multipoles:	dict of lists
-                    The natural logarithm of the negative
-                    of the multipole moments as
-                    a list [time, multipole1, multipole2, multipole3(if exists)].
-
-    data_duration:	dict of floats
+    ROOTDIR : string
+              Root directory as a string containing the simulation folders.
+    WAVDIR : string
+             Root directory as a string containing the simulation directies containing the wavefom data.
+    data_dir : string
+               The path of the folder containing data relative to the simulation direcory.
+    strain_dir : string
+                 The path of the folder containing the waveform data relative to the strain directory.
+    aliaseas : a list of strings
+               The names/aliases for the simulations.
+    multipoles : dict of lists
+                 The multipole moments of the simulation as a dictionary.
+                 Each entry is a list of width 4 with axis 0 the timeaxis of multipoles.
+    mass1 : dict of floats
+            The BH1 horizon mass.
+    mass2 : dict of floats
+            The BH2 horizon mass.
+    mass3 : dict of floats
+            The BH3 horizon mass.
+    delta_t : dict of floats
+              The time stepping in simulation units (delta_t/M).
+    timeaxis : dict of 1d arrays
+               The timeaxis of the simulations.
+    distance : dict of 1d arrays
+               The distances of simulations.
+    merger_ind : dict of ints
+                 The merger index/ common horizon formation index of simulations.
+    dinit : dict of floats
+            The initial distances.
+    multipoles : dict of lists
+                 The two sets of  mass multipoles of the three horizons. Axis 0 is usuall the time array.
+    mass_multipoles : dict of lists
+                      The mass multipoles upto (ell=8).
+    spin_multipoles : dict of lists
+                      The spin multipoles upto (l=8).
+    data_length : dict of float
+                  The data length of the multipole simulation data loaded.
+    dist_data_length : dict of ints
+                       The data length of distances of simulations.
+    merger_distance : dict of floats
+                      The distance between the blackholes at the merger index.
+    true_merger_dist : dict of floats
+                       The true merger distance (non-normalized).
+    sampling_f : dict of floats
+                 The sampling frequency of simulations (1/delta_t).
+    merger_time : dict of floats
+                  The cctk_time stamp at merger.
+    massratio : dict of floats
+                The massratio of the simulations.
+    chirpmass : dict of floats
+                The chirpmass of the simulations.
+    totalmass : dict of floats
+                The total mass of the simulations.
+    log_multipoles : dict of lists
+                     The natural logarithm of the negative
+                     of the multipole moments as
+                     a list [time, multipole1, multipole2, multipole3(if exists)].
+    data_duration : dict of floats
                     The total cctk_time units of simulations present.
-    BH_locations:	dict of lists.
-                    A dictionary of values containing BH
-                    locations of every simulation. Each
-                    simulation has three lists, one for
-                    each black hole.
-
-    CoM_locations:	dict of lists
+    BH_locations : dict of lists.
+                   A dictionary of values containing BH
+                   locations of every simulation. Each
+                   simulation has three lists, one for
+                   each black hole.
+    CoM_locations : dict of lists
                     A dictionary of lists containing the
                     X, Y and Z locations of the CoM of the simulations.
-    NP_1d:	dict
-                    A dict of dicts of lists containig
-                    the 1d Newman Penrose data from simulations.
+    NP_1d : dict
+            A dict of dicts of lists containig
+            the 1d Newman Penrose data from simulations.
 
     Methods
     -------
     calc_ref_multipoles
             Calculate the reference multipoles
             as time average of first few timesclices
             of (2) multipole moment data.
@@ -273,109 +244,142 @@
         self.ref_multipoles = ref_multipoles
         self.indjn = indjn
         self.NP_1d = NP_1d
 
     @property
     def data_duration(self):
         """Compute and return the data duration of the simulations."""
-        return {alias: self.data_length[alias] * self.delta_t[alias] for alias in self.aliases}
+        return {
+            alias: self.data_length[alias] * self.delta_t[alias]
+            for alias in self.aliases
+        }
 
     @property
     def comm_data_duration(self):
         """Compute and return the duration of
         the common data (multipole and Bhdiag/distance)
         of the simulations."""
-        return {alias: self.comm_data_length[alias] * self.delta_t[alias] for alias in self.aliases}
+        return {
+            alias: self.comm_data_length[alias] * self.delta_t[alias]
+            for alias in self.aliases
+        }
 
     @property
     def pm_data_duration(self):
         """Compute and return the duration
         of post-merger data present in the simulations."""
-        return {alias: self.data_duration[alias] - self.merger_time[alias] for alias in self.aliases}
+        return {
+            alias: self.data_duration[alias] - self.merger_time[alias]
+            for alias in self.aliases
+        }
 
     @property
     def pm_data_length(self):
         """Compute and return the post merger
         data length avaialable for all simulations."""
-        return {alias: self.data_length[alias] - self.merger_ind[alias] for alias in self.aliases}
+        return {
+            alias: self.data_length[alias] - self.merger_ind[alias]
+            for alias in self.aliases
+        }
 
     @property
     def merger_distance(self):
         """Compute and return the distance
         at the merger index of the simulations."""
         merger_dist = {}
         for alias in self.aliases:
             try:
-                merger_dist.update({alias: self.distance[alias][self.merger_ind[alias]]})
+                merger_dist.update(
+                    {alias: self.distance[alias][self.merger_ind[alias]]}
+                )
             except IndexError:
                 if (self.merger_ind[alias] - len(self.distance[alias])) == 1:
-                    merger_dist.update({alias: self.distance[alias][self.merger_ind[alias] - 1]})
+                    merger_dist.update(
+                        {
+                            alias: self.distance[alias][
+                                self.merger_ind[alias] - 1
+                            ]
+                        }
+                    )
                 else:
-                    message("%s :Distance upto merger not defined. Setting final value" % alias)
+                    message(
+                        "%s :Distance upto merger not defined. Setting final value"
+                        % alias
+                    )
                     merger_dist.update({alias: self.distance[alias][-1]})
         return merger_dist
 
     @property
     def true_merger_distance(self):
         """Compute and return the true
         (i.e. non-normalized) distance at merger for the simulations."""
-        return {alias: self.dinit[alias] * self.merger_distance[alias] for alias in self.aliases}
+        return {
+            alias: self.dinit[alias] * self.merger_distance[alias]
+            for alias in self.aliases
+        }
 
     @property
     def sampling_f(self):
         """Compute and return the sampling frequency of the simulations."""
         return {alias: 1.0 / self.delta_t[alias] for alias in self.aliases}
 
     @property
     def merger_time(self):
         """Compute and return the
         cctk_time stamp at the merger
         for the simulations."""
-        return {alias: self.merger_ind[alias] * self.delta_t[alias] for alias in self.aliases}
+        return {
+            alias: self.merger_ind[alias] * self.delta_t[alias]
+            for alias in self.aliases
+        }
 
     @property
     def massratio(self):
         """Compute and return the massratio of the simulations."""
-        return {alias: self.mass2[alias] / self.mass1[alias] for alias in self.aliases}
+        return {
+            alias: self.mass2[alias] / self.mass1[alias]
+            for alias in self.aliases
+        }
 
     @property
     def chirpmass(self):
         """Compute and return the chirp mass of the simulations."""
         return {
             alias: ((self.mass1[alias] * self.mass2[alias]) ** (3.0 / 5))
             / (self.mass1[alias] + self.mass2[alias]) ** (1.0 / 5)
             for alias in self.aliases
         }
 
     @property
     def totalmass(self):
         """Compute and return the total mass of the simulations."""
-        return {alias: self.mass1[alias] + self.mass2[alias] for alias in self.aliases}
+        return {
+            alias: self.mass1[alias] + self.mass2[alias]
+            for alias in self.aliases
+        }
 
     def calc_junkend(self, tjn=200.0):
         """Compute the indices and the starting distances
         of the system at timestamp t = 200.
 
         Parameters
         ----------
-
-        tjn:	float
-                        The definition of time end of junk radiation. Default is 200.
+        tjn : float
+              The definition of time end of junk radiation. Default is 200.
 
         Notes
         -----
-        Computes:
+        Computes :
 
-        self.indjn:	dict
-                                        A dictionary containing the index location
+        self.indjn :    dict
+                        A dictionary containing the index location
                                         corresponding to timestamp tjn.
-        self.distjn:	dict
-                                        A dictionary containing the normalized co-ordinate
-                                        distance between the two BHs at tjn.
-
+        self.distjn :   dict
+                        A dictionary containing the normalized co-ordinate
+                        distance between the two BHs at tjn.
         """
 
         # Find the starting distance at t = 200M.
         # Initialize the directory.
         self.indjn = {}
         for alias in self.aliases:
             # Iterate over simulations.
@@ -427,16 +431,24 @@
                 self.comm_data_length[alias] = ml_length
                 self.distance[alias] = self.distance[alias][:ml_length]
             message(item.shape)
             log_mult.update(
                 {
                     alias: [
                         item[: self.comm_data_length[alias], 0],
-                        np.log(np.absolute(-item[: self.comm_data_length[alias], 1])),
-                        np.log(np.absolute(-item[: self.comm_data_length[alias], 2])),
+                        np.log(
+                            np.absolute(
+                                -item[: self.comm_data_length[alias], 1]
+                            )
+                        ),
+                        np.log(
+                            np.absolute(
+                                -item[: self.comm_data_length[alias], 2]
+                            )
+                        ),
                         np.log(np.absolute(-item[self.merger_ind[alias] :, 3])),
                     ]
                 }
             )
         self.log_multipoles = log_mult
 
     def calc_delta_multipoles(self):
@@ -467,15 +479,22 @@
             Ml22_ref = np.mean(Ml22[30:100])
             Ml32_ref = np.mean(Ml32[-100:])
             dMl12 = Ml12 - Ml12_ref
             dMl22 = Ml22 - Ml22_ref
             dMl32 = Ml32 - Ml32_ref
 
             log_deltmult.update(
-                {alias: [time, np.log(np.absolute(-dMl12)), np.log(np.absolute(-dMl22)), np.log(np.absolute(-dMl32))]}
+                {
+                    alias: [
+                        time,
+                        np.log(np.absolute(-dMl12)),
+                        np.log(np.absolute(-dMl22)),
+                        np.log(np.absolute(-dMl32)),
+                    ]
+                }
             )
 
         self.log_deltamultipoles = log_deltmult
 
     def calc_log_multipoles2(self):
         """Compute and assign the natural logarithm of the (l=2) multipoles to sim.log_multipoles of the simulations."""
         log_mult = {}
@@ -526,42 +545,44 @@
             Ml12_ref = np.mean(Ml12[30:100])
             Ml22_ref = np.mean(Ml22[30:100])
             Ml32_ref = np.mean(Ml32[-100:])
             dMl12 = Ml12 - Ml12_ref
             dMl22 = Ml22 - Ml22_ref
             dMl32 = Ml32 - Ml32_ref
 
-            log_deltmult.update({alias: [time, np.log(-dMl12), np.log(-dMl22), np.log(dMl32)]})
+            log_deltmult.update(
+                {alias: [time, np.log(-dMl12), np.log(-dMl22), np.log(dMl32)]}
+            )
 
         self.log_deltamultipoles2 = log_deltmult
 
     def load_data(self):
         """Load data of the simulations.
 
         Notes
         -----
+        Data is assigned to:
 
-        Data is assigned to
-
-                        multipoles:	list
-                        mass_multipoles:	list
-                        spin_multipoles:	list
-                        timeaxis:	list
-                        mass1:	float
-                        mass2:	float
-                        mass3:	float
-                        delta_t:	float
-                        distance:	list
-                        merger_ind:	int
-                        actmerger_time:	float
-                        dinit:	float
-                        data_length:	int
-                        dist_data_length:	int
+                        multipoles: list
+                        mass_multipoles:    list
+                        spin_multipoles:    list
+                        timeaxis:   list
+                        mass1:  float
+                        mass2:  float
+                        mass3:  float
+                        delta_t:    float
+                        distance:   list
+                        merger_ind: int
+                        actmerger_time: float
+                        dinit:  float
+                        data_length:    int
+                        dist_data_length:   int
 
         """
+
         """ Common variables """
         multipoles_one = []
         masses_one = []
         masses_one_all = []
         M1_one = []
         M2_one = []
         M3_one = []
@@ -599,15 +620,18 @@
             # Loop over simulations.
 
             message(self.aliases[sim_index])
             message("------------------")
 
             # Load the qlm_multipole moment data.
             file0 = np.genfromtxt(
-                self.ROOTDIR + sim1[sim_index] + self.data_dir + "quasilocalmeasures-qlm_multipole_moments..asc"
+                self.ROOTDIR
+                + sim1[sim_index]
+                + self.data_dir
+                + "quasilocalmeasures-qlm_multipole_moments..asc"
             )
 
             # Assign the timeaxis.
             cctk_time = file0[:, 8]
 
             # Assign the multipole data lengths to a list.
             ml_data_length.append(len(cctk_time))
@@ -619,17 +643,17 @@
             # Load the BH horizon masses.
             M1_one_all = file0[:, 12]
             M2_one_all = file0[:, 13]
             M3_one_all = file0[:, 14]
 
             ###################################################################
             # I.
-            # 	1. Load multipole data.
-            # 	2. Mass data.
-            # 	3. Find merger index.
+            #   1. Load multipole data.
+            #   2. Mass data.
+            #   3. Find merger index.
             ###################################################################
 
             # Lists to hold mass multipole data of the three horizons of a
             # simulation.
             amm1 = []
             amm2 = []
             amm3 = []
@@ -708,15 +732,17 @@
 
             try:
                 # Try to find the jump location of the horizon mass1 data.
                 merger_one = np.where(np.diff(M1_one_all) > 0.1)[0]
 
             except BaseException:
                 merger_one = len(M1_one_all)
-                message("Mass1 has no jumps. Merger has probably not happened. Reverting to data length.")
+                message(
+                    "Mass1 has no jumps. Merger has probably not happened. Reverting to data length."
+                )
 
             message("Merger index (through jump in mass1):", merger_one)
 
             if merger_one_a.any() and merger_one.any():
                 # If both indices have been found, select the least of the two
                 # as merger index.
                 merger_one = min(merger_one_a[0], merger_one[0])
@@ -733,15 +759,17 @@
                 message("No merger data exists")
                 merger_one = -1
 
             else:
                 # If both indices are not equal, declare inconsistency but
                 # accept the result from either.
 
-                message("Merger index inconsistency found. Mergertime may not be correct")
+                message(
+                    "Merger index inconsistency found. Mergertime may not be correct"
+                )
 
                 try:
                     # First try with non-zero mass3 index.
                     merger_one = merger_one[0]
                     message("Merger time set from Mass3")
                 except BaseException:
                     # Else assign from mass1 jump.
@@ -781,38 +809,54 @@
             # Gather the mass and spin multipoles together.
             all_mass_multipoles_one.append([amm1, amm2, amm3])
             all_spin_multipoles_one.append([asm1, asm2, asm3])
 
             # message(len(cctk_time))
 
             # Gather the l=2 mass multipoles.
-            multipoles_one.append(np.array([cctk_time, Ml12_one, Ml22_one, Ml32_one]))
+            multipoles_one.append(
+                np.array([cctk_time, Ml12_one, Ml22_one, Ml32_one])
+            )
 
             # Gather the masses.
             masses_one.append([M1_one, M2_one, M3_one])
             masses_one_all.append([M1_one_all, M2_one_all, M3_one_all])
 
             ###################################################################
             # II . Load the distance data.
             # Compute the distance using the coordinate positions in BHdiagnostics files.
             ###################################################################
-            temp0 = np.genfromtxt(self.ROOTDIR + sim1[sim_index] + self.data_dir + "BH_diagnostics.ah1.gp")
-            temp1 = np.genfromtxt(self.ROOTDIR + sim1[sim_index] + self.data_dir + "BH_diagnostics.ah2.gp")
+            temp0 = np.genfromtxt(
+                self.ROOTDIR
+                + sim1[sim_index]
+                + self.data_dir
+                + "BH_diagnostics.ah1.gp"
+            )
+            temp1 = np.genfromtxt(
+                self.ROOTDIR
+                + sim1[sim_index]
+                + self.data_dir
+                + "BH_diagnostics.ah2.gp"
+            )
 
             t_coord_0 = temp0[:, 1]
             x_coord_0_locs = temp0[:, 2]
             y_coord_0_locs = temp0[:, 3]
 
             message("Coord len", len(t_coord_0))
             t_coord_1 = temp1[:, 1]
             x_coord_1_locs = temp1[:, 2]
             y_coord_1_locs = temp1[:, 3]
 
-            temp0 = np.transpose(np.array([t_coord_0, x_coord_0_locs, y_coord_0_locs]))
-            temp1 = np.transpose(np.array([t_coord_1, x_coord_1_locs, y_coord_1_locs]))
+            temp0 = np.transpose(
+                np.array([t_coord_0, x_coord_0_locs, y_coord_0_locs])
+            )
+            temp1 = np.transpose(
+                np.array([t_coord_1, x_coord_1_locs, y_coord_1_locs])
+            )
 
             message("Dist shapes", temp0.shape, temp1.shape)
             # check for data continuity.
             # Load data.
             data0 = temp0
             data1 = temp1
 
@@ -831,23 +875,30 @@
 
             # message('Time step',delta_t)
 
             # Retrieve merger index.
             mergerind = ind_merger_one[sim_index]
 
             # Update the merger time list.
-            merger_time_one.append(ind_merger_one[sim_index] * delta_t_one[sim_index])
+            merger_time_one.append(
+                ind_merger_one[sim_index] * delta_t_one[sim_index]
+            )
 
             # Find the shorter data. BHdiag1,2 or multipole data.
             act_len = min(shape0[0], shape1[0], ml_data_length[sim_index])
 
             # If BHdiag 1 and 2 are equal in length and equal to multipole
             # length:
-            if shape0[0] == shape1[0] and shape0[0] == ml_data_length[sim_index]:
-                message("BH_data length is consistent with multipole data length")
+            if (
+                shape0[0] == shape1[0]
+                and shape0[0] == ml_data_length[sim_index]
+            ):
+                message(
+                    "BH_data length is consistent with multipole data length"
+                )
 
             # If the shortest data length is different from multipole length.
             if act_len == shape0[0] or act_len == shape1[0]:
                 message("BH_diagnostics data is shorter")
 
             # If multipole data is shorter.
             else:
@@ -861,65 +912,72 @@
             # act_shape_one.append()#
             # act_shape_one.append(min(shape1[0],shape2[0]))
             # message(temp0.shape,temp1.shape)
 
             # Try to load BHdiag3 file if present.
             try:
                 # Try to load the BH_diagnostics file for BH3.
-                temp2 = np.genfromtxt(self.ROOTDIR + sim1[sim_index] + self.data_dir + "BH_diagnostics.ah3.gp")[
-                    :, np.r_[1, 2, 3]
-                ]
+                temp2 = np.genfromtxt(
+                    self.ROOTDIR
+                    + sim1[sim_index]
+                    + self.data_dir
+                    + "BH_diagnostics.ah3.gp"
+                )[:, np.r_[1, 2, 3]]
 
                 # If merger index is not found from masses set using BH_diag3.
 
                 # If the merger_ind from masses is greater than the BHdiag3
                 # data length.
 
                 if mergerind * delta_t >= int(temp2[0, 0]):
                     merger_time_one[sim_index] = temp2[0, 0]
                     mergerind = int(temp2[0, 0] / delta_t)
                     ind_merger_one[sim_index] = mergerind
-                    message("Merger time acquired from BHdiag3", mergerind * delta_t)
-                    message("Merger index has been updated with info from BHdiag3")
+                    message(
+                        "Merger time acquired from BHdiag3", mergerind * delta_t
+                    )
+                    message(
+                        "Merger index has been updated with info from BHdiag3"
+                    )
             except BaseException:
                 message("Merger time acquired from masses", mergerind * delta_t)
 
             message("Merger index", mergerind)
 
             # FInd shape of data.
             shape0 = temp0.shape
             shape1 = temp1.shape
 
             # if shape0[0] < shape0[1]:
-            # 	 temp1 = np.transpose(temp1)
+            #    temp1 = np.transpose(temp1)
 
             # if shape1[0] < shape1[1]:
-            # 	 temp2 = np.transpose(temp2)
+            #    temp2 = np.transpose(temp2)
 
             # Assign the centroid locations to variables.
 
             # t_coord_0 = t_coord_0  # temp0[:, 0]
             x_coord_0 = x_coord_0_locs  # temp0[:, 1]
             y_coord_0 = y_coord_0_locs  # temp0[:, 2]
 
             # t_coord_1 = t_coord_1  # temp1[:, 0]
             x_coord_1 = x_coord_1_locs  # temp1[:, 1]
             y_coord_1 = y_coord_1_locs  # temp1[:, 2]
 
-            # t_coord_0		 =	 temp0[:, 0]
-            # x_coord_0		 =	 temp0[:, 1]
-            # y_coord_0		 =	 temp0[:, 2]
+            # t_coord_0      =   temp0[:, 0]
+            # x_coord_0      =   temp0[:, 1]
+            # y_coord_0      =   temp0[:, 2]
             #
-            # t_coord_1		 =	 temp1[:, 0]
-            # x1		 =	 temp1[:, 1]
-            # y1		 =	 temp1[:, 2]
+            # t_coord_1      =   temp1[:, 0]
+            # x1         =   temp1[:, 1]
+            # y1         =   temp1[:, 2]
 
             # if int((x_coord_0-x_coord_0_locs)[0])!=0:
-            # 	 message('ERRORRRRRRR!')
-            # 	 sys.exit(0)
+            #    message('ERRORRRRRRR!')
+            #    sys.exit(0)
             # Compute lengths
 
             len_0 = len(t_coord_0)
             len_1 = len(t_coord_1)
 
             # Find minimum
             lmin = min(len_0, len_1)
@@ -954,15 +1012,20 @@
             d0_one.append(d0_sim)
             d_sim = d_sim / d0_sim
             # d_one.append(np.sqrt((temp0[:act_shape_one[sim_index],1]-temp1[:act_shape_one[sim_index],1])**2
             # + (temp0[:act_shape_one[sim_index],2]-temp1[:act_shape_one[sim_index],2])**2))
             d_one.append([t_coord_0, d_sim])
             message(
                 "ml_timeaxis_length: %d, Multipole data length: %d, BHdiag length: %d, Distance length: %d"
-                % (len(timeaxis_one[sim_index]), ml_data_length[sim_index], shape1[0], len(d_one[sim_index]))
+                % (
+                    len(timeaxis_one[sim_index]),
+                    ml_data_length[sim_index],
+                    shape1[0],
+                    len(d_one[sim_index]),
+                )
             )
             dist_data_length.append(len(d_sim))
 
         # multipoles = np.array(multipoles)
         # Convert the acquired data lists into numpy arrays.
         masses_one = np.array(masses_one)
         M1_one = np.array(M1_one)
@@ -982,29 +1045,49 @@
         # d_one.shape
 
         # Plot the distance
         # message('multipoles length',len(multipoles_one))
 
         # Assign data to sim variables.
         for sim_index in range(0, len(self.aliases)):
-            self.multipoles.update({self.aliases[sim_index]: multipoles_one[sim_index]})
-            self.mass_multipoles.update({self.aliases[sim_index]: all_mass_multipoles_one[sim_index]})
-            self.spin_multipoles.update({self.aliases[sim_index]: all_spin_multipoles_one[sim_index]})
-            self.timeaxis.update({self.aliases[sim_index]: timeaxis_one[sim_index]})
+            self.multipoles.update(
+                {self.aliases[sim_index]: multipoles_one[sim_index]}
+            )
+            self.mass_multipoles.update(
+                {self.aliases[sim_index]: all_mass_multipoles_one[sim_index]}
+            )
+            self.spin_multipoles.update(
+                {self.aliases[sim_index]: all_spin_multipoles_one[sim_index]}
+            )
+            self.timeaxis.update(
+                {self.aliases[sim_index]: timeaxis_one[sim_index]}
+            )
             self.mass1.update({self.aliases[sim_index]: M1_one[sim_index]})
             self.mass2.update({self.aliases[sim_index]: M2_one[sim_index]})
             self.mass3.update({self.aliases[sim_index]: M3_one[sim_index]})
-            self.delta_t.update({self.aliases[sim_index]: delta_t_one[sim_index]})
+            self.delta_t.update(
+                {self.aliases[sim_index]: delta_t_one[sim_index]}
+            )
             self.distance.update({self.aliases[sim_index]: d_one[sim_index]})
-            self.merger_ind.update({self.aliases[sim_index]: ind_merger_one[sim_index]})
-            self.actmerger_time.update({self.aliases[sim_index]: merger_time_one[sim_index]})
+            self.merger_ind.update(
+                {self.aliases[sim_index]: ind_merger_one[sim_index]}
+            )
+            self.actmerger_time.update(
+                {self.aliases[sim_index]: merger_time_one[sim_index]}
+            )
             self.dinit.update({self.aliases[sim_index]: d0_one[sim_index]})
-            self.data_length.update({self.aliases[sim_index]: ml_data_length[sim_index]})
-            self.comm_data_length.update({self.aliases[sim_index]: act_shape_one[sim_index]})
-            self.dist_data_length.update({self.aliases[sim_index]: dist_data_length[sim_index]})
+            self.data_length.update(
+                {self.aliases[sim_index]: ml_data_length[sim_index]}
+            )
+            self.comm_data_length.update(
+                {self.aliases[sim_index]: act_shape_one[sim_index]}
+            )
+            self.dist_data_length.update(
+                {self.aliases[sim_index]: dist_data_length[sim_index]}
+            )
         # message(self.multipoles)
 
         # Resize the multipoles data if merger index was updated from BHdiag3.
         self._resize_multipoles()
         # Reverse the BH1 and BH2 data if BH mass2>mass1.
         self._ifreversal()
 
@@ -1029,15 +1112,18 @@
     def _resize_multipoles(self):
         """Private method to resize the (l=2) multipole data. Useful when merger index was updated from BHdiag3."""
         for alias in self.aliases:
             # Loop over simulations.
             # message(alias)
             # self.timeaxis[alias] = [item[:self.dist_data_length[alias]] for item in self.timeaxis[alias]]
             # Resize the lengths of the data.
-            self.multipoles[alias] = [item[: self.dist_data_length[alias]] for item in self.multipoles[alias]]
+            self.multipoles[alias] = [
+                item[: self.dist_data_length[alias]]
+                for item in self.multipoles[alias]
+            ]
             # self.data_length.update({alias : len(self.multipoles[alias][0])})
             # self.mass_multipoles[alias] = [item[:self.dist_data_length[alias] for item in self.mass_multipoles[alias]]]
             # self.spin_multipoles[alias] = [item[:self.dist_data_length[alias]
             # for item in self.spin_multipoles[alias]]]
 
     def _ifreversal(self):
         """Private method to reverse the (l=2) multipole data if mass2>mass1.
@@ -1056,51 +1142,77 @@
             # Loop over simulations.
             message("Check for puncture reversal, %s" % alias)
             if alias != "q1a0_a" and alias != "q1a0_b":
                 # Condition for reversal decision.
                 if self.mass1[alias] < self.mass2[alias]:
                     # Toggle the flag.
                     flag = 1
-                    message("**************************************************")
+                    message(
+                        "**************************************************"
+                    )
                     message("BH 1 and 2 reversal found!!! \n Reversing data...")
-                    message("**************************************************")
-                    message("original mass1:%f, mass2: %f" % (self.mass1[alias], self.mass2[alias]))
+                    message(
+                        "**************************************************"
+                    )
+                    message(
+                        "original mass1:%f, mass2: %f"
+                        % (self.mass1[alias], self.mass2[alias])
+                    )
                     # Reverse the data.
-                    self.mass1[alias], self.mass2[alias] = self.mass2[alias], self.mass1[alias]
+                    self.mass1[alias], self.mass2[alias] = (
+                        self.mass2[alias],
+                        self.mass1[alias],
+                    )
                     # Unpack the multipoles data.
-                    time, multipole1, multipole2, multipole3 = self.multipoles[alias]
+                    time, multipole1, multipole2, multipole3 = self.multipoles[
+                        alias
+                    ]
                     # Reverse the multipole data.
                     multipole1, multipole2 = multipole2, multipole1
                     # Repack the data.
-                    self.multipoles[alias] = np.array([time, multipole1, multipole2, multipole3])
+                    self.multipoles[alias] = np.array(
+                        [time, multipole1, multipole2, multipole3]
+                    )
             if not flag:
                 message("Data O.K.")
             return 1.0
 
     def load_strain(self, start_index=0):
         """Method to load the shear data of simulations."""
 
         for sim_index in range(0, len(self.aliases)):
             # Loop over simulations.
             alias = self.aliases[sim_index]
             # Set the starting index for data.
             start_index = 0  # start_index = 0#int(190/deltat[j])
             # Load the strain data.
             sim_strain_data = np.genfromtxt(
-                self.WAVDIR + self.aliases[sim_index] + "/" + self.strain_dir + "/strain_" + str(alias) + "_wavextcpm.dat"
+                self.WAVDIR
+                + self.aliases[sim_index]
+                + "/"
+                + self.strain_dir
+                + "/strain_"
+                + str(alias)
+                + "_wavextcpm.dat"
             )
 
             # Load the timeaxis, plus and cross polarized data.
             htdat = sim_strain_data[start_index:, 0]
             hpdat = sim_strain_data[start_index:, 1]
             hxdat = sim_strain_data[start_index:, 2]
 
             message("The strain file is")
             message(
-                self.WAVDIR + self.aliases[sim_index] + "/" + self.strain_dir + "/strain_" + str(alias) + "_wavextcpm.dat"
+                self.WAVDIR
+                + self.aliases[sim_index]
+                + "/"
+                + self.strain_dir
+                + "/strain_"
+                + str(alias)
+                + "_wavextcpm.dat"
             )
 
             # Align the peak of the strain with the formation of the common
             # horizon (merger index).
 
             Lpeak_loc = np.argmax(np.diff(hpdat) ** 2 + np.diff(hxdat) ** 2)
 
@@ -1147,55 +1259,82 @@
 
             # Load the plus and cross polarized strain data.
             hpdat = self.strain[alias][1]
             hxdat = self.strain[alias][2]
             # Load the time stepping.
             delta_t = self.delta_t[alias]
             # Extract and update the amplitude and phases.
-            self.strain_phase.update({alias: (xtract_cphase(hpdat, hxdat, delta_t=delta_t, to_plot="yes"))})
+            self.strain_phase.update(
+                {
+                    alias: (
+                        xtract_cphase(
+                            hpdat, hxdat, delta_t=delta_t, to_plot="yes"
+                        )
+                    )
+                }
+            )
             self.strain_amplitude.update({alias: xtract_camp(hpdat, hxdat)})
-            self.strain_frequency.update({alias: np.diff(self.strain_phase[alias]) / delta_t})
+            self.strain_frequency.update(
+                {alias: np.diff(self.strain_phase[alias]) / delta_t}
+            )
         return 1
 
     def ret_horizon_radii(self):
         """Retrieve the radius of the common horizon at the time of formation."""
 
         # Dictionary to hold the areal radii of the horizons.
         self.areal_radii = {}
         for alias in self.aliases:
             # Loop over simulations.
 
             # Load the BHdiagnostics file to load the radius.
-            ar_rad0 = np.genfromtxt(self.ROOTDIR + alias + "/" + self.data_dir + "BH_diagnostics.ah1.gp")[:, 27]
-            ar_rad1 = np.genfromtxt(self.ROOTDIR + alias + "/" + self.data_dir + "BH_diagnostics.ah2.gp")[:, 27]
+            ar_rad0 = np.genfromtxt(
+                self.ROOTDIR
+                + alias
+                + "/"
+                + self.data_dir
+                + "BH_diagnostics.ah1.gp"
+            )[:, 27]
+            ar_rad1 = np.genfromtxt(
+                self.ROOTDIR
+                + alias
+                + "/"
+                + self.data_dir
+                + "BH_diagnostics.ah2.gp"
+            )[:, 27]
             ar_rad2 = 1.75
             try:
-                ar_rad2 = np.genfromtxt(self.ROOTDIR + alias + "/" + self.data_dir + "BH_diagnostics.ah3.gp")[:, 27]
+                ar_rad2 = np.genfromtxt(
+                    self.ROOTDIR
+                    + alias
+                    + "/"
+                    + self.data_dir
+                    + "BH_diagnostics.ah3.gp"
+                )[:, 27]
             except BaseException:
                 message("No BHdiagnostics 3 file found for %s" % alias)
 
             # Load the data for this simulation in to a dictionary.
             self.areal_radii.update({alias: [ar_rad0, ar_rad1, ar_rad2]})
 
         return 1
 
     def get_BH_locations(self, alias=None):
         """Get the co-ordinate locations of the BHs.
 
         Parameters
         ----------
 
-        alias  :    str, optional.
-                                The simulation label. If not specified, then
-                                all available simulationswill be processed.
+        alias : str, optional.
+                The simulation label. If not specified, then
+                all available simulationswill be processed.
 
-        Returns
+        Assigns
         -------
-
-
+        `BH_locations`
         """
 
         # A dictionary to store BH location data
         self.BH_locations = {}
 
         if not alias:
             list_of_aliases = self.aliases
@@ -1210,18 +1349,24 @@
 
             # Masses of the horizons
             m1 = self.mass1[alias]
             m2 = self.mass2[alias]
             # M = m1 + m2
 
             flag = 1
-            bh1 = np.genfromtxt(self._get_file_path_from_str(string="*.ah1.gp", alias=alias))
-            bh2 = np.genfromtxt(self._get_file_path_from_str(string="*.ah2.gp", alias=alias))
+            bh1 = np.genfromtxt(
+                self._get_file_path_from_str(string="*.ah1.gp", alias=alias)
+            )
+            bh2 = np.genfromtxt(
+                self._get_file_path_from_str(string="*.ah2.gp", alias=alias)
+            )
             try:
-                bh3 = np.genfromtxt(self._get_file_path_from_str(string="*.ah3.gp", alias=alias))
+                bh3 = np.genfromtxt(
+                    self._get_file_path_from_str(string="*.ah3.gp", alias=alias)
+                )
             except Exception as excep:
                 message("BH3 file not found!", excep)
                 flag = -1
 
             # Read co-ordinates.
 
             bhd1_time = bh1[:, 1]
@@ -1252,29 +1397,26 @@
             self.BH_locations.update({alias: [bh1_loc, bh2_loc, bh3_loc]})
 
     def get_CoM_locations(self, alias=None):
         """Get the CoM location of the given simulation.
 
         Parameters
         ----------
-
-        alias  :    str, optional.
-                                The simulation label. If not specified, then
-                                all available simulationswill be processed.
+        alias : str, optional.
+                The simulation label. If not specified, then
+                all available simulationswill be processed.
 
         Returns
         -------
-
-        self.CoM_locations :    dict
-                                                        A dictionary of lists containing
-                                                        CoM locations of the simulations.
+        self.CoM_locations : dict
+                             A dictionary of lists containing
+                             CoM locations of the simulations.
 
         Notes
         -----
-
         This fetches the location of the BHs from data files.
         """
 
         # Storage for CoM locations
         self.CoM_locations = {}
 
         # Aliases to run over.
@@ -1305,46 +1447,54 @@
             total_mass = mass1 + mass2
 
             # End time
             max_len = min(self.merger_ind[alias], len(bh1_time), len(bh2_time))
 
             # CoM location
             T_com = bh1_time[:max_len]
-            X_com = (mass1 * bh1_x[:max_len] + mass2 * bh2_x[:max_len]) / (total_mass)
-            Y_com = (mass1 * bh1_y[:max_len] + mass2 * bh2_y[:max_len]) / (total_mass)
-            Z_com = (mass1 * bh1_z[:max_len] + mass2 * bh2_z[:max_len]) / (total_mass)
+            X_com = (mass1 * bh1_x[:max_len] + mass2 * bh2_x[:max_len]) / (
+                total_mass
+            )
+            Y_com = (mass1 * bh1_y[:max_len] + mass2 * bh2_y[:max_len]) / (
+                total_mass
+            )
+            Z_com = (mass1 * bh1_z[:max_len] + mass2 * bh2_z[:max_len]) / (
+                total_mass
+            )
 
             self.CoM_locations.update({alias: [T_com, X_com, Y_com, Z_com]})
 
     def get_CoM_mean_motion(self, alias=None):
         """Get the mean motion of the CoM.
 
         Parameters
         ----------
-
-        alias  :    str, optional.
-                                The simulation label. If not specified, then
-                                all available simulationswill be processed.
+        alias : str, optional.
+                The simulation label. If not specified, then
+                all available simulationswill be processed.
 
         Returns
         -------
-
-        alpha :     dict
-                                A dictionary containing the
-                                mean CoM displacement array.
-
-        beta :     dict
-                           A dictionary containing the
-                           mean CoM velocity array.
+        alpha : dict
+                A dictionary containing the
+                mean CoM displacement array.
+
+        beta : dict
+               A dictionary containing the
+               mean CoM velocity array.
 
         """
         CoM_motion_params = {}
         # Aliases to run over.
 
-        from waveformtools.CoM import X_com_moments, compute_com_alpha, compute_com_beta
+        from waveformtools.CoM import (
+            X_com_moments,
+            compute_com_alpha,
+            compute_com_beta,
+        )
 
         if not alias:
             list_of_aliases = self.aliases
 
         else:
             list_of_aliases = [alias]
 
@@ -1357,16 +1507,20 @@
                 taxis, X_com, Y_com, Z_com = self.CoM_locations[alias]
 
             all_coords = [X_com, Y_com, Z_com]
 
             zeroth_moments = X_com_moments(taxis, all_coords, 0)
             first_moments = X_com_moments(taxis, all_coords, 1)
 
-            Xcom_0 = np.array([zeroth_moments[label][0] for label in zeroth_moments.keys()])
-            Xcom_1 = np.array([first_moments[label][0] for label in zeroth_moments.keys()])
+            Xcom_0 = np.array(
+                [zeroth_moments[label][0] for label in zeroth_moments.keys()]
+            )
+            Xcom_1 = np.array(
+                [first_moments[label][0] for label in zeroth_moments.keys()]
+            )
 
             ti = taxis[0]
             tf = taxis[-1]
 
             alpha = compute_com_alpha(ti, tf, Xcom_0, Xcom_1)
             beta = compute_com_beta(ti, tf, Xcom_0, Xcom_1)
 
@@ -1375,31 +1529,28 @@
 
     def _get_file_path_from_str(self, alias, string=None):
         """Get the path of a file that contains
         the given string in its name.
 
         Parameters
         ----------
+        alias : str, optional.
+                The simulation label. If not specified, then
+                all available simulationswill be processed.
 
-        alias  :    str, optional.
-                                The simulation label. If not specified, then
-                                all available simulationswill be processed.
-
-        string :    str
-                                The string of a part of a file name.
+        string : str
+                 The string of a part of a file name.
 
         Returns
         -------
-
         file_path : str
-                                The full path of the file
+                    The full path of the file
 
         Notes
         -----
-
         The first occuring instance of the file is returned
         if there are multiple files found.
         """
 
         from pathlib import Path
 
         # The directory to look into.
@@ -1425,31 +1576,46 @@
         if self.NP_1d is None:
             self.NP_1d = {}
 
         np_data_alias_dict = {}
 
         for alias in self.aliases:
             if source == "qlm":
-                file_string = f"{self.data_dir}quasilocalmeasures-qlm_newman_penrose..asc"
+                file_string = (
+                    f"{self.data_dir}quasilocalmeasures-qlm_newman_penrose..asc"
+                )
             elif source == "ih":
-                file_string = f"{self.data_dir}isolatedhorizon-ih_newman_penrose..asc"
+                file_string = (
+                    f"{self.data_dir}isolatedhorizon-ih_newman_penrose..asc"
+                )
 
-            full_file_path = self._get_file_path_from_str(alias, string=file_string)
+            full_file_path = self._get_file_path_from_str(
+                alias, string=file_string
+            )
 
             with open(full_file_path, "r") as file:
                 for line_index in range(15):
                     fline = next(file)
                     # message(fline)
                     str_match = re.search(f"\d\d:qlm_np{np_qty}", fline)
                     # message(str_match)
                     if str_match is not None:
                         start_col = int(str_match[0][:2])
                         # message(start_col)
                         break
 
             NP_all_data = np.genfromtxt(full_file_path)[
-                :, np.r_[8, start_col - 1, start_col, start_col + 1, start_col + 2, start_col + 3, start_col + 4]
+                :,
+                np.r_[
+                    8,
+                    start_col - 1,
+                    start_col,
+                    start_col + 1,
+                    start_col + 2,
+                    start_col + 3,
+                    start_col + 4,
+                ],
             ]
 
             np_data_alias_dict.update({alias: NP_all_data})
 
         self.NP_1d.update({np_qty: np_data_alias_dict})
```

### Comparing `waveformtools-2023.5.19/waveformtools/spherical.py` & `waveformtools-2023.6.3/waveformtools/spherical.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,58 +3,52 @@
 ##################################
 # Imports
 #################################
 
 import numpy as np
 
 
-def decompose_in_SWSHs(waveform, gridinfo, spin_weight=-2, ell_max=8, emm_list="all"):
+def decompose_in_SWSHs(
+    waveform, gridinfo, spin_weight=-2, ell_max=8, emm_list="all"
+):
     """Decompose a given function on a sphere in Spin Weighted Spherical Harmonics
 
     Parameters
     ----------
-
-    waveform:		list
-                    A list that contains as its items the waveform
-                    defined on the sphere as an array of shape
-                    [ntheta, nphi]. Each item in the list may denote
-                    an instant of time or frequency.
-
-    spin_weight:	 int, optional
-                    The spin weight of the waveform.
-                    It defaults to -2 for a gravitational waveform.
-
-    ell_max:	int, optional
-                The maximum value of the :math:`\\ell'
-                polar quantum number. Defaults to 6=8.
-
-    gridinfo:		class instance
-                    The class instance that contains
-                    the properties of the spherical grid.
-
+    waveform : list
+               A list that contains as its items the waveform
+               defined on the sphere as an array of shape
+               [ntheta, nphi]. Each item in the list may denote
+               an instant of time or frequency.
+    spin_weight : int, optional
+                  The spin weight of the waveform.
+                  It defaults to -2 for a gravitational waveform.
+    ell_max : int, optional
+              The maximum value of the :math:`\\ell'
+              polar quantum number. Defaults to 6=8.
+    gridinfo : class instance
+               The class instance that contains
+               the properties of the spherical grid.
 
     Returns
     -------
-
-    SWSH_coeffs:	list
-                    The SWSH coefficients of the waveform.
-                    It may be a list composed of a single
-                    floating point number or a 1d array
-                    (denoting time or frequency dimension).
-                    The waveform can have angular as well
-                    as time dimentions. The nesting order
-                    will be that, given the list
-                    `non_boosted_waveform', each
-                    item refers to a one dimensional array in
-                    time/ frequency of SWSH coefficients.
-
+    SWSH_coeffs : list
+                  The SWSH coefficients of the waveform.
+                  It may be a list composed of a single
+                  floating point number or a 1d array
+                  (denoting time or frequency dimension).
+                  The waveform can have angular as well
+                  as time dimentions. The nesting order
+                  will be that, given the list
+                  `non_boosted_waveform', each
+                  item refers to a one dimensional array in
+                  time/ frequency of SWSH coefficients.
 
     Notes
     -----
-
     Assumes that the sphere on which this decomposition is carried out is so far out
     that the coordinate system is spherical polar and the poper area is the
     same as its co-ordinate area.
 
     """
 
     # Find out if the unboosted waveform is a single number or defined on a spherical grid.
@@ -111,61 +105,58 @@
             for emm_index in range(len(emm_list)):
                 # Decompose into seperate m modes.
 
                 # m value.
                 emm_val = int(emm_list[emm_index])
 
                 # Spin weighted spherical harmonic function at (theta, phi)
-                Ybasis_fun = Yslm_vec(spin_weight, ell_index, emm_val, theta, phi)
+                Ybasis_fun = Yslm_vec(
+                    spin_weight, ell_index, emm_val, theta, phi
+                )
 
                 # Integrate to obtain the multipole of order l.
 
                 # Integration for real and imaginary parts of the data separately.
                 # Integrate the function
 
                 # Using quad
-                multipole_emm = quad_on_sphere(integrand_ij * Ybasis_fun * darea, gridinfo)
-                # multipole_emm	 =	 np.sum(integrand_ij * Ybasis_fun * darea)
+                multipole_emm = quad_on_sphere(
+                    integrand_ij * Ybasis_fun * darea, gridinfo
+                )
+                # multipole_emm  =   np.sum(integrand_ij * Ybasis_fun * darea)
 
                 multipoles_ell.update({emm_val: multipole_emm})
             multipoles_all.update({ell_index: multipoles_ell})
 
         # Return the computed multipole.
         return multipoles_all
 
 
 def quad_on_sphere(integrand, gridinfo, kind="third"):
     """Integrate on a sphere using the scipy.quad method
 
     Parameters
     ----------
+    integrand : 2d array
+                The two dimensional integrand array defined on the sphere.
+    info : class instance
+           The class instance that contains the properties of the spherical grid.
+    kind : str
+           The interpolation order to use in integration.
 
-    integrand:		2d array
-                                    The two dimensional integrand array defined on the sphere.
-
-    info:		class instance
-                            The class instance that contains the properties of the spherical grid.
-
-    kind:		str
-                            The interpolation order to use in integration.
     Returns
     -------
-
     final_integral : float
-                              The given integrand integrated over the sphere.
-
-    final_errs:	float
-                                    The accumulated errors.
+                     The given integrand integrated over the sphere.
+    final_errs : float
+                 The accumulated errors.
 
     Notes
     -----
-
     Assumes that the sphere is a unit round sphere.
-
-
     """
 
     # Step 0: Get the grid properties
 
     # Compute the meshgrid for theta and phi.
     theta_1d = gridinfo.theta_1d
     # theta
@@ -183,27 +174,31 @@
         # Interpolate the integrand.
 
         integrand_phi = integrand[:, phi_index]
 
         integrand_phi_interp_func = interp1d(theta_1d, integrand_phi, kind=kind)
 
         # Integrate on the phi plane
-        integral_phi_vals, integral_phi_errs = quad(integrand_phi_interp_func, 0, np.pi)
+        integral_phi_vals, integral_phi_errs = quad(
+            integrand_phi_interp_func, 0, np.pi
+        )
 
         theta_first_integral_vals.append(integral_phi_vals)
         theta_first_integral_errs.append(integral_phi_errs)
 
     # Step 2: integrate along the phi direction
 
     # Interpolate the integrand.
 
     integrand_theta = theta_first_integral_vals
 
     integrand_theta_interp_func = interp1d(phi_1d, integrand_theta, kind=kind)
 
     # Integrate on the theta plane
-    final_integral, semi_final_errs = quad(integrand_theta_interp_func, 0, 2 * np.pi)
+    final_integral, semi_final_errs = quad(
+        integrand_theta_interp_func, 0, 2 * np.pi
+    )
 
     # Get final errors
     final_errs = semi_final_errs + np.sum(np.array(theta_first_integral_errs))
 
     return final_integral, final_errs
```

### Comparing `waveformtools-2023.5.19/waveformtools/transforms.py` & `waveformtools-2023.6.3/waveformtools/transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,121 +9,110 @@
 
 # @njit(parallel=True)
 def compute_fft(udata_x, delta_x):
     """Find the FFT of the samples in time-space, and return with the frequencies.
 
     Parameters
     ----------
-
-    udata_x:	1d array
-                                                    The samples in time-space.
-
-    delta_x:	float
-                                                    The stepping delta_x
+    udata_x : 1d array
+              The samples in time-space.
+    delta_x : float
+              The stepping delta_x
 
     Returns
     -------
-
-    freqs:	1d array
-                                    The frequency axis, shifted approriately.
-    utilde:	1d array
-                                                    The samples in frequency space, with conventions applied.
-
+    freqs : 1d array
+            The frequency axis, shifted approriately.
+    utilde : 1d array
+             The samples in frequency space, with conventions applied.
     """
 
     # import necessary libraries.
     from numpy.fft import fft
 
     # FFT
     utilde_orig = fft(udata_x)
 
     # Apply conventions.
     utilde = set_fft_conven(utilde_orig)
 
     # Get frequency axes.
     Nlen = len(utilde)
     # message(Nlen)
-    # Naxis			= np.arange(Nlen)
-    # freq_orig		= fftfreq(Nlen)
-    # freq_axis		= fftshift(freq_orig)*Nlen
-    # delta_x		 = xdata[1] - xdata[0]
+    # Naxis         = np.arange(Nlen)
+    # freq_orig     = fftfreq(Nlen)
+    # freq_axis     = fftshift(freq_orig)*Nlen
+    # delta_x        = xdata[1] - xdata[0]
 
-    # Naxis			 = np.arange(Nlen)
+    # Naxis          = np.arange(Nlen)
     freq_axis = np.linspace(-0.5 / delta_x, 0.5 / delta_x, Nlen)
 
     return freq_axis, utilde
 
 
 # @njit(parallel=True)
 def compute_ifft(utilde, delta_f):
     """Find the inverse FFT of the samples in frequency-space, and return with the time axis.
 
     Parameters
     ----------
-
-    utilde	:	1d array
-                                                    The samples in frequency-space.
-
-    delta_f:	float
-                                                    The frequency stepping
+    utilde : 1d array
+             The samples in frequency-space.
+    delta_f : float
+              The frequency stepping
 
     Returns
     -------
-
-    time_axis:	1d array
-                                                    The time axis.
-
-    udata_time:	1d array
-                                                                    The samples in time domain.
-
+    time_axis : 1d array
+                The time axis.
+    udata_time : 1d array
+                 The samples in time domain.
     """
 
     # import necessary libraries.
     from numpy.fft import ifft
 
     # FFT
     utilde_orig = unset_fft_conven(utilde)
 
     # Inverse transform
     udata_time = ifft(utilde_orig)
 
     # Get frequency axes.
     Nlen = len(udata_time)
     # message(Nlen)
-    # Naxis			= np.arange(Nlen)
-    # freq_orig		= fftfreq(Nlen)
-    # freq_axis		= fftshift(freq_orig)*Nlen
-    # delta_x		 = xdata[1] - xdata[0]
+    # Naxis         = np.arange(Nlen)
+    # freq_orig     = fftfreq(Nlen)
+    # freq_axis     = fftshift(freq_orig)*Nlen
+    # delta_x        = xdata[1] - xdata[0]
 
-    # Naxis			 = np.arange(Nlen)
+    # Naxis          = np.arange(Nlen)
     delta_t = 1.0 / (delta_f * Nlen)
-    # Dt				= Nlen * delta_f/2
+    # Dt                = Nlen * delta_f/2
 
     time_axis = np.linspace(0, delta_t * Nlen, Nlen)
 
     return time_axis, udata_time
 
 
 # @njit(parallel=True)
 def set_fft_conven(utilde_orig):
     """Make a numppy fft consistent with the chosen conventions.
                     This takes care of the zero mode factor and array position.
                     Also, it shifts the negative frequencies using numpy's fftshift.
 
     Parameters
     ----------
-
-    utilde_orig:	1d array
-                                                                    The result of a numpy fft.
+    utilde_orig : 1d array
+                  The result of a numpy fft.
 
     Returns
     -------
-
-    utilde_conven:	1d array
-                                                                    The fft with set conventions.
+    utilde_conven : 1d array
+                    The fft with set conventions.
     """
 
     # Multiply by 2, take conjugate.
     utilde_conven = 2 * np.conj(utilde_orig) / len(utilde_orig)
     # Restore the zero mode.
     utilde_conven[0] = utilde_conven[0] / 2
     # Shift the frequency axis.
@@ -131,27 +120,26 @@
 
     return utilde_conven
 
 
 # @njit(parallel=True)
 def unset_fft_conven(utilde_conven):
     """Make an actual conventional fft consistent with numpy's conventions.
-                    The inverse of set_conv.
+    The inverse of set_conv.
 
 
     Parameters
     ----------
-
-    utilde_conven:	1d array
-                                                                    The conventional fft data vector.
+    utilde_conven : 1d array
+                    The conventional fft data vector.
 
     Returns
     -------
-
-    utilde_np
+    utilde_np : 1darray
+                The fft in numpy convention
     """
 
     utilde_np = np.fft.ifftshift(utilde_conven)
 
     utilde_np = len(utilde_np) * np.conj(utilde_np) / 2
     # message(utilde_original[0])
     utilde_np[0] *= 2
@@ -161,35 +149,33 @@
 
 
 def Yslm(spin_weight, ell, emm, theta, phi):
     """Spin-weighted spherical harmonics fast evaluation.
 
     Parameters
     ----------
-
-    spin_weight :	int
-                                    The Spin weight.
-    ell :	int
-                    The mode number :math:`\\ell'.
-    emm :	int
-                    The azimuthal mode number :math:`m'.
+    spin_weight : int
+                  The Spin weight.
+    ell : int
+          The mode number :math:`\\ell'.
+    emm : int
+          The azimuthal mode number :math:`m'.
     theta : float
-                    The polar angle  :math:`\\theta` in radians,
-    phi :	float
-                    The aximuthal angle :math:`\\phi' in radians.
+            The polar angle  :math:`\\theta` in radians,
+    phi : float
+          The aximuthal angle :math:`\\phi' in radians.
 
     Returns
     --------
-    Yslm :	float
-                    The value of Yslm at :math:`\\theta, phi'.
-
-            Note
-            ----
-            This is accurate upto 14 decimals for L upto 25.
+    Yslm : float
+           The value of Yslm at :math:`\\theta, phi'.
 
+    Notes
+    -----
+    This is accurate upto 14 decimals for L upto 25.
     """
     import sympy as sp
 
     # theta, phi = sp.symbols('theta phi')
 
     fact = np.math.factorial
     # fact = sp.factorial
@@ -200,180 +186,197 @@
         factor = (-1) ** ell
         theta = np.pi - theta
         phi += np.pi
 
     abs_spin_weight = abs(spin_weight)
 
     for aar in range(ell - abs_spin_weight + 1):
-        if (aar + abs_spin_weight - emm) < 0 or (ell - aar - abs_spin_weight) < 0:
+        if (aar + abs_spin_weight - emm) < 0 or (
+            ell - aar - abs_spin_weight
+        ) < 0:
             message(f"Skippin r {aar}", message_verbosity=3)
             continue
         else:
             Sum += (
                 sp.binomial(ell - abs_spin_weight, aar)
-                * sp.binomial(ell + abs_spin_weight, aar + abs_spin_weight - emm)
+                * sp.binomial(
+                    ell + abs_spin_weight, aar + abs_spin_weight - emm
+                )
                 * np.power((-1), (ell - aar - abs_spin_weight))
                 * np.exp(1j * emm * phi)
                 / np.power(np.tan(theta / 2), (2 * aar + abs_spin_weight - emm))
             )
 
     Sum = complex(Sum)
     Yslm = (-1) ** emm * (
         np.sqrt(
             fact(ell + emm)
             * fact(ell - emm)
             * (2 * ell + 1)
-            / (4 * np.pi * fact(ell + abs_spin_weight) * fact(ell - abs_spin_weight))
+            / (
+                4
+                * np.pi
+                * fact(ell + abs_spin_weight)
+                * fact(ell - abs_spin_weight)
+            )
         )
         * np.sin(theta / 2) ** (2 * ell)
         * Sum
     )
 
     return factor * Yslm
 
 
 def Yslm_vec(spin_weight, ell, emm, theta_grid, phi_grid):
     """Spin-weighted spherical harmonics fast evaluations on numpy arrays for vectorized evaluations.
 
-    Inputs
-    -----------
-
-    spin_weight :	int
-                                    The Spin weight.
-    ell :	int
-                    The mode number :math:`\\ell'.
-    emm :	int
-                    The azimuthal mode number :math:`m'.
+    Parameters
+    ----------
+    spin_weight : int
+                  The Spin weight.
+    ell : int
+          The mode number :math:`\\ell'.
+    emm : int
+          The azimuthal mode number :math:`m'.
     theta : float
-                    The polar angle  :math:`\\theta` in radians,
-    phi :	float
-                    The aximuthal angle :math:`\\phi' in radians.
+            The polar angle  :math:`\\theta` in radians,
+    phi : float
+          The aximuthal angle :math:`\\phi' in radians.
 
     Returns
-    --------
-    Yslm :	float
-                    The value of Yslm at :math:`\\theta, phi'.
+    -------
+    Yslm : float
+           The value of Yslm at :math:`\\theta, phi'.
 
-            Note
-            ----
-            This is accurate upto 14 decimals for L upto 25.
+    Notes
+    -----
+    This is accurate upto 14 decimals for `L` upto 25.
     """
 
     from math import comb
 
     fact = np.math.factorial
 
     theta_grid = np.array(theta_grid)
     phi_grid = np.array(phi_grid)
 
     Sum = 0 + 1j * 0
 
     factor = 1
     if spin_weight < 0:
         factor = (-1) ** ell
-        theta = np.pi - theta
-        phi += np.pi
+        theta_grid = np.pi - theta_grid
+        phi_grid += np.pi
 
     abs_spin_weight = abs(spin_weight)
 
     for aar in range(0, ell - abs_spin_weight + 1):
         subterm = 0
 
-        if (aar + abs_spin_weight - emm) < 0 or (ell - aar - abs_spin_weight) < 0:
+        if (aar + abs_spin_weight - emm) < 0 or (
+            ell - aar - abs_spin_weight
+        ) < 0:
             message(f"Skipping r {aar}", message_verbosity=3)
             continue
         else:
             term1 = comb(ell - abs_spin_weight, aar)
             term2 = comb(ell + abs_spin_weight, aar + abs_spin_weight - emm)
             term3 = np.power(float(-1), (ell - aar - abs_spin_weight))
             term4 = np.exp(1j * emm * phi_grid)
-            term5 = np.power(np.tan(theta_grid / 2), (-2 * aar - abs_spin_weight + emm))
+            term5 = np.power(
+                np.tan(theta_grid / 2), (-2 * aar - abs_spin_weight + emm)
+            )
             subterm = term1 * term2 * term3 * term4 * term5
 
             Sum += subterm
 
     Yslmv = float(-1) ** emm * (
         np.sqrt(
             fact(ell + emm)
             * fact(ell - emm)
             * (2 * ell + 1)
-            / (4 * np.pi * fact(ell + abs_spin_weight) * fact(ell - abs_spin_weight))
+            / (
+                4
+                * np.pi
+                * fact(ell + abs_spin_weight)
+                * fact(ell - abs_spin_weight)
+            )
         )
         * np.sin(theta_grid / 2) ** (2 * ell)
         * Sum
     )
 
     return factor * Yslmv
 
 
 def Yslm_prec(spin_weight, ell, emm, theta, phi, prec=24):
     """Spin-weighted spherical harmonics function with precise computations.
                             Uses a symbolic method evaluated at the degree of precision requested
                             by the user.
     Parameters
     ----------
-
-    spin_weight :	int
-                                    The Spin weight.
-    ell :	int
-                    The mode number :math:`\\ell'.
-    emm :	int
-                    The azimuthal mode number :math:`m'.
+    spin_weight : int
+                  The Spin weight.
+    ell : int
+          The mode number :math:`\\ell'.
+    emm : int
+          The azimuthal mode number :math:`m'.
     theta : float
-                    The polar angle  :math:`\\theta` in radians,
-    phi :	float
-                    The aximuthal angle :math:`\\phi' in radians.
+            The polar angle  :math:`\\theta` in radians,
+    phi : float
+          The aximuthal angle :math:`\\phi' in radians.
     pres : int, optional
-               The precision i.e. number of digits to compute
-               upto. Default value is 16.
+           The precision i.e. number of digits to compute
+           upto. Default value is 16.
+
     Returns
     --------
-    Yslm :	float
-                    The value of Yslm at :math:`\\theta, phi'.
-
+    Yslm : float
+           The value of Yslm at :math:`\\theta, phi'.
     """
     import sympy as sp
 
     # tv, pv = theta, phi
     th, ph = sp.symbols("theta phi")
 
     Yslm_expr = Yslm_prec_sym(spin_weight, ell, emm)
 
     if spin_weight < 0:
         theta = np.pi - theta
         phi = np.pi + phi
 
-    return Yslm_expr.evalf(prec, subs={th: sp.Float(f"{theta}"), ph: sp.Float(f"{phi}")})
+    return Yslm_expr.evalf(
+        prec, subs={th: sp.Float(f"{theta}"), ph: sp.Float(f"{phi}")}
+    )
 
 
 def Yslm_prec_sym(spin_weight, ell, emm):
     """Spin-weighted spherical harmonics precise, symbolic computation for deferred evaluations.
        Is dependent on variables th: theta and ph:phi.
+
     Parameters
     ----------
-
-    spin_weight :	int
-                                    The Spin weight.
-    ell :	int
-                    The mode number :math:`\\ell'.
-    emm :	int
-                    The azimuthal mode number :math:`m'.
+    spin_weight : int
+                  The Spin weight.
+    ell : int
+          The mode number :math:`\\ell'.
+    emm : int
+          The azimuthal mode number :math:`m'.
     theta : float
-                    The polar angle  :math:`\\theta` in radians,
-    phi :	float
-                    The aximuthal angle :math:`\\phi' in radians.
+            The polar angle  :math:`\\theta` in radians,
+    phi : float
+          The aximuthal angle :math:`\\phi' in radians.
     pres : int, optional
-               The precision i.e. number of digits to compute
-               upto. Default value is 16.
+           The precision i.e. number of digits to compute
+           upto. Default value is 16.
 
     Returns
     --------
-    Yslm :	sym
-                    The value of Yslm at :math:`\\theta, phi'.
-
+    Yslm : sym
+           The value of Yslm at :math:`\\theta, phi'.
     """
     import sympy as sp
 
     th, ph = sp.symbols("theta phi")
 
     fact = sp.factorial
     Sum = 0
@@ -382,15 +385,17 @@
     # To get negative spin weight SWSH
     # in terms of positive spin weight
     factor = 1
     if spin_weight < 0:
         factor = sp.Pow(-1, ell)
 
     for aar in range(ell - abs_spin_weight + 1):
-        if (aar + abs_spin_weight - emm) < 0 or (ell - aar - abs_spin_weight) < 0:
+        if (aar + abs_spin_weight - emm) < 0 or (
+            ell - aar - abs_spin_weight
+        ) < 0:
             # message('Continuing')
             continue
         else:
             # message('r, l, s, m', r, l, s, m)
             # a1 = sp.binomial(ell - spin_weight, aar)
             # message(a1)
             # a2 = sp.binomial(ell + spin_weight, aar + spin_weight - emm)
@@ -398,26 +403,33 @@
             # a3 = sp.exp(1j * emm * phi)
             # message(a3)
             # a4 = sp.tan(theta / 2)
             # message(a4)
 
             Sum += (
                 sp.binomial(ell - abs_spin_weight, aar)
-                * sp.binomial(ell + abs_spin_weight, aar + abs_spin_weight - emm)
+                * sp.binomial(
+                    ell + abs_spin_weight, aar + abs_spin_weight - emm
+                )
                 * sp.Pow((-1), (ell - aar - abs_spin_weight))
                 * sp.exp(sp.I * emm * ph)
                 * sp.Pow(sp.cot(th / 2), (2 * aar + abs_spin_weight - emm))
             )
 
     Yslm_expr = sp.Pow(-1, emm) * (
         sp.sqrt(
             fact(ell + emm)
             * fact(ell - emm)
             * (2 * ell + 1)
-            / (4 * sp.pi * fact(ell + abs_spin_weight) * fact(ell - abs_spin_weight))
+            / (
+                4
+                * sp.pi
+                * fact(ell + abs_spin_weight)
+                * fact(ell - abs_spin_weight)
+            )
         )
         * sp.Pow(sp.sin(th / 2), (2 * ell))
         * Sum
     )
 
     Yslm_expr = factor * sp.simplify(Yslm_expr)
 
@@ -427,25 +439,25 @@
 def rotate_polarizations(wf, alpha):
     """Rotate the polarizations of the time domain
     observer waveform by :math:`2\alpha`
 
     Parameters
     ----------
     wf : 1d array
-             The complex observer waveform to rotate.
+         The complex observer waveform to rotate.
     alpha : float
-                    The coordinate angle to rotate the polarizations
-                    in radians. Note that the polarizarions would
-                    rotate by :math:`2 \alpha` on a cordinate
-                    rotation of :math:`\alpha`.
+            The coordinate angle to rotate the polarizations
+            in radians. Note that the polarizarions would
+            rotate by :math:`2 \alpha` on a cordinate
+            rotation of :math:`\alpha`.
 
     Returns
     -------
     rot_wf : 1d array
-                     The rotated waveform.
+             The rotated waveform.
     """
 
     h1, h2 = wf.real, wf.imag
 
     rh1 = np.cos(2 * alpha) * h1 - np.sin(2 * alpha) * h2
     rh2 = np.sin(2 * alpha) * h1 + np.cos(2 * alpha) * h2
```

### Comparing `waveformtools-2023.5.19/waveformtools/waveforms.py` & `waveformtools-2023.6.3/waveformtools/waveforms.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,138 +1,134 @@
 """ Classes for handling the waveform modes or data defined on spheres.
 
 
 Classes
 -------
-spherical_array:	A 2D data-type.
-					Stores and manages two-dimensional data on surfaces of spherical topology.
-modes_array: A data-type.
-			 Handle and work with mode coefficients.
+spherical_array : A 2D data-type.
+                  Stores and manages two-dimensional data on surfaces of spherical topology.
+modes_array : A data-type.
+              Handle and work with mode coefficients.
 """
 
 import sys
 
 import h5py
 import numpy as np
 
 from waveformtools import dataIO
-from waveformtools.dataIO import construct_mode_list
+from waveformtools.dataIO import (
+    construct_mode_list,
+    get_iteration_numbers_from_keys,
+    sort_keys,
+)
 from waveformtools.grids import spherical_grid
 from waveformtools.transforms import Yslm_vec
 from waveformtools.waveformtools import interp_resam_wfs, message
 
 #####################
 # Units
 #####################
-
 G = 6.67428 * 10 ** (-11.0)  # m^3 /kg /s^2
 # c = 3.0 * 10**8  # m/s
 c = 299_792_458.0  # m/s
 # Msun = 1.32712440041e20
-Msun = 1.988500 * 10**30.0  # g, SI
+Msun = 1.988500 * 10**30.0	# g, SI
 muc = c**2 / (G * Msun)  # g, NR to SI
 tuc = G * Msun / (c**3)  # s, NR to SI
 # dMpc = 3.0857 * 10 ** (22)  # m
 dMpc = 3.0856775814913672789139379577965e22
 
-#################################################
-# Spherical array class
-################################################
-
-
 # @jitclass(spec_sp)
 class spherical_array:
     """A class for handling waveforms on a sphere.
 
-
     Attributes
     ----------
-
-    label:	str
-                                                                                                                                    The label of the waveform data.
-    time_axis:	1d array
-                                                                                                                                                                                                    The time axis of the data.
-    frequency_axis: 1d array
-                                                                                                                                                                                                                                                                    The frequency axis if the data
-                                                                                                                                                                                                                                                                    is represented in frequency domain.
-    grid_info:	spherical_grid
-                                                                                                                                                                                                    An instance of the `spherical_grid` class.
-    data_len:	int
-                                                                                                                                                                                                    The length of the data along the time axis.
+    label : str
+            The label of the waveform data.
+    time_axis : 1d array
+                The time axis of the data.
+    frequency_axis : 1d array
+                     The frequency axis if the data
+                     is represented in frequency domain.
+    grid_info : spherical_grid
+                An instance of the `spherical_grid` class.
+    data_len : int
+               The length of the data along the time axis.
 
     Methods
     -------
-
-    delta_t:
-                                                                                                                                    Fetch the time stepping `delta_t`.
-    to_modes_array:
-                                                                                                                                                                                                                                                                    Find the waveform expressed in the
-                                                                                                                                                                                                                                                                    SWSH basis.
-    boost:
-                                                                                                                                    Boost the waveform.
-    supertranslate:
-                                                                                                                                                                                                                                                                    Supertranslate the waveform.
-
+    delta_t
+        Fetch the time stepping `delta_t`.
+    to_modes_array
+            Find the waveform expressed in the SWSH basis.
+    boost
+        Boost the waveform.
+    supertranslate
+                Supertranslate the waveform.
     """
 
     def __init__(
         self,
         label=None,
         time_axis=None,
         frequency_axis=None,
         data=None,
         data_dir=None,
         file_name=None,
         grid_info=None,
         spin_weight=2,
     ):
         self.label = label
-        # self.base_dir = base_dir	# The base directory containing the
+        # self.base_dir = base_dir  # The base directory containing the
         self.data = data
         self.file_name = file_name
         self.data_dir = data_dir
         self.time_axis = time_axis
         self.frequency_axis = frequency_axis
         self.grid_info = grid_info
         self.spin_weight = spin_weight
 
     def delta_t(self, value=None):
         """Sets and returns the value of time stepping :math:`dt`.
 
         Parameters
         ----------
         value : float, optional
-                                                                                                                                                                                                                                                                        The value of :math:`dt`
-                                                                                                                                                                                                                                                                        to set to the attribute.
+                The value of :math:`dt`
+                to set to the attribute.
 
         Returns
         -------
-        delta_t:	float
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         Sets the attribute.
+        delta_t : float
+                  Sets the attribute.
         """
 
         # if not self.delta_t:
         if not value:
             try:
                 delta_t = self.time_axis[1] - self.time_axis[0]
             except Exception as ex:
-                message("Please input the value of `delta_t` or supply the `time_axis` to the waveform.", ex)
+                message(
+                    "Please input the value of `delta_t` or supply the `time_axis` to the waveform.",
+                    ex,
+                )
         else:
             delta_t = value
 
         return delta_t
 
     @property
     def data_len(self):
         """Returns the length of the time/frequency axis.
 
         Returns
         -------
-        data_len:	int
-                                                                                                                                                                                                                                                                                                                                                                                                        The length of the time/frequency axis.
+        data_len : int
+                   The length of the time/frequency axis.
         """
 
         try:
             data_len = len(self.time_axis)
 
         except Exception as ex:
             data_len = len(self.frequency_axis)
@@ -142,25 +138,29 @@
 
     def to_modes_array(self, grid_info=None, spin_weight=None, ell_max=8):
         """Decompose a given spherical array function on a sphere
         into Spin Weighted Spherical Harmonic modes.
 
         Parameters
         ----------
-        spin_weight:	int, optional
-                                                                                                                                                                                                                                                                        The spin weight of the waveform. It defaults to -2 for a gravitational waveform.
-        ell_max:	int, optional
-                                                                                                                                                                                                        The maximum value of the :math:`\\ell` polar quantum number. Defaults to 8.
-        grid_info:	class instance
-                                                                                                                                                                                                        The class instance that contains the properties of the spherical grid.
+        spin_weight : int, optional
+                      The spin weight of the waveform. It defaults
+                      to -2 for a gravitational waveform.
+        ell_max : int, optional
+                  The maximum value of the :math:`\\ell`
+                  polar quantum number. Defaults to 8.
+        grid_info : class instance
+                    The class instance that contains
+                    the properties of the spherical grid.
 
         Returns
         -------
-        waveforms_modes:	modes_array
-                                                                                                                                                                                                                                                                                                                                        An instance of the `modes_array` class containing the decomposed modes.
+        waveforms_modes : modes_array
+                          An instance of the `modes_array`
+                          class containing the decomposed modes.
 
         Notes
         -----
         1. Assumes that the sphere on which this decomposition is carried out is so far out
            that the coordinate system is spherical polar on a round sphere.
         2. Assumes that the poper area is the same as its co-ordinate area.
         3. Ensure that the label of the input spherical array indicates whether
@@ -195,26 +195,30 @@
 
         if not self.label:
             label = "decomposed_time_domain"
         else:
             label = self.label
 
         # Create a mode array for the decomposed_waveform
-        waveform_modes = modes_array(label=label, ell_max=ell_max, spin_weight=spin_weight)
+        waveform_modes = modes_array(
+            label=label, ell_max=ell_max, spin_weight=spin_weight
+        )
 
         # Inherit the time or frequency axis.
         if "time" in label:
             # axis = self.time_axis
             waveform_modes.time_axis = self.time_axis
         else:
             # axis = self.frequency_axis
             waveform_modes.frequency_axis = self.frequency_axis
 
         # Create the modes_array
-        waveform_modes.create_modes_array(ell_max=ell_max, data_len=self.data_len)
+        waveform_modes.create_modes_array(
+            ell_max=ell_max, data_len=self.data_len
+        )
         waveform_modes.modes_list = modes_list
         # The area element on the sphere
         # Compute the meshgrid for theta and phi.
         theta, phi = grid_info.meshgrid
 
         # sqrt_met_det = np.sin(theta)
         sqrt_met_det = np.sqrt(np.power(np.sin(theta), 2))
@@ -227,109 +231,118 @@
             ell_value, all_emm_values = mode
 
             for emm_value in all_emm_values:
                 # m value.
 
                 # Spin weighted spherical harmonic function at (theta, phi)
 
-                Ybasis_fun = np.conj(Yslm_vec(spin_weight, ell=ell_value, emm=emm_value, theta_grid=theta, phi_grid=phi))
+                Ybasis_fun = np.conj(
+                    Yslm_vec(
+                        spin_weight,
+                        ell=ell_value,
+                        emm=emm_value,
+                        theta_grid=theta,
+                        phi_grid=phi,
+                    )
+                )
 
                 Ydarea = Ybasis_fun * darea
                 # print(Ydarea.shape)
                 # print(full_integrand)
                 # Using quad
-                multipole_ell_emm = np.tensordot(self.data, Ydarea, axes=((0, 1), (0, 1)))
+                multipole_ell_emm = np.tensordot(
+                    self.data, Ydarea, axes=((0, 1), (0, 1))
+                )
 
                 # print(f'l{ell_value}m{emm_value}', multipole_ell_emm)
 
-                waveform_modes.set_mode_data(ell_value, emm_value, multipole_ell_emm)
+                waveform_modes.set_mode_data(
+                    ell_value, emm_value, multipole_ell_emm
+                )
 
         return waveform_modes
 
     def boost(self, conformal_factor, grid_info=None):
         """Boost the waveform given the unboosted
         waveform and the boost conformal factor.
 
         Parameters
         ----------
-
-        self:	  spherical_array
-                                                                                                                                                                                                                                                                                                                                                                                                        A class instance of `spherical array`.
-
-        conformal_factor:		2d array
-                                                                                                                                                                                                                                                                                                                                                                                                        The conformal factor for the Lorentz transformation.
-                                                                                                                                                                                                                                                                                                                                                                                                        It may be a single floating point number or an array
-                                                                                                                                                                                                                                                                                                                                                                                                        on a spherical grid. The array will be of dimensions
-                                                                                                                                                                                                                                                                                                                                                                                                        [ntheta, nphi]
-
-        grid_info:		 class instance
-                                                                                                                                                                                                                                                                        The class instance that contains the properties of the spherical grid.
-
+        self : spherical_array
+               A class instance of `spherical array`.
+        conformal_factor : 2d array
+                           The conformal factor for the Lorentz transformation.
+                           It may be a single floating point number or an array
+                           on a spherical grid. The array will be of dimensions
+                           [ntheta, nphi]
+
+        grid_info : class instance
+                    The class instance that contains the properties of the spherical grid.
 
         Returns
         -------
-
-        boosted_waveform:	  sp_array
-                                                                                                                                                                                                                                                                                                                                          The class instance `sp_array` that
-                                                                                                                                                                                                                                                                                                                                          contains the boosted waveform.
+        boosted_waveform : sp_array
+                           The class instance `sp_array` that
+                           contains the boosted waveform.
         """
 
         from waveformtools.waveforms import spherical_array
 
-        if grid_info is None:
-            grid_info = self.grid_info
-
-        # Compute the boosted waveform on the spherical grid on all the elements.
+		inv_file_name = f"qlm_inv_z[{bh}].xy.h5"
 
-        boosted_waveform_data = np.transpose(self.data, (2, 0, 1)) * conformal_factor
+        boosted_waveform_data = (
+            np.transpose(self.data, (2, 0, 1)) * conformal_factor
+        )
         # boosted_waveform_data = np.multiply(self.data, conformal_factor[:, :, None])
         # boosted_waveform_data = boosted_waveform_item
         # boosted_waveform_data = np.array([np.transpose(item)*conformal_factor
         # for item in np.transpose(self.data)])
 
         # Construct a 2d waveform array object
         boosted_waveform = spherical_array(
-            grid_info=grid_info, data=np.transpose(np.array(boosted_waveform_data), (1, 2, 0))
+            grid_info=grid_info,
+            data=np.transpose(np.array(boosted_waveform_data), (1, 2, 0)),
         )
 
         # Assign other attributes.
         boosted_waveform.label = "boosted " + self.label
         boosted_waveform.time_axis = self.time_axis
 
         return boosted_waveform
 
     def supertranslate(self, supertransl_alpha_sp, order=1):
         """Supertranslate the :math:`\\Psi_{4\\ell m}` waveform modes, give the,
         the supertranslation parameter and the order.
 
         Parameters
         ----------
-        supertransl_alpha_modes :  modes_array
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           The modes_array containing the
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           supertranslation mode coefficients.
-        grid_info:		class instance
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        The class instance that contains
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        the properties of the spherical grid
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        using which the computations are
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        carried out.
-        order:		int
-                                                                                                                                                                                                                                                                                                                                                                                                        The number of terms to use to
-                                                                                                                                                                                                                                                                                                                                                                                                        approximate the supertranslation.
+        supertransl_alpha_modes : modes_array
+                                  The modes_array containing the
+                                  supertranslation mode coefficients.
+        grid_info : class instance
+                    The class instance that contains
+                    the properties of the spherical grid
+                    using which the computations are
+                    carried out.
+        order : int
+                The number of terms to use to
+                approximate the supertranslation.
 
         Returns
         -------
-        Psi4_supertransl:	  modes_array
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          A class instance containg the
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          modes of the supertranslated
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          waveform :math:`\\Psi_4`.
+        Psi4_supertransl : modes_array
+                           A class instance containg the
+                           modes of the supertranslated
+                           waveform :math:`\\Psi_4`.
         """
 
         # Create a spherical_array to hold the supertranslated waveform
         Psi4_supertransl_sp = spherical_array(
-            grid_info=self.grid_info, label="{} -> supertranslated time".format(self.label)
+            grid_info=self.grid_info,
+            label="{} -> supertranslated time".format(self.label),
         )
 
         delta_t = float(self.delta_t())
 
         # Set the data.
         data = 0
         # data = self.data
@@ -345,53 +358,45 @@
                 # print(f'differentiating {dorder+1} times')
                 dPsidu = differentiate5_vec_numba(dPsidu, delta_t)
 
             message("Incrementing...")
             # delta = np.power(supertransl_alpha_sp.data, index+1) * dPsidu / np.math.factorial(index+1)
             # print(delta/self.data)
 
-            data += np.power(supertransl_alpha_sp.data, index + 1) * dPsidu / np.math.factorial(index + 1)  # delta
+            data += (
+                np.power(supertransl_alpha_sp.data, index + 1)
+                * dPsidu
+                / np.math.factorial(index + 1)
+            )  # delta
 
         data += self.data
         message("Equal to original waveform?", (data == self.data).all())
 
         Psi4_supertransl_sp.data = data
         Psi4_supertransl_sp.time_axis = self.time_axis
         message("Done.")
         return Psi4_supertransl_sp
 
-    def load_qlm_data(self, data_dir=None, grid_info=None, bh=0, variable="sigma"):
+    def load_qlm_data(
+        self, data_dir=None, grid_info=None, bh=0, variable="sigma"
+    ):
         """Load the 2D shear data from h5 files.
 
         Parameters
         ----------
-        file_name: str
-                                                                                                                                                                                                        The name of the file containing data.
-        data_dir: str
-                                                                                                                                                                                                        The name of the directory containing data.
-        grid_info: class instance
-                                                                                                                                                                                                        An instance of the grid_info class.
-        bh: int
-                                                                        The black hole number (0, 1 or 2)
-
+        file_name : str
+                    The name of the file containing data.
+        data_dir : str
+                   The name of the directory containing data.
+        grid_info : class instance
+                    An instance of the grid_info class.
+        bh : int
+             The black hole number (0, 1 or 2)
         """
 
-        # import sys
-        # import re
-        # import json
-
-        # if file_name is None:
-        # 	if self.file_name is None:
-        # 		print('Please supply the file name!')
-        # 	else:
-        # 		file_name = self.file_name
-        # else:
-        # 	if self.file_name is None:
-        # 		self.file_name = file_name
-
         if data_dir is None:
             if self.data_dir is None:
                 print("Please supply the data directory!")
             else:
                 data_dir = self.data_dir
         else:
             if self.data_dir is None:
@@ -420,119 +425,145 @@
         # Open the modes file.
         with h5py.File(full_path, "r") as wfile:
             # Get all the mode keys.
             modes_keys_list = list(wfile.keys())
             # modes_keys_list = sorted(modes_keys_list)
 
             # Get the mode keys containing the data.
-            modes_keys_list = [item for item in modes_keys_list if "it=" in item]
+            modes_keys_list = [
+                item for item in modes_keys_list if "it=" in item
+            ]
 
             # Get the itaration numbers.
-            iteration_numbers = sorted(get_iteration_numbers_from_keys(modes_keys_list))
+            iteration_numbers = sorted(
+                get_iteration_numbers_from_keys(modes_keys_list)
+            )
             # sargs = np.argsort(iteration_numbers)
             # iteration_numbers = iteration_numbers[sargs]
             modes_keys_list = sort_keys(modes_keys_list)
             # Construct the data array.
 
             data_array = []
 
             for key in modes_keys_list:
                 # data_item = np.array(wfile[key])
                 # print(data_item.shape)
-                data_item = np.array(wfile[key])[nghosts : nphi - nghosts, nghosts : ntheta - nghosts]
+                data_item = np.array(wfile[key])[
+                    nghosts : nphi - nghosts, nghosts : ntheta - nghosts
+                ]
                 try:
                     data_item = data_item["real"] + 1j * data_item["imag"]
                 except Exception as ex:
                     message(ex)
                     pass
 
-                data_array.append(data_item)
-
-        self.data = np.transpose(np.array(data_array), (2, 1, 0))
-
-        self.iteration_axis = np.array(iteration_numbers)
-
-        #########################################################
-        # Load inv_coords data
-        #########################################################
-
-        inv_file_name = f"qlm_inv_z[{bh}].xy.h5"
-
-        # get the full path.
-        full_path = self.data_dir + inv_file_name
-
-        # Open the modes file.
-        with h5py.File(full_path, "r") as wfile:
-            # Get all the mode keys.
-            modes_keys_list = list(wfile.keys())
-            # modes_keys_list = sorted(modes_keys_list)
+		# Open the modes file.
+		with h5py.File(full_path, "r") as wfile:
+			# Get all the mode keys.
+			modes_keys_list = list(wfile.keys())
+			# modes_keys_list = sorted(modes_keys_list)
+
+			# Get the mode keys containing the data.
+			modes_keys_list = [item for item in modes_keys_list if "it=" in item]
+
+			modes_keys_list = sort_keys(modes_keys_list)
+			data_array = []
+
+			for key in modes_keys_list:
+				data_item = np.array(wfile[key])[nghosts : nphi - nghosts, nghosts : ntheta - nghosts]
+				# data_item = data_item['real'] + 1j*data_item['imag']
+				data_array.append(data_item)
+
+		self.invariant_coordinates_data = np.transpose(np.array(data_array), (2, 1, 0))
+
+		#########################################################
+		# Load metric determinant  data
+		#########################################################
+
+		twometric_qtt_file_name = f"qlm_qtt[{bh}].xy.h5"
+		twometric_qtp_file_name = f"qlm_qtp[{bh}].xy.h5"
+		twometric_qpp_file_name = f"qlm_qpp[{bh}].xy.h5"
 
             # Get the mode keys containing the data.
-            modes_keys_list = [item for item in modes_keys_list if "it=" in item]
-
-            modes_keys_list = sort_keys(modes_keys_list)
-            data_array = []
+            modes_keys_list = [
+                item for item in modes_keys_list if "it=" in item
+            ]
+
+		# Open the modes file.
+		with h5py.File(full_path, "r") as wfile:
+			# Get all the mode keys.
+			modes_keys_list = list(wfile.keys())
+			# modes_keys_list = sorted(modes_keys_list)
 
             for key in modes_keys_list:
-                data_item = np.array(wfile[key])[nghosts : nphi - nghosts, nghosts : ntheta - nghosts]
+                data_item = np.array(wfile[key])[
+                    nghosts : nphi - nghosts, nghosts : ntheta - nghosts
+                ]
                 # data_item = data_item['real'] + 1j*data_item['imag']
                 data_array.append(data_item)
 
-        self.invariant_coordinates_data = np.transpose(np.array(data_array), (2, 1, 0))
+        self.invariant_coordinates_data = np.transpose(
+            np.array(data_array), (2, 1, 0)
+        )
 
-        #########################################################
-        # Load metric determinant  data
-        #########################################################
-
-        twometric_qtt_file_name = f"qlm_qtt[{bh}].xy.h5"
-        twometric_qtp_file_name = f"qlm_qtp[{bh}].xy.h5"
-        twometric_qpp_file_name = f"qlm_qpp[{bh}].xy.h5"
+			qtt_data_array = []
 
-        # set the full path.
-        full_path = self.data_dir + twometric_qtt_file_name
+			for key in modes_keys_list:
+				data_item = np.array(wfile[key])[nghosts : nphi - nghosts, nghosts : ntheta - nghosts]
+				# data_item = data_item['real'] + 1j*data_item['imag']
+				qtt_data_array.append(data_item)
 
-        # Open the modes file.
-        with h5py.File(full_path, "r") as wfile:
-            # Get all the mode keys.
-            modes_keys_list = list(wfile.keys())
-            # modes_keys_list = sorted(modes_keys_list)
+		qtt_data_array = np.array(qtt_data_array)
+		qtt_data_array = np.transpose(qtt_data_array, (2, 1, 0))
+
+		# set the full path.
+		full_path = self.data_dir + twometric_qtp_file_name
 
             # Get the mode keys containing the data.
-            modes_keys_list = [item for item in modes_keys_list if "it=" in item]
+            modes_keys_list = [
+                item for item in modes_keys_list if "it=" in item
+            ]
 
-            modes_keys_list = sort_keys(modes_keys_list)
+			# Get the mode keys containing the data.
+			modes_keys_list = [item for item in modes_keys_list if "it=" in item]
 
-            qtt_data_array = []
+			modes_keys_list = sort_keys(modes_keys_list)
 
             for key in modes_keys_list:
-                data_item = np.array(wfile[key])[nghosts : nphi - nghosts, nghosts : ntheta - nghosts]
+                data_item = np.array(wfile[key])[
+                    nghosts : nphi - nghosts, nghosts : ntheta - nghosts
+                ]
                 # data_item = data_item['real'] + 1j*data_item['imag']
                 qtt_data_array.append(data_item)
 
-        qtt_data_array = np.array(qtt_data_array)
-        qtt_data_array = np.transpose(qtt_data_array, (2, 1, 0))
+			for key in modes_keys_list:
+				data_item = np.array(wfile[key])[nghosts : nphi - nghosts, nghosts : ntheta - nghosts]
+				# data_item = data_item['real'] + 1j*data_item['imag']
+				qtp_data_array.append(data_item)
 
-        # set the full path.
-        full_path = self.data_dir + twometric_qtp_file_name
+		qtp_data_array = np.array(qtp_data_array)
+		qtp_data_array = np.transpose(qtp_data_array, (2, 1, 0))
 
-        # Open the modes file.
-        with h5py.File(full_path, "r") as wfile:
-            # Get all the mode keys.
-            modes_keys_list = list(wfile.keys())
-            # modes_keys_list = sorted(modes_keys_list)
+		# set the full path.
+		full_path = self.data_dir + twometric_qpp_file_name
 
             # Get the mode keys containing the data.
-            modes_keys_list = [item for item in modes_keys_list if "it=" in item]
+            modes_keys_list = [
+                item for item in modes_keys_list if "it=" in item
+            ]
 
-            modes_keys_list = sort_keys(modes_keys_list)
+			# Get the mode keys containing the data.
+			modes_keys_list = [item for item in modes_keys_list if "it=" in item]
 
-            qtp_data_array = []
+			modes_keys_list = sort_keys(modes_keys_list)
 
             for key in modes_keys_list:
-                data_item = np.array(wfile[key])[nghosts : nphi - nghosts, nghosts : ntheta - nghosts]
+                data_item = np.array(wfile[key])[
+                    nghosts : nphi - nghosts, nghosts : ntheta - nghosts
+                ]
                 # data_item = data_item['real'] + 1j*data_item['imag']
                 qtp_data_array.append(data_item)
 
         qtp_data_array = np.array(qtp_data_array)
         qtp_data_array = np.transpose(qtp_data_array, (2, 1, 0))
 
         # set the full path.
@@ -541,218 +572,104 @@
         # Open the modes file.
         with h5py.File(full_path, "r") as wfile:
             # Get all the mode keys.
             modes_keys_list = list(wfile.keys())
             # modes_keys_list = sorted(modes_keys_list)
 
             # Get the mode keys containing the data.
-            modes_keys_list = [item for item in modes_keys_list if "it=" in item]
+            modes_keys_list = [
+                item for item in modes_keys_list if "it=" in item
+            ]
 
             modes_keys_list = sort_keys(modes_keys_list)
 
             qpp_data_array = []
 
             for key in modes_keys_list:
-                data_item = np.array(wfile[key])[nghosts : nphi - nghosts, nghosts : ntheta - nghosts]
+                data_item = np.array(wfile[key])[
+                    nghosts : nphi - nghosts, nghosts : ntheta - nghosts
+                ]
                 # data_item = data_item['real'] + 1j*data_item['imag']
                 qpp_data_array.append(data_item)
 
         qpp_data_array = np.array(qpp_data_array)
         qpp_data_array = np.transpose(qpp_data_array, (2, 1, 0))
 
         sqrt_met_det = np.sqrt(
             np.linalg.det(
-                np.transpose(np.array([[qtt_data_array, qtp_data_array], [qtp_data_array, qpp_data_array]]), (2, 3, 4, 0, 1))
+                np.transpose(
+                    np.array(
+                        [
+                            [qtt_data_array, qtp_data_array],
+                            [qtp_data_array, qpp_data_array],
+                        ]
+                    ),
+                    (2, 3, 4, 0, 1),
+                )
             )
         )
 
         self.sqrt_met_det_data = sqrt_met_det
 
-    def to_shear_modes_array(self, grid_info=None, spin_weight=None, ell_max=8):
-        """Decompose a given spherical array function on a sphere
-        into Spin Weighted Spherical Harmonic modes.
-
-        Parameters
-        ----------
-        spin_weight:	int, optional
-                                                                                                                                                                                                                                                                        The spin weight of the waveform. It defaults to -2 for a gravitational waveform.
-        ell_max:	int, optional
-                                                                                                                                                                                                        The maximum value of the :math:`\\ell` polar quantum number. Defaults to 8.
-        grid_info:	class instance
-                                                                                                                                                                                                        The class instance that contains the properties of the spherical grid.
-
-        Returns
-        -------
-        waveforms_modes:	modes_array
-                                                                                                                                                                                                                                                                                                                                        An instance of the `modes_array` class containing the decomposed modes.
-
-        Notes
-        -----
-        1. Assumes that the sphere on which this decomposition is carried out is so far out
-           that the coordinate system is spherical polar on a round sphere.
-        2. Assumes that the poper area is the same as its co-ordinate area.
-        3. Ensure that the label of the input spherical array indicates whether
-           it is a time domain data or frequency domain data.
-        """
-
-        if grid_info is None:
-            if self.grid_info is None:
-                message("Please specify the grid specs. Assuming defaults.")
-                grid_info = spherical_grid()
-                self.grid_info = grid_info
-            else:
-                grid_info = self.grid_info
-
-        if spin_weight is None:
-            if self.spin_weight is None:
-                message("Please specify spin weight. Assuming 2")
-                spin_weight = 2
-                self.spin_weight = spin_weight
-
-            else:
-                spin_weight = self.spin_weight
-
-        spin_weight = abs(spin_weight)
-        # Compute the meshgrid for theta and phi.
-        theta, phi = grid_info.meshgrid
-
-        # Create a modes array object
-
-        # Create a modes list.
-        modes_list = construct_mode_list(ell_max, spin_weight=spin_weight)
-
-        if not self.label:
-            label = "decomposed_time_domain"
-        else:
-            label = self.label
-
-        # Create a mode array for the decomposed_waveform
-        waveform_modes = modes_array(label=label, ell_max=ell_max, spin_weight=spin_weight)
-
-        # Inherit the time or frequency axis.
-        if "time" in label:
-            # axis = self.time_axis
-            waveform_modes.time_axis = self.time_axis
-        else:
-            # axis = self.frequency_axis
-            waveform_modes.frequency_axis = self.frequency_axis
-
-        # Create the modes_array
-        waveform_modes.time_axis = self.time_axis[:]
-        # sargs = np.argsort(waveform_modes.time_axis)
-        # message(sargs)
-        waveform_modes.time_axis = waveform_modes.time_axis
-
-        waveform_modes.create_modes_array(ell_max=ell_max, data_len=self.data_len)
-        waveform_modes.modes_list = modes_list
-        # The area element on the sphere
-        # Compute the meshgrid for theta and phi.
-        theta, phi = grid_info.meshgrid
-
-        phi = np.transpose(np.array([phi for index in range(len(self.time_axis))]), (1, 2, 0))
-
-        # sqrt_met_det = np.sin(theta)
-        # sqrt_met_det = np.sqrt(np.power(np.sin(theta), 2))
-
-        darea = self.sqrt_met_det_data * grid_info.dtheta * grid_info.dphi
-
-        theta = np.emath.arccos(self.invariant_coordinates_data)
-
-        modes_list = [item for item in modes_list if item[0] >= spin_weight]
-
-        for mode in modes_list:
-            ell_value, all_emm_values = mode
-
-            for emm_value in all_emm_values:
-                # m value.
-                # message(f'Processing l{ell_value} m{emm_value}')
-                # Spin weighted spherical harmonic function at (theta, phi)
-
-                Ybasis_fun = np.conj(
-                    Yslm_vec(spin_weight=spin_weight, ell=ell_value, emm=emm_value, theta_grid=theta, phi_grid=phi)
-                )
-                # Ybasis_fun = np.array([np.conj(Yslm_vec(spin_weight=spin_weight,
-                # ell=ell_value, emm=emm_value, theta_grid=theta[:, :, index],
-                # phi_grid=phi[:, :, index])) for index in range(self.data_len)])
-                # Ybasis_fun = np.transpose(Ybasis_fun, (1, 2, 0))
-                # message('Ybasis_fun', Ybasis_fun.shape)
-                Ydarea = Ybasis_fun * darea
-                # message('Ydarea', Ydarea.shape)
-                # message(full_integrand)
-                # Using quad
-                # message('self.data', self.data.shape)
-                # multipole_ell_emm = np.tensordot(self.data, Ydarea, axes=((0, 1), (0, 1)))
-                multipole_ell_emm = np.sum(self.data * Ydarea, (0, 1))
-
-                # message(f'l{ell_value}m{emm_value}', multipole_ell_emm)
-
-                # message('multipole_ell_emm', multipole_ell_emm.shape)
-                waveform_modes.set_mode_data(ell_value, emm_value, data=multipole_ell_emm)
-
-        return waveform_modes
-
 
 # @jitclass(spec_ma)
 class modes_array:
     """A class that holds mode array of waveforms
 
     Attributes
     ----------
-    label: str
-                                                                                                                                                                                                                                                                    The label of the modes array.
-    r_ext: float
-                                                                                                                                                                                                                                                                    The extraction radius.
-    modes_list: list
-                                                                                                                                                                                                                                                                                                                                                                                                     The list of available modes
-                                                                                                                                                                                                                                                                                                                                                                                                     in the format [l1, [m values], [l2, [m values], ...]]
-    ell_max:	int
-                                                                                                                                                                                                                                                                                                                                                                                                    The maximum :math:`\\ell`
-                                                                                                                                                                                                                                                                                                                                                                                                    mode available.
-    modes_data: 3d array
-                                                                                                                                                                                                                                                                                                                                                                                                     The three dimensional array
-                                                                                                                                                                                                                                                                                                                                                                                                     containing modes in time/frequency
-                                                                                                                                                                                                                                                                                                                                                                                                     space. The axis of the array is
-                                                                                                                                                                                                                                                                                                                                                                                                     (:math:`\\ell`, :math:`m`, time/freq).
-    base_dir:	str
-                                                                                                                                                                                                                                                                                                                                                                                                    The base directory containing the
-                                                                                                                                                                                                                                                                                                                                                                                                    modes data.
-    data_dir:	str
-                                                                                                                                                                                                                                                                                                                                                                                                    The subdirectory in which to look
-                                                                                                                                                                                                                                                                                                                                                                                                    for the data.
-    filename: str
-                                                                                                                                                                                                                                                                                                                                                                                                    The filename containg the modes data.
-
+    label : str
+            The label of the modes array.
+    r_ext : float
+            The extraction radius.
+    modes_list : list
+                 The list of available modes
+                 in the format [l1, [m values], [l2, [m values], ...]]
+    ell_max : int
+              The maximum :math:`\\ell` mode available.
+    modes_data : 3d array
+                 The three dimensional array
+                 containing modes in time/frequency
+                 space. The axis of the array is
+                 (:math:`\\ell`, :math:`m`, time/freq).
+    base_dir : str
+               The base directory containing the
+               modes data.
+    data_dir : str
+               The subdirectory in which to look
+               for the data.
+    filename : str
+               The filename containg the modes data.
 
     Methods
     -------
-    get_metadata:
-                                                                                                                                                                                                                                                                    Get the metadata associated with the modes_array.
-    mode:
-                                                                                                                                    Get the data for the given :math:`\\ell, m` mode.
-    create_modes_array:
-                                                                                                                                                                                                                                                                                                                                    A private method to create an empty modes_array of given shape.
-    delta_t:
-                                                                                                                                    Set the attribute `delta_t` and/ or return its value.
-    load_modes:
-                                                                                                                                                                                                    Load the waveform modes from a specified h5 file.
-    save_modes:
-                                                                                                                                                                                                    Save the waveform modes to a specified h5 file.
-    set_mode_data:
-                                                                                                                                                                                                                                                                    Set the `mode` data of specified modes.
-    to_frequency_basis:
-                                                                                                                                                                                                                                                                                                                                    Get the `modes_array` in frequency basis from its time basis representation.
-    to_time_basis:
-                                                                                                                                                                                                                                                                    Get the `modes_array` in temporal basis from its frequency basis representation.
-    extrap_to_inf:
-                                                                                                                                                                                                                                                                    Extrapolate the modes to infinity.
-    supertranslate:
-                                                                                                                                                                                                                                                                    Supertranslate the waveform modes.
-    boost:
-                                                                                                                                    Boost the waveform modes.
-
+    get_metadata
+            Get the metadata associated with the modes_array.
+    mode
+        Get the data for the given :math:`\\ell, m` mode.
+    create_modes_array
+                A private method to create an empty modes_array of given shape.
+    delta_t
+        Set the attribute `delta_t` and/ or return its value.
+    load_modes
+            Load the waveform modes from a specified h5 file.
+    save_modes
+            Save the waveform modes to a specified h5 file.
+    set_mode_data
+            Set the `mode` data of specified modes.
+    to_frequency_basis
+            Get the `modes_array` in frequency basis from its time basis representation.
+    to_time_basis
+            Get the `modes_array` in temporal basis from its frequency basis representation.
+    extrap_to_inf
+            Extrapolate the modes to infinity.
+    supertranslate
+            Supertranslate the waveform modes.
+    boost
+        Boost the waveform modes.
     """
 
     def __init__(
         self,
         data_dir=None,
         file_name=None,
         modes_data=None,
@@ -790,16 +707,16 @@
         self.actions = actions
 
     def get_metadata(self):
         """Get the metadata associated with the instance.
 
         Returns
         -------
-        metadata:	dict
-                                                                                                                                                                                                                                                                                                                                                                                                        A dictionary of metedata.
+        metadata : dict
+                   A dictionary of metedata.
         """
         # The metadata dict
         unnecessary_keys = ["_time_axis", "_modes_data", "freq_axis"]
 
         # Get all attributes
         # metadata = self.__dict__
         metadata = {}
@@ -807,34 +724,34 @@
         for key, val in self.__dict__.items():
             if key in unnecessary_keys:
                 pass
             else:
                 metadata.update({key: val})
 
         # for item in unnecessary_keys:
-        # 	metadata.pop(item, None)
+        # metadata.pop(item, None)
 
         # self.metadata = metadata
 
         return metadata
 
     def mode(self, ell, emm):
         """The modes array data structure to hold waveform modes.
 
         Parameters
         ----------
-        ell:		int
-                                                                                                                                                                                                                                                                                                                                                                                                        The :math:`\\ell` index of the mode.
-        emm:		int
-                                                                                                                                                                                                                                                                                                                                                                                                        The :math:`m` index of the mode.
+        ell : int
+              The :math:`\\ell` index of the mode.
+        emm : int
+              The :math:`m` index of the mode.
 
         Returns
         -------
-        mode_data:		array
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        The array of the requested mode.
+        mode_data : array
+                    The array of the requested mode.
         """
 
         emm_index = ell + emm
 
         return self.modes_data[ell, emm_index, :]
 
     @property
@@ -856,23 +773,23 @@
         self._modes_data = modes_data
 
     def create_modes_array(self, ell_max=None, data_len=None):
         """Create a modes array and initialize it with zeros.
 
         Parameters
         ----------
-        ell_max:	 int
-                                                                                                                                                                                                                                                                                                                                                                                                         The maximum :math:`\\ell` value of the modes.
-        data_len:	int
-                                                                                                                                                                                                                                                                                                                                                                                                        The number of points along the third (time / frequency) axis.
+        ell_max : int
+                  The maximum :math:`\\ell` value of the modes.
+        data_len : int
+                   The number of points along the third (time / frequency) axis.
 
         Returns
         -------
-        self.modes_array:		 modes_array
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         sets the `self.modes_array` attribute.
+        self.modes_array : modes_array
+                           sets the `self.modes_array` attribute.
         """
         import datetime
         import time
 
         # Check ell_max
         if ell_max is None:
             try:
@@ -885,18 +802,22 @@
             try:
                 data_len = self.data_len
             except Exception as ex:
                 message(ex)
                 raise NameError("Please supply data_len")
 
         if self.modes_list is None:
-            self.modes_list = construct_mode_list(ell_max=ell_max, spin_weight=self.spin_weight)
+            self.modes_list = construct_mode_list(
+                ell_max=ell_max, spin_weight=self.spin_weight
+            )
 
         # self.modes_data = np.zeros([ell_max + 1, 2 * (ell_max + 1) + 1, data_len], dtype=np.complex128)
-        self.modes_data = np.zeros((ell_max + 1, 2 * (ell_max + 1) + 1, data_len), dtype=np.complex128)
+        self.modes_data = np.zeros(
+            (ell_max + 1, 2 * (ell_max + 1) + 1, data_len), dtype=np.complex128
+        )
 
         # Set the time metadata
         time_now = time.localtime()
         time_now = time.strftime("%H:%M:%S", time_now)
 
         date_now = str(datetime.date.today())
 
@@ -907,16 +828,16 @@
 
     @property
     def data_len(self):
         """Returns the length of the time/frequency axis.
 
         Returns
         -------
-        data_len:	int
-                                                                                                                                                                                                                                                                                                                                                                                                        THe length of the time/frequency axis.
+        data_len : int
+                   The length of the time/frequency axis.
         """
 
         try:
             data_len = len(self.time_axis)
 
         except Exception as ex:
             message(ex)
@@ -930,54 +851,61 @@
 
     def delta_t(self, value=None):
         """Sets and returns the value of time stepping :math:`dt`.
 
         Parameters
         ----------
         value : float, optional
-                                                                                                                                                                                                                                                                        The value of :math:`dt`
-                                                                                                                                                                                                                                                                        to set to the attribute.
+                The value of :math:`dt`
+                to set to the attribute.
+
         Returns
         -------
-        self.delta_t:	 float
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         Sets the attribute.
+        self.delta_t : float
+                       Sets the attribute.
         """
 
         if not value:
             try:
                 delta_t = self.time_axis[1] - self.time_axis[0]
             except Exception as ex:
-                message("Please input the value of `delta_t` or supply the `time_axis` to the waveform.", ex)
+                message(
+                    "Please input the value of `delta_t` or supply the `time_axis` to the waveform.",
+                    ex,
+                )
         else:
             delta_t = value
 
         return delta_t
 
     @property
     def delta_f(self, value=None):
         """Sets and returns the value of frequency stepping :math:`df`.
 
         Parameters
         ----------
         value : float, optional
-                                                                                                                                                                                                                                                                        The value of :math:`df`
-                                                                                                                                                                                                                                                                        to set to the attribute.
+                The value of :math:`df`
+                to set to the attribute.
 
         Returns
         -------
-        delta_f:	 float
-                                                                                                                                                                                                                                                                                                                                                                                                         Sets the attribute.
+        delta_f : float
+                  Sets the attribute.
         """
 
         # if not self.delta_t:
         if not value:
             try:
                 delta_f = self.frequency_axis[1] - self.frequency_axis[0]
             except Exception as ex:
-                message("Please input the value of `delta_f` or supply the `frequency_axis` to the waveform.", ex)
+                message(
+                    "Please input the value of `delta_f` or supply the `frequency_axis` to the waveform.",
+                    ex,
+                )
         else:
             delta_f = value
 
         return delta_f
 
     def load_modes(
         self,
@@ -1002,46 +930,47 @@
         debug=False,
     ):
         """Load the waveform mode data from an hdf file.
 
         Parameters
         ----------
         extrap_order : int, optional
-                                                                                                                                                                                                           For SpEC waveforms only. This is the order of extrapolation to use.
+                       For SpEC waveforms only. This is the order of extrapolation to use.
 
-        pre_key:	str, optional
-                                                                                                                                                                                                                                                                                                                                                                                                        A string containing the key of the group in
-                                                                                                                                                                                                                                                                                                                                                                                                        the HDF file in which the modes` dataset exists.
-                                                                                                                                                                                                                                                                                                                                                                                                        It defaults to `None`.
-        mode_numbers:	list
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        The mode numbers to load from the file.
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        Each item in the list is a list that
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        contains two integrer numbers, one for
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        the mode index :math:`\\ell` and the
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        other for the mode index :math:`m`.
-        crop:	bool
-                                                                                                                                                                                                                                                                        Whether or not to crop the beginning of the input
-                                                                                                                                                                                                                                                                        waveform. If yes, the first :math:`t=r_{ext}`
-                                                                                                                                                                                                                                                                        length of data will be discarded.
+        pre_key : str, optional
+                  A string containing the key of the group in
+                  the HDF file in which the modes` dataset exists.
+                  It defaults to `None`.
+        mode_numbers : list
+                       The mode numbers to load from the file.
+                       Each item in the list is a list that
+                       contains two integrer numbers, one for
+                       the mode index :math:`\\ell` and the
+                       other for the mode index :math:`m`.
+        crop : bool
+               Whether or not to crop the beginning of the input
+               waveform. If yes, the first :math:`t=r_{ext}`
+               length of data will be discarded.
 
         Returns
         -------
-        waveform_obj:	3d array
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        Sets the three dimensional array `waveform.modes` that contains
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        the required :math:`\\ell, m` modes.
+        waveform_obj : 3d array
+                       Sets the three dimensional array `waveform.modes` that contains
+                       the required :math:`\\ell, m` modes.
 
         Examples
         --------
         # Note
         # Update this!
-        #>>> from waveformtools.waveforms import waveform
-        #>>> waveform.set_basedir('./')
-        #>>> waveform.set_datadir('data/')
-        #>>> mode_numbers = [[2, 2], [3, 3]]
-        #>>> waveform.load_data(mode_numbers=mode_numbers)
+        #>>> from waveformtools.waveforms import modes_array
+        #>>> wf = modes_array(label='wf', spin_weight=-2)
+        #>>> wf.data_dir = './'
+        #>>> wf.filename = 'wf_file.h5'
+        #>>> wf.modes_list = [[2, -2, -1, 0, 1, 2], [3, -3, 3]]
+        #>>> waveform.load_modes()
         """
 
         if debug is False:
             wfs_nl = 1
         if not data_dir:
             data_dir = self.data_dir
         else:
@@ -1057,23 +986,34 @@
         else:
             self.ell_max = ell_max
 
         if not label:
             label = self.label
 
         # if self.data_dir is not None:
-        # 	data_dir = self.data_dir
+        # data_dir = self.data_dir
 
         # if self.file_name is not None:
-        # 	file_name = self.file_name
+        # file_name = self.file_name
         message(f"Passing {data_dir}/{file_name}", message_verbosity=2)
 
         if ftype == "generic":
             dataIO.load_gen_data_from_disk(
-                self, label, data_dir, file_name, r_ext, ell_max, pre_key, modes_list, crop, centre, key_ex, r_ext_factor
+                self,
+                label,
+                data_dir,
+                file_name,
+                r_ext,
+                ell_max,
+                pre_key,
+                modes_list,
+                crop,
+                centre,
+                key_ex,
+                r_ext_factor,
             )
 
         elif (ftype) == "RIT" or (ftype == "GT"):
             if var_type == "Psi4":
                 dataIO.load_RIT_Psi4_data_from_disk(
                     wfa=self,
                     data_dir=data_dir,
@@ -1156,30 +1096,30 @@
         compression_opts=0,
         r_ext=None,
     ):
         """Save the waveform mode data to an hdf file.
 
         Parameters
         ----------
-        pre_key:	str, optional
-                                                                                                                                                                                                                                                                                                                                                                                                        A string containing the key of the group in
-                                                                                                                                                                                                                                                                                                                                                                                                        the HDF file in which the modes` dataset exists.
-                                                                                                                                                                                                                                                                                                                                                                                                        It defaults to `None`.
-        mode_numbers:	list
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        The mode numbers to load from the file.
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        Each item in the list is a list that
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        contains two integrer numbers, one for
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        the mode index :math:`\\ell` and the
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        other for the mode index :math:`m`.
+        pre_key : str, optional
+                  A string containing the key of the group in
+                  the HDF file in which the modes` dataset exists.
+                  It defaults to `None`.
+        mode_numbers : list
+                       The mode numbers to load from the file.
+                       Each item in the list is a list that
+                       contains two integrer numbers, one for
+                       the mode index :math:`\\ell` and the
+                       other for the mode index :math:`m`.
 
         Returns
         -------
-        waveform_obj:	3d array
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        Sets the three dimensional array `waveform.modes` that contains
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        the required :math:`\\ell, m` modes.
+        waveform_obj : 3d array
+                       Sets the three dimensional array `waveform.modes`
+                       that contains the required :math:`\\ell, m` modes.
 
         Examples
         --------
         >>> from waveformtools.waveforms import waveform
         >>> waveform.set_basedir('./')
         >>> waveform.set_datadir('data/')
         >>> mode_numbers = [[2, 2], [3, 3]]
@@ -1206,51 +1146,49 @@
         raise NotImplementedError
 
     def set_mode_data(self, ell_value, emm_value, data):
         """Set the mode array data for the respective :math:`(\\ell, m)` mode.
 
         Parameters
         ----------
-        ell_value:		int
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        The :math:`\\ell` polar mode number.
-        emm_value:		int
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        The :math:`emm` azimuthal mode number.
-        data:		1d array
-                                                                                                                                                                                                                                                                                                                                                                                                        The array consisting of mode data for the requested mode.
+        ell_value : int
+                    The :math:`\\ell` polar mode number.
+        emm_value : int
+                    The :math:`emm` azimuthal mode number.
+        data : 1d array
+               The array consisting of mode data for the requested mode.
 
         Returns
         -------
-        self.mode_data: modes_data
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        The updated modes data.
+        self.mode_data : modes_data
+                         The updated modes data.
         """
         # Compute the emm index given ell.
         emm_index = emm_value + ell_value
 
         # Set the mode data.
         self._modes_data[ell_value, emm_index] = data
 
     def to_spherical_array(self, grid_info, meth_info, spin_weight=None):
         """Obtain the spherical array from the modes array.
 
         Parameters
         ----------
-
-        grid_info:	cls instance
-                                                                                                                                                                                                        An instance of the "spherical_grid" class
-                                                                                                                                                                                                        to hold the grid info.
+        grid_info : cls instance
+                    An instance of the "spherical_grid" class
+                    to hold the grid info.
         meth_info : cls instance
-                                                                                                                                                                                                        An instance of the class waveformtools.diagnostics.method_info that
-                                                                                                                                                                                                        provides information on what methods to use for integration.
+                    An instance of the class waveformtools.diagnostics.method_info that
+                    provides information on what methods to use for integration.
+
         Returns
         -------
-
-        waveform_sp:	spherical_array
-                                                                                                                                                                                                                                                                        A member of the "spherical_array" class
-                                                                                                                                                                                                                                                                        constructed from the given "modes_rray".
-
+        waveform_sp : spherical_array
+                      A member of the "spherical_array" class
+                      constructed from the given "modes_rray".
         """
 
         # Create a spherical array.
         waveform_sp = spherical_array(label=self.label, grid_info=grid_info)
 
         if spin_weight is None:
             if self.spin_weight is not None:
@@ -1271,49 +1209,57 @@
         # Get the coordinate meshgrid
         theta, phi = grid_info.meshgrid
 
         s1, s2 = theta.shape
         s3 = self.data_len
         sp_data = np.zeros((s1, s2, s3), dtype=np.complex128)
 
-        modes_list = [item for item in self.modes_list if item[0] >= spin_weight]
+        modes_list = [
+            item for item in self.modes_list if item[0] >= spin_weight
+        ]
         for item in modes_list:
             # Get modes.
             ell, emm_list = item
             # if ell<spin_weight:
-            # 	continue
+            # continue
 
             for emm in emm_list:
                 # For every l, m
                 sp_data += np.multiply.outer(
-                    Yslm_vec(spin_weight, ell=ell, emm=emm, theta_grid=theta, phi_grid=phi), self.mode(ell, emm)
+                    Yslm_vec(
+                        spin_weight,
+                        ell=ell,
+                        emm=emm,
+                        theta_grid=theta,
+                        phi_grid=phi,
+                    ),
+                    self.mode(ell, emm),
                 )
                 # message(sp_data)
         # Set the data of the spherical array.
         waveform_sp.data = sp_data
         try:
             waveform_sp.time_axis = self.time_axis
         except Exception as ex:
             message(ex)
             waveform_sp.frequency_axis = self.frequency_axis
         return waveform_sp
 
     def trim(self, trim_upto_time=None):
         """Trim the modes_array at the beginning and center about
-                                                                        the peak of the 2,2 mode.
+        the peak of the 2,2 mode.
 
         Parameters
         ----------
-        time:	float
-                                                                                                                                        The time unit upto which to discard.
+        time : float
+               The time unit upto which to discard.
 
         Returns
         -------
         Re-sets the `time_axis` and `modes_array` data.
-
         """
         if trim_upto_time is None:
             trim_upto_time = self.r_ext
 
         # Compute the start index
         start = int(trim_upto_time / self.delta_t())
 
@@ -1328,65 +1274,77 @@
         self._time_axis = self.time_axis - self.time_axis[max_ind]
 
     def to_frequency_basis(self):
         """Compute the modes in frequency basis.
 
         Returns
         -------
-        waveform_tilde_modes:	modes_array
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        A modes_array containing the modes
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        in frequency basis.
+        waveform_tilde_modes : modes_array
+                               A modes_array containing the modes
+                               in frequency basis.
         """
 
         # Create a new modes array
-        waveform_tilde_modes = modes_array(label=f"{self.label} -> frequency_domain")
-        waveform_tilde_modes.create_modes_array(ell_max=self.ell_max, data_len=self.data_len)
+        waveform_tilde_modes = modes_array(
+            label=f"{self.label} -> frequency_domain"
+        )
+        waveform_tilde_modes.create_modes_array(
+            ell_max=self.ell_max, data_len=self.data_len
+        )
 
         from waveformtools.transforms import compute_fft
 
         for mode in self.modes_list:
             # Extrapolate every mode
 
             # Ge the ell value
             ell_value, emm_list = mode
 
             for emm_value in emm_list:
-                freq_axis, freq_data = compute_fft(self.mode(ell_value, emm_value), self.delta_t())
+                freq_axis, freq_data = compute_fft(
+                    self.mode(ell_value, emm_value), self.delta_t()
+                )
 
-                waveform_tilde_modes.set_mode_data(ell_value, emm_value, freq_data)
+                waveform_tilde_modes.set_mode_data(
+                    ell_value, emm_value, freq_data
+                )
 
         waveform_tilde_modes.frequency_axis = freq_axis
         waveform_tilde_modes.ell_max = self.ell_max
         waveform_tilde_modes.modes_list = self.modes_list
         return waveform_tilde_modes
 
     def to_time_basis(self):
         """Compute the modes in time basis.
 
         Returns
         -------
-        waveform_modes :  modes_array
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          A modes_array containing the modes
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          in frequency basis.
+        waveform_modes: modes_array
+                        A modes_array containing the modes
+                        in frequency basis.
         """
 
         # Create a new modes array
         waveform_modes = modes_array(label=f"{self.label} -> time_domain")
-        waveform_modes.create_modes_array(ell_max=self.ell_max, data_len=self.data_len)
+        waveform_modes.create_modes_array(
+            ell_max=self.ell_max, data_len=self.data_len
+        )
 
         from waveformtools.transforms import compute_ifft
 
         for mode in self.modes_list:
             # Extrapolate every mode
 
             # Ge the ell value
             ell_value, emm_list = mode
 
             for emm_value in emm_list:
-                time_axis, time_data = compute_ifft(self.mode(ell_value, emm_value), self.delta_f)
+                time_axis, time_data = compute_ifft(
+                    self.mode(ell_value, emm_value), self.delta_f
+                )
 
                 waveform_modes.set_mode_data(ell_value, emm_value, time_data)
 
         try:
             maxloc = np.argmax(np.absolute(waveform_modes.mode(2, 2)))
         except Exception as ex:
             message(ex)
@@ -1394,44 +1352,52 @@
 
         maxtime = time_axis[maxloc]
 
         waveform_modes.time_axis = time_axis - maxtime
 
         return waveform_modes
 
-    def extrap_to_inf(self, mass=1, spin=None, modes_list="all", method="SIO", r_ext_factor=1):
+    def extrap_to_inf(
+        self,
+        mass=1,
+        spin=None,
+        modes_list="all",
+        method="SIO",
+        r_ext_factor=1,
+        diff_method="CS",
+        diff_degree=24,
+    ):
         """Extrapolate the :math:`\\Psi_4` modes to infinity
         using the perturbative improved second order method.
 
         Parameters
         ----------
-        mass:		float
-                                                                                                                                                                                                                                                                                                                                                                                                        The effective total mass of the system.
-        spin:		float
-                                                                                                                                                                                                                                                                                                                                                                                                        The effective spin of the system.
-        modes:		modes array, optional
-                                                                                                                                                                                                        The modes to extrapolate. Defaults
-                                                                                                                                                                                                        to `all` if not specified.
-        method: str
-                                                                                                                                                                                                        The method to use for extrapolation. The available methods are:
+        mass : float
+               The effective total mass of the system.
+        spin : float
+               The effective spin of the system.
+        modes : modes array, optional
+                The modes to extrapolate. Defaults
+                to `all` if not specified.
+        method : str
+                 The method to use for extrapolation. The available methods are:
 
         +------------+--------------------------------------+
-        | Method str | Name									|
+        | Method str | Name                                 |
         +------------+--------------------------------------+
-        |'FO'		 | First order							|
-        |'SO'		 | Second order							|
-        |'SIO'		 | Second improved order				|
-        |'NM'		 | Numerical method (not ready yet)		|
+        |'FO'        | First order                          |
+        |'SO'        | Second order                         |
+        |'SIO'       | Second improved order                |
+        |'NM'        | Numerical method (not ready yet)     |
         +------------+--------------------------------------+
 
         Returns
         -------
-        waveform_inf_modes: modes array
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        A new modes array that contains
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        the extrapolated modes.
+        waveform_inf_modes : modes array
+                             A new modes array that contains the extrapolated modes.
         """
 
         from functools import partial
 
         # Prepare the extrapolating method.
         if method == "SIO":
             from waveformtools.extrapolate import (
@@ -1440,14 +1406,16 @@
 
             extrap_method = partial(
                 waveextract_to_inf_perturbative_twop5_order,
                 delta_t=self.delta_t(),
                 areal_radius=self.r_ext,
                 mass=mass,
                 spin=spin,
+                method=diff_method,
+                degree=diff_degree,
             )
 
         if method == "SO":
             from waveformtools.extrapolate import (
                 waveextract_to_inf_perturbative_two_order,
             )
 
@@ -1461,30 +1429,38 @@
 
         if method == "FO":
             from waveformtools.extrapolate import (
                 waveextract_to_inf_perturbative_one_order,
             )
 
             extrap_method = partial(
-                waveextract_to_inf_perturbative_one_order, u_ret=self.time_axis, areal_radius=self.r_ext, mass=mass
+                waveextract_to_inf_perturbative_one_order,
+                u_ret=self.time_axis,
+                areal_radius=self.r_ext,
+                mass=mass,
             )
 
         if method == "NM":
             message("This method is not available yet! ")
 
         # Prepare the modes to be extrapolated.
         if modes_list == "all":
-            modes_list = construct_mode_list(self.ell_max)
+            modes_list = construct_mode_list(self.ell_max, self.spin_weight)
 
         # Create a mode array for the extrapolated waveform.
         extrap_wf = modes_array(
-            label=f"{self.label} -> rPsi4_inf", modes_list=self.modes_list, ell_max=self.ell_max, r_ext=self.r_ext
+            label=f"{self.label} -> rPsi4_inf",
+            modes_list=self.modes_list,
+            ell_max=self.ell_max,
+            r_ext=self.r_ext,
         )
 
-        extrap_wf.create_modes_array(ell_max=self.ell_max, data_len=self.data_len)
+        extrap_wf.create_modes_array(
+            ell_max=self.ell_max, data_len=self.data_len
+        )
 
         # Retain the time axis.
         extrap_wf.time_axis = self.time_axis
         for mode in modes_list:
             # Extrapolate every mode
 
             # Ge the ell value
@@ -1508,237 +1484,278 @@
 
     def supertranslate(self, supertransl_alpha_modes, grid_info, order=4):
         """Supertranslate the :math:`\\Psi_{4\\ell m}` waveform modes, give the,
         the supertranslation parameter and the order.
 
         Parameters
         ----------
-        supertransl_alpha_modes :  modes_array
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           The modes_array containing the
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           supertranslation mode coefficients.
-        grid_info:		class instance
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        The class instance that contains
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        the properties of the spherical grid
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        using which the computations are
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        carried out.
-        order:		int
-                                                                                                                                                                                                                                                                                                                                                                                                        The number of terms to use to
-                                                                                                                                                                                                                                                                                                                                                                                                        approximate the supertranslation.
+        supertransl_alpha_modes : modes_array
+                                  The modes_array containing the supertranslation
+                                  mode coefficients.
+        grid_info : grids class instance
+                    The class instance that contains
+                    the properties of the spherical grid
+                    using which the computations are carried out.
+        order : int
+                The number of terms to use to approximate the supertranslation.
 
         Returns
         -------
-        Psi4_supertransl:	  modes_array
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          A class instance containg the
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          modes of the supertranslated
-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          waveform :math:`\\Psi_4`.
+        Psi4_supertransl : modes_array
+                           A class instance containg the
+                           modes of the supertranslated
+                           waveform :math:`\\Psi_4`.
         """
 
         import BMS
 
         ell_max = self.ell_max
         # Step 0: Get the grid properties for integrations
 
         # Compute the meshgrid for theta and phi.
         theta, phi = grid_info.meshgrid
         # theta
         # Step 1: get the grid function for supertranslation parameter
-        supertransl_alpha_sphere = BMS.compute_supertransl_alpha(supertransl_alpha_modes, theta, phi)
+        supertransl_alpha_sphere = BMS.compute_supertransl_alpha(
+            supertransl_alpha_modes, theta, phi
+        )
 
         # The supertranslation is carried out in frequency space.
         # Step 2: get the FFT of the mode coefficients of Psi4
         Psi4_tilde_modes = self.to_frequency_basis()
 
         # Get the 2d angular frequency array
         omega_axis_2d = Psi4_tilde_modes.omega
 
         # Construct the supertranslation factor
         supertransl_factor = np.sum(
-            np.array([np.power((-1j * omega_axis_2d * supertransl_alpha_sphere), index) for index in range(order)]),
+            np.array(
+                [
+                    np.power(
+                        (-1j * omega_axis_2d * supertransl_alpha_sphere), index
+                    )
+                    for index in range(order)
+                ]
+            ),
             axis=0,
         )
 
         # Multiply with the fourier modes.
-        supertransl_spherical_factor = Psi4_tilde_modes.multiply(supertransl_factor)
+        supertransl_spherical_factor = Psi4_tilde_modes.multiply(
+            supertransl_factor
+        )
 
         # Reconstruct the modes
 
         # Check!
-        supertransl_spherical_grid = np.zeros(supertransl_spherical_factor.shape, dtype=np.complex128)
+        supertransl_spherical_grid = np.zeros(
+            supertransl_spherical_factor.shape, dtype=np.complex128
+        )
 
         for ell_value in range(ell_max + 1):
             for emm_value in range(-ell_value, ell_value + 1):
                 # Multiply with the SWSH basis.
-                supertransl_spherical_grid += supertransl_spherical_factor * Yslm_vec(
-                    spin_weight=-2, ell=ell_value, emm=emm_value, theta=theta, phi=phi
+                supertransl_spherical_grid += (
+                    supertransl_spherical_factor
+                    * Yslm_vec(
+                        spin_weight=-2,
+                        ell=ell_value,
+                        emm=emm_value,
+                        theta=theta,
+                        phi=phi,
+                    )
                 )
 
                 # Step 3: Reconstruct the function on the sphere
 
         # Create a spherical_array to hold the supertranslated waveform
         supertransl_spherical_waveform = spherical_array(grid_info=grid_info)
 
         # Set the data.
         supertransl_spherical_waveform.data = supertransl_spherical_grid
 
         # Get modes_array from spherical_array
-        Psi4_supertransl_modes = supertransl_spherical_waveform.to_modes_array(ell_max=ell_max)
+        Psi4_supertransl_modes = supertransl_spherical_waveform.to_modes_array(
+            ell_max=ell_max
+        )
 
         return Psi4_supertransl_modes
 
     def boost(self, conformal_factor, grid_info=None):
         """Boost the waveform given the unboosted waveform and the boost conformal factor.
 
         Parameters
         ----------
-        conformal_factor:		2d array
-                                                                                                                                                                                                                                                                                                                                                                                                        The conformal factor for the Lorentz transformation.
-                                                                                                                                                                                                                                                                                                                                                                                                        It may be a single floating point number or an array
-                                                                                                                                                                                                                                                                                                                                                                                                        on a spherical grid. The array will be of dimensions
-                                                                                                                                                                                                                                                                                                                                                                                                        [ntheta, nphi]
+        conformal_factor : 2d array
+                           The conformal factor for the Lorentz transformation.
+                           It may be a single floating point number or an array
+                           on a spherical grid. The array will be of dimensions
+                           [ntheta, nphi]
 
         Returns
         -------
-        boosted_waveform:	  spherical_array
-                                                                                                                                                                                                                                                                                                                                          The class instance `spherical_array`
-                                                                                                                                                                                                                                                                                                                                          that contains the boosted waveform.
+        boosted_waveform : spherical_array
+                           The class instance `spherical_array`
+                           that contains the boosted waveform.
         """
 
         from waveformtools.grids import spherical_grid
 
         # Construct a spherical grid.
         if grid_info is None:
             grid_info = spherical_grid()
 
         # Get spherical array from modes.
         unboosted_waveform = self.to_spherical_array(grid_info)
 
         boosted_waveform_data = unboosted_waveform.boost(conformal_factor)
 
         # Construct a 2d waveform array object
-        boosted_waveform = spherical_array(grid_info=unboosted_waveform.grid_info, data=np.array(boosted_waveform_data))
+        boosted_waveform = spherical_array(
+            grid_info=unboosted_waveform.grid_info,
+            data=np.array(boosted_waveform_data),
+        )
         boosted_waveform.label = "boosted"
 
         # Get modes from spherical data.
         # boosted_waveform_modes = boosted_waveform.to_modes_array()
 
         # return boosted_waveform_modes
         return boosted_waveform
 
     def get_strain_from_psi4(self, omega0="auto"):
         """Get the strain `modes_array` from :math:`\\Psi_4` by
         fixed frequency integration.
 
         Parameters
         ----------
-        omega0: float, optional
-                                                                                                                                        The lower cutoff angular frequency for FFI.
-                                                                                                                                        By default, it computes this from the mode
-                                                                                                                                        data.
+        omega0 : float, optional
+                 The lower cutoff angular frequency for FFI.
+                 By default, it computes this from the mode data.
 
         Returns
         -------
-
-        strain_waveform:	modes_array
-                                                                                                                                                                                                                                                                                                                                        The computed strain modes.
-
+        strain_waveform : modes_array
+                          The computed strain modes.
         """
 
         # Initialize a mode array for strain.
         strain_waveform = modes_array(
-            label="{} strain from Psi4".format(self.label), r_ext=self.r_ext, ell_max=8, modes_list=self.modes_list
+            label="{} strain from Psi4".format(self.label),
+            r_ext=self.r_ext,
+            ell_max=8,
+            modes_list=self.modes_list,
         )
 
         strain_waveform.time_axis = self.time_axis
         strain_waveform.ell_max = self.ell_max
 
         data_len = self.data_len
 
-        strain_waveform.create_modes_array(ell_max=self.ell_max, data_len=data_len)
+        strain_waveform.create_modes_array(
+            ell_max=self.ell_max, data_len=data_len
+        )
 
         # Integrate,
         from waveformtools.integrate import fixed_frequency_integrator
-        from waveformtools.waveformtools import get_starting_angular_frequency as sang_f
+        from waveformtools.waveformtools import (
+            get_starting_angular_frequency as sang_f,
+        )
 
         omega_st = omega0
         for item in self.modes_list[:]:
             ell, emm_list = item
             for emm in emm_list:
                 mode_data = self.mode(ell, emm)
                 if omega0 == "auto":
-                    omega_st = abs(sang_f(mode_data, delta_t=self.delta_t())) / 10
+                    omega_st = (
+                        abs(sang_f(mode_data, delta_t=self.delta_t())) / 10
+                    )
                 strain_mode_data, _ = fixed_frequency_integrator(
-                    udata_time=mode_data, delta_t=self.delta_t(), omega0=omega_st, order=2
+                    udata_time=mode_data,
+                    delta_t=self.delta_t(),
+                    omega0=omega_st,
+                    order=2,
                 )
                 strain_waveform.set_mode_data(ell, emm, data=strain_mode_data)
 
         return strain_waveform
 
     def get_news_from_psi4(self, omega0="auto"):
         """Get the News `modes_array` from :math:`\\Psi_4` by
         fixed frequency integration.
 
         Parameters
         ----------
-        omega0: float, optional
-                                                                                                                                        The lower cutoff angular frequency for FFI.
-                                                                                                                                        By default, it computes this as one tenth of
-                                                                                                                                        the starting frequency of the mode data.
+        omega0 : float, optional
+                 The lower cutoff angular frequency for FFI.
+                 By default, it computes this as one tenth of
+                 the starting frequency of the mode data.
 
         Returns
         -------
-        news_waveform:	modes_array
-                                                                                                                                                                                                                                                                        The computed strain modes.
-
+        news_waveform : modes_array
+                        The computed strain modes.
         """
 
         # Initialize a mode array for strain.
         # news_waveform = modes_array(label=f'{self.label} news from Psi4', r_ext=500, ell_max=8, modes_list=self.modes_list)
         news_waveform = modes_array(
-            label="{} news from Psi4".format(self.label), r_ext=500, ell_max=8, modes_list=self.modes_list
+            label="{} news from Psi4".format(self.label),
+            r_ext=500,
+            ell_max=8,
+            modes_list=self.modes_list,
         )
 
         news_waveform.time_axis = self.time_axis
         news_waveform.ell_max = self.ell_max
 
         data_len = self.data_len
 
-        news_waveform.create_modes_array(ell_max=self.ell_max, data_len=data_len)
+        news_waveform.create_modes_array(
+            ell_max=self.ell_max, data_len=data_len
+        )
 
         # Integrate,
         from waveformtools.integrate import fixed_frequency_integrator
-        from waveformtools.waveformtools import get_starting_angular_frequency as sang_f
+        from waveformtools.waveformtools import (
+            get_starting_angular_frequency as sang_f,
+        )
 
         omega_st = omega0
         for item in self.modes_list[:]:
             ell, emm_list = item
             for emm in emm_list:
                 mode_data = self.mode(ell, emm)
                 if omega0 == "auto":
-                    omega_st = abs(sang_f(mode_data, delta_t=self.delta_t())) / 10
+                    omega_st = (
+                        abs(sang_f(mode_data, delta_t=self.delta_t())) / 10
+                    )
                 news_mode_data, _ = fixed_frequency_integrator(
-                    udata_time=mode_data, delta_t=self.delta_t(), omega0=omega_st, order=1
+                    udata_time=mode_data,
+                    delta_t=self.delta_t(),
+                    omega0=omega_st,
+                    order=1,
                 )
                 news_waveform.set_mode_data(ell, emm, data=news_mode_data)
 
         return news_waveform
 
     def taper(self, zeros="auto"):
         """Taper a waveform at both ends and insert zeros if needed
 
         Parameters
         ----------
-
-        zeros:	int
-                                                                                                                                        The number of zeros to add at rach end
+        zeros : int
+                The number of zeros to add at rach end
 
         Returns
         -------
-
-        tapered_modes:	modes_array
-                                                                                                                                                                                                                                                                        Modes array with tapered mode data.
+        tapered_modes : modes_array
+                        Modes array with tapered mode data.
         """
 
         from waveformtools.waveformtools import taper
 
         if zeros == "auto":
             # Decide the number of zeros
             data_len = self.data_len
@@ -1770,221 +1787,300 @@
                     tapered_modes = modes_array(
                         label="tapered {}".format(self.label),
                         r_ext=self.r_ext,
                         modes_list=self.modes_list,
                         ell_max=self.ell_max,
                     )
 
-                    tapered_modes.create_modes_array(ell_max=self.ell_max, data_len=new_data_len)
+                    tapered_modes.create_modes_array(
+                        ell_max=self.ell_max, data_len=new_data_len
+                    )
                 tapered_data = tapered_data_re + 1j * tapered_data_im
 
                 # message(len(tapered_data_re))
                 tapered_modes.set_mode_data(ell, emm, data=tapered_data)
 
         # Set the time axis
-        new_time_axis = np.arange(0, new_data_len * self.delta_t(), self.delta_t())
+        new_time_axis = np.arange(
+            0, new_data_len * self.delta_t(), self.delta_t()
+        )
 
         tapered_modes.time_axis = new_time_axis
 
         # Recenter the modes.
         tapered_modes.trim(trim_upto_time=0)
 
         return tapered_modes
 
-    def taper_tanh(self, time_axis=None, zeros="auto", duration=10, sides="both"):
+    def taper_tanh(
+        self, time_axis=None, zeros="auto", duration=10, sides="both"
+    ):
         """Taper a waveform at both ends and insert zeros if needed
 
         Parameters
         ----------
-
-        zeros:	int
-                                                                                                                                        The number of zeros to add at rach end
+        zeros : int
+                The number of zeros to add at rach end
 
         Returns
         -------
-
-        tapered_modes:	modes_array
-                                                                                                                                                                                                                                                                        Modes array with tapered mode data.
+        tapered_modes : modes_array
+                        Modes array with tapered mode data.
         """
 
-        from waveformtools.waveformtools import taper_tanh
+		for item in self.modes_list[:]:
+			ell, emm_list = item
+			for emm in emm_list:
+				input_data_re = self.mode(ell, emm).real
+				input_data_im = self.mode(ell, emm).imag
 
-        if zeros == "auto":
-            # Decide the number of zeros
-            data_len = self.data_len
+				tapered_data_re = taper(input_data_re, zeros=zeros)
+				tapered_data_im = taper(input_data_im, zeros=zeros)
 
-            nearest_power = int(np.log(data_len) / np.log(2))
-            req_len = np.power(2, nearest_power + 1)
-            zeros = req_len - data_len
-            # message('num_zeros', zeros)
+				# tapered_data_re = taper_tanh(input_data_re, delta_t=self.delta_t())
+				# tapered_data_im = taper_tanh(input_data_im, delta_t=self.delta_t())
 
-        # New modes array.
+				new_data_len = len(tapered_data_re)
 
-        tapered_modes = None
+				if tapered_modes is None:
+					tapered_modes = modes_array(
+						label="tapered {}".format(self.label),
+						r_ext=self.r_ext,
+						modes_list=self.modes_list,
+						ell_max=self.ell_max,
+					)
 
-        for item in self.modes_list[:]:
-            ell, emm_list = item
-            for emm in emm_list:
-                input_data_re = self.mode(ell, emm).real
-                input_data_im = self.mode(ell, emm).imag
+					tapered_modes.create_modes_array(ell_max=self.ell_max, data_len=new_data_len)
+				tapered_data = tapered_data_re + 1j * tapered_data_im
 
-                # tapered_data_re = taper(input_data_re, zeros=zeros)
-                # tapered_data_im = taper(input_data_im, zeros=zeros)
+				# message(len(tapered_data_re))
+				tapered_modes.set_mode_data(ell, emm, data=tapered_data)
 
-                _, tapered_data_re = taper_tanh(input_data_re, delta_t=self.delta_t(), duration=duration, sides=sides)
-                _, tapered_data_im = taper_tanh(input_data_im, delta_t=self.delta_t(), duration=duration, sides=sides)
+                _, tapered_data_re = taper_tanh(
+                    input_data_re,
+                    delta_t=self.delta_t(),
+                    duration=duration,
+                    sides=sides,
+                )
+                _, tapered_data_im = taper_tanh(
+                    input_data_im,
+                    delta_t=self.delta_t(),
+                    duration=duration,
+                    sides=sides,
+                )
 
-                new_data_len = len(tapered_data_re)
+		tapered_modes.time_axis = new_time_axis
 
-                if tapered_modes is None:
-                    tapered_modes = modes_array(
-                        label="tapered {}".format(self.label),
-                        r_ext=self.r_ext,
-                        modes_list=self.modes_list,
-                        ell_max=self.ell_max,
-                    )
+		# Recenter the modes.
+		tapered_modes.trim(trim_upto_time=0)
 
-                    tapered_modes.create_modes_array(ell_max=self.ell_max, data_len=new_data_len)
+                    tapered_modes.create_modes_array(
+                        ell_max=self.ell_max, data_len=new_data_len
+                    )
                 tapered_data = tapered_data_re + 1j * tapered_data_im
 
-                # message(len(tapered_data_re))
-                tapered_modes.set_mode_data(ell, emm, data=tapered_data)
+	def taper_tanh(self, time_axis=None, zeros="auto", duration=10, sides="both"):
+		"""Taper a waveform at both ends and insert zeros if needed
 
         # Set the time axis
-        new_time_axis = np.arange(0, new_data_len * self.delta_t(), self.delta_t())
+        new_time_axis = np.arange(
+            0, new_data_len * self.delta_t(), self.delta_t()
+        )
 
-        tapered_modes.time_axis = new_time_axis
+		Returns
+		-------
+		tapered_modes:	modes_array
+																																										Modes array with tapered mode data.
+		"""
 
-        # Recenter the modes.
-        tapered_modes.trim(trim_upto_time=0)
+		from waveformtools.waveformtools import taper_tanh
 
-        return tapered_modes
+		if zeros == "auto":
+			# Decide the number of zeros
+			data_len = self.data_len
 
-    def low_cut(self, omega0=0.03, order=2):
-        """Apply the low cut filter from waveformtools.low_cut_filter
+			nearest_power = int(np.log(data_len) / np.log(2))
+			req_len = np.power(2, nearest_power + 1)
+			zeros = req_len - data_len
+			# message('num_zeros', zeros)
 
         Parameters
         ----------
-        order:	   int, optional
-                                                                                                                                                                                                        The order of the butterworth filter.
-        omega0:		float, optional
-                                                                                                                                                                                                        The cutoff frequency of the butterworth filter.
+        order : int, optional
+                The order of the butterworth filter.
+        omega0 : float, optional
+                The cutoff frequency of the butterworth filter.
 
-        Returns:
+        Returns
         --------
-        filtered_modes: modes_array
-                                                                                                                                                                                                                                                                        A modes array object containing filtered modes.
-
+        filtered_modes : modes_array
+                         A modes array object containing filtered modes.
         """
 
-        # modes_array for filtered data.
-        filtered_modes = None
+				# tapered_data_re = taper(input_data_re, zeros=zeros)
+				# tapered_data_im = taper(input_data_im, zeros=zeros)
 
-        # Import the filter
-        from waveformtools.waveformtools import low_cut_filter
+				_, tapered_data_re = taper_tanh(input_data_re, delta_t=self.delta_t(), duration=duration, sides=sides)
+				_, tapered_data_im = taper_tanh(input_data_im, delta_t=self.delta_t(), duration=duration, sides=sides)
 
-        for item in self.modes_list:
-            # Iterate over available modes.
-            ell, emm_list = item
-            for emm in emm_list:
-                if filtered_modes is None:
-                    # Create filtered_modes
-                    filtered_modes = modes_array(
-                        label="lc filtered {}".format(self.label),
-                        r_ext=self.r_ext,
-                        modes_list=self.modes_list,
-                        ell_max=self.ell_max,
-                    )
+				new_data_len = len(tapered_data_re)
 
-                    filtered_modes.create_modes_array(ell_max=self.ell_max, data_len=self.data_len)
+                    filtered_modes.create_modes_array(
+                        ell_max=self.ell_max, data_len=self.data_len
+                    )
 
                 # Get filtered mode data.
-                filtered_data = low_cut_filter(self.mode(ell, emm), self.frequency_axis, omega0=omega0, order=order)
+                filtered_data = low_cut_filter(
+                    self.mode(ell, emm),
+                    self.frequency_axis,
+                    omega0=omega0,
+                    order=order,
+                )
 
-                # Set the mode data.
-                filtered_modes.set_mode_data(ell, emm, data=filtered_data)
+				# message(len(tapered_data_re))
+				tapered_modes.set_mode_data(ell, emm, data=tapered_data)
 
-        # Set the f axis.
-        filtered_modes.frequency_axis = self.frequency_axis
+		# Set the time axis
+		new_time_axis = np.arange(0, new_data_len * self.delta_t(), self.delta_t())
 
-        return filtered_modes
+		tapered_modes.time_axis = new_time_axis
 
-    def to_td_waveform(self, Mtotal=1, theta=0, phi=0, alpha=None, distance=1, delta_t=None, method="precise", k=None):
+    def to_td_waveform(
+        self,
+        Mtotal=1,
+        theta=0,
+        phi=0,
+        alpha=None,
+        distance=1,
+        delta_t=None,
+        method="precise",
+        k=None,
+    ):
         """Get the plus and cross polarizations of
         of the waveform time series by summing the modes.
 
         Parameters
         ----------
         theta, phi : float
-                                                                                                                                        The inclination and the azimuthal
-                                                                                                                                        angular position of the observer
-                                                                                                                                        in the NR coodinate system.
+                     The inclination and the azimuthal
+                     angular position of the observer
+                     in the NR coodinate system.
 
         distance : float
+                   The distance to the source
 
         method : str
-                                                                                                                                         The method to use to generate
-                                                                                                                                         the SWSH basis. This can be
-                                                                                                                                         `precise` or `fast`.
+                 The method to use to generate
+                 the SWSH basis. This can be
+                 `precise` or `fast`.
+
         Returns
         -------
         taxis, hp, hc : 1d arrays
-                                                                                                                                         The 1d arrays of the time axis and
-                                                                                                                                         the polarizations of the waveforms.
+                        The 1d arrays of the time axis and
+                        the polarizations of the waveforms.
 
         Notes
         -----
-
         This does not rotate the polarizations. The rotation
         must be done separately using the `rotate_polarizations`
         function of `waveformtools.transforms`
 
         For precessing systems and to obtain the waveform
         in the LAL convention, one should use the
         nrcatalogtools package to obtain the correct
         angles first.
-
         """
 
-        if method == "fast":
-            message("Using fast SWSH method")
-            from waveformtools.transforms import Yslm
-        elif method == "precise":
-            message("Using precise SWSH method")
-            from waveformtools.transforms import Yslm_prec as Yslm
-        else:
-            raise NotImplementedError(f"Unknown method {method}")
-
-        wts = 0
-        all_yslm = []
-        flat_modes = []
-
-        for ell, emm_list in self.modes_list:
-            for emm in emm_list:
-                Y = Yslm(self.spin_weight, ell, emm, theta=theta, phi=phi)
-
-                all_yslm.append(np.complex256(Y))
-                flat_modes.append(self.mode(ell, emm))
-
-        all_yslm = np.complex256(all_yslm)
-
-        wts = np.dot(all_yslm, flat_modes)
-
-        # Rescale the time axis
-        taxis = self.time_axis * tuc * Mtotal
+					filtered_modes.create_modes_array(ell_max=self.ell_max, data_len=self.data_len)
 
-        if isinstance(delta_t, float):
-            # Resample the waveform
-            new_taxis = np.arange(taxis[0], taxis[-1], delta_t)
-            wts = interp_resam_wfs(wts, taxis, new_taxis, k=k)
-            taxis = new_taxis
+				# Get filtered mode data.
+				filtered_data = low_cut_filter(self.mode(ell, emm), self.frequency_axis, omega0=omega0, order=order)
 
-        # Rescale the magnitude of the waveform
-        wts = Mtotal * wts / (distance * dMpc * muc)
+				# Set the mode data.
+				filtered_modes.set_mode_data(ell, emm, data=filtered_data)
 
-        # Rotate polarizations
-        if alpha is not None:
-            from waveformtools.transforms import rotate_polarizations
+		# Set the f axis.
+		filtered_modes.frequency_axis = self.frequency_axis
+
+		return filtered_modes
+
+	def to_td_waveform(self, Mtotal=1, theta=0, phi=0, alpha=None, distance=1, delta_t=None, method="precise", k=None):
+		"""Get the plus and cross polarizations of
+		of the waveform time series by summing the modes.
+
+		Parameters
+		----------
+		theta, phi:	float
+					The inclination and the azimuthal
+					angular position of the observer
+					in the NR coodinate system.
+
+				distance:	float
+										The distance to the source
+
+		method:	str
+				The method to use to generate
+				the SWSH basis. This can be
+								`precise` or `fast`.
+
+		Returns
+		-------
+		taxis, hp, hc:	1d arrays
+												The 1d arrays of the time axis and
+						the polarizations of the waveforms.
+
+		Notes
+		-----
+		This does not rotate the polarizations. The rotation
+		must be done separately using the `rotate_polarizations`
+		function of `waveformtools.transforms`
+
+		For precessing systems and to obtain the waveform
+		in the LAL convention, one should use the
+		nrcatalogtools package to obtain the correct
+		angles first.
+		"""
+
+		if method == "fast":
+			message("Using fast SWSH method")
+			from waveformtools.transforms import Yslm
+		elif method == "precise":
+			message("Using precise SWSH method")
+			from waveformtools.transforms import Yslm_prec as Yslm
+		else:
+			raise NotImplementedError(f"Unknown method {method}")
+
+		wts = 0
+		all_yslm = []
+		flat_modes = []
+
+		for ell, emm_list in self.modes_list:
+			for emm in emm_list:
+				Y = Yslm(self.spin_weight, ell, emm, theta=theta, phi=phi)
+
+				all_yslm.append(np.complex256(Y))
+				flat_modes.append(self.mode(ell, emm))
+
+		all_yslm = np.complex256(all_yslm)
+
+		wts = np.dot(all_yslm, flat_modes)
+
+		# Rescale the time axis
+		taxis = self.time_axis * tuc * Mtotal
+
+		if isinstance(delta_t, float):
+			# Resample the waveform
+			new_taxis = np.arange(taxis[0], taxis[-1], delta_t)
+			wts = interp_resam_wfs(wts, taxis, new_taxis, k=k)
+			taxis = new_taxis
+
+		# Rescale the magnitude of the waveform
+		wts = Mtotal * wts / (distance * dMpc * muc)
+
+		# Rotate polarizations
+		if alpha is not None:
+			from waveformtools.transforms import rotate_polarizations
 
-            wts = rotate_polarizations(wts, alpha)
+			wts = rotate_polarizations(wts, alpha)
 
-        return taxis, wts.real, -wts.imag
+		return taxis, wts.real, -wts.imag
```

### Comparing `waveformtools-2023.5.19/waveformtools/waveformtools.py` & `waveformtools-2023.6.3/waveformtools/waveformtools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 # pylint: disable=C0301
 """  This module contains a set of tools to handle data from numerical relativity simulations and gravitational waves.
-
+It consists of a bunch of functions that were frequently used for handling NR data.
+Notes
+1. Some functions here display plots. If you intend to use these on the
+cluster and if xterm is not adequately setup, you may have to
+either comment the plot codes or use the`Agg` mode for plotting
+and save the figures instead of showing by changing the appropriate
+lines in the code.
+2. These is a module consisting of functions, not completely optimized
+for speed. This will happen in future.
+3. These functions are not defined in classes as they mostly use and
+operate on the objects of pycbc's builtin classes.
+4. Any suggestions, comments, critisism invited to vaishak@gmail.com!
 """
 
 import datetime
 import os
 import pickle
 
 # import statistics
@@ -25,66 +36,54 @@
 
 import scipy
 
 # matplotlib.use('Agg')
 from matplotlib import pyplot as plt
 from termcolor import colored
 
-##########################################################################
-""" Basic functions """
-##########################################################################
-
 
 def message(
-    *args, message_verbosity=2, print_verbosity=config.print_verbosity, log_verbosity=config.log_verbosity, **kwargs
+    *args,
+    message_verbosity=2,
+    print_verbosity=config.print_verbosity,
+    log_verbosity=config.log_verbosity,
+    **kwargs,
 ):
     """The print function with verbosity levels and logging facility.
 
     Notes
     -----
-
     Verbosity choices:
 
-                                    message_verbosity	:	Each message carries with it a verbosity level.
-                                                                                    More the verbosity less the priority.
-                                                                                    Default value is 2 i.e. informational.
-
-                                    print_verbosity		:	prints all messages above this level of verbosity.
-
-                                    log_verbosity		:	logs all messages above this level of verbosity.
-
-    Verbosity  levels:
-
-                                    0: Errors
-
-                                    1: Warnings
-
-                                    2: Information
+    * message_verbosity : Each message carries with it a verbosity level.
+                          More the verbosity less the priority.
+                          Default value is 2 i.e. informational.
+    * print_verbosity : prints all messages above this level of verbosity.
+    * log_verbosity : logs all messages above this level of verbosity.
+
+    Verbosity  levels :
+    * 0 : Errors
+    * 1 : Warnings
+    * 2 : Information
 
     Parameters
     ----------
-
-                                    ``*args`			:	non-keyword arguments
-                                                                                    same arguments as to that of the print functions,
-
-                                    message_verbosity	:	int
-
-                                    print_verbosity		:	int
-
-                                    log_verbosity		:	int
-
-                                    ``**kwargs``		:	keyword arguments
-                                                                                    Same as that of the print function.
+    ``*args` : non-keyword arguments
+               same arguments as to that of the print functions,
+    message_verbosity : int
+    print_verbosity : int
+    log_verbosity : int
+    ``**kwargs`` : keyword arguments
+                   Same as that of the print function.
 
     Returns
     -------
-
-                                    1					:	int
-                                                                                    messages to stdout and logging of messages,
-                                                                                    while the function returns 1.
+    1 : int
+        messages to stdout and logging of messages,
+        while the function returns 1.
     """
 
     # If message verbosity matches the global verbosity level, then print
     if message_verbosity <= print_verbosity:
         print(*args, **kwargs)
     if log_verbosity <= message_verbosity:
         now = str(datetime.datetime.now())
@@ -95,89 +94,66 @@
             os.mkdir("logs")
 
         with open("logs/" + tstamp + ".log", "a") as log_file:
             if message_verbosity == -1:
                 for line in traceback.format_stack():
                     log_file.write(line.strip())
             log_file.write("\n")
-            log_file.write("{}:{}\t{}".format(caller.filename, caller.lineno, *args))
+            log_file.write(
+                "{}:{}\t{}".format(caller.filename, caller.lineno, *args)
+            )
             log_file.write("\n")
     return 1
 
 
 def mode(a_list):
     """Find the mode of a list
 
     Parameters
     ----------
-    a_list: list
-                    The list whose mode is to be found
+    a_list : list
+             The list whose mode is to be found
 
     Returns
     -------
-    list_mode:	float
-                            The mode of the list.
-
+    list_mode : float
+                The mode of the list.
     """
 
     a_list = list(a_list)
 
     return max(set(a_list), key=a_list.count)
 
 
-##########################################################################
-""" Data handling functions """
-##########################################################################
-""" This library consists of a bunch of functions that were frequently used
- for handling NR data. """
-""" Notes
-1. Some functions here display plots. If you intend to use these on the
-cluster and if xterm is not adequately setup, you may have to
-either comment the plot codes or use the`Agg` mode for plotting
-and save the figures instead of showing by changing the appropriate
-lines in the code.
-
-2. These is a module consisting of functions, not completely optimized
-for speed. This will happen in future.
-3. These functions are not defined in classes as they mostly use and
-operate on the objects of pycbc's builtin classes.
-4. Any suggestions, comments, critisism invited to vaishak@gmail.com!"""
-
-# Data I/O functions
-
-
 def save_obj(obj, name, obj_dir="./", protocol=pickle.HIGHEST_PROTOCOL):
     """A function to save python objects to disk using pickle.
 
     Parameters
     ----------
-
-    obj						:	object
-                                                                                                                    The python object to be saved.
-    name					:	string
-                                                                                                                    The filename.
-    obj_dir					:	string
-                                                                                                                    The path to directory to be saved in. Defaults to PWD
-    protocol				:	int
-                                                                                                                    The protocol to be used to save. Default is binary.
+    obj : object
+          The python object to be saved.
+    name : string
+           The filename.
+    obj_dir : string
+              The path to directory to be saved in. Defaults to PWD
+    protocol : int
+               The protocol to be used to save. Default is binary.
 
     Notes
     -----
     Protocols:
 
-    0						: Text
-    5						: Binary
+    * 0 : Text
+    * 5 : Binary
 
     See the man page of pickle for more details.
 
     Returns
     -------
-
     Nothing (other than saving the data to the disk).
-
     """
 
     # Create the directory dir if it doesn't exist.
     if not os.path.isdir(obj_dir):
         os.mkdir(obj_dir)
 
     # Pickle the file to disk.
@@ -187,51 +163,47 @@
 
 def load_obj(name, obj_dir="./"):
     """A function to load python objects from the disk using pickle.
 
     Parameters
     ----------
 
-    name:	string
-                                                                    The filename.
-    obj_dir :	string
-                                                                                                    The path to directory in which file exists. Defaults to PWD.
+    name : string
+           The filename.
+    obj_dir : string
+              The path to directory in which file exists. Defaults to PWD.
 
     Returns
     -------
-
-    obj:	object
-                                                                    A python object with the contents of the file.
+    obj : object
+          A python object with the contents of the file.
     """
 
     # Load the pickled data
     with open(obj_dir + name + ".pkl", "rb") as data_file:
         return pickle.load(data_file)
 
 
 def removeNans(xdata, ydata):
     """Remove Nans from (xdata,ydata) data pair.
     Removes Nans in xdata and ydata and the
     corresponding y and x entries.
 
     Parameters
     ----------
-
-    xdata:	1d array
-                                    The x axis of the data.
+    xdata : 1d array
+            The x axis of the data.
     ydata : 1d array
-                                    The y axis of the data.
+            The y axis of the data.
 
     Returns
     -------
-
-    x_no_nan:	1d array
-    y_no_nan:	1d,array
-                                    The data pair x,y with Nans removed.
-
+    x_no_nan : 1d array
+    y_no_nan : 1d array
+               The data pair x,y with Nans removed.
     """
 
     # Find the location of x Nans to be removed.
     nan_locs = np.where(np.isnan(xdata))[0]
     # Remove the xdata and the corresponding y entries.
     xdata = np.delete(xdata, nan_locs)
     ydata = np.delete(ydata, nan_locs)
@@ -256,78 +228,83 @@
 
 
 def differentiate(data, delta_t=None, TS=False):
     """Differentiate a timeseries in time domain using the Simple Euler method
 
     Parameters
     ----------
-    data:	1d array \\ a pycbc TimeSeries object
-                                                                    The time series to be differentiated.
-    delta_t:	float
-                            The grid spacing delta_t.
-                            Supplying delta_t overrides
-                            the delta_t attribute of TimeSeries.
+    data : 1d array
+           a pycbc TimeSeries object
+           The time series to be differentiated.
+    delta_t : float
+              The grid spacing delta_t.
+              Supplying delta_t overrides
+              the delta_t attribute of TimeSeries.
 
     Returns
     -------
-    ddt_data:	pycbc TimeSeries object
-                            The differentiated 1d data
-                            as pycbc TimeSeries"""
+    ddt_data : pycbc TimeSeries object
+               The differentiated 1d data
+               as pycbc TimeSeries"""
 
     if not delta_t:
         try:
             delta_t = data.delta_t
         except BaseException:
-            message("Input is not a TimeSeries. Please supply gridspacing as delta_t", message_verbosity=0)
+            message(
+                "Input is not a TimeSeries. Please supply gridspacing as delta_t",
+                message_verbosity=0,
+            )
 
     dydx = np.diff((np.array(data))) / delta_t
 
     if TS is True:
         dydx = pycbc.types.timeseries.TimeSeries(dydx, delta_t)
 
     return dydx
 
 
-def integrate_first_order(data, t_start=None, t_end=None, delta_t=None, to_taper=False, TS=False):
+def integrate_first_order(
+    data, t_start=None, t_end=None, delta_t=None, to_taper=False, TS=False
+):
     """Integrate a timeseries using first order method.
 
     Notes
     -----
-    Capabilities
-
-    Simple Euler integrator, option to taper the ends.
+    Capabilities:
+        Simple Euler integrator, option to taper the ends.
 
     Parameters
     ----------
-
-    data:	1d array or a pycbc TimeSeries object
-                    The input function to be integrated.
-    delta_t:	float
-                            The grid spacing delta_t,
-    to_taper:	bool
-                            True or False. Whether or not
-                            to taper the input series.
+    data : 1d array or a pycbc TimeSeries object
+           The input function to be integrated.
+    delta_t : float
+              The grid spacing delta_t,
+    to_taper : bool
+               True or False. Whether or not
+               to taper the input series.
 
     Returns
     -------
-
-    int_data:	a pycbc TimeSeries object
-                            TimeSeries of the time integrated data"""
+    int_data : a pycbc TimeSeries object
+               TimeSeries of the time integrated data"""
 
     # Check if object is pycbc timeseries. Recover delta_t, t_start, t_end if yes.
     if not delta_t:
         try:
             # Find sampling time_step
             delta_t = data.delta_t
             data_time = data.sample_times
             t_start_dat, t_end_dat = data_time[0], data_time[-1]
 
         except BaseException:
             message(
-                "Input is not a TimeSeries." "Please input a pycbc TimeSeries" "or supply gridspacing as delta_t",
+                "Input is not a TimeSeries."
+                "Please input a pycbc TimeSeries"
+                "or supply gridspacing as delta_t",
                 message_verbosity=0,
             )
     else:
         t_start_dat = 0
         t_end_dat = len(data) * delta_t
 
     if not t_start:
@@ -361,147 +338,134 @@
 
     data = np.array(data)
 
     for i in range(1, end_index - start_index):
         integdat[i] = integdat[i - 1] + (data[start_index + i - 1]) * delta_t
 
     if TS is True:
-        integdat = pycbc.types.timeseries.TimeSeries(integdat, delta_t, epoch=t_start)
+        integdat = pycbc.types.timeseries.TimeSeries(
+            integdat, delta_t, epoch=t_start
+        )
 
     return integdat
 
 
 def compute_frequencies(t_coal, t_val, chirp_mass):
     """Compute the Newtonian instantaneous frequency
     of strain waveform from coalescence time and
     chirp mass, from the Finn-Chernoff model.
 
     Parameters
     ----------
-
-    t_coal: float
-                                                    The coalescence time,
-    t_val:	1d array
-                                    The time,
-    chirp_mass: float
-                                                                    The chirpmass.
+    t_coal : float
+             The coalescence time,
+    t_val : 1d array
+            The time,
+    chirp_mass : float
+                 The chirpmass.
 
     Returns
     -------
-
-    freqs:	float
-                                    The instantaneous frequency of the strain waveform."""
-    freqs = (1.0 / (np.pi * chirp_mass)) * (5.0 / 256) ** (3.0 / 8) * (chirp_mass / (t_coal - t_val)) ** (3.0 / 8)
+    freqs : float
+            The instantaneous frequency of the strain waveform."""
+    freqs = (
+        (1.0 / (np.pi * chirp_mass))
+        * (5.0 / 256) ** (3.0 / 8)
+        * (chirp_mass / (t_coal - t_val)) ** (3.0 / 8)
+    )
 
     return freqs
 
 
 def totalmass(mass_ratio, chirp_mass):
     """Find total mass from mass ratio and chirpmass.
 
     Parameters
     ----------
-
-    mass_ratio: float
-                                                                    The mass ratio of the system.
-    mchirp: float
-                                                    The chirp mass of the system.
+    mass_ratio : float
+                 The mass ratio of the system.
+    mchirp : float
+             The chirp mass of the system.
 
     Returns
     -------
+    total_mass : float
+                 The total mass of the system.
+    """
 
-    total_mass: float
-                                                                    The total mass of the system."""
-
-    return (chirp_mass * (1.0 + mass_ratio) ** (6.0 / 5)) / mass_ratio ** (3.0 / 5)
+    return (chirp_mass * (1.0 + mass_ratio) ** (6.0 / 5)) / mass_ratio ** (
+        3.0 / 5
+    )
 
 
 def massratio(chirp_mass):
     """Compute the mass ratio from chirpmass. Assumes total mass to be 1.
 
     Parameters
     ----------
-
-    mchirp: float
-                                                    The chirp mass of the system.
+    mchirp : float
+             The chirp mass of the system.
 
     Returns
     -------
-
-    mass_ratio: float
-                                                                    The Mass ratio of the system
+    mass_ratio : float
+                 The Mass ratio of the system
     """
     mass_ratio = (
-        chirp_mass ** (1.0 / 3) - 2.0 * chirp_mass**2.0 - np.sqrt(chirp_mass ** (2.0 / 3) - 4.0 * chirp_mass ** (7.0 / 3))
+        chirp_mass ** (1.0 / 3)
+        - 2.0 * chirp_mass**2.0
+        - np.sqrt(chirp_mass ** (2.0 / 3) - 4.0 * chirp_mass ** (7.0 / 3))
     ) / (2.0 * chirp_mass**2.0)
 
     return mass_ratio
 
 
-# Defining function for calculating Chirpmass from a2
-
-
 def compute_chirp_mass(a2_param):
     """Compute the chirpmass from a2, the coefficient of time of the Finn-Chernoff waform model.
 
     Parameters
     ----------
-
-    a2_param:	1d array \\ float
-                                                    The a2 parameter in the Finn Chernoff model.
+    a2_param : 1d array or float
+               The a2 parameter in the Finn Chernoff model.
 
     Returns
     -------
-
-    chirp_mass: float
-                                                                    The chirp mass
+    chirp_mass : float
+                 The chirp mass
     """
     chirp_mass = 2 ** (8.0 / 5) / (5 * np.array(a2_param) ** (8.0 / 5))
     return chirp_mass
 
 
 def lengtheq(data_a, data_b, delta_t=None, is_ts=False):
     """Equalize the length of two timeseries/array by
     appending zeros at the end of the array. No tapering.
 
-    Procedure
-    ---------
-
-    1. Check if input data are timeseries.
-       If not then construct timeseries using delta_t.
-    2. Check data length.
-       If they are already equal then skip and return the inputs.
-    3. Check if data_a is smaller then data_b ( or vice versa).
-       Then augment zeroes at either ends of array to data_a
-       (data_b) and return.
-
-
     Parameters
     ----------
-    data_a: list
-                                                    The input waveform A
-    data_b: list
-                                                    The input waveform B.
-    delta_t:	float
-                                                    The time steping. Defaults to `None`.
-    is_ts:	bool
-                    To determine whether the given data
-                    is a pycbc TimeSeries.
+    data_a : list
+             The input waveform A
+    data_b : list
+             The input waveform B.
+    delta_t : float
+              The time steping. Defaults to `None`.
+    is_ts : bool
+            To determine whether the given data
+            is a pycbc TimeSeries.
     Returns
     -------
-
     equalized_signals : list
-                                            The Tapered, length equalized waveforms data_a and data_b,
-                                            and a flag denoting which waveform was changed, `a` or `b`.
+                        The Tapered, length equalized waveforms data_a and data_b,
+                        and a flag denoting which waveform was changed, `a` or `b`.
 
     Notes
     -----
-    Recommended usage:
+    Recommended usage :
 
-    Change length of waveform `a` to match with that of waveform `b`.
+            Change length of waveform `a` to match with that of waveform `b`.
 
     """
 
     # Check if input data vectors are pycbc TimeSeries. If yes, create a copy
     # of data and extract delta_t.
     # ts = isinstance(data_a, pycbc.types.timeseries.Timeseries)
     # and isinstance(data_b, pycbc.types.timeseries.Timeseries)
@@ -541,24 +505,32 @@
         lflag = "ab"
 
     # If data_a < data_b
     elif len(data_a) < len(data_b):
         # add zeros to data_a when a is smaller
         lflag = "a"
         zers = len(data_b) - len(data_a)
-        signala = np.transpose(np.concatenate((np.transpose(data_a), np.transpose(np.zeros([zers])))))
+        signala = np.transpose(
+            np.concatenate(
+                (np.transpose(data_a), np.transpose(np.zeros([zers])))
+            )
+        )
         # signala = pycbc.types.timeseries.TimeSeries(signala, delta_t)
         # return pycbc.types.timeseries.TimeSeries(signalb,delta_t),lflag
     # If data_b < data_a
     else:
         # message("Error!")
         # add zeros to b when b is smaller
         lflag = "b"
         zers = len(data_a) - len(data_b)
-        signalb = np.transpose(np.concatenate((np.transpose(data_b), np.transpose(np.zeros([zers])))))
+        signalb = np.transpose(
+            np.concatenate(
+                (np.transpose(data_b), np.transpose(np.zeros([zers])))
+            )
+        )
         # signalb = pycbc.types.timeseries.TimeSeries(signalb, delta_t)
         # return pycbc.types.timeseries.TimeSeries(signala,delta_t),lflag
 
     # Returns a list containing the length equalized arrays and the flag.
     if not is_ts:
         signala = np.array(signala)
         signalb = np.array(signalb)
@@ -567,29 +539,27 @@
 
 
 def taperlengtheq(data_a, data_b, delta_t=None):
     """Taper and equalize the lengths of two arrays.
 
     Parameters
     ----------
-
-    data_a: list
-                                                                                                    The input waveform A.
-    data_b: list
-                                                                                                    The input waveform B.
-    delta_t:	float
-                                                                    The time steping.
+    data_a : list
+             The input waveform A.
+    data_b : list
+             The input waveform B.
+    delta_t : float
+              The time steping.
 
     Returns
     -------
-
-    equalized_signals:	list
-                                            The Tapered, length equalized waveforms
-                                            data_a and data_b, and a flag denoting
-                                            which waveform was changed, `a` or `b`.
+    equalized_signals : list
+                        The Tapered, length equalized waveforms
+                        data_a and data_b, and a flag denoting
+                        which waveform was changed, `a` or `b`.
     """
 
     # Check if input data is pycbc TimeSeries. If yes, then ectract delta_t.
     if not delta_t:
         signala = data_a
         signalb = data_b
 
@@ -597,532 +567,324 @@
             delta_t = signala.delta_t
 
         except AttributeError:
             try:
                 delta_t = signalb.delta_t
             except BaseException:
                 message(
-                    "Input is not a TimeSeries." "Please supply a pycbc TimeSeries object " "or the gridspacing as delta_t",
+                    "Input is not a TimeSeries."
+                    "Please supply a pycbc TimeSeries object "
+                    "or the gridspacing as delta_t",
                     message_verbosity=0,
                 )
 
     # Ensure data is numpy array.
     signalb = np.array(data_b)
     # Taper waveform A.
     signala = np.array(taper(data_a, delta_t))
 
     # equalize the length of a to match with b and return the length equalized
     # arrays.
     return lengtheq(signala, signalb, delta_t)
 
 
-# Check data for discontinuity
-
-
-def iscontinuous_old(timeaxis, delta_t=0):
+def iscontinuous(time_axis, delta_t=None, toldt=1e-3):
     """Check if the data has discontinuities. This checks for repetitive time rows and jumps.
 
     Notes
     -----
     Types of discontunuities
 
     0: Continuous.
     1: Repetitive rows.
     2: Jumps in timeaxis.
 
     Parameters
     ----------
-
-    timeaxis:	list
-                            Input as a single 1d time axis
-                            or a list of 1d arrays [time, data1, data2, ...].
-                            All the data share the common time axis `time`
-    delta_t:	float
-                            The time stepping.
+    data : list
+           Input as a list of 1d arrays [time, data1, data2, ...].
+           All the data share the common time axis `time`
+    delta_t : float
+              The time stepping.
     toldt : float
-                    The tolerance for error in checking.
-                    Defaluts to toldt=1e-3.
+            The tolerance for error in checking. defaluts to toldt=1e-3.
 
     Returns
     -------
+    discontinuity_details : dict.
+                            It contains a dict of the details
+                            of discontinuity type. For each
+                            discontinuity type:
+                                1. Repetitiion
+                                2. Jumps
+                            It contains a list whose elements
+                            are
+                                1. a flag denoting if the discontinuity
+                                   of the given type exists (1).
+                                2. index locations of discontinuities
+                                    in the original array.
+    """
 
-    discontinuity_details : a list.
-                                                    It contains: [ the actual location of discontinuity along
-                                                    the time axis,
-                                                    value of time location of original array,
-                                                    the type of discontinuity].
+    time_axis = np.sort(time_axis)
 
-    """
+    dt_axis = np.diff(time_axis)
 
-    # If data array is supplied, assign first column as timeaxis
-    if np.array(timeaxis).ndim > 1:
-        timeaxis = timeaxis[:, 0]
-    # Check data for continuity.
-    # If not timeseries
-    if delta_t == 0:
-        delta_t = timeaxis[1] - timeaxis[0]
-    # Set epoch to first element of timeaxis
-    epoch = timeaxis[0]
-    # List to hold discintinuity details
-    discontinuity_details = []
-    # List to hold indices
-    # indices = []
-    # Set start index,epoch_index to 0
-    # index = 0
-    epoch_index = 0
-    # List to hold discontinuity type
-    discontinuity_type = []
-
-    for timestamp in timeaxis:
-        # Iterate over every timestamp in timeaxis
-        # Check for discontinuity
-        if timestamp != timeaxis[0] + epoch_index * delta_t:
-            # Check for type of discontinuity
-            # Repetitive rows
-            if timestamp < timeaxis[0] + epoch_index * delta_t:
-                discontinuity_type = 1
-            # Missing rows
-            elif epoch > timeaxis[0] + epoch_index + delta_t:
-                discontinuity_type = 2
-            # Append [index location,correct timestamp
-            discontinuity_details.append([epoch_index, timeaxis[epoch_index], discontinuity_type])
-        epoch_index += 1
-        # message("Progress: %f%%\r"%(epoch_index*100./len(timeaxis)))
-
-    # Print the result
-    # changed discontinuity_timestamps to discontinuity details May 5 2022
-    if len(discontinuity_details) != 0:
-        message("The data is discontinuous!")
-    else:
-        message("The data is continuous!")
-    # Return the details of discontinuity
-    return discontinuity_details
+    if not delta_t:
+        from scipy.stats import mode
 
+        delta_t = mode(dt_axis)[0][0]
 
-# Check data for discontinuity
+    discontinuity_type = 0
+    discontinuity_dict = {}
+    discont_locs = None
 
+    if ((dt_axis - delta_t) > (toldt) * delta_t).any():
+        discont_locs = np.where((dt_axis - delta_t) > (toldt) * delta_t)[0]
+        discontinuity_type = 1
 
-def iscontinuous(data, delta_t=0, toldt=1e-3):
-    """Check if the data has discontinuities. This checks for repetitive time rows and jumps.
+    discontinuity_dict.update({"gaps": [discontinuity_type, discont_locs]})
 
-    Notes
-    -----
-    Types of discontunuities
+    discontinuity_type = 0
+
+    rep_locs = None
+    if ((dt_axis - delta_t) < -toldt * delta_t).any():
+        rep_locs = np.where((dt_axis - delta_t) < -(toldt) * delta_t)[0]
+        discontinuity_type = 1
+
+    discontinuity_dict.update({"repetitions": [discontinuity_type, rep_locs]})
+
+    return discontinuity_dict
 
-    0: Continuous.
-    1: Repetitive rows.
-    2: Jumps in timeaxis.
+
+def sort_data(data):
+    """Sort the data according to its
+    time axis. The first axis is assumend to be
+    the time axis.
 
     Parameters
     ----------
-
-    data:	list
-                                                                    Input as a list of 1d arrays [time, data1, data2, ...].
-                                                                    All the data share the common time axis `time`
-    delta_t:	float
-                                                                    The time stepping.
-    toldt : float
-                                                                    The tolerance for error in checking. defaluts to toldt=1e-3.
+    data : ndarray
+           The data array with shape (naxis, time_steps)
+           The first axis is assumed to be the time axis.
 
     Returns
     -------
-
-    discontinuity_details:	a list.
-                                                    It contains:
-                                                    1. A list. details of discontinuity:  index location of original array,
-                                                                                                                            the corresponding discinbtinuity type.
-                                                    2. A float. the global discontinuity type.
+    sorted_data : ndarray
+                  The sorted data array
     """
 
-    # Check the data (time,datar,datai) for locations of repetition and
-    # discontinuities.
-    message("Checking continuity of data", message_verbosity=1)
-    # Ensure data as numpy array
     data = np.array(data)
-    message("Data shape:", (data.shape), message_verbosity=3)
-    # Find if data contanins more than timeaxis
+
+    # message("Data shape:", (data.shape), message_verbosity=3)
+    # Set axis along which to remove
     axis = data.ndim - 1
     message("Axis:%d" % axis, message_verbosity=3)
+
     # Associate data[0] as timeaxis
     if axis > 0:
         shapes = data.shape
         if shapes[0] > shapes[1]:
             data = np.transpose(data)
-        timeaxis = data[0, :]
-        message("The time axis is :%s" % timeaxis, message_verbosity=3)
+        time = data[0, :]
+        message("The time array:%s" % time, message_verbosity=3)
     else:
-        timeaxis = data
-    message("shape of data:", (data.shape), message_verbosity=3)
-
-    # If data array is supplied, assign first column as timeaxis
-    # if np.array(timeaxis).ndim>1:
-    # 		 timeaxis=np.array([item[0] for item in timeaxis])
-    # message('Timeaxis`,timeaxis,message_verbosity=3)
-    # Check data for continuity.
-    # If delta_t is not supplied
-    if delta_t == 0:
-        # delta_t = statistics.mode(np.diff(timeaxis))
-        delta_t = mode(np.diff(timeaxis))
-
-    # Set epoch to first element of timeaxis
-    epoch = timeaxis[0]
-    # List to hold discintinuity details
-    discontinuity_details = []
-    # List to hold indices
-    # indices = []
-    # Initialize start index,epoch_index to 0
-    index = 0
-    # Initialize epoch to start of timeaxis
-    epoch = timeaxis[0]
-    # Initialize epoch_index to 0
-    epoch_index = 0
-    # Repetition flag
-    repetition = 0
-    # Discountinuity flag
-    discont = 0
-    # Discontinuity type
-    discont_type = 0
-    # List to hold discontinuity type
-    discont_type_details = []
-    # Counters
-    repetition_counter = 0
-    discont_counter = 0
-    # Iterate over every timestamp in timeaxis.
-    # Note the type of discontinuity.
-    # Ignore repetition and check for actual discontinuity i.e. missing rows.
-
-    while index < len(timeaxis):
-        # Read original timestamp at the location of operation number
-        original_timestamp = timeaxis[index]
-        # Calculate the recentered timestamp starting at epoch where previous
-        # discontinuity was found.
-        recentered_timestamp = epoch + (index - epoch_index) * delta_t
-        # message(original_timestamp,recentered_timestamp)
-        # Check for next discontinuity
-        if abs(original_timestamp - recentered_timestamp) >= toldt * delta_t:
-            # Reset epoch, epoch_index
-            epoch = original_timestamp
-            epoch_index = index
-            # Check for type of discontinuity
-            # Repetitive rows
-            if (original_timestamp == recentered_timestamp) or (
-                recentered_timestamp - original_timestamp
-            ) >= toldt * delta_t:
-                # if recentered_timestamp-original_timestamp<=0.01*delta_t:
-                # 		 message("Error!!",message_verbosity=0)
-                repetition = 1
-                discont_type = repetition
-                message(
-                    "Repetitive rows found at index: %d,timestamp: %f" % (index, original_timestamp),
-                    message_verbosity=3,
-                )
-                message(
-                    "Repetition at timestamp original: %f correct %f\n" % (original_timestamp, recentered_timestamp),
-                    message_verbosity=3,
-                )
-                repetition_counter += 1
-            # Missing rows
-            if (original_timestamp - recentered_timestamp) >= (1.0 + toldt) * delta_t:
-                discont = 2
-                discont_type = discont
-                message(
-                    "Jump discountinuity in data found at index:%d,timestamp:%f" % (index, original_timestamp),
-                    message_verbosity=2,
-                )
-                message("delta_t=%f" % delta_t, message_verbosity=1)
-                message(
-                    "Jump at timestamp original: %f correct %f\n Dt = %f"
-                    % (original_timestamp, recentered_timestamp, (original_timestamp - recentered_timestamp) / delta_t),
-                    message_verbosity=1,
-                )
-                discont_counter += 1
-            # message("timei: %f timef %f\n"%(timeaxis[index-1],timeaxis[index]),message_verbosity=3)
+        time = data
 
-            # discont_type=repetition+discont
-            discont_type_details.append([index, discont_type])
-            # Append [index location,recentered timestamp
-            # discontinuity_details.append([index,recentered_timestamp,discontinuity_type])
-        # Increment the no. of total operations
-        index += 1
-        # message("Progress: %f%%\r"%(epoch_index*100./len(timeaxis)))
-    # discont_type=(repetition+discont)
-    # Print the result
-    if discont_type:
-        message("The data is not clean!", message_verbosity=1)
-        global_discont_type = repetition + discont
-        message("Discontinuity type:", global_discont_type, message_verbosity=1)
-        if global_discont_type == 1:
-            message("The data has repetitive rows at %d locations" % repetition_counter, message_verbosity=1)
-        elif global_discont_type == 2:
-            message("The data has %d discontinuities" % discont_counter, message_verbosity=1)
-        else:
-            message("The data has repetitive rows and is discontinious", message_verbosity=1)
+    order = np.argsort(time)
 
-        discontinuity_details = [discont_type_details, global_discont_type]
+    if axis > 0:
+        sorted_data = data[:, order]
     else:
-        message("Data is continuous", message_verbosity=2)
-        discontinuity_details = [[0, 0], 0]
-    # Return the details of discontinuity
-
-    return discontinuity_details
-
+        sorted_data = np.sort(time)
 
-# cleaning data for repeatative values
+    return sorted_data
 
+    return sorted_data
 
-def cleandata_old(data, verbose=False):
-    """Old version. Check the data (time,datar,datai) for repetetive rows and remove them.
+def remove_repetitive_rows(data, delta_t=1, toldt=1e-3):
+    """Remove repeated rows in the data
 
     Parameters
     ----------
+    data : ndarray
+           Data array where the first axis refers to different
+           columns of data. The zeroth column is time axis.
+           The second axis refers to entries at different time
+           steps.
 
-    data:	list
-                                                                    Input as a list of 1d arrays [time, data1, data2, ...].
-                                                                    All the data share the common time axis `time`
-    verbose : bool
-                                                                    A verbosity flag.
+    delta_t : float
+              The tim stepping.
+    toldt : float
+            The tolerance for error in checking. defaluts to toldt=1e-3.
 
     Returns
     -------
-
-    cleaned_data:	nd array
-                                    The cleaned data array with repetitive
-                                    rows and gaps (if bridge=True) removed
+    cleaned_data : list
+                   The cleaned data array with repetitive
+                   rows removed.
     """
+    message("Checking data for repetative rows...\n", message_verbosity=2)
+    data = sort_data(data)
 
-    # Ensure data as numpy array
-    data = np.array(data)
-    if verbose == "yes":
-        message("Data shape:", data.shape)
+    # message("Data shape:", (data.shape), message_verbosity=3)
     # Set axis along which to remove
     axis = data.ndim - 1
-    if verbose == "yes":
-        message("Axis:", axis)
+    message("Axis:%d" % axis, message_verbosity=3)
+
     # Associate data[0] as timeaxis
     if axis > 0:
         shapes = data.shape
         if shapes[0] > shapes[1]:
             data = np.transpose(data)
         time = data[0, :]
-        if verbose == "yes":
-            message("The time array:", time)
+        message("The time array:%s" % time, message_verbosity=3)
     else:
         time = data
-    # Assign delta_t
-    # delta_t = statistics.mode(np.diff(time))
-    delta_t = mode(np.diff(time))
 
-    if verbose:
-        message("length,shape of data", len(data), data.shape)
-    # Reassign data without time_array
-    # data=data[:,1:]
-    # message("++++++++++++++++++++++++++++++++++++++++++++++++++++++\n")
-    # message("Checking data for repetative rows...\n")
     # Index of ros to delete
     dind = []
-    # Initial data length
-    ki_index = len(time)
-    # message("length of old array is %d\n" %ki_index)
-    # Row iteration variable
-    ii_index = 0
-    # Flag to identify if any repetetive rows were found
-    rep_row_index = 0
-    # ci=0
-    # rowcounter=np.zeros([])
-    # Iterate over rows
-    while ii_index < ki_index - 1:
-        # Repetition condition :if the successive time stamp is less than or
-        # equal to the present, delete the row.
-        if (time[ii_index + 1] - time[ii_index]) <= -0.1 * delta_t:
-            # Set flag to 1 if repetition condition is met.
-            rep_row_index = 1
-            if verbose == "yes":
-                message("found a repeating row at %d, time %f\n" % (ii_index + 1, time[ii_index + 1]))
-                message("timei: %f timef %f\n" % (time[ii_index], time[ii_index + 1]))
-            # ci = ci+1
-            # Delete the entire row
-            time = np.delete(time, ii_index + 1)
-            # data = np.delete(data,ii_index,1)
-            # data = [np.delete(item,ii_index+1) for item in data]
-            data = np.delete(data, ii_index + 1, axis)
-            # Append the deleted index to the bookkeeping array
-            dind.append(ii_index + 1)
-            # If a row is deleted, step back the iter variable by one step
-            ii_index = ii_index - 1
-        # Advance the iter variable
-        ii_index = ii_index + 1
-        # Recalculate the array length
-        ki_index = len(time)
-    if verbose == "yes":
-        if rep_row_index == 1:
-            message("No. of points removed = %d\n" % len(dind))
-            message("length of new array is %d\n" % len(time))
-        else:
-            message("No points removed\n")
-        # message("++++++++++++++++++++++++++++++++++++++++++++++++++++++\n")
+
+    discontinuities = iscontinuous_new(time)
+
+    repetition = bool(discontinuities["repetitions"][0])
+
+    if repetition:
+        rep_rows = discontinuities["repetitions"][1]
+
+        data = np.delete(data, rep_rows)
+
+    else:
+        message("No points removed\n", message_verbosity=2)
+
     # Return the "cleaned" data matrix
     cleaned_data = data
-    # cleaned_data=[time]
-    # for item in data:
-    # 	 cleaned_data.append(item)
-    # cleaned_data.append(item for item in data)
-    # Transpose the data back to original shape
-    if shapes[0] > shapes[1]:
-        cleaned_data = np.transpose(cleaned_data)
+
     return cleaned_data
 
 
-#################################################
-# cleaning data for repeatative values
-# ToDo: breakdown this function into sub methods
-#################################################
+def fill_gaps_in_data(data, k=5):
+    """Fill gaps in data by interpolation
+
+    Parameters
+    ----------
+    data : list
+           Input as a list of 1d arrays [time, data1, data2, ...].
+           All the data share the common time axis `time`
+    k : int, optional
+        The interpolation order. Defaults to 5
+
+    Returns
+    -------
+    cleaned_data : list
+                   The cleaned data array with repetitive
+                   rows and gaps (if bridge=True) removed.
+
+    See Also
+    --------
+    scipy.interpolate.InterpolatedUnivariateSpline
+    """
+
+    data = sort_data(data)
+    time = data[0]
+
+    s1, l = data.shape
+
+    from scipy.stats import mode
 
+    delta_t = mode(np.diff(time))[0][0]
 
-def cleandata(data, toldt=1e-3, bridge="no"):
+    discontinuities = iscontinuous_new(time)
+
+    gaps = bool(discontinuties["gaps"][0])
+
+    if gaps:
+        gap_rows = discontinuoties["gaps"][1]
+        message(
+            "The data will be interpolated to bridge the gaps",
+            message_verbosity=2,
+        )
+
+        # Interpolate the data to fill in the discontinuities
+        t_final = time[-1]
+        t_initial = time[0]
+
+        proper_timeaxis = np.arange(t_initial, t_final, delta_t)
+
+        interp_data = []
+        interp_data.append(proper_timeaxis)
+
+        from scipy.interpolate import (
+            InterpolatedUnivariateSpline as interpolator,
+        )
+
+        for index in range(1, s1):
+            interp_data.append(
+                interpolator(time, data[index, :], k=k)(proper_timeaxis)
+            )
+
+        cleaned_data = np.array(interp_data)
+        message("The data has been interpolated", message_verbosity=3)
+    else:
+        message("No jumps found in the data", message_verbosity=2)
+
+    return cleaned_data
+
+
+def cleandata(data, toldt=1e-3, bridge=False, k=5):
     """Check the data (time,datar,datai) for repetetive rows and remove them.
 
     Parameters
     ----------
-
-    data:	list
-                                                                    Input as a list of 1d arrays [time, data1, data2, ...].
-                                                                    All the data share the common time axis `time`
+    data : list
+           Input as a list of 1d arrays [time, data1, data2, ...].
+           All the data share the common time axis `time`
     toldt : float
-                                                                    The tolerance for error in checking. defaluts to toldt=1e-3.
+            The tolerance for error in checking. defaluts to toldt=1e-3.
     bridge : bool
-                                                                    A bridge flag to decide whether or not to interpolate and
-                                                                    resample to fill in jump discontinuities.
+             A bridge flag to decide whether or not to interpolate and
+             resample to fill in jump discontinuities.
+    k : int, optional
+        The interpolation order. Defaults to 5
 
     Returns
     -------
-
-    cleaned_data:	list
-                                    The cleaned data array with repetitive
-                                    rows and gaps (if bridge=True) removed.
-
+    cleaned_data : list
+                   The cleaned data array with repetitive
+                   rows and gaps (if bridge=True) removed.
     """
 
     # Check the data (time,datar,datai) for repetetive rows and remove them.
     # Ensure data as numpy array
     data = np.array(data)
-    message("Data shape:", (data.shape), message_verbosity=3)
+
+    # message("Data shape:", (data.shape), message_verbosity=3)
     # Set axis along which to remove
     axis = data.ndim - 1
     message("Axis:%d" % axis, message_verbosity=3)
 
     # Associate data[0] as timeaxis
     if axis > 0:
         shapes = data.shape
         if shapes[0] > shapes[1]:
             data = np.transpose(data)
         time = data[0, :]
         message("The time array:%s" % time, message_verbosity=3)
     else:
         time = data
 
+    time = np.sort(time)
     # delta_t = statistics.mode(np.diff(time))
     delta_t = mode(np.diff(time))
 
     message("shape of data:", (data.shape), message_verbosity=3)
 
-    # Reassign data without time_array
-    # data=data[:,1:]
-    # message("++++++++++++++++++++++++++++++++++++++++++++++++++++++\n")
-    # message("Checking data for repetative rows...\n")
-    # Index of ros to delete
-    dind = []
-
-    # Initial data length
-    ki_index = len(time)
-
-    # message("length of old array is %d\n" %ki)
-    # Row iteration variable
-    ii_index = 0
-
-    # Flag to identify if any repetetive rows were found
-    rep_row_index = 0
-
-    # ci=0
-    # rowcounter
-    counter = 0
-
-    # Iterate over rows
-    while ii_index < ki_index - 1:
-        # Repetition condition :if the successive time stamp is less than or
-        # equal to the present, delete the row.
-        if (time[ii_index + 1] == time[ii_index]) or (time[ii_index] - time[ii_index + 1]) >= toldt * delta_t:
-            # if time[ii_index]-time[ii_index+1]<=0.01*delta_t:
-            # 		 message("Error!!",message_verbosity=0)
-            # Set flag to 1 if repetition condition is met.
-            rep_row_index = 1
-            counter += 1
-            message("found a repeating row at %d, time %f\n" % (ii_index + 1, time[ii_index + 1]), message_verbosity=3)
-            message("timei: %f timef %f\n" % (time[ii_index], time[ii_index + 1]), message_verbosity=3)
-            # ci = ci+1
-            # Delete the entire row
-            time = np.delete(time, ii_index + 1, 0)
-            # data = np.delete(data,ii_index,1)
-            # data = [np.delete(item,ii_index+1) for item in data]
-            data = np.delete(data, ii_index + 1, axis)
-            # Append the deleted index to the bookkeeping array
-            dind.append(ii_index + 1)
-            # If a row is deleted, step back the iter variable by one step
-            ii_index = ii_index - 1
-        # Advance the iter variable
-        ii_index = ii_index + 1
-        # Recalculate the array length
-        ki_index = len(time)
-
-    if rep_row_index == 1:
-        message("Repetitive rows were removed", message_verbosity=2)
-        message("No. of rows removed = %d\n" % counter, message_verbosity=2)
-        message("Length of new array is %d\n" % len(time), message_verbosity=3)
-
-    else:
-        message("No points removed\n", message_verbosity=2)
-        # message("++++++++++++++++++++++++++++++++++++++++++++++++++++++\n")
-    # Return the "cleaned" data matrix
-    cleaned_data = data
-
-    if bridge and iscontinuous(cleaned_data)[-1] >= 2:
-        message("The data will be interpolated to bridge the gaps", message_verbosity=2)
-
-        # from scipy import interpolate
-
-        # Interpolate the data to fill in the discontinuities
-        t_final = time[-1]
-        t_initial = time[0]
-
-        # Find delta_t
-        delta_t = time[1] - time[0]
-        index = 1
-
-        # If second row is repetitive (If its discontinuous, help!)
-        while delta_t <= 0:
-            delta_t = np.diff(time)[index]
-            index += 1
-        proper_timeaxis = np.arange(t_initial, t_final, delta_t)
-        interp_data = []
-        interp_data.append(proper_timeaxis)
-        if axis > 0:
-            from scipy.interpolate import interp1d
-
-            for index in range(1, min(shapes[0], shapes[1])):
-                interp_datai = interp1d(time, data[index, :])
-                interp_data.append(interp_datai(proper_timeaxis))
-
-        cleaned_data = np.array(interp_data)
-        message("The data has been interpolated", message_verbosity=2)
-    message("Cleaned!", message_verbosity=2)
+    cleaned_data = remove_repetitive_rows(data, delta_t=delta_t, toldt=toldt)
 
-    # cleaned_data=[time]
-    # for item in data:
-    # 	 cleaned_data.append(item)
-    # cleaned_data.append(item for item in data)
-    # Transpose the data back to original shape
+    if bridge:
+        cleaned_data = fill_gaps_in_data(cleaned_data, k=k)
 
     if axis > 0:
         if shapes[0] > shapes[1]:
             cleaned_data = np.transpose(cleaned_data)
     return cleaned_data
 
 
@@ -1130,56 +892,63 @@
     """Timeshift an array. IMP: After timeshifting, the original
     length of the array is retained by clipping last(first) when
     ind > 0(ind <0) `ind` number of points!!. Make sure the input array
     already has number of zeros z > ind (z<ind) initially at the end.
 
     Parameters
     ----------
-    hdat:	1d array or a pycbc TimeSeries object
-                                                                    The input waveform to be shifted in time.
-    ind:	int
-                                                                    The numper of places to shift the input waveform.
-    delta_t:	int
-                                                                    the grid spacing in time.
+    hdat : 1d array or a pycbc TimeSeries object
+           The input waveform to be shifted in time.
+    ind : int
+          The numper of places to shift the input waveform.
+    delta_t : int
+              the grid spacing in time.
 
     Returns
     -------
-    shifted_wf: a pycbc TimeSeries object
-                            The waveform array of same length timeshifted by
-                            `ind` units by prepending zeros.
+    shifted_wf : a pycbc TimeSeries object
+                 The waveform array of same length timeshifted by
+                 `ind` units by prepending zeros.
     """
 
     if is_ts:
         if not delta_t:
             try:
                 delta_t = hdat.delta_t
             except BaseException:
-                message("Input is not a TimeSeries. Please supply gridspacing as delta_t", message_verbosity=0)
+                message(
+                    "Input is not a TimeSeries. Please supply gridspacing as delta_t",
+                    message_verbosity=0,
+                )
 
     if ind > 0:
         # ind>0 case for shifting array to the right
         # message hdat
         # Length of the data
         # l = len(hdat)
         # Array holding zeroes to be appended
         zeros = np.zeros([ind])
         # The shifted array
-        shifted_wf = np.transpose(np.concatenate((np.transpose(zeros), np.transpose(hdat))))[:-ind]
+        shifted_wf = np.transpose(
+            np.concatenate((np.transpose(zeros), np.transpose(hdat)))
+        )[:-ind]
         # message msig
         # message msig[:-ind]
         # Return the clipped, shifted timeseries
 
     elif ind < 0:
         # ind <0 case for shifting array to the left
         # Length of the data
         # l = len(hdat)
         # Array holding zeroes to be appended
         zeros = np.zeros([ind])
         # The shifted array
-        shifted_wf = np.transpose(np.concatenate((np.transpose(hdat), np.transpose(zeros))))[ind:]
+        shifted_wf = np.transpose(
+            np.concatenate((np.transpose(hdat), np.transpose(zeros)))
+        )[ind:]
         # message msig
         # message msig[:-ind]
         # Return a timeseries
 
     else:
         shifted_wf = hdat
 
@@ -1193,21 +962,20 @@
 def unwrap_phase(phi0):
     """Unwrap the phase by finding turning points in phi0.
     Finding turning points for unwrapping arctan2 function
 
     Parameters
     ----------
     phi0 : 1darray
-               The wrapped phase which takes values in the
-               range (0, 2pi).
+           The wrapped phase which takes values in the
+           range (0, 2pi).
     Returns
     -------
     phic : 1darray
-               The unwrapped phase.
-
+           The unwrapped phase.
     """
 
     # Bookkeeping for upper (tpu) and lower (tpd) turning points
     tpu = []
     tpd = []
     # j = 0
     # k = 0
@@ -1249,38 +1017,36 @@
 
 # Complex Phase-Amplitude representation of data
 def xtract_cphase(tsdata_p, tsdata_x, delta_t=None, to_plot=False):
     """Given real and imaginary parts of a complex timeseries, extract the phase of the waveform :arctan_(Img(data)/Re(data))
 
     Parameters
     ----------
-    tsdata_p:	1d array / a pycbc TimeSeries
-    tsdata_x:	1d array / a pycbc TimeSeries
-                                                    The plus and cross polarized components of the waveforms.
-    delta_t:	float, optional
-                                                    The time step. Overrides the timestep from pycbc TS object if given.
-    to_plot:	bool, optional
-                                                                                                    True or False. Whether to plot the data or not
+    tsdata_p, tsdata_x : 1d array / a pycbc TimeSeries
+                         The plus and cross polarized components of the waveforms.
+    delta_t : float, optional
+              The time step. Overrides the timestep from pycbc TS object if given.
+    to_plot : bool, optional
+              True or False. Whether to plot the data or not
 
     Returns
     -------
-
-    phic:	1d array
-                                                                    The 1d array of the phase of the waveform.
+    phic : 1d array
+           The 1d array of the phase of the waveform.
     """
 
     # Assign the timestep. Real and imaginary parts are assumed to have same timestep.
     # if not delta_t:
-    # 	try:
-    # 		delta_t = tsdata_p.delta_t
-    # 	except AttributeError:
-    # 		try:
-    # 			delta_t = tsdata_x.delta_t
-    # 		except:
-    # 			message("Input is not a TimeSeries. Please supply gridspacing as delta_t", message_verbosity=0)
+    #   try:
+    #       delta_t = tsdata_p.delta_t
+    #   except AttributeError:
+    #       try:
+    #           delta_t = tsdata_x.delta_t
+    #       except:
+    #           message("Input is not a TimeSeries. Please supply gridspacing as delta_t", message_verbosity=0)
 
     # Assign the timestep. Real and imaginary parts are assumed to have same timestep.
     # Convert the data in numpy arrays
 
     datap = np.array(tsdata_p)
     datax = np.array(tsdata_x)
 
@@ -1315,30 +1081,29 @@
         plt.show()
         # Return a 1d list containing the unwrapped phase
     return phic
 
 
 def xtract_camp(tsdata_p, tsdata_x, to_plot=False):
     """Given real and imaginary parts of a complex timeseries,
-    extract the amplitude of the complex
-    data vector : (tsdata_p + i * tsdata_x)
+    extract the amplitude of the complex data vector
+    : (tsdata_p + i * tsdata_x)
 
     Parameters
     ----------
-    tsdata_p:	1d array / a pycbc TimeSeries
-    tsdata_x:	1d array / a pycbc TimeSeries
-                                                                                                    The plus and cross polarized components of the waveforms.
-    to_plot:	bool
-                                                                                                    True or False. Whether to plot the data or not
+    tsdata_p, tsdata_x : pycbc TimeSeries/1darray
+                         The plus and cross polarized components of the waveforms.
+    to_plot : bool
+              True or False. Whether to plot the data or not
 
     Returns
     -------
-
-    camp:	1d array
-                                                                    The 1d array of extracted amplitudes of the waveform."""
+    camp : 1d array
+           The 1d array of extracted amplitudes of the waveform.
+    """
 
     # Assign the timestep. Real and imaginary parts are assumed to have same timestep.
     # Complex modulous of the data
     camp = np.sqrt(np.array(tsdata_p) ** 2 + np.array(tsdata_x) ** 2)
 
     if to_plot:
         # Plot amplitude vs time
@@ -1354,86 +1119,70 @@
 
 
 def xtract_camp_phase(tsdata_1, tsdata_2):
     """Wrapper for extracting the amplitude and the phase of the complex vector.
 
     Parameters
     ----------
-
-    tsdata_1:	1d array or pycbc TimeSeries object
-    tsdata_2:	1d array or pycbc TimeSeries object
-                            The two input waveforms as timeseries
-                            vectors, the plus and cross polarized
-                            components.
-    delta_t:	float
-                                                                    The timestepping delta_t.
+    tsdata_1, tsdata_2 : 1d array or pycbc TimeSeries object
+                         The two input waveforms as timeseries
+                         vectors, the plus and cross polarized
+                         components.
+    delta_t : float
+              The timestepping delta_t.
 
     Returns
     -------
-
-    amplitude:	1d array
-                            A list containing complex amplitude
-                            (list) and phase (list).
+    amplitude : 1d array
+                A list containing complex amplitude
+                (list) and phase (list).
     """
 
     return xtract_camp(tsdata_1, tsdata_2), xtract_cphase(tsdata_1, tsdata_2)
 
 
-def get_waveform_angular_frequency(waveform, delta_t, timeaxis=None, method="FD"):
+def get_waveform_angular_frequency(
+    waveform, delta_t, timeaxis=None, method="FD"
+):
     """Get the angular frequency of the waveform given
     the complex waveform time step. The phase is
     extracted and is differentiated using one of
     the available methods to compute the angular
     frequency.
 
-
-
-
     Parameters
     ----------
-
-    waveform:		1d array
-                                                                    The 1d complex array of the input
-                                                                    waveform.
-
-    delta_t:	 float
-                                                     The time step.
-
-    timeaxis:	 1d array, optional
-                                                     The time axis of the waveform.
-                                                     Recommended especially when the sampling
-                                                     is non-uniform and Chebyshev method
-                                                     is chosen.
-    method: str
-                                                    The method for computing the derivative.
-                                                    Can be `FD` or `CS`. See below for more
-                                                    information.
+    waveform : 1d array
+               The 1d complex array of the input waveform.
+    delta_t : float
+              The time step.
+    timeaxis : 1d array, optional
+               The time axis of the waveform.
+               Recommended especially when the sampling
+               is non-uniform and Chebyshev method is chosen.
+    method : str
+             The method for computing the derivative.
+             Can be `FD` or `CS`. See below for more
+             information.
 
     Returns
     -------
-
-    omega:		1d array
-                                                    The real instantaneous frequency of the waveform.
-
-
+    omega : 1d array
+            The real instantaneous frequency of the waveform.
 
     Notes
     -----
-
     Available methods
 
-    Chebyshev series (`CS`):	The phase is expanded in
-                                                                                                                    a Chebyshev series and
-                                                                                                                    then the differentiated.
+    Chebyshev series (`CS`) : The phase is expanded in
+                              a Chebyshev series and
     Finite Differencing (`FD`) : A 11 point finite difference
-                                                                                                                     scheme is used to differentiate
-                                                                                                                     the phase, and is then smoothened
-                                                                                                                     using the Savgol filter.
-
-
+                                 scheme is used to differentiate
+                                 the phase, and is then smoothened
+                                 using the Savgol filter.
     """
     # Get the real and imaginary parts.
     waveform_p = waveform.real
     waveform_x = waveform.imag
     # Get the phase
     phase = xtract_cphase(waveform_p, waveform_x)
     # Compute the derivative
@@ -1468,36 +1217,28 @@
 
 def get_starting_angular_frequency(waveform, delta_t, npoints=400):
     """Get the approximate starting frequency of the
     input data by averaging over the first `npoints` number of points.
 
     Parameters
     ----------
-
-    waveform:		1d array
-                                                                    The 1d complex array of the input
-                                                                    waveform.
-
-    delta_t:	 float
-                                                     The time step.
-
-
-    npoints:	 int
-                                                     The number of points to average over.
+    waveform : 1d array
+               The 1d complex array of the input waveform.
+    delta_t : float
+              The time step.
+    npoints : int
+              The number of points to average over.
 
     Returns
     -------
-
-    omega0: float
-                                                    The approximate starting angular frequency.
-
+    omega0 : float
+             The approximate starting angular frequency.
 
     Notes
     -----
-
     Please suppy a conditioned input waveform that is neatly clipped,
     and not tapered.
     """
 
     # Get angular frequencies
     omegas = get_waveform_angular_frequency(waveform, delta_t)
 
@@ -1509,27 +1250,23 @@
 
 # Simple overlap. #Error. Add frequency domain overlap computation.
 def olap(data1, data2, psd=1):
     """Calcuate the overlap between two data vectors weighted by the given psd.
 
     Parameters
     ----------
-
-    data1:	1d array or a pycbc TimeSeries object
-    data2 : 1d array or a pycbc RimeSeries object
-                                                                    The input waveforms
-    psd:	1d array
-                                                                    The power spectral density to weight.
+    data1, data2 : 1d array or a pycbc RimeSeries object
+                   The input waveforms
+    psd : 1d array
+          The power spectral density to weight.
 
     Returns
     -------
-
-    overlap:	float
-                                                                                                    The overlap divided by the psd.
-
+    overlap : float
+              The overlap divided by the psd.
     """
 
     if psd == 1:
         data1 = np.array(data1)
         data2 = np.array(data2)
         overlap = np.sum(data1 * data2) / psd
 
@@ -1540,25 +1277,23 @@
 
 
 def norm(hdat, psd=1.0):
     """Calculate the norm of a vector.
 
     Parameters
     ----------
-
-    hdat:	1d array or a pycbc TimeSeries object.
-                                                                    The input waveform.
-    psa:	1d array
-                                                                    The noise power spectral density of the inner product.
+    hdat : 1d array or a pycbc TimeSeries object.
+           The input waveform.
+    psa : 1d array
+          The noise power spectral density of the inner product.
 
     Returns
     -------
-
-    norm_f: float
-                                                                    The norm with weighting by the psd.
+    norm_f : float
+             The norm with weighting by the psd.
     """
 
     hdat = np.array(hdat)
 
     norm_f = np.sqrt(np.sum(hdat * hdat) / np.array(psd))
 
     # message("Norm is %f"%normfa)
@@ -1569,23 +1304,21 @@
     """Flatten a (3rd order) list of list of lists.
     i.e. a three tier list [[[],[]], [[],[]] ---> [].
     This is useful e.g. when combining the data from
     the list output of multiple MPI ranks.
 
     Parameters
     ----------
-
-    nflist: a third tier list
-                    A list of list of lists (a list of depth three).
+    nflist : a third tier list
+             A list of list of lists (a list of depth three).
 
     Returns
     -------
-
-    flattened_list: a list
-                                    The flattened list i.e. a tier one list.
+    flattened_list : a list
+                     The flattened list i.e. a tier one list.
     """
 
     flattened_list = []
 
     for item in nflist:
         for sub_item in item:
             flattened_list.append(sub_item)
@@ -1596,78 +1329,77 @@
 
 
 def startend(data):
     """Identify the start and endpoints of the data.
 
     Notes
     -----
-
     The starting and ending index of the non-zero part
     of the data is the identification criterion.
     Requires the data to be exactly zero outside
     a certain domain.
 
     Parameters
     ----------
-
-    data:	1d array or a pycbc TimeSeries object
-                                                                    The input waveform.
+    data : 1d array or a pycbc TimeSeries object
+           The input waveform.
 
     Returns
     -------
-
-    start_index, end_index: int (2)
-                                                    The pair of indices denoting
-                                                    the start and end points of an array
-
+    start_index, end_index : int (2)
+                             The pair of indices denoting the start
+                             and end points of an array
     """
 
     try:
         start_index = np.where(np.array(data) != 0)[0][0]
     except BaseException:
-        message(colored("Warning! Start index not found!!", "red"), message_verbosity=1)
+        message(
+            colored("Warning! Start index not found!!", "red"),
+            message_verbosity=1,
+        )
         start_index = 0
 
     try:
         end_index = np.where(np.array(data) != 0)[0][-1] + 1
     except BaseException:
-        message(colored("Warning! End index not found!!", "red"), message_verbosity=1)
+        message(
+            colored("Warning! End index not found!!", "red"),
+            message_verbosity=1,
+        )
         end_index = 0
     return start_index, end_index
 
 
 def apxstartend(data, tol=1e-5):
     """Identify the Approximate start and endpoints of the data.
 
     Notes
     -----
-
     The starting and ending index of the peak
-    tol (default 1e-5)	part of the data is
+    tol (default 1e-5)  part of the data is
     the identification criterion. Requires
     the data to fall off to tol*peak absolute
     value outside a certain range.
 
     Parameters
     ----------
-
-    data:	1d array or a pycbc TimeSeries object
-                    The input waveform whose start and
-                    end points need to be identified based
-                    on a given tolerance value.
-    tol:	float
-                    The tolerance value below which
-                    the signal is assumed to be absent.
+    data : 1d array or a pycbc TimeSeries object
+           The input waveform whose start and
+           end points need to be identified based
+           on a given tolerance value.
+    tol : float
+          The tolerance value below which
+          the signal is assumed to be absent.
 
     Returns
     --------
-
-    loc_pair:	int (2)
-                            The pair of indices denoting
-                            the start and end points of an array
+    loc_pair : int (2)
+               The pair of indices denoting
+               the start and end points of an array
     """
 
     data = np.array(data)
     locs = np.where(data > np.amax(data) * tol)[0]
 
     loc_pair = locs[0], locs[-1] + 1
 
@@ -1676,143 +1408,156 @@
 
 
 def addzeros(data, zeros):
     """Append zeros to an array without tapering.
 
     Parameters
     ----------
-
-    data	:	1d array or a pycbc TimeSeries
-                    The waveform data as list or numpy array or pycbc timeseries.
-
-    zeros	:	int
-                    The number of zeros to be added.
+    data : 1d array or a pycbc TimeSeries
+           The waveform data as list or numpy array or pycbc timeseries.
+    zeros : int
+            The number of zeros to be added.
 
     Returns
     -------
-
-    data with `zeros` number of zeros concatenated at the end as numpy 1d array :	trial
+    data : 1darray
+           data with `zeros` number of zeros concatenated
+           at the end as numpy 1d array
     """
 
-    return np.transpose(np.concatenate((np.transpose(np.array(data)), np.transpose(np.zeros([zeros])))))
+    return np.transpose(
+        np.concatenate(
+            (np.transpose(np.array(data)), np.transpose(np.zeros([zeros])))
+        )
+    )
 
 
 def removezeros(data, delta_t):
     """Remove zeros from the input waveform from either sides.
     Similar to startend but return the truncated array.
 
     Parameters
     ----------
-
-    data:	1d array or a pycbc TimeSeries
-                                                                    The input waveform.
-    delta_t:	float, optional
-                                                                    The time stepping.
+    data : 1d array or a pycbc TimeSeries
+           The input waveform.
+    delta_t : float, optional
+              The time stepping.
 
     Returns
     -------
-
-    short_ts:	a list
-                            A list containing  waveforms with zeros removed on either sides,
-                            the start and end indices in the format [short_ts, [start_index, end_index]]
+    short_ts : a list
+               A list containing waveforms with zeros
+               removed on either sides,
+               the start and end indices in the format [short_ts, [start_index, end_index]]
 
     """
 
     # Assign the timestep. Real and imaginary parts are assumed to have same
     # timestep.
     if not delta_t:
         try:
             delta_t = data.delta_t
         except BaseException:
-            message("Input is not a TimeSeries." " Please supply gridspacing as delta_t", message_verbosity=0)
+            message(
+                "Input is not a TimeSeries."
+                " Please supply gridspacing as delta_t",
+                message_verbosity=0,
+            )
 
     starti, endi = startend(data)
-    ret_data = pycbc.types.timeseries.TimeSeries(np.array(data)[starti:endi], delta_t)
+    ret_data = pycbc.types.timeseries.TimeSeries(
+        np.array(data)[starti:endi], delta_t
+    )
 
     short_ts = [ret_data, [starti, endi]]
 
     return short_ts
 
 
 def shorten(tsdata, start, end, delta_t=None):
     """Shorten an array given the start and end points.
 
     Parameters
     ----------
-
-    tsdata: 1d array or a pycbc TimeSeries object
-                                                                                                    The waveform data.
-    start:	int
-                                                                    The start index of the data.
-
-    end:	int
-                                                                    The end index of the data.
-    delta_t:	float, optional
-                                    The time stepping.
-
+    tsdata : 1d array or a pycbc TimeSeries object
+             The waveform data.
+    start : int
+            The start index of the data.
+    end : int
+          The end index of the data.
+    delta_t : float, optional
+              The time stepping.
 
     Returns
     -------
-
-    short_ts:	a pycbc TimeSeries object
-                                                                                                    The shortened data, clipped before start and after end.
+    short_ts : a pycbc TimeSeries object
+               The shortened data, clipped before start and after end.
     """
     # Assign the timestep.
     # Real and imaginary parts
     # are assumed to have same
 
     # timestep.
     if not delta_t:
         try:
             delta_t = tsdata.delta_t
         except BaseException:
-            message("Input is not a TimeSeries." "Please supply gridspacing as delta_t", message_verbosity=0)
+            message(
+                "Input is not a TimeSeries."
+                "Please supply gridspacing as delta_t",
+                message_verbosity=0,
+            )
 
-    short_ts = pycbc.types.timeseries.TimeSeries(np.array(tsdata)[start:end], delta_t)
+    short_ts = pycbc.types.timeseries.TimeSeries(
+        np.array(tsdata)[start:end], delta_t
+    )
 
     return short_ts
 
 
-def taper_tanh(waveform, time_axis=None, delta_t=None, duration=10, sides="both"):
+def taper_tanh(
+    waveform, time_axis=None, delta_t=None, duration=10, sides="both"
+):
     """
     Taper a waveform with a :math:`tanh` function
     at either ends
 
     Parameters
     ----------
-    waveform:	 1d array
-                             A 1d array of waveform data.
-    delta_t:	 float, optional
-                             The time stepping `delta_t`.
-                             Optional if `time_axis` is given.
-    percent:	 int, optional
-                             The percent of data to taper. This
-                             is equally distributed on either
-                             sides of the array. Defaults to 10.
-    sides:		 str
-                             A string indicating which sides to taper.
-                             `beg` tapers the beginning, `end` tapers the end
-                            and `both` tapers both the ends.
-    Returns
-    -------
-    time_axis, waveform:	1d array
-                                                    The timeaxis and the waveform data
-                                                    of the tapered waveform.
+    waveform : 1d array
+               A 1d array of waveform data.
+    delta_t : float, optional
+              The time stepping `delta_t`.
+              Optional if `time_axis` is given.
+    percent : int, optional
+              The percent of data to taper. This
+              is equally distributed on either
+              sides of the array. Defaults to 10.
+    sides : str
+            A string indicating which sides to taper.
+            `beg` tapers the beginning, `end` tapers the end
+            and `both` tapers both the ends.
+
+    Returns
+    -------
+    time_axis, waveform : 1d array
+                          The timeaxis and the waveform data
+                          of the tapered waveform.
     """
 
     data_len = len(waveform)
 
     if delta_t is None:
         try:
             delta_t = time_axis[1] - time_axis[0]
         except Exception as excep:
             delta_t = 1
             message("Assuming unity for time step", excep)
 
-    # 	 delta_t = 1
+    #    delta_t = 1
     if time_axis is None:
         # Try to construct using `delta_t`
         try:
             time_axis = np.arange(0, data_len * delta_t, delta_t)
             # message('time axis', time_axis)
         except Exception as excep:
             message("Please suppy the time axis or delta_t!", excep)
@@ -1828,71 +1573,76 @@
     nstart_points = data_delta_len - nend_points
 
     # message('N startend points', nend_points, nstart_points)
     # message('New time axis', new_time_axis)
     tfinal = data_len * delta_t
 
     # start_axis = np.linspace(-1, 1, nstart_points)
-    # end_axis	 = np.linspace(1, -1, nend_points)
+    # end_axis   = np.linspace(1, -1, nend_points)
 
     # norm_time_axis = time_axis/max(time_axis)
 
     # n_delta_t = delta_t/data_len
 
     # from scipy.interpolate import interpolate
-    waveform_widened = np.concatenate((np.zeros([nstart_points]), waveform, np.zeros([nend_points - 1])))
+    waveform_widened = np.concatenate(
+        (np.zeros([nstart_points]), waveform, np.zeros([nend_points - 1]))
+    )
     new_time_axis = np.linspace(
-        time_axis[0] - nstart_points * delta_t, time_axis[-1] + nend_points * delta_t, len(waveform_widened)
+        time_axis[0] - nstart_points * delta_t,
+        time_axis[-1] + nend_points * delta_t,
+        len(waveform_widened),
     )
 
-    start_win = (np.tanh(3 * (new_time_axis - duration / 2) / (duration / 2)) + 1) / 2
-    end_win = (np.tanh(3 * (-new_time_axis + (tfinal - duration / 2)) / (duration / 2)) + 1) / 2
+    start_win = (
+        np.tanh(3 * (new_time_axis - duration / 2) / (duration / 2)) + 1
+    ) / 2
+    end_win = (
+        np.tanh(3 * (-new_time_axis + (tfinal - duration / 2)) / (duration / 2))
+        + 1
+    ) / 2
 
     # plt.scatter(new_time_axis, waveform_widened, s=1)
     # plt.show()
 
     if sides == "both":
         tapered_waveform = start_win * end_win * waveform_widened
     elif sides == "beg":
         tapered_waveform = start_win * waveform_widened
     elif sides == "end":
         tapered_waveform = end_win * waveform_widened
     else:
-        message("Please specify valid sides argument. Sides can be beg, end or both.")
+        message(
+            "Please specify valid sides argument. Sides can be beg, end or both."
+        )
 
     # plt.scatter(new_time_axis, tapered_waveform, s=1)
     # plt.show()
 
     return new_time_axis, tapered_waveform
 
 
 def taper(data, delta_t=1, zeros=150):
     """A method to taper and append additional zeros
     at either ends, using the `taper` function of
     the pycbc TimeSeries object.
 
     Parameters
     ----------
-
-
-    data:	1d array or a pycbc TimeSeries
-                    The waveform data as list or numpy
-                    array or pycbc timeseries.
-    delta_t:	float
-                                                    The timestepping.
-    zeros:	int
-                                    The number of zeros to be added.
+    data : 1d array or a pycbc TimeSeries
+           The waveform data
+    delta_t : float
+              The timestepping.
+    zeros : int
+            The number of zeros to be added.
 
     Returns
     -------
-
-    tapered_data:	1d array or a pycbc TimeSeries object
-                                    The waveform data tapered and zero padded.
-                                    Returns a pycbc TimeSeries object.
-
+    tapered_data : 1d array or a pycbc TimeSeries
+                   The waveform data tapered and zero padded.
 
     Notes
     -----
     See `taper_timeseries` from pycbc.waveform.utils for more details."""
 
     import pycbc
 
@@ -1914,43 +1664,47 @@
 
     # Append the zeros
     tapered_data = np.array(tapered_data)
 
     # Pad ends with extra zeros
     zeros = np.zeros([zeros])
     # Prepend with z zeros
-    tapered_data = np.transpose(np.concatenate((np.transpose(zeros), np.transpose(tapered_data))))
+    tapered_data = np.transpose(
+        np.concatenate((np.transpose(zeros), np.transpose(tapered_data)))
+    )
     # Append with extra zeros
-    tapered_data = np.transpose(np.concatenate((np.transpose(tapered_data), np.transpose(zeros))))
+    tapered_data = np.transpose(
+        np.concatenate((np.transpose(tapered_data), np.transpose(zeros)))
+    )
 
     # Convert back to timeseries if the input was a time series.
     tapered_data = pycbc.types.timeseries.TimeSeries(tapered_data, delta_t)
 
     # Return the timeseries
     return tapered_data
 
 
 def low_cut_filter(utilde, freqs, order=2, omega0=0.03):
     """Apply low frequency cut filter using a butterworth filter.
 
     Parameters
     ----------
-    utilde:    1d array
-                       The frequency domain data.
-    freqs:	   1d array
-                       The frequencies.
-    order:	   int
-                       The order of the butterworth filter.
-    omega0:    float
-                       The cutoff frequency of the butterworth filter.
+    utilde : 1d array
+             The frequency domain data.
+    freqs : 1d array
+            The frequencies.
+    order : int
+            The order of the butterworth filter.
+    omega0 : float
+             The cutoff frequency of the butterworth filter.
 
     Returns
     -------
-    utilde_lc:	  1d array
-                              The filtered data.
+    utilde_lc : 1d array
+                The filtered data.
     """
 
     from scipy import signal
     from scipy.interpolate import interp1d
 
     # import matplotlib.pyplot as plt
 
@@ -1971,41 +1725,26 @@
     return filtered_signal
 
 
 def center(wvp, wvc=None, delta_t=None):
     """Center a waveform (wvp, wvc) at the peak
     of the complex modulous sqrt(wvp**2 + wvc**2).
 
-
-
     Parameters
     ----------
-
-
-    wvp:	1d array or a pycbc TimeSeries object
-    wvc:	1d array or a pycbc TimeSeries object
-                    The one/two components of the waveforms
-                    as 1d list or numpy arrays or pycbc timeseries.
-    delta_t:	float
-                            The timestepping delta_t.
+    wvp, wvc : 1d array or a pycbc TimeSeries object
+               The one/two components of the waveforms
+               as 1d list or numpy arrays or pycbc timeseries.
+    delta_t : float
+              The timestepping delta_t.
 
     Returns
     -------
-
-    centered_wf:	a pycbc TimeSeries objet
-                                    The two 1d centered waveform(s) as individual pycbc timeseries.
-
-
-    Procedure
-    ---------
-
-    1. Findout if both polarizations are supplied. If not assume cross pol is plus.
-    2. Find the absolute magnitde location in the array.
-    3. Construct the time limits using this information.
-    3. Construct timeseries with epoch as first index of the array.
+    centered_wf : a pycbc TimeSeries object
+                  The two 1d centered waveform(s) as individual pycbc timeseries.
 
     """
     # Flag to find out if both polarizations are supplied or not.
     flag = 0
     # If only one waveform is provided, assume cross pol = plus pol.
     if not wvc:
         flag = 1
@@ -2015,60 +1754,63 @@
     if not delta_t:
         try:
             delta_t = wvp.delta_t
         except AttributeError:
             try:
                 delta_t = wvc.delta_t
             except BaseException:
-                message("Input is not a TimeSeries." "Please supply gridspacing as delta_t", message_verbosity=0)
+                message(
+                    "Input is not a TimeSeries."
+                    "Please supply gridspacing as delta_t",
+                    message_verbosity=0,
+                )
 
     datap = np.array(wvp)
     datac = np.array(wvc)
 
     # Assign the complex amplitude
     amp = np.power(datap, 2) + np.power(datac, 2)
     # Find the location of the max amplitude
     ind = np.where(amp == np.max(amp))[0][0]
     # Calculate the epoch
     tlim = [-ind * delta_t, (len(datap) - ind) * delta_t]
     # Returns the centered wvp and wvc if wvc was provided else returns just
     # the former.
 
     if flag == 1:
-        centered_wf = pycbc.types.timeseries.TimeSeries(datap, delta_t, epoch=tlim[0])
+        centered_wf = pycbc.types.timeseries.TimeSeries(
+            datap, delta_t, epoch=tlim[0]
+        )
     else:
         centered_wf = (
             pycbc.types.timeseries.TimeSeries(datap, delta_t, epoch=tlim[0]),
             pycbc.types.timeseries.TimeSeries(datac, delta_t, epoch=tlim[0]),
         )
 
     return centered_wf
 
 
 def get_centered_taxis(time_ax, amps):
     """Get the time axis of the waveform centered
-            at its maximum absolute amplitude.
+    at its maximum absolute amplitude.
 
     Parameters
     ----------
+    time_ax : 1d array
+              The 1d array containg the original
+              (uncentered)time axis of the wveform.
 
-    time_ax:	1d array
-                                                    The 1d array containg
-                                                    the original (uncentered)time axis of the wveform.
-
-
-    amps	:	1d array
-                                                    The amplitude of the waveform.
+    amps : 1d array
+           The amplitude of the waveform.
 
     Returns
     -------
-
-    time_centered:	1d array
-                                    The centered time axis of the waveform.
-                                    The maximum amplitude timestap will be at :math:`t=0`.
+    time_centered : 1d array
+                    The centered time axis of the waveform.
+                    The maximum amplitude timestap will be at :math:`t=0`.
     """
 
     # Get the maximum amplitude
     amps_max = np.argmax(abs(amps))
     # Get the time stamp of the max amp location.
     time_max = time_ax[amps_max]
     # Center the time axis.
@@ -2078,99 +1820,88 @@
 
 
 def plot(xdata, func_x, save="no"):
     """A Basic plotting function.
 
     Parameters
     ----------
-
-    xdata:	1d array
-                                    The x axis of the function,
-    func_x: 1d array
-                                                                    The y axis of the function f(x),
-    save:	bool.
-                                                                    True or False. Whether the plot should be saved or not.
+    xdata : 1d array
+            The x axis of the function,
+    func_x : 1d array
+             The y axis of the function f(x),
+    save : bool.
+           True or False. Whether the plot should be saved or not.
 
     Returns
     -------
-
-    1:	(int)
-    plots:	figures to stdout and disk
-                                    Displays the plot, and Saves with the filename provided.
+    1 : int
+    plots : figures to stdout and disk
+            Displays the plot, and Saves with the filename provided.
     """
 
     plt.plot(np.array(xdata), np.array(func_x))
     plt.title("f(x) vs x")
     plt.grid(which="both", axis="both")
     plt.xlabel("xdata")
     plt.ylabel("f(x)")
     if save != "no":
         plt.savefig(save + ".pdf")
     plt.show()
     return 1
 
 
-# Custom coalign function
-
-
 def coalignwfs(tsdata1, tsdata2, delta_t=None):
-    """Coalign two timeseries.
-            Wrapper and modification around pycbc functions
-            with some additional functionalities.
-
+    """Coalign two timeseries. Wrapper and modification around
+    pycbc functions with some additional functionalities.
 
     Parameters
     ----------
-
-    tsdata1:	list, 1d array or a pycbc TimeSeries
-    tsdata2:	list, 1d array or a pycbc TimeSeries
-                            The two data vectors as 1d lists or
-                            numpy arrays or pycbc TimeSeries
-    delta_t:	float
-                            The time stepping.
+    tsdata1, tsdata2 : list, 1d array or a pycbc TimeSeries
+                       The two data vectors as 1d lists or
+                       numpy arrays or pycbc TimeSeries
+    delta_t : float
+              The time stepping.
 
     Returns
     -------
+    ctsdata1, tsdata2 : a pycbc TimeSeries
+                        A pair of pycbc TimeSeries objects
+                        the aligned first waveform and the second.
 
-    ctsdata1:	a pycbc TimeSeries
-    tsdata2:	a pycbc TimeSeries
-                            A pair of pycbc TimeSeries objects;
-                            the aligned first waveform and the second.
-
-    Procedure
-    ---------
-
-    1. Adjust length of either waveforms if needed
-    2. Compute The complex SNR.
-    3. Shift and roll the first.
-
+    Notes
+    -----
+    The first waveform is changed.
     """
 
     # Lengths of the two input timeseries
     # len1 = len(tsdata1)
     # len2 = len(tsdata2)
 
     # Add zeros at the end of waveform 1 without tapering if len2>len1
     # if len2>len1:
-    # 				 tsdata1,lflag = lengtheq(tsdata2,tsdata1,tsdata1.delta_t)
+    #                tsdata1,lflag = lengtheq(tsdata2,tsdata1,tsdata1.delta_t)
     # Add zeros at the end of waveform 2 without tapering if len1>len2
     # elif len1>len2:
-    # 				 tsdata2,lflag = lengtheq(tsdata2,tsdata1,tsdata1.delta_t)
+    #                tsdata2,lflag = lengtheq(tsdata2,tsdata1,tsdata1.delta_t)
 
     # Assign the timestep. Real and imaginary parts are assumed to have same
     # timestep.
 
     if not delta_t:
         try:
             delta_t = tsdata1.delta_t
         except AttributeError:
             try:
                 delta_t = tsdata2.delta_t
             except BaseException:
-                message("Input is not a TimeSeries." "Please supply gridspacing as delta_t", message_verbosity=0)
+                message(
+                    "Input is not a TimeSeries."
+                    "Please supply gridspacing as delta_t",
+                    message_verbosity=0,
+                )
 
     tsdata1, tsdata2, _ = lengtheq(tsdata1, tsdata2, delta_t, is_ts=True)
 
     # Calculate complex SNR using pycbc function. Note: This complex SNR is
     # actually the complex SNR * norm of the timeseries.
     csnr = pycbc.filter.matchedfilter.matched_filter(tsdata1, tsdata2)
     # Find the absolute value of the complex SNR timeseries
@@ -2200,50 +1931,31 @@
 
     return ctsdata1, tsdata2
 
 
 def coalignwfs2(tsdata1, tsdata2, delta_t=None):
     """Coalign two waveforms function 2.
 
-
     Parameters
     ----------
-
-    tsdata1:	1d array or a pycbc TimeSeries
-    tsdata2:	1d array or a pycbc TimeSeries
-                            two data vectors as 1d lists or
-                            numpy arrays or pycbc timeseries.
+    tsdata1, tsdata2 : 1d array or a pycbc TimeSeries
+                       two data vectors as 1d lists or
+                       numpy arrays or pycbc timeseries.
 
     Returns
     --------
-
-    aligned_waveforms:	 list
-                                            The aligned waveforms in the format
-                                            [aligned_wf1,
-                                            aligned_wf2,
-                                            [norm1, norm2, location of maximum]].
-
+    aligned_waveforms : list
+                        The aligned waveforms in the format
+                        [aligned_wf1,
+                        aligned_wf2,
+                        [norm1, norm2, location of maximum]].
 
     Notes
     -----
-
-    Procedure:
-
-    1. Adjust length of either waveforms if needed
-
-    2. Normalize the two timeseries
-
-    3. Compute The complex SNR
-
-    4. Shift and roll the first
-
-    5. Returns normalized waveforms
-
-
-    See coalignwfs for description. This algorithm does not use
+    See coalignwfs for more description. This algorithm does not use
     the builtin coalign function from pycbc. This involves normalization
     of the data vectors explicitly and identifiies the timeshift by computing
     the complex SNR and finding the maximum element.
     """
     # Lengths of the two input timeseries
     len1 = len(tsdata1)
     len2 = len(tsdata2)
@@ -2264,15 +1976,15 @@
         try:
             start, end = startend(np.array(tsdata1))
         except BaseException:
             start, end = apxstartend(np.array(tsdata1))
 
     # Add zeros at the end of waveform 1 without tapering if len2>len1
     if len2 > len1:
-        # 		tsdata1,lflag = lengtheq(tsdata2,tsdata1,tsdata1.delta_t)
+        #       tsdata1,lflag = lengtheq(tsdata2,tsdata1,tsdata1.delta_t)
         try:
             start, end = startend(np.array(tsdata1))
         except BaseException:
             start, end = apxstartend(np.array(tsdata1))
 
     # Add zeros at the end of waveform 2 without tapering if len1>len2
     elif len1 > len2:
@@ -2284,34 +1996,48 @@
 
     # match,shift=pycbc.filter.matchedfilter.match(tsdata1,tsdata2)
 
     # Normalize the waveforms
     norm1 = norm(np.array(tsdata1[start:end]))
     norm2 = norm(np.array(tsdata2[start:end]))
 
-    tsdata1_cropped = pycbc.types.timeseries.TimeSeries(np.array(tsdata1[start:end]) / norm1, delta_t)
-    tsdata2_cropped = pycbc.types.timeseries.TimeSeries(np.array(tsdata2[start:end]) / norm2, delta_t)
+    tsdata1_cropped = pycbc.types.timeseries.TimeSeries(
+        np.array(tsdata1[start:end]) / norm1, delta_t
+    )
+    tsdata2_cropped = pycbc.types.timeseries.TimeSeries(
+        np.array(tsdata2[start:end]) / norm2, delta_t
+    )
 
-    max_match, max_shift = pycbc.filter.matchedfilter.match(tsdata1_cropped, tsdata2_cropped)
+    max_match, max_shift = pycbc.filter.matchedfilter.match(
+        tsdata1_cropped, tsdata2_cropped
+    )
 
-    tsdata1 = pycbc.types.timeseries.TimeSeries(np.array(tsdata1) / norm1, delta_t)
-    tsdata2 = pycbc.types.timeseries.TimeSeries(np.array(tsdata2) / norm2, delta_t)
+    tsdata1 = pycbc.types.timeseries.TimeSeries(
+        np.array(tsdata1) / norm1, delta_t
+    )
+    tsdata2 = pycbc.types.timeseries.TimeSeries(
+        np.array(tsdata2) / norm2, delta_t
+    )
 
     # Calculate complex SNR using pycbc function. Note: This complex SNR is
     # actually the complex SNR * norm of the timeseries.
     csnr = pycbc.filter.matchedfilter.matched_filter(tsdata1, tsdata2)
 
     # Find the absolute value of the complex SNR timeseries
     acsnr = np.array(np.abs(csnr))
     # message(acsnr,np.max(acsnr))
 
     # Find the location of the maximum element in acsnr
     maxloc = (np.where(acsnr == np.max(acsnr)))[0][0]
     mmatch = np.amax(acsnr)
-    message(f"Max location is {maxloc}," f"match is {mmatch}" f"max shift is {max_shift}")
+    message(
+        f"Max location is {maxloc},"
+        f"match is {mmatch}"
+        f"max shift is {max_shift}"
+    )
 
     # Shift the waveform 1 in time using maxloc
     tsdata1 = shiftmatched(tsdata1, maxloc, delta_t, is_ts=True)
 
     # Phase shift ( rotate) the waveform 1 by multipying
     # the frequency series of waveform 1 with the phase
     # of the max element in acsnr
@@ -2321,42 +2047,50 @@
     rotation = csnr[maxloc] / np.absolute(csnr[maxloc])
 
     # Rotate and take the inverse Fourier transform
     ctsdata1 = (rotation * tsdata1.to_frequencyseries()).to_timeseries()
 
     # Recenter waveform 0 and assign the timeaxis of waveform 0 to waveform1
     ctsdata1, dummy = center(ctsdata1, ctsdata1)
-    tsdata2 = pycbc.types.timeseries.TimeSeries(np.array(tsdata2), tsdata2.delta_t, epoch=ctsdata1.sample_times[0])
+    tsdata2 = pycbc.types.timeseries.TimeSeries(
+        np.array(tsdata2), tsdata2.delta_t, epoch=ctsdata1.sample_times[0]
+    )
 
     # Return the normalized, time and phase shifted waveform 1 to coalign with
     # 2 and waveform 2.
-    aligned_waveforms = {"wf1": ctsdata1, "wf2": tsdata2, "norms": [norm1, norm2], "shift": maxloc, "match": max_match}
+    aligned_waveforms = {
+        "wf1": ctsdata1,
+        "wf2": tsdata2,
+        "norms": [norm1, norm2],
+        "shift": maxloc,
+        "match": max_match,
+    }
 
     return aligned_waveforms
 
 
 def resample_wfs(both_time_axes, both_waveforms, delta_t="auto", Plot=False):
     """Resample the waveform pairs.
 
     Parameters
     ----------
     both_time_axes : list
-                                     A list containing two 1d arrays representing the time axes.
+                     A list containing two 1d arrays representing the time axes.
     both_waveforms : list
-                                     A list containing two 1d arrays respresenting the waveforms.
-    delta_t		   : string, float
-                                     The time step to resample at. Auto uses the finest of the two available.
-                                     A float value can be provided by the user as well.
+                     A list containing two 1d arrays respresenting the waveforms.
+    delta_t : string, float
+              The time step to resample at. Auto uses the finest of the two available.
+              A float value can be provided by the user as well.
 
     Returns
     -------
     both_time_axes_resam : 1d array
-                                               A 1d array representing the resampled time axes.
+                           A 1d array representing the resampled time axes.
     both_waveforms_resam : list
-                                               A list containing two 1d arrays respresenting the resampled waveforms.
+                           A list containing two 1d arrays respresenting the resampled waveforms.
     """
 
     # from waveformtools.waveformtools import lengtheq
 
     # from scipy.interpolate import interp1d
 
     waveform1, waveform2 = both_waveforms
@@ -2384,62 +2118,61 @@
     # waveform1, waveform2, flag = lengtheq(waveform1, waveform2, delta_t=delta_t)
 
     new_time_axis = np.arange(min_t, max_t, delta_t)
 
     wf1_amp, wf1_phase = xtract_camp_phase(waveform1.real, waveform1.imag)
     wf2_amp, wf2_phase = xtract_camp_phase(waveform2.real, waveform2.imag)
 
-    # wf1_amp_int_fun	  = interp1d(time_axis1, wf1_amp, kind='cubic')
+    # wf1_amp_int_fun     = interp1d(time_axis1, wf1_amp, kind='cubic')
     # wf1_phase_int_fun   = interp1d(time_axis1, wf1_phase, kind='cubic')
 
-    # wf1_amp_resam		  = wf1_amp_int_fun(new_time_axis)
-    # wf1_phase_resam	  = wf1_phase_int_fun(new_time_axis)
+    # wf1_amp_resam       = wf1_amp_int_fun(new_time_axis)
+    # wf1_phase_resam     = wf1_phase_int_fun(new_time_axis)
 
     wf1_amp_resam = interp_resam_wfs(wf1_amp, time_axis1, new_time_axis)
     wf1_phase_resam = interp_resam_wfs(wf1_phase, time_axis1, new_time_axis)
 
     wf1_resam = wf1_amp_resam * np.exp(1j * wf1_phase_resam)
 
     wf2_amp_resam = interp_resam_wfs(wf2_amp, time_axis2, new_time_axis)
     wf2_phase_resam = interp_resam_wfs(wf2_phase, time_axis2, new_time_axis)
 
-    # wf2_amp_resam		  = wf2_amp_int_fun(new_time_axis)
-    # wf2_phase_resam	  = wf2_phase_int_fun(new_time_axis)
+    # wf2_amp_resam       = wf2_amp_int_fun(new_time_axis)
+    # wf2_phase_resam     = wf2_phase_int_fun(new_time_axis)
 
     wf2_resam = wf2_amp_resam * np.exp(1j * wf2_phase_resam)
 
     return new_time_axis, wf1_resam, wf2_resam
 
 
 def match_wfs(all_time_axes, all_waveforms, delta_t="auto"):
     """Match two waveforms and return the time shift,
     phase shift, normalized waveforms and match coefficient.
 
     Parameters
     ----------
-    time_axes: list
-                    A list containing the time axes
-                    of the two waveforms
-
-    waveforms: list
-                            A list of two waveforms.
-                            Each is a 1d array.
-    delta_t: float, string, optional
-                     The time step of the resampled arrays.
-                     Can be A, B, auto or any float value.
+    time_axes : list
+                A list containing the time axes
+                of the two waveforms
+    waveforms : list
+                A list of two waveforms.
+                Each is a 1d array.
+    delta_t : float, string, optional
+              The time step of the resampled arrays.
+              Can be A, B, auto or any float value.
 
     Returns
     -------
-    match_details: dict
-                                    A dictionary containing the
-                                    i). match coeffient
-                                    ii). time_shift
-                                    iii). phase shift in radians
-                                    iv). normalized, resampled, waveforms and their
-                                             time-axes.
+    match_details : dict
+                                                                                                                                                                                                                                                                    A dictionary containing the
+                                                                                                                                                                                                                                                                    i). match coeffient
+                                                                                                                                                                                                                                                                    ii). time_shift
+                                                                                                                                                                                                                                                                    iii). phase shift in radians
+                                                                                                                                                                                                                                                                    iv). normalized, resampled, waveforms
+                           and their time-axes.
 
     Note
     ----
     The shifts give by how much the first waveform has to be shifted to match with the second.
 
     """
 
@@ -2459,15 +2192,17 @@
 
             # delta_t = min(delta_t_A, delta_t_B)
         elif delta_t == "A":
             delta_t = delta_t_A
         elif delta_t == "B":
             delta_t = delta_t_B
         else:
-            raise ValueError(f"Did not understand speification for delta_t {delta_t}")
+            raise ValueError(
+                f"Did not understand speification for delta_t {delta_t}"
+            )
 
     # message(type(time_axis1), type(time_axis2))
     # message(time_axis1-time_axis2)
     # message(time_axis1==time_axis2)
 
     # Don't interpolate if the time axis are identical
     Interp = True
@@ -2483,15 +2218,17 @@
             # tsorted = sorted(time_axis1)
             # delta_t = tsorted[0] - tsorted[1]
 
             # delta_t = mode(np.diff(time_axis1))
 
     if Interp is True:
         message("Interpolating time axis")
-        time_axis, wf1, wf2 = resample_wfs(all_time_axes, all_waveforms, delta_t)
+        time_axis, wf1, wf2 = resample_wfs(
+            all_time_axes, all_waveforms, delta_t
+        )
         # message(time_axis, wf1, wf2)
 
     from waveformtools.transforms import compute_fft, compute_ifft
 
     # The Fspace waveforms
     faxis, wf1_tilde = compute_fft(wf1, delta_t)
     _, wf2_tilde = compute_fft(wf2, delta_t)
@@ -2509,15 +2246,17 @@
     # max_snr = np.amax(Acsnr)
 
     Tshift_rec = (len(time_axis) - Tshift_rec_index) * delta_t
     # Phase shift
     Pshift_rec = csnr[Tshift_rec_index] / np.absolute(csnr[Tshift_rec_index])
     Pshift_rec_rad = np.log(Pshift_rec) / (1j)
 
-    message("-----------------------------------\n Shift information for waveform 2 against 1 \n")
+    message(
+        "-----------------------------------\n Shift information for waveform 2 against 1 \n"
+    )
     message(f"Recovered Time shift: {Tshift_rec}")
     message(f"Recovered Phase shift: {Pshift_rec}, {Pshift_rec_rad} in radians")
     message("-----------------------------------")
 
     # Apply the time shift to the second waveform
 
     if Tshift_rec_index != 0:
@@ -2539,15 +2278,17 @@
 
     norm1 = np.sqrt(np.sum(wf1 * np.conjugate(wf1)))
     norm2 = np.sqrt(np.sum(wf2_TPrec * np.conjugate(wf2_TPrec)))
 
     waveform1_aligned = wf1 / norm1
     waveform2_aligned = wf2_TPrec / norm2
 
-    match_score = np.sum(waveform1_aligned * np.conjugate(waveform2_aligned))  # max_snr/(norm1*norm2)
+    match_score = np.sum(
+        waveform1_aligned * np.conjugate(waveform2_aligned)
+    )  # max_snr/(norm1*norm2)
 
     match_details = {
         "match_score": match_score,
         "time_shift": Tshift_rec,
         "phase_shift": Pshift_rec_rad,
         "time": time_axis,
         "aligned_waveforms": [waveform1_aligned, waveform2_aligned],
@@ -2558,34 +2299,33 @@
 
 def match_wfs_pycbc(all_time_axes, all_waveforms):
     """Match two waveforms using pycbc subroutines and return the time shift,
     phase shift, normalized waveforms and match coefficient.
 
     Parameters
     ----------
-    time_axes: list
-                    A list containing the time axes
-                    of the two waveforms
-
-    waveforms: list
-                            A list of two waveforms.
-                            Each is a 1d array.
-
-    change: int
-                    Which waveform to change, 1 or 2.
+    time_axes : list
+                A list containing the time axes
+                of the two waveforms
+
+    waveforms : list
+                A list of two waveforms.
+                Each is a 1d array.
+
+    change : int
+             Which waveform to change, 1 or 2.
 
     Returns
     -------
-    match_details: dict
-                                    A dictionary containing the
-                                    i). match coeffient
-                                    ii). time_shift
-                                    iii). phase shift
-                                    iv). normalized waveforms and their
-                                             time-axes.
+    match_details : dict
+                                                                                                                                                                                                                                                                    A dictionary containing the
+                                                                                                                                                                                                                                                                    i). match coeffient
+                                                                                                                                                                                                                                                                    ii). time_shift
+                                                                                                                                                                                                                                                                    iii). phase shift
+                                                                                                                                                                                                                                                                    iv). normalized waveforms and their time-axes.
     """
 
     # Step 1: resample
     from scipy.interpolate import interp1d
 
     # from waveformtools.waveformtools import match_wfs
     # from waveformtools.waveformtools import lengtheq
@@ -2666,15 +2406,17 @@
 
     mlen = min(len(wf1_aligned_cropped), len(wf2_shifted))
 
     waveform1_aligned = wf1_aligned_cropped[:mlen] / norm1
     waveform2_aligned = wf2_shifted[:mlen] / norm2
 
     aligned_time_axis = aligned_time_axis[:mlen]
-    match_score = np.dot(wf1_aligned_cropped[:mlen], np.conjugate(wf2_shifted[:mlen])) / (norm1 * norm2)
+    match_score = np.dot(
+        wf1_aligned_cropped[:mlen], np.conjugate(wf2_shifted[:mlen])
+    ) / (norm1 * norm2)
 
     match_details = {
         "match_score": match_score,
         "time_shift": shift * delta_t,
         "phase_shift": phase_shift,
         "time": aligned_time_axis,
         "aligned_waveforms": [waveform1_aligned, waveform2_aligned],
@@ -2682,136 +2424,124 @@
 
     return match_details
 
 
 def simplematch_wfs_old(waveforms, delta_t=None):
     """Simple match the given waveforms. Does not clip the waveforms at either ends.
 
-    Procedure
-    ---------
-
-    1. For each pair of waveforms as a list:
-                                                            a. Findout if delt has been specified.
-                                                            b. Findout if the object has attribute delta_t
-                                                            to discern whether it is a pycbc timeseries (
-                                                            not exactly. ). If not then exit.
-                                                            c. Equalize the lengths.
-                                                            d. Compute the match score and shift using
-                                                            the pycbc shift function.
-                                                            e. Findout the start and the end of
-                                                            the waveform using handles.startend.
-                                                            f. Reconstruct normalized and clipped
-                                                            pycbc.timeseries of the waveforms.
-                                                            g. Confirm the equalization of the lengths of the waveoforms.
-                                                            h. Append the match details to an
-                                                            array [ waveform list, [ match score, shift, start_index, end_index]]
-    2. Retun the match details for all the waveforms.
-
-
     Parameters
     ----------
-
-    waveforms:	list
-                                                    A list of pairs [waveform A, waveform B] of waveforms.
-    delta_t:	float, optional
-                                                    The time stepping.
+    waveforms : list
+                A list of pairs [waveform A, waveform B] of waveforms.
+    delta_t : float, optional
+              The time stepping.
 
     Notes
     -----
-
     The time stepping delta_t is the same for each pair of waveforms in the list.
 
     Returns
     -------
-
-    match:	list
-                    A list of dicts [{ Aligned waveforms} ,
-                    {match score (float), shift (number)}]
-                    containing the match information for all
-                    the input waveform pairs.
+    match : list
+            A list of dicts [{ Aligned waveforms} ,
+                            {match score (float), shift (number)}]
+            containing the match information for all the input waveform pairs.
     """
 
     match = []
     # Iterate over (signal,template) pairs in waveforms
     for waveformdat in waveforms:
         # Carryout the match
         if not delta_t:
             try:
                 delta_t = waveformdat[0].delta_t
             except BaseException:
-                message("Waveform is not a pycbc TimeSeries." "Please provide the gridspacing delt")
+                message(
+                    "Waveform is not a pycbc TimeSeries."
+                    "Please provide the gridspacing delt"
+                )
                 sys.exit(0)
         # Match procedure
         # signaldat = lengtheq(waveformdat[0], waveformdat[1], delta_t)
-        waveform1, waveform2, _ = lengtheq(waveformdat[0], waveformdat[1], delta_t)
+        waveform1, waveform2, _ = lengtheq(
+            waveformdat[0], waveformdat[1], delta_t
+        )
 
         # waveform1 = signaldat[0]
         # waveform2 = signaldat[1]
 
         # alignedwvs = pycbc.waveform.utils.coalign_waveforms(signaldat,hpa)
         # Compute the match to calculate match and shift.
         # Note: The match function from pycbc returns the match of the
         # normalized templates
-        (match_score, shift) = pycbc.filter.matchedfilter.match(waveform1, waveform2)
+        (match_score, shift) = pycbc.filter.matchedfilter.match(
+            waveform1, waveform2
+        )
 
         # Coalign the waveforms using pycbc coalign.
-        waveform1, waveform2 = pycbc.waveform.utils.coalign_waveforms(waveform1, waveform2)
+        waveform1, waveform2 = pycbc.waveform.utils.coalign_waveforms(
+            waveform1, waveform2
+        )
 
         # Normalize the waveforms
 
         waveform1 = waveform1 / norm(waveform1)
         waveform2 = waveform2 / norm(waveform2)
 
         try:
-            (match_score, shift) = pycbc.filter.matchedfilter.match(waveform1, waveform2)
+            (match_score, shift) = pycbc.filter.matchedfilter.match(
+                waveform1, waveform2
+            )
         except BaseException:
             message("Final match couldn't be found!")
             match_score = None
             shift = None
 
-        match.append({"Waveforms": [waveform1, waveform2], "Match score": match_score, "Shift": shift})
+        match.append(
+            {
+                "Waveforms": [waveform1, waveform2],
+                "Match score": match_score,
+                "Shift": shift,
+            }
+        )
     return match
 
 
 def pmmatch_wfs(waveforms, offset=25, crop=None):
     """
     Match function for post merger waveforms.
 
-
     Procedure
     ---------
-
     1. Equalize the lengths
     2. Crop the waveforms if necessary.
     3. Normalize to their respective maximum amplitudes.
     4. Align the waveforms in phase.
     5. Compute the match score.
 
     Parameters
     ----------
-
-    waveforms:	a list of pairs
-                            The pairs of waveforms to match
-                            in the format
-                            [[wf1_pair1, wf2_pair2], [wf1_pair_2, wf2_pair2], ...].
-    offset: int
-                    Number of indices to shift the data.
-    crop:	string
-                    A string to decide how to crop the waveforms.
-                    The available Options are 1. `signal` 2. `template` 3. `both`.
+    waveforms : a list of pairs
+                The pairs of waveforms to match
+                in the format
+                [[wf1_pair1, wf2_pair2], [wf1_pair_2, wf2_pair2], ...].
+    offset : int
+             Number of indices to shift the data.
+    crop : string
+           A string to decide how to crop the waveforms.
+           The available Options are 1. `signal` 2. `template` 3. `both`.
 
     Returns
     -------
-
-    matchdet:	a list of dicts
-                            A list of dictionaries.
-                            Each contains
-                            1. the waveform pair,
-                            2. the match score,
-                            3. the shift index. to maximize the match.
+    matchdet : a list of dicts
+               A list of dictionaries.
+               Each contains
+                   1. the waveform pair,
+                   2. the match score,
+                   3. the shift index. to maximize the match.
 
     """
     matchdet = []
     for waveformdat in waveforms:
         signal, template = waveformdat
 
         # message(type(signal), type(template))
@@ -2850,43 +2580,51 @@
             delta_t = template.delta_t
         except BaseException:
             delta_t = 1
             template = pycbc.types.timeseries.TimeSeries(template, delta_t)
 
         # message(type(signal), type(template))
         # Align the waveforms in phase
-        signal_al, template_al = pycbc.waveform.utils.coalign_waveforms(signal, template)
+        signal_al, template_al = pycbc.waveform.utils.coalign_waveforms(
+            signal, template
+        )
 
         # message(np.where(np.array(signalp_al)!=0))
 
         # Compute the match score
-        (matchscore, finalshift) = pycbc.filter.matchedfilter.match(signal_al, template_al)
+        (matchscore, finalshift) = pycbc.filter.matchedfilter.match(
+            signal_al, template_al
+        )
 
         # message('+ The match score, shift are %f, %d'%(matchscore, finalshift))
-        matchdet.append({"Waveforms": [signal_al, template_al], "Match score": matchscore, "Shift": finalshift})
+        matchdet.append(
+            {
+                "Waveforms": [signal_al, template_al],
+                "Match score": matchscore,
+                "Shift": finalshift,
+            }
+        )
 
     return matchdet
 
 
 def roll(tsdata, i_roll, is_ts=False):
     """Roll the data circularly. Circular counterpart of shiftmatched function.
 
     Parameters
     ----------
-
-    tsdata: 1d array or pycbc TimeSeries
-                                                    1D data vector in the form of a list/ numpy array or timeseries.
-    i_roll: int
-                                                    The number of indices to roll the array.
+    tsdata : 1d array or pycbc TimeSeries
+            1D data vector in the form of a list/ numpy array or timeseries.
+    i_roll : int
+             The number of indices to roll the array.
 
     Returns
     -------
-
-    rolled_waveform:	1d array or(pycbc TimeSeries object
-                                                                                    The rolled wavefrom.
+    rolled_waveform : 1d array or(pycbc TimeSeries object
+                      The rolled wavefrom.
     """
 
     flag = 0
     if is_ts:
         try:
             # Assign the time step.
             delta_t = tsdata.delta_t
@@ -2898,53 +2636,50 @@
     tsdata = np.array(tsdata)
     # Break the array into two parts as last i + first i entries.
     arr1 = tsdata[-i_roll:]
     arr2 = tsdata[:-i_roll]
     # Join the two arrays and return them
     if flag == 1:
         rolled_waveform = pycbc.types.timeseries.TimeSeries(
-            np.transpose(np.concatenate((np.transpose(arr1), np.transpose(arr2)))), delta_t
+            np.transpose(
+                np.concatenate((np.transpose(arr1), np.transpose(arr2)))
+            ),
+            delta_t,
         )
 
     else:
-        rolled_waveform = np.transpose(np.concatenate((np.transpose(arr1), np.transpose(arr2))))
+        rolled_waveform = np.transpose(
+            np.concatenate((np.transpose(arr1), np.transpose(arr2)))
+        )
 
     return rolled_waveform
 
 
-##################################################################
-""" Data soothening functions """
-##################################################################
-
-
 def smoothen(func_x, win, order, xdata=None, to_plot=False):
     """Use the Savitzky-Golay Filter to smoothen the data.
-    Show the plots if plot=`yes`.
+	Show the plots if plot=`yes`.
 
-    Parameters
+	Parameters
     ----------
-
-    func_x: 1d array
-                                                    The y axis.
-    win:	int
-                                                                    Window for smoothening. Must be odd.
-    order:	int
-                                                                    The order of the polynomial used for interpolation.
-    x:	1d array, optional.
-            The 1D list or numpy array, to plot
-            the smoothened function. Only required
-            if to_plot=True.
-    to_plot:	bool
-                                                                                                    True or False. Whether or not to display the plot.
+    func_x : 1d array
+             The y axis.
+    win :  int
+          Window for smoothening. Must be odd.
+    order : int
+            The order of the polynomial used for interpolation.
+    x : 1d array, optional.
+        The 1D list or numpy array, to plot the smoothened function.
+        Only required if to_plot=True.
+    to_plot : bool
+              True or False. Whether or not to display the plot.
 
     Returns
     -------
-
-    ydata:	1d array
-                                    The Savgol filtered list.
+    ydata : 1d array
+            The Savgol filtered list.
 
     """
 
     # Apply the filter
     ydata = scipy.signal.savgol_filter(func_x, win, order)
     # Show plots
     if to_plot:
@@ -2959,57 +2694,63 @@
 
 
 def bintp(xdata, func_x, width, order, to_plot=True):
     """Function to bin the data and interpolate it at specified width and order.
 
     Parameters
     ----------
-
-    xdata:	1d array
-                                    1D list or numpy array.
-    func_x: 1d array
-                                                                    The y axis.
-    width:	int
-                                                                    Window size for smoothening,
-    order:	int
-                                                                    Order of the polynomial used for interpolation.
-    to_plot:	bool
-                                                                                                    True or False. To plot or not plot the results.
+    xdata :  1d array
+             1D list or numpy array.
+    func_x : 1d array
+             The y axis.
+    width : int
+            Window size for smoothening,
+    order : int
+            Order of the polynomial used for interpolation.
+    to_plot : bool
+              True or False. To plot or not plot the results.
 
     Returns
     -------
-
-    hist:	a list
-                    [binloc, yvals], The location of the bins and
-                    the y values associated with the bins.
+    hist : list
+           [binloc, yvals], The location of the bins and
+           the y values associated with the bins.
 
     """
 
     # Interpolation orders
     kind = [0, "linear", "quadratic", "cubic"]
     # Parse width
     width = int(width)
     # Number of bins
     nbins = int(len(xdata) / width)
     # Location of the bins
-    binloc = [np.mean(xdata[width * index : width * index + width]) for index in range(0, nbins + 1)]
+    binloc = [
+        np.mean(xdata[width * index : width * index + width])
+        for index in range(0, nbins + 1)
+    ]
     # message(binloc)
     # Assigning y values to the bins
-    yvals = [np.mean(func_x[width * index : width * index + width]) for index in range(0, nbins + 1)]
+    yvals = [
+        np.mean(func_x[width * index : width * index + width])
+        for index in range(0, nbins + 1)
+    ]
     # Assigning x values to the smoothened data
     # xf=x[width:-(width)/2]
     y_final = yvals
     # Interpolate if specified order is more than 0
     if order != 0:
-        y_interp_func = scipy.interpolate.interp1d(binloc, yvals, kind=kind[order])
+        y_interp_func = scipy.interpolate.interp1d(
+            binloc, yvals, kind=kind[order]
+        )
     # Reassign yf
     y_final = y_interp_func(binloc)
     # Set xf to binloc if order=0
     # if order==0:
-    # 		xf=binloc
+    #       xf=binloc
     # y = signal.savgol_filter(func_x,win,order)
     if to_plot:
         # Plot the filtered data
         plt.plot(xdata, func_x, label="data")
         plt.plot(binloc, y_final, label="smoothened data")
         plt.title("Smoothened data by binning and interpolation")
         plt.grid(which="both", axis="both")
@@ -3021,25 +2762,23 @@
 
 
 def mavg(func_x, width):
     """Function to smoothen data. Moving average over the window width.
 
     Parameters
     ----------
-
-    func_x: 1d array
-                                                    A list or numpy array of y axis.
-    Width:	int
-                                    The width of the moving average window.
+    func_x : 1d array
+             A list or numpy array of y axis.
+    Width : int
+            The width of the moving average window.
 
     Returns
     -------
-
-    func_x_avgd:	1d array
-                                                                    1D array of moving averaged y axis.
+    func_x_avgd : 1d array
+                  1D array of moving averaged y axis.
 
     """
 
     # message(len(func_x))
     # List to store smoothened data
     func_x_avgd = []
     # Calculate the moving-average upto last but width num of points
@@ -3057,46 +2796,47 @@
 
 def interpolate_wfs(ts_data, interp_func, delta_t=None, **kwargs):
     """Function to interpolate a list of timeseries data using
     the user specified interp_func function and the keyword arguments.
 
     Parameters
     ----------
-
-    ts_data:	list
-                            The 1d data. A list of waveforms
-                            as a list or numpy array or
-                            pycbc TimeSeries.
-    interp_fun: function
-                                                                                                                                    An interpolating function.
-    delta_t:	float
-                                                                    Timestep.
-    ``**kwargs``:	keyword arguments
-                                                                                                                                    additional arguments to the user specified interp_func.
+    ts_data : list
+              The 1d data. A list of waveforms
+              as a list or numpy array or
+              pycbc TimeSeries.
+    interp_fun : function
+                An interpolating function.
+    delta_t : float
+              Timestep.
+    ``**kwargs`` : keyword arguments
+                   additional arguments to the user specified interp_func.
 
     Returns
     -------
-
-    interp_data:	list
-                                                                                                                                    A list containing interpolated data.
+    interp_data : list
+                  A list containing interpolated data.
 
     """
 
     # List for storing the interpolated data function
     interp_data = []
     # Loop over items in input
     for wfs in ts_data:
         if not delta_t:
             try:
                 # Find sampling time_step
                 delta_t = wfs.delta_t
                 timeaxis = wfs.sample_times
 
             except BaseException:
-                message("Input is not a TimeSeries. Please supply gridspacing as delta_t", message_verbosity=0)
+                message(
+                    "Input is not a TimeSeries. Please supply gridspacing as delta_t",
+                    message_verbosity=0,
+                )
         else:
             timeaxis = np.arange(0, len(wfs) * delta_t, delta_t)
 
         # Interpolate using the supplied function. The keyword arguments
         # supplied to the fuction are the keyword arguments to be supplied
         # to the interpolating function)
         # Append to the list of interpolated data function
@@ -3107,81 +2847,91 @@
 
 def resample(interp_data, new_delta_t, epoch, length, old_delta_t=None):
     """Function to generate timeseries out of the given interpolated data
     function, epoch,sampling frequency, length(duration).
 
     Parameters
     ----------
-
-    interp_data:	1d array
-                                                                                                                                    The yaxis to be interpolated.
-    epoch:	float
-                                                                    The starting point in time.
-    delta_t:	float
-                                                                    New grid spacing to be sampled at.
-    length: int
-                                                                                                    The duration of x axis.
+    interp_data : 1d array
+                  The yaxis to be interpolated.
+    epoch : float
+            The starting point in time.
+    delta_t : float
+              New grid spacing to be sampled at.
+    length : int
+             The duration of x axis.
 
     Returns
     -------
 
-    data:	list
-                                                                    A list containing resampled data as pycbc TimeSeries.
+    data : list
+           A list containing resampled data as pycbc TimeSeries.
     """
 
     data = []
     # Loop over objects in interp_data
     for i in range(len(interp_data)):
         if not old_delta_t:
             try:
                 old_delta_t = interp_data[i].delta_t
 
             except BaseException:
-                message("Input is not a TimeSeries. Please supply gridspacing as delta_t", message_verbosity=0)
+                message(
+                    "Input is not a TimeSeries. Please supply gridspacing as delta_t",
+                    message_verbosity=0,
+                )
         else:
-            interp_data[i] = pycbc.types.timeseries.TimeSeries(interp_data[i], old_delta_t)
+            interp_data[i] = pycbc.types.timeseries.TimeSeries(
+                interp_data[i], old_delta_t
+            )
 
         # Prepare timeaxis
         timeaxis = np.linspace(epoch, epoch + length, int(length / new_delta_t))
         # Append the timeseries to the data list
         ydata = interp_data[i](timeaxis)
-        data.append(pycbc.types.timeseries.TimeSeries(ydata, new_delta_t, epoch=epoch))
+        data.append(
+            pycbc.types.timeseries.TimeSeries(ydata, new_delta_t, epoch=epoch)
+        )
     # Return the list of samples timeseries
     return data
 
 
 def interp_resam_wfs(wavf_data, old_taxis, new_taxis, kind="cubic", k=None):
     """Wrapper function for interpolation and resampling.
 
     Parameters
     ----------
-
-    wavf_data:	1d array
-                            The yaxis to be interpolated,
-    old_taxis, new_taxis:	1darray
-                                                    Old and New time axis.
+    wavf_data : 1d array
+                The yaxis to be interpolated,
+    old_taxis, new_taxis : 1darray
+                           Old and New time axis.
 
     Returns
     -------
-    resam_wf_data:	1d array
-                                    Interpolated and resampled data.
+    resam_wf_data : 1d array
+                    Interpolated and resampled data.
     """
     # from scipy.interpolate import interp1d
 
     amp, phase = xtract_camp_phase(wavf_data.real, wavf_data.imag)
 
     # Interpolate
     if k is not None:
-        from scipy.interpolate import InterpolatedUnivariateSpline as interpolator
+        from scipy.interpolate import (
+            InterpolatedUnivariateSpline as interpolator,
+        )
 
         interp_amp_data = interpolator(old_taxis, amp, k=k)
         amp_res = interp_amp_data.get_residual()
         interp_phase_data = interpolator(old_taxis, phase, k=k)
         phase_res = interp_phase_data.get_residual()
-        message(f"Amplitude residue {amp_res} \t Phase residue {phase_res}", message_verbosity=2)
+        message(
+            f"Amplitude residue {amp_res} \t Phase residue {phase_res}",
+            message_verbosity=2,
+        )
     else:
         from scipy.interpolate import interp1d as interpolator
 
         interp_amp_data = interpolator(old_taxis, amp, kind=kind)
         interp_phase_data = interpolator(old_taxis, phase, kind=kind)
 
     # Resample
@@ -3194,33 +2944,32 @@
 
 
 def progressbar(present_count, total_counts, normalize="yes"):
     """Display the progress bar to std out from present_count and total_count.
 
     Parameters
     ----------
-
-    present_count:	int
-                                                                                                                                    The present count state.
-    total_counts:	int
-                                                                                                                                    The final state.
-
+    present_count : int
+                    The present count state.
+    total_counts : int
+                   The final state.
 
     Returns
     -------
 
     1 : int
-                                    The progress bar is messageed to stdout.
-
+        The progress bar is messageed to stdout.
     """
 
     if normalize == "yes":
         final_progress = 98
         normalized_total_counts = final_progress * 10
-        present_count = int(normalized_total_counts * present_count / total_counts)
+        present_count = int(
+            normalized_total_counts * present_count / total_counts
+        )
         total_counts = normalized_total_counts
 
     # present_count = comm.gather(count,root=rank)
     else:
         final_progress = int(total_counts / 10)
 
     present_stage = int(present_count / 10)
```

### Comparing `waveformtools-2023.5.19/waveformtools.egg-info/PKG-INFO` & `waveformtools-2023.6.3/waveformtools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveformtools
-Version: 2023.5.19
+Version: 2023.6.3
 Summary:  Tools for working with numerical relativity and waveforms data 
 Home-page: https://gitlab.com/vaishakp/waveformtools
 Author: Vaishak Prasad
 Author-email: Vaishak Prasad <vaishakprasad@gmail.com>
 Project-URL: Homepage, https://gitlab.com/vaishakp/waveformtools
 Project-URL: Bug Tracker, https://gitlab.com/vaishakp/waveformtools/issues
 Classifier: Programming Language :: Python :: 3
@@ -125,68 +125,58 @@
 
 * Standard packages (come with full anaconda installation)
     * [`numpy`](http://www.numpy.org/)
     * [`scipy`](http://scipy.org/)
     * [`statistics`](https://docs.python.org/3/library/statistics.html)
     * [`matplotlib`](http://matplotlib.org/)
     * [`h5py`](http://www.h5py.org/)
-* The pyCBC module
-    * [`pyCBC`](https://pycbc.org/).
-* Third party modules
     * [`termcolor`](https://pypi.org/project/termcolor/)
+    * 
+* Optional dependencies (labelled [EXT])
+    * For use with PyCBC data analysis packages.
+        * [`pyCBC`](https://pycbc.org/)
+        * [`lalsuite`](https://git.ligo.org/lscsoft/lalsuite)
+        * [`ligo-common`](https://git.ligo.org/lscsoft/ligo-common)
+    * [`gmpy2`](https://gmpy2.readthedocs.io/en/latest/)
 
 
 ## Recommended method
 
-I recommend installing this module using anaconda with python 3. 
-
-* First, clone this repository:
-
-```sh
-git clone https://gitlab.com/vaishakp/waveformtools.git
-
-```
-
-* Second, create an environment with dependencies resolved, and activate it.
-```sh
-conda create env -f docs/environment.yml
-conda activate wftools
-```
-
-
-* Third, add the path to the $PYTHONPATH variable
-
+I recommend installing this module through pypi:
 ```sh
-PYTHONPATH="/path/to/this/cloned/repo":$PYTHONPATH
-export PYTHONPATH
+pip install waveformtools
 ```
+## Alternate method
 
-* Alternatively, steps 1-2 can be replaced by a manual environment creation and conda package installation.
+Manual install directly from gitlab:
 
+```pip install git+https://gitlab.com/vaishakp/waveformtools@main```
 
-## Manual method
+Or from a clone:
 
-This is not recommended. One can also install this using the pip commands on this git repository:
+* First, clone this repository:
 
 ```sh
-pip install git+https://gitlab.com/vaishakp/waveformtools.git
+git clone https://gitlab.com/vaishakp/waveformtools.git
+
 ```
-or by running python setup file on the cloned repository:
+* Second, run python setup from the `waveformtools` directory:
+```sh
+cd waveformtools
+python setup.py install --prefix="<path to your preferred installation dir>"
+``` 
 
+## Manually setup conda environment
 
+* To create an environment with automatic dependency resolution and activate it, run
 ```sh
-python setyp.py install
+conda create env -f docs/environment.yml
+conda activate wftools
 ```
 
-This is not recommended because of various reasons:
-
-* The commands are better run on user privelages, and using virtual environments, so as to 
-    * not cause system version conflicts 
-    * Avoid dependency issues
-
 
 # Using this code
 ```
 >>> from waveformtools.waveforms import modes_array
 >>> fdir = "<path to data dir>"
 >>> fname = 'ExtrapStrain_RIT-BBH-0001-n100.h5'
 >>> wf1 = modes_array(label='RIT001', spin_weight=-2)
@@ -238,12 +228,17 @@
 
 # Documentation
 
 The documentation for this module is available at [Link to the Documentation](https://waveformtools.readthedocs.io/en/latest/). This was built automatically using Read the Docs.
 
 In some case where the repo has run out of gitlab CI minutes, the documentation is not automatically built. In such cases, we request the user to access the documentation through the `index.html` file in `docs` directory.
 
+
+# Bug tracker
+If you run into any issues while using this package, please report the issue on the [issue tracker](https://gitlab.com/vaishakp/waveformtools/-/issues).
+
+ 
 # Acknowledgements
 
 This project has been hosted, as you can see, on gitlab. Several gitlab tools are used in the deployment of the code, its testing, version control.
 
 The work of this was developed in aiding my PhD work at Inter-University Centre for Astronomy and Astrophysics (IUCAA, Pune, India)](https://www.iucaa.in/). The PhD is in part supported by the [Shyama Prasad Nukherjee Fellowship](https://csirhrdg.res.in/Home/Index/1/Default/2006/59) awarded to me by the [Council of Scientific and Industrial Research (CSIR, India)](https://csirhrdg.res.in/). Resources of the [Inter-University Centre for Astronomy and Astrophysics (IUCAA, Pune, India)](https://www.iucaa.in/) were are used in part.
```

### Comparing `waveformtools-2023.5.19/waveformtools.egg-info/SOURCES.txt` & `waveformtools-2023.6.3/waveformtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

