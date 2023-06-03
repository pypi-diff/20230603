# Comparing `tmp/ec_ecology_toolbox-0.0.4.tar.gz` & `tmp/ec_ecology_toolbox-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec_ecology_toolbox-0.0.4.tar", last modified: Mon May  1 18:20:36 2023, max compression
+gzip compressed data, was "ec_ecology_toolbox-0.0.6.tar", last modified: Sat Jun  3 03:14:09 2023, max compression
```

## Comparing `ec_ecology_toolbox-0.0.4.tar` & `ec_ecology_toolbox-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:36.323943 ec_ecology_toolbox-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-01 18:20:15.000000 ec_ecology_toolbox-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-01 18:20:36.323943 ec_ecology_toolbox-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-01 18:20:15.000000 ec_ecology_toolbox-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:36.323943 ec_ecology_toolbox-0.0.4/ec_ecology_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-01 18:20:36.000000 ec_ecology_toolbox-0.0.4/ec_ecology_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-01 18:20:36.000000 ec_ecology_toolbox-0.0.4/ec_ecology_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:20:36.000000 ec_ecology_toolbox-0.0.4/ec_ecology_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:20:36.000000 ec_ecology_toolbox-0.0.4/ec_ecology_toolbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 18:20:36.000000 ec_ecology_toolbox-0.0.4/ec_ecology_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 18:20:36.000000 ec_ecology_toolbox-0.0.4/ec_ecology_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-01 18:20:15.000000 ec_ecology_toolbox-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-01 18:20:36.323943 ec_ecology_toolbox-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-01 18:20:15.000000 ec_ecology_toolbox-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:36.323943 ec_ecology_toolbox-0.0.4/source/
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-01 18:20:15.000000 ec_ecology_toolbox-0.0.4/source/wrapper.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:20:36.323943 ec_ecology_toolbox-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-01 18:20:15.000000 ec_ecology_toolbox-0.0.4/tests/test_toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:09.662514 ec_ecology_toolbox-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-03 03:13:53.000000 ec_ecology_toolbox-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-03 03:14:09.662514 ec_ecology_toolbox-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-03 03:13:53.000000 ec_ecology_toolbox-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:09.662514 ec_ecology_toolbox-0.0.6/ec_ecology_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-03 03:14:09.000000 ec_ecology_toolbox-0.0.6/ec_ecology_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-03 03:14:09.000000 ec_ecology_toolbox-0.0.6/ec_ecology_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 03:14:09.000000 ec_ecology_toolbox-0.0.6/ec_ecology_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 03:14:09.000000 ec_ecology_toolbox-0.0.6/ec_ecology_toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-03 03:14:09.000000 ec_ecology_toolbox-0.0.6/ec_ecology_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 03:14:09.000000 ec_ecology_toolbox-0.0.6/ec_ecology_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-03 03:13:53.000000 ec_ecology_toolbox-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-03 03:14:09.662514 ec_ecology_toolbox-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-03 03:13:53.000000 ec_ecology_toolbox-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:09.662514 ec_ecology_toolbox-0.0.6/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-03 03:13:53.000000 ec_ecology_toolbox-0.0.6/source/wrapper.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:09.662514 ec_ecology_toolbox-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-03 03:13:53.000000 ec_ecology_toolbox-0.0.6/tests/test_toolbox.py
```

### Comparing `ec_ecology_toolbox-0.0.4/LICENSE` & `ec_ecology_toolbox-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ec_ecology_toolbox-0.0.4/README.md` & `ec_ecology_toolbox-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ec_ecology_toolbox-0.0.4/setup.py` & `ec_ecology_toolbox-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # Available at setup time due to pyproject.toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
-__version__ = "0.0.4"
+__version__ = "0.0.6"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
```

### Comparing `ec_ecology_toolbox-0.0.4/source/wrapper.cc` & `ec_ecology_toolbox-0.0.6/source/wrapper.cc`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
               (optional) The epsilon value to use (if you want epsilon-lexicase selection probabilities; default value is 0, which is equivalent to standard lexicase selection).  
 
             Returns
             -------
             List of floats
               The probabilities of each individual in pop being selected by lexicase selection.            
             )mydelimiter",
-          py::arg("pop"), py::arg("epsilon") = 0.0);
+          py::arg("pop"), py::arg("epsilon") = 0.0, py::arg("binary") = false);
 
     m.def("LexicaseFitnessIndividual", &LexicaseFitnessIndividual<emp::vector<double>>, 
             R"mydelimiter(
             Returns the probability that a single individual is selected by lexicase selection.
 
             Note: calculating these probabilities is an NP-Hard problem (Dolson, 2023). This function is optimized, but if you try to use it with too large of input
             it might take a very a long time. This version is faster than LexicaseFitness if you just need the probability for a single individual, but is still worst-case O(N!)
@@ -52,14 +52,32 @@
             Returns
             -------
             float
               The probability of individual i being selected by lexicase selection.
             )mydelimiter", 
           py::arg("pop"), py::arg("i"), py::arg("epsilon") = 0.0);
 
+        m.def("LexicaseFitnessIndividualBinary", &SolveBinary<emp::vector<double>>, 
+            R"mydelimiter(
+            Returns the probability that a single individual is selected by lexicase selection in the case where all scores are either 0 or 1.
+
+            Parameters
+            ----------
+            pop: list of lists of floats 
+              The scores of a population on each test case/fitness criterion.
+            i: int
+              The index of the individual in pop to calculate selection probability for
+            
+            Returns
+            -------
+            float
+              The probability of individual i being selected by lexicase selection.
+            )mydelimiter", 
+          py::arg("pop"), py::arg("i"));
+
     m.def("SharingFitness", &SharingFitness<emp::vector<double>>, 
             R"mydelimiter(
             Return a vector containing the probability that each member of the population will be selected under tournament selection with fitness sharing.
 
             The numbers in the pop parameter are assumed to be scores on a set of test cases/fitness criteria/tasks.
             Similarity will be calculated as the euclidean distance between these scores.
             Overall "Fitness" will be calculated as the sum of these scores, divided by the fitness sharing niche count.
@@ -102,11 +120,16 @@
               The probabilities of each individual in pop being selected.            
             )mydelimiter",
           py::arg("pop"), py::arg("t_size") = 2);
 
     py::class_<emp::Random>(m, "Random")
       .def(py::init<int>());
 
+    py::class_<emp::BitVector>(m, "BitVector")
+      .def(py::init<std::string>());
+
     py::class_<emp::NKLandscape>(m, "NKLandscape")
       .def(py::init<size_t, size_t, emp::Random&>())
-      .def("GetFitness", static_cast<double (emp::NKLandscape::*)(size_t, size_t) const>(&emp::NKLandscape::GetFitness));
+      .def("GetFitness", static_cast<double (emp::NKLandscape::*)(size_t, size_t) const>(&emp::NKLandscape::GetFitness))
+      .def("GetFitnesses", static_cast<emp::vector<double> (emp::NKLandscape::*)(emp::BitVector) const>(&emp::NKLandscape::GetFitnesses))
+      ;
 }
```

