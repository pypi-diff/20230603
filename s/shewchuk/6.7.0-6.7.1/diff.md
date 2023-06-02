# Comparing `tmp/shewchuk-6.7.0.tar.gz` & `tmp/shewchuk-6.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shewchuk-6.7.0.tar", last modified: Thu May 11 00:21:19 2023, max compression
+gzip compressed data, was "shewchuk-6.7.1.tar", last modified: Fri Jun  2 21:48:26 2023, max compression
```

## Comparing `shewchuk-6.7.0.tar` & `shewchuk-6.7.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:21:19.961995 shewchuk-6.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-11 00:21:06.000000 shewchuk-6.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 00:21:06.000000 shewchuk-6.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-11 00:21:19.961995 shewchuk-6.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-11 00:21:06.000000 shewchuk-6.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-11 00:21:06.000000 shewchuk-6.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 00:21:19.961995 shewchuk-6.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-11 00:21:06.000000 shewchuk-6.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:21:19.961995 shewchuk-6.7.0/shewchuk/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-11 00:21:06.000000 shewchuk-6.7.0/shewchuk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-11 00:21:06.000000 shewchuk-6.7.0/shewchuk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    69147 2023-05-11 00:21:06.000000 shewchuk-6.7.0/shewchuk/_shewchuk.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:21:06.000000 shewchuk-6.7.0/shewchuk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:21:19.961995 shewchuk-6.7.0/shewchuk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-11 00:21:19.000000 shewchuk-6.7.0/shewchuk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-11 00:21:19.000000 shewchuk-6.7.0/shewchuk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:21:19.000000 shewchuk-6.7.0/shewchuk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:21:19.000000 shewchuk-6.7.0/shewchuk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 00:21:19.000000 shewchuk-6.7.0/shewchuk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 00:21:19.000000 shewchuk-6.7.0/shewchuk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:21:19.961995 shewchuk-6.7.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)   124073 2023-05-11 00:21:06.000000 shewchuk-6.7.0/src/shewchuk.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:21:19.961995 shewchuk-6.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-11 00:21:06.000000 shewchuk-6.7.0/tests/test_incircle_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-11 00:21:06.000000 shewchuk-6.7.0/tests/test_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-11 00:21:06.000000 shewchuk-6.7.0/tests/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-11 00:21:06.000000 shewchuk-6.7.0/tests/test_vectors_cross_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-11 00:21:06.000000 shewchuk-6.7.0/tests/test_vectors_dot_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:48:26.860701 shewchuk-6.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-02 21:48:17.000000 shewchuk-6.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-02 21:48:17.000000 shewchuk-6.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-06-02 21:48:26.860701 shewchuk-6.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-02 21:48:17.000000 shewchuk-6.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-02 21:48:17.000000 shewchuk-6.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 21:48:26.860701 shewchuk-6.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-02 21:48:17.000000 shewchuk-6.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:48:26.860701 shewchuk-6.7.1/shewchuk/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-02 21:48:17.000000 shewchuk-6.7.1/shewchuk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-02 21:48:17.000000 shewchuk-6.7.1/shewchuk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    69147 2023-06-02 21:48:17.000000 shewchuk-6.7.1/shewchuk/_shewchuk.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:48:17.000000 shewchuk-6.7.1/shewchuk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:48:26.860701 shewchuk-6.7.1/shewchuk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-06-02 21:48:26.000000 shewchuk-6.7.1/shewchuk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-02 21:48:26.000000 shewchuk-6.7.1/shewchuk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:48:26.000000 shewchuk-6.7.1/shewchuk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:48:26.000000 shewchuk-6.7.1/shewchuk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-02 21:48:26.000000 shewchuk-6.7.1/shewchuk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 21:48:26.000000 shewchuk-6.7.1/shewchuk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:48:26.860701 shewchuk-6.7.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)   125651 2023-06-02 21:48:17.000000 shewchuk-6.7.1/src/shewchuk.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:48:26.860701 shewchuk-6.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-02 21:48:17.000000 shewchuk-6.7.1/tests/test_incircle_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-02 21:48:17.000000 shewchuk-6.7.1/tests/test_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-02 21:48:17.000000 shewchuk-6.7.1/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-02 21:48:17.000000 shewchuk-6.7.1/tests/test_vectors_cross_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-02 21:48:17.000000 shewchuk-6.7.1/tests/test_vectors_dot_product.py
```

### Comparing `shewchuk-6.7.0/LICENSE` & `shewchuk-6.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shewchuk-6.7.0/PKG-INFO` & `shewchuk-6.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shewchuk
-Version: 6.7.0
+Version: 6.7.1
 Home-page: https://github.com/lycantropos/shewchuk/
 Download-URL: https://github.com/lycantropos/shewchuk/archive/master.zip
 Author-email: Azat Ibrakov <azatibrakov@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Azat Ibrakov
```

### Comparing `shewchuk-6.7.0/README.md` & `shewchuk-6.7.1/README.md`

 * *Files identical despite different names*

### Comparing `shewchuk-6.7.0/pyproject.toml` & `shewchuk-6.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shewchuk-6.7.0/setup.py` & `shewchuk-6.7.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,16 +17,20 @@
 
     class BuildExt(build_ext):
         def build_extensions(self) -> None:
             compile_args = []
             compiler_type = self.compiler.compiler_type
             if compiler_type == 'unix':
                 compile_args.append('-Werror')
+                compile_args.append('-Wall')
+                compile_args.append('-Wextra')
+                compile_args.append('-Wconversion')
             elif compiler_type == 'msvc':
                 compile_args.append('/WX')
+                compile_args.append('/W3')
             for extension in self.extensions:
                 extension.extra_compile_args += compile_args
             super().build_extensions()
 
 
     parameters.update(
             cmdclass={build_ext.__name__: BuildExt},
```

### Comparing `shewchuk-6.7.0/shewchuk/__init__.py` & `shewchuk-6.7.1/shewchuk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Robust floating point operations."""
 
-__version__ = '6.7.0'
+__version__ = '6.7.1'
 
 try:
     from ._cshewchuk import (Expansion,
                              incircle_test,
                              kind,
                              orientation,
                              vectors_cross_product,
```

### Comparing `shewchuk-6.7.0/shewchuk/__init__.pyi` & `shewchuk-6.7.1/shewchuk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `shewchuk-6.7.0/shewchuk/_shewchuk.py` & `shewchuk-6.7.1/shewchuk/_shewchuk.py`

 * *Files identical despite different names*

### Comparing `shewchuk-6.7.0/shewchuk.egg-info/PKG-INFO` & `shewchuk-6.7.1/shewchuk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shewchuk
-Version: 6.7.0
+Version: 6.7.1
 Home-page: https://github.com/lycantropos/shewchuk/
 Download-URL: https://github.com/lycantropos/shewchuk/archive/master.zip
 Author-email: Azat Ibrakov <azatibrakov@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Azat Ibrakov
```

### Comparing `shewchuk-6.7.0/src/shewchuk.c` & `shewchuk-6.7.1/src/shewchuk.c`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 #include <pymath.h>
 #include <stddef.h>
 #include <stdio.h>
 #include <structmember.h>
 #define EPSILON (DBL_EPSILON / 2.0)
 #define PY39_OR_MORE PY_VERSION_HEX >= 0x03090000
 
-static int to_sign(double value) { return value > 0.0 ? 1 : (!value ? 0 : -1); }
+static int to_sign(double value) {
+  return value > 0.0 ? 1 : (value == 0.0 ? 0 : -1);
+}
 
-const static size_t BIT_LENGTHS_TABLE[32] = {0, 1, 2, 2, 3, 3, 3, 3, 4, 4, 4,
+static const size_t BIT_LENGTHS_TABLE[32] = {0, 1, 2, 2, 3, 3, 3, 3, 4, 4, 4,
                                              4, 4, 4, 4, 4, 5, 5, 5, 5, 5, 5,
                                              5, 5, 5, 5, 5, 5, 5, 5, 5, 5};
 
 size_t bit_length(const size_t value) {
   size_t result = 0;
   size_t step = value;
   while (step >= 32) {
@@ -157,24 +159,25 @@
 static size_t add_double_in_place(size_t size, double *components, double value,
                                   double *result) {
   size_t result_size = 0;
   double accumulator = value;
   for (size_t index = 0; index < size; index++) {
     double tail;
     two_add(accumulator, components[index], &accumulator, &tail);
-    if (!!tail) result[result_size++] = tail;
+    if (tail != 0.0) result[result_size++] = tail;
   }
-  if (!!accumulator || !result_size) result[result_size++] = accumulator;
+  if (accumulator != 0.0 || result_size == 0)
+    result[result_size++] = accumulator;
   return result_size;
 }
 
 static int add_double(size_t size, double *components, double value,
                       size_t *result_size, double **result) {
   *result = (double *)PyMem_Malloc((size + 1) * sizeof(double));
-  if (!*result) {
+  if (*result == NULL) {
     PyErr_NoMemory();
     return -1;
   }
   *result_size = add_double_in_place(size, components, value, *result);
   if (!PyMem_Resize(*result, double, *result_size)) {
     PyErr_NoMemory();
     return -1;
@@ -221,23 +224,23 @@
           components[size - 2] < 0.0);
 }
 
 static int components_to_fractions(const size_t size, double *const components,
                                    size_t *result_size,
                                    double **result_components) {
   *result_components = (double *)PyMem_Malloc(size * sizeof(double));
-  if (!*result_components) {
+  if (*result_components == NULL) {
     PyErr_NoMemory();
     return -1;
   }
   double _;
   size_t index;
   for (index = 0; index < size; ++index)
     (*result_components)[index] = modf(components[index], &_);
-  for (; index > 1 && !(*result_components)[index - 1]; --index) {
+  for (; index > 1 && (*result_components)[index - 1] == 0.0; --index) {
   }
   *result_size = index;
   if (!PyMem_Resize(*result_components, double, *result_size)) {
     PyErr_NoMemory();
     return -1;
   }
   return 0;
@@ -246,26 +249,25 @@
 static double components_to_accumulated_fraction(
     const size_t size, const double *const components) {
   double _;
   double result = 0.0;
   size_t index;
   for (index = 0; index < size; ++index) {
     double component_fraction = modf(components[index], &_);
-    if (!component_fraction) break;
+    if (component_fraction == 0.0) break;
     result += component_fraction;
   }
   assert(result == 0.0 && index == 0 ||
          result == modf(components[index - 1], &_));
   return result;
 }
 
-static int do_components_have_fraction(const size_t size,
-                                       const double *const components) {
+static int do_components_have_fraction(const double *const components) {
   double _;
-  return !!modf(components[0], &_);
+  return modf(components[0], &_) != 0.0;
 }
 
 static int is_double_lesser_than_components(double value, const size_t size,
                                             double *const components) {
   return value < components[size - 1] ||
          (size > 1 && value == components[size - 1] &&
           components[size - 2] > 0.0);
@@ -273,40 +275,40 @@
 
 static size_t compress_components_single(size_t size, double *components) {
   size_t bottom = size - 1;
   double accumulator = components[bottom];
   for (Py_ssize_t index = (Py_ssize_t)(bottom)-1; index >= 0; --index) {
     double head, tail;
     two_add(accumulator, components[index], &head, &tail);
-    if (!!tail) {
+    if (tail != 0.0) {
       components[bottom--] = head;
       accumulator = tail;
     } else
       accumulator = head;
   }
   size_t top = 0;
   for (size_t index = bottom + 1; index < size; ++index) {
     double head, tail;
     two_add(components[index], accumulator, &head, &tail);
-    if (!!tail) components[top++] = tail;
+    if (tail != 0.0) components[top++] = tail;
     accumulator = head;
   }
-  if (!!accumulator || !top) components[top++] = accumulator;
+  if (accumulator != 0.0 || top == 0) components[top++] = accumulator;
   return top;
 }
 
 static void copy_components(size_t size, double *source, double *destination) {
   for (size_t index = 0; index < size; ++index)
     destination[index] = source[index];
 }
 
 static size_t compress_components(size_t size, double *components) {
   const size_t original_size = size;
   double *next_components = (double *)PyMem_Malloc(size * sizeof(double));
-  if (!next_components) {
+  if (next_components == NULL) {
     PyErr_NoMemory();
     return 0;
   }
   copy_components(size, components, next_components);
   for (size_t step = 0; step < original_size; ++step) {
     const size_t next_size = compress_components_single(size, next_components);
     if (are_components_equal(next_size, next_components, size, components))
@@ -335,33 +337,34 @@
                                         double scalar, double *result) {
   double scalar_high, scalar_low;
   split(scalar, &scalar_high, &scalar_low);
   double accumulator, tail;
   two_multiply_presplit(components[0], scalar, scalar_high, scalar_low,
                         &accumulator, &tail);
   size_t result_size = 0;
-  if (!!tail) result[result_size++] = tail;
+  if (tail != 0.0) result[result_size++] = tail;
   for (size_t index = 1; index < size; ++index) {
     double product, product_tail;
     two_multiply_presplit(components[index], scalar, scalar_high, scalar_low,
                           &product, &product_tail);
     double interim;
     two_add(accumulator, product_tail, &interim, &tail);
-    if (!!tail) result[result_size++] = tail;
+    if (tail != 0.0) result[result_size++] = tail;
     fast_two_add(product, interim, &accumulator, &tail);
-    if (!!tail) result[result_size++] = tail;
+    if (tail != 0.0) result[result_size++] = tail;
   }
-  if (!!accumulator || !result_size) result[result_size++] = accumulator;
+  if (accumulator != 0.0 || result_size == 0)
+    result[result_size++] = accumulator;
   return result_size;
 }
 
 static int scale_components(size_t size, double *components, double scalar,
                             size_t *result_size, double **result) {
   *result = (double *)PyMem_Malloc(2 * size * sizeof(double));
-  if (!*result) {
+  if (*result == NULL) {
     PyErr_NoMemory();
     return -1;
   }
   *result_size = scale_components_in_place(size, components, scalar, *result);
   if (!PyMem_Resize(*result, double, *result_size)) {
     PyErr_NoMemory();
     return -1;
@@ -370,19 +373,19 @@
 }
 
 static size_t subtract_double_in_place(size_t minuend_size, double *minuend,
                                        double subtrahend, double *result) {
   return add_double_in_place(minuend_size, minuend, -subtrahend, result);
 }
 
-static size_t subtract_double(size_t minuend_size, double *minuend,
-                              double subtrahend, size_t *result_size,
-                              double **result) {
+static int subtract_double(size_t minuend_size, double *minuend,
+                           double subtrahend, size_t *result_size,
+                           double **result) {
   *result = (double *)PyMem_Malloc((minuend_size + 1) * sizeof(double));
-  if (!*result) {
+  if (*result == NULL) {
     PyErr_NoMemory();
     return -1;
   }
   *result_size =
       subtract_double_in_place(minuend_size, minuend, subtrahend, *result);
   if (!PyMem_Resize(*result, double, *result_size)) {
     PyErr_NoMemory();
@@ -396,25 +399,26 @@
                                             double *subtrahend,
                                             double *result) {
   size_t result_size = 0;
   double accumulator = minuend;
   for (size_t index = 0; index < subtrahend_size; index++) {
     double tail;
     two_add(accumulator, -subtrahend[index], &accumulator, &tail);
-    if (!!tail) result[result_size++] = tail;
+    if (tail != 0.0) result[result_size++] = tail;
   }
-  if (!!accumulator || !result_size) result[result_size++] = accumulator;
+  if (accumulator != 0.0 || result_size == 0)
+    result[result_size++] = accumulator;
   return result_size;
 }
 
 static int subtract_from_double(double minuend, size_t subtrahend_size,
                                 double *subtrahend, size_t *result_size,
                                 double **result) {
   *result = (double *)PyMem_Malloc((subtrahend_size + 1) * sizeof(double));
-  if (!*result) {
+  if (*result == NULL) {
     PyErr_NoMemory();
     return -1;
   }
   *result_size = subtract_from_double_in_place(minuend, subtrahend_size,
                                                subtrahend, *result);
   if (!PyMem_Resize(*result, double, *result_size)) {
     PyErr_NoMemory();
@@ -448,47 +452,48 @@
       fast_two_add(left_component, accumulator, &head, &tail);
       left_component = left[++left_index];
     } else {
       fast_two_add(right_component, accumulator, &head, &tail);
       right_component = right[++right_index];
     }
     accumulator = head;
-    if (!!tail) result[result_size++] = tail;
+    if (tail != 0.0) result[result_size++] = tail;
     while ((left_index < left_size) && (right_index < right_size)) {
       if ((right_component > left_component) ==
           (right_component > -left_component)) {
         two_add(accumulator, left_component, &head, &tail);
         left_component = left[++left_index];
       } else {
         two_add(accumulator, right_component, &head, &tail);
         right_component = right[++right_index];
       }
       accumulator = head;
-      if (!!tail) result[result_size++] = tail;
+      if (tail != 0.0) result[result_size++] = tail;
     }
   }
   for (; left_index < left_size; ++left_index) {
     two_add(accumulator, left[left_index], &head, &tail);
     accumulator = head;
-    if (!!tail) result[result_size++] = tail;
+    if (tail != 0.0) result[result_size++] = tail;
   }
   for (; right_index < right_size; ++right_index) {
     two_add(accumulator, right[right_index], &head, &tail);
     accumulator = head;
-    if (!!tail) result[result_size++] = tail;
+    if (tail != 0.0) result[result_size++] = tail;
   }
-  if (!!accumulator || !result_size) result[result_size++] = accumulator;
+  if (accumulator != 0.0 || result_size == 0)
+    result[result_size++] = accumulator;
   return result_size;
 }
 
 static int add_components(const size_t left_size, const double *const left,
                           const size_t right_size, const double *const right,
                           size_t *result_size, double **result) {
   *result = (double *)PyMem_Malloc((left_size + right_size) * sizeof(double));
-  if (!*result) {
+  if (*result == NULL) {
     PyErr_NoMemory();
     return -1;
   }
   *result_size =
       add_components_in_place(left_size, left, right_size, right, *result);
   if (!PyMem_Resize(*result, double, *result_size)) {
     PyErr_NoMemory();
@@ -498,20 +503,20 @@
 }
 
 static size_t multiply_components_in_place(size_t left_size, double *left,
                                            size_t right_size, double *right,
                                            double *result) {
   double *next_components =
       (double *)PyMem_Malloc(2 * left_size * (right_size - 1) * sizeof(double));
-  if (!next_components) {
+  if (next_components == NULL) {
     PyErr_NoMemory();
     return 0;
   }
   double *step = (double *)PyMem_Malloc(2 * left_size * sizeof(double));
-  if (!step) {
+  if (step == NULL) {
     PyMem_Free(next_components);
     PyErr_NoMemory();
     return 0;
   }
   size_t result_size =
       scale_components_in_place(left_size, left, right[0], result);
   for (size_t index = 1; index < right_size; ++index) {
@@ -526,15 +531,15 @@
   return result_size;
 }
 
 static int multiply_components(size_t left_size, double *left,
                                size_t right_size, double *right,
                                size_t *result_size, double **result) {
   *result = (double *)PyMem_Malloc(2 * left_size * right_size * sizeof(double));
-  if (!*result) {
+  if (*result == NULL) {
     PyErr_NoMemory();
     return -1;
   }
   *result_size = left_size < right_size
                      ? multiply_components_in_place(right_size, right,
                                                     left_size, left, *result)
                      : multiply_components_in_place(left_size, left, right_size,
@@ -569,51 +574,52 @@
       fast_two_add(minuend_component, accumulator, &head, &tail);
       minuend_component = minuend[++minuend_index];
     } else {
       fast_two_add(subtrahend_component, accumulator, &head, &tail);
       subtrahend_component = -subtrahend[++subtrahend_index];
     }
     accumulator = head;
-    if (!!tail) result[result_size++] = tail;
+    if (tail != 0.0) result[result_size++] = tail;
     while ((minuend_index < minuend_size) &&
            (subtrahend_index < subtrahend_size)) {
       if ((subtrahend_component > minuend_component) ==
           (subtrahend_component > -minuend_component)) {
         two_add(accumulator, minuend_component, &head, &tail);
         minuend_component = minuend[++minuend_index];
       } else {
         two_add(accumulator, subtrahend_component, &head, &tail);
         subtrahend_component = -subtrahend[++subtrahend_index];
       }
       accumulator = head;
-      if (!!tail) result[result_size++] = tail;
+      if (tail != 0.0) result[result_size++] = tail;
     }
   }
   while (minuend_index < minuend_size) {
     two_add(accumulator, minuend_component, &head, &tail);
     minuend_component = minuend[++minuend_index];
     accumulator = head;
-    if (!!tail) result[result_size++] = tail;
+    if (tail != 0.0) result[result_size++] = tail;
   }
   while (subtrahend_index < subtrahend_size) {
     two_add(accumulator, subtrahend_component, &head, &tail);
     subtrahend_component = -subtrahend[++subtrahend_index];
     accumulator = head;
-    if (!!tail) result[result_size++] = tail;
+    if (tail != 0.0) result[result_size++] = tail;
   }
-  if (!!accumulator || !result_size) result[result_size++] = accumulator;
+  if (accumulator != 0.0 || result_size == 0)
+    result[result_size++] = accumulator;
   return result_size;
 }
 
 static int subtract_components(size_t minuend_size, double *minuend,
                                size_t subtrahend_size, double *subtrahend,
                                size_t *result_size, double **result) {
   *result =
       (double *)PyMem_Malloc((minuend_size + subtrahend_size) * sizeof(double));
-  if (!*result) {
+  if (*result == NULL) {
     PyErr_NoMemory();
     return -1;
   }
   *result_size = subtract_components_in_place(
       minuend_size, minuend, subtrahend_size, subtrahend, *result);
   if (!PyMem_Resize(*result, double, *result_size)) {
     PyErr_NoMemory();
@@ -625,54 +631,54 @@
 static int invert_components(const size_t size, double *const components,
                              size_t *result_size, double **result_components) {
   double first_approximation = 1.0 / components[size - 1];
   double first_approximation_high, first_approximation_low;
   split(first_approximation, &first_approximation_high,
         &first_approximation_low);
   if (!isfinite(first_approximation_high)) {
-    PyObject *components_object = PyList_New(size);
-    if (!components_object) return -1;
+    PyObject *components_object = PyList_New((Py_ssize_t)(size));
+    if (components_object == NULL) return -1;
     for (size_t index = 0; index < size; ++index) {
       PyObject *component_object = PyFloat_FromDouble(components[index]);
-      if (!component_object) {
+      if (component_object == NULL) {
         Py_DECREF(components_object);
         return -1;
       }
-      PyList_SET_ITEM(components_object, index, component_object);
+      PyList_SET_ITEM(components_object, (Py_ssize_t)(index), component_object);
     }
     PyErr_Format(PyExc_OverflowError,
                  "Components %R are not finitely invertible.",
                  components_object);
     Py_DECREF(components_object);
     return -1;
   }
   size_t iterations_count = 6 + ceil_log2(size);
   size_t max_result_size = (iterations_count - 1) * iterations_count *
                            (1 + 2 * size * (2 * iterations_count - 1) / 3);
   double *step_components =
       (double *)PyMem_Malloc(max_result_size * sizeof(double));
-  if (!step_components) return -1;
+  if (step_components == NULL) return -1;
   step_components[0] = first_approximation;
   size_t step_size = 1;
   double *negated_components = (double *)PyMem_Malloc(size * sizeof(double));
-  if (!negated_components) {
+  if (negated_components == NULL) {
     PyMem_Free(step_components);
     return -1;
   }
   size_t negated_size = negate_components(size, components, negated_components);
   double *tmp_components =
       (double *)PyMem_Malloc(max_result_size * sizeof(double));
-  if (!tmp_components) {
+  if (tmp_components == NULL) {
     PyMem_Free(negated_components);
     PyMem_Free(step_components);
     return -1;
   }
   double *other_tmp_components =
       (double *)PyMem_Malloc(max_result_size * sizeof(double));
-  if (!other_tmp_components) {
+  if (other_tmp_components == NULL) {
     PyMem_Free(tmp_components);
     PyMem_Free(negated_components);
     PyMem_Free(step_components);
     return -1;
   }
   for (size_t _ = 0; _ < iterations_count; ++_) {
     size_t tmp_size =
@@ -699,15 +705,15 @@
     }
     swap(&step_components, &tmp_components);
   }
   PyMem_Free(other_tmp_components);
   PyMem_Free(tmp_components);
   PyMem_Free(negated_components);
   step_size = compress_components(step_size, step_components);
-  if (!step_size) return 0;
+  if (step_size == 0) return 0;
   if (!PyMem_Resize(step_components, double, step_size)) {
     PyErr_NoMemory();
     return 0;
   }
   *result_size = step_size;
   *result_components = step_components;
   return 0;
@@ -721,100 +727,100 @@
   if (invert_components(divisor_size, divisor, &divisor_reciprocal_size,
                         &divisor_reciprocal) < 0)
     return -1;
   if (multiply_components(divisor_reciprocal_size, divisor_reciprocal,
                           dividend_size, dividend, result_size, result) < 0)
     return -1;
   PyMem_Free(divisor_reciprocal);
-  if (!*result_size) {
+  if (*result_size == 0) {
     PyMem_Free(*result);
     return -1;
   }
   *result_size = compress_components(*result_size, *result);
   if (!PyMem_Resize(*result, double, *result_size)) return -1;
   return 0;
 }
 
 static int is_PyLong_odd(PyObject *value) {
   PyObject *one = PyLong_FromLong(1);
-  if (!one) return -1;
+  if (one == NULL) return -1;
   PyObject *first_bit = PyNumber_And(value, one);
   Py_DECREF(one);
-  if (!first_bit) return -1;
+  if (first_bit == NULL) return -1;
   const int result = PyObject_IsTrue(first_bit);
   Py_DECREF(first_bit);
   return result;
 }
 
 static int is_PyLong_one(PyObject *value) {
   PyObject *one = PyLong_FromLong(1);
-  if (!one) return -1;
+  if (one == NULL) return -1;
   int result = PyObject_RichCompareBool(value, one, Py_EQ);
   Py_DECREF(one);
   return result;
 }
 
 static PyObject *components_to_PyLong(const size_t size,
                                       const double *const components) {
   PyObject *result = PyLong_FromDouble(components[size - 1]);
-  if (!result) return NULL;
+  if (result == NULL) return NULL;
   for (size_t offset = 2; offset <= size; ++offset) {
     PyObject *component_integer = PyLong_FromDouble(components[size - offset]);
-    if (!component_integer) {
+    if (component_integer == NULL) {
       Py_DECREF(result);
       return NULL;
     }
     if (PyObject_Not(component_integer)) break;
     PyObject *tmp = result;
     result = PyNumber_InPlaceAdd(result, component_integer);
     Py_DECREF(tmp);
     Py_DECREF(component_integer);
-    if (!result) return NULL;
+    if (result == NULL) return NULL;
   }
   return result;
 }
 
 static int PyLong_to_components(PyObject *value, size_t *size,
                                 double **components) {
   if (PyObject_Not(value)) {
     *components = (double *)PyMem_Malloc(sizeof(double));
-    if (!*components) {
+    if (*components == NULL) {
       PyErr_NoMemory();
       return -1;
     }
     *size = 1;
     *components[0] = 0.0;
     return 0;
   }
   PyObject *rest = PyNumber_Long(value);
-  if (!rest) return -1;
+  if (rest == NULL) return -1;
   double component = PyFloat_AsDouble(rest);
   if (component == -1.0 && PyErr_Occurred()) {
     Py_DECREF(rest);
     return -1;
   }
   assert(component >= 1.0 || component <= -1.0);
   int exponent;
   frexp(component, &exponent);
   size_t max_components_count = 1 + ((size_t)exponent - 1) / DBL_MANT_DIG;
   double *reversed_components =
       (double *)PyMem_Malloc(max_components_count * sizeof(double));
-  if (!reversed_components) {
+  if (reversed_components == NULL) {
     PyErr_NoMemory();
     return -1;
   }
   size_t result_size = 0;
   for (;;) {
     reversed_components[result_size++] = component;
     assert(result_size <= max_components_count);
     PyObject *component_integer = PyLong_FromDouble(component);
     PyObject *tmp = rest;
     rest = PyNumber_InPlaceSubtract(rest, component_integer);
     Py_DECREF(tmp);
-    if (!rest) {
+    if (rest == NULL) {
       PyMem_Free(reversed_components);
       return -1;
     }
     int is_zero = PyObject_Not(rest);
     if (is_zero < 0) {
       PyMem_Free(reversed_components);
       Py_DECREF(rest);
@@ -826,15 +832,15 @@
       PyMem_Free(reversed_components);
       Py_DECREF(rest);
       return -1;
     }
   }
   Py_DECREF(rest);
   *components = (double *)PyMem_Malloc(result_size * sizeof(double));
-  if (!*components) {
+  if (*components == NULL) {
     PyMem_Free(reversed_components);
     PyErr_NoMemory();
     return -1;
   }
   *size = result_size;
   for (size_t index = 0; index < result_size; ++index) {
     (*components)[result_size - 1 - index] = reversed_components[index];
@@ -842,17 +848,17 @@
   PyMem_Free(reversed_components);
   return 0;
 }
 
 static int Rational_to_components(PyObject *value, size_t *size,
                                   double **components) {
   PyObject *denominator = PyObject_GetAttrString(value, "denominator");
-  if (!denominator) return -1;
+  if (denominator == NULL) return -1;
   PyObject *numerator = PyObject_GetAttrString(value, "numerator");
-  if (!numerator) {
+  if (numerator == NULL) {
     Py_DECREF(denominator);
     return -1;
   }
   assert(PyLong_Check(denominator));
   assert(PyLong_Check(numerator));
   double *numerator_components;
   size_t numerator_size;
@@ -892,15 +898,15 @@
   PyMem_Free(denominator_components);
   return 0;
 }
 
 static int are_components_equal_to_PyLong(const size_t size,
                                           const double *const components,
                                           PyObject *value) {
-  if (do_components_have_fraction(size, components)) return 0;
+  if (do_components_have_fraction(components)) return 0;
   PyObject *components_integer = components_to_PyLong(size, components);
   int result = PyObject_RichCompareBool(components_integer, value, Py_EQ);
   Py_DECREF(components_integer);
   return result;
 }
 
 static int are_components_lesser_than_PyLong(const size_t size,
@@ -1022,15 +1028,15 @@
     double second_squared_length[4], double third_squared_length[4]) {
   double first_buffer_16[16], second_buffer_16[16], third_buffer_16[16];
   double first_buffer_32[32], second_buffer_32[32], buffer_48[48];
   size_t first_buffer_16_limit, second_buffer_16_limit, third_buffer_16_limit;
   size_t first_buffer_32_limit, second_buffer_32_limit, buffer_48_limit;
   size_t first_dx_tail_second_third_cross_product_size = 0;
   double first_dx_tail_second_third_cross_product[8];
-  if (!!first_dx_tail) {
+  if (first_dx_tail != 0.0) {
     first_dx_tail_second_third_cross_product_size =
         scale_components_in_place(4, second_third_cross_product, first_dx_tail,
                                   first_dx_tail_second_third_cross_product);
     first_buffer_16_limit =
         scale_components_in_place(first_dx_tail_second_third_cross_product_size,
                                   first_dx_tail_second_third_cross_product,
                                   2.0 * first_dx, first_buffer_16);
@@ -1057,15 +1063,15 @@
     final_size =
         add_components_in_place(final_size, *final_components, buffer_48_limit,
                                 buffer_48, *accumulated_components);
     swap(final_components, accumulated_components);
   }
   size_t first_dy_tail_second_third_cross_product_size = 0;
   double first_dy_tail_second_third_cross_product[8];
-  if (!!first_dy_tail) {
+  if (first_dy_tail != 0.0) {
     first_dy_tail_second_third_cross_product_size =
         scale_components_in_place(4, second_third_cross_product, first_dy_tail,
                                   first_dy_tail_second_third_cross_product);
     first_buffer_16_limit =
         scale_components_in_place(first_dy_tail_second_third_cross_product_size,
                                   first_dy_tail_second_third_cross_product,
                                   2.0 * first_dy, first_buffer_16);
@@ -1095,21 +1101,21 @@
     swap(final_components, accumulated_components);
   }
   double dx_tail_dy_head_head, dx_head_dy_tail_head;
   double dx_tail_dy_head_tail, dx_head_dy_tail_tail;
   double buffer_8[8], buffer_64[64];
   size_t buffer_8_limit, buffer_64_limit;
   double first_buffer_4[4], second_buffer_4[4];
-  if (!!first_dx_tail || !!first_dy_tail) {
+  if (first_dx_tail != 0.0 || first_dy_tail != 0.0) {
     size_t second_third_cross_product_bodies_size,
         second_third_cross_product_tails_size;
     double second_third_cross_product_bodies[8],
         second_third_cross_product_tails[4];
-    if (!!second_dx_tail || !!second_dy_tail || !!third_dx_tail ||
-        !!third_dy_tail) {
+    if (second_dx_tail != 0.0 || second_dy_tail != 0.0 ||
+        third_dx_tail != 0.0 || third_dy_tail != 0.0) {
       two_multiply(second_dx_tail, third_dy, &dx_tail_dy_head_head,
                    &dx_tail_dy_head_tail);
       two_multiply(second_dx, third_dy_tail, &dx_head_dy_tail_head,
                    &dx_head_dy_tail_tail);
       two_two_add(dx_tail_dy_head_head, dx_tail_dy_head_tail,
                   dx_head_dy_tail_head, dx_head_dy_tail_tail,
                   &first_buffer_4[3], &first_buffer_4[2], &first_buffer_4[1],
@@ -1138,15 +1144,15 @@
       second_third_cross_product_tails_size = 4;
     } else {
       second_third_cross_product_bodies[0] = 0.0;
       second_third_cross_product_bodies_size = 1;
       second_third_cross_product_tails[0] = 0.0;
       second_third_cross_product_tails_size = 1;
     }
-    if (!!first_dx_tail) {
+    if (first_dx_tail != 0.0) {
       first_buffer_16_limit = scale_components_in_place(
           first_dx_tail_second_third_cross_product_size,
           first_dx_tail_second_third_cross_product, first_dx_tail,
           first_buffer_16);
       double first_dx_tail_second_third_cross_product_bodies[16];
       size_t first_dx_tail_second_third_cross_product_bodies_size =
           scale_components_in_place(
@@ -1160,25 +1166,25 @@
       buffer_48_limit = add_components_in_place(
           first_buffer_16_limit, first_buffer_16, first_buffer_32_limit,
           first_buffer_32, buffer_48);
       final_size = add_components_in_place(final_size, *final_components,
                                            buffer_48_limit, buffer_48,
                                            *accumulated_components);
       swap(final_components, accumulated_components);
-      if (!!second_dy_tail) {
+      if (second_dy_tail != 0.0) {
         buffer_8_limit = scale_components_in_place(4, third_squared_length,
                                                    first_dx_tail, buffer_8);
         first_buffer_16_limit = scale_components_in_place(
             buffer_8_limit, buffer_8, second_dy_tail, first_buffer_16);
         final_size = add_components_in_place(
             final_size, *final_components, first_buffer_16_limit,
             first_buffer_16, *accumulated_components);
         swap(final_components, accumulated_components);
       }
-      if (!!third_dy_tail) {
+      if (third_dy_tail != 0.0) {
         buffer_8_limit = scale_components_in_place(4, second_squared_length,
                                                    -first_dx_tail, buffer_8);
         first_buffer_16_limit = scale_components_in_place(
             buffer_8_limit, buffer_8, third_dy_tail, first_buffer_16);
         final_size = add_components_in_place(
             final_size, *final_components, first_buffer_16_limit,
             first_buffer_16, *accumulated_components);
@@ -1209,15 +1215,15 @@
           first_buffer_32_limit, first_buffer_32, second_buffer_32_limit,
           second_buffer_32, buffer_64);
       final_size = add_components_in_place(final_size, *final_components,
                                            buffer_64_limit, buffer_64,
                                            *accumulated_components);
       swap(final_components, accumulated_components);
     }
-    if (!!first_dy_tail) {
+    if (first_dy_tail != 0.0) {
       first_buffer_16_limit = scale_components_in_place(
           first_dy_tail_second_third_cross_product_size,
           first_dy_tail_second_third_cross_product, first_dy_tail,
           first_buffer_16);
       double first_dy_tail_second_third_cross_product_bodies[16];
       size_t first_dy_tail_second_third_cross_product_bodies_size =
           scale_components_in_place(
@@ -1316,16 +1322,16 @@
   if ((result >= threshold) || (-result >= threshold)) return result;
   double first_dx_tail = two_subtract_tail(first_x, point_x, first_dx);
   double first_dy_tail = two_subtract_tail(first_y, point_y, first_dy);
   double second_dx_tail = two_subtract_tail(second_x, point_x, second_dx);
   double second_dy_tail = two_subtract_tail(second_y, point_y, second_dy);
   double third_dx_tail = two_subtract_tail(third_x, point_x, third_dx);
   double third_dy_tail = two_subtract_tail(third_y, point_y, third_dy);
-  if (!first_dx_tail && !second_dx_tail && !third_dx_tail && !first_dy_tail &&
-      !second_dy_tail && !third_dy_tail)
+  if (first_dx_tail == 0.0 && second_dx_tail == 0.0 && third_dx_tail == 0.0 &&
+      first_dy_tail == 0.0 && second_dy_tail == 0.0 && third_dy_tail == 0.0)
     return result;
   static const double second_upper_bound_coefficient =
       (44.0 + 576.0 * EPSILON) * EPSILON * EPSILON;
   static const double result_coefficient = (3.0 + 8.0 * EPSILON) * EPSILON;
   threshold = second_upper_bound_coefficient * upper_bound +
               result_coefficient * fabs(result);
   result += ((first_dx * first_dx + first_dy * first_dy) *
@@ -1341,27 +1347,28 @@
             ((third_dx * third_dx + third_dy * third_dy) *
                  ((first_dx * second_dy_tail + second_dy * first_dx_tail) -
                   (first_dy * second_dx_tail + second_dx * first_dy_tail)) +
              2.0 * (third_dx * third_dx_tail + third_dy * third_dy_tail) *
                  (first_dx * second_dy - first_dy * second_dx));
   if ((result >= threshold) || (-result >= threshold)) return result;
   double first_squared_length[4] = {0};
-  if (!!second_dx_tail || !!second_dy_tail || !!third_dx_tail ||
-      !!third_dy_tail)
+  if (second_dx_tail != 0.0 || second_dy_tail != 0.0 || third_dx_tail != 0.0 ||
+      third_dy_tail != 0.0)
     squared_length(first_dx, first_dy, &first_squared_length[3],
                    &first_squared_length[2], &first_squared_length[1],
                    &first_squared_length[0]);
   double second_squared_length[4] = {0};
-  if (!!third_dx_tail || !!third_dy_tail || !!first_dx_tail || !!first_dy_tail)
+  if (third_dx_tail != 0.0 || third_dy_tail != 0.0 || first_dx_tail != 0.0 ||
+      first_dy_tail != 0.0)
     squared_length(second_dx, second_dy, &second_squared_length[3],
                    &second_squared_length[2], &second_squared_length[1],
                    &second_squared_length[0]);
   double third_squared_length[4] = {0};
-  if (!!first_dx_tail || !!first_dy_tail || !!second_dx_tail ||
-      !!second_dy_tail)
+  if (first_dx_tail != 0.0 || first_dy_tail != 0.0 || second_dx_tail != 0.0 ||
+      second_dy_tail != 0.0)
     squared_length(third_dx, third_dy, &third_squared_length[3],
                    &third_squared_length[2], &third_squared_length[1],
                    &third_squared_length[0]);
   double *final_components = first_buffer;
   double second_buffer_1152[1152];
   double *accumulated_components = second_buffer_1152;
   final_size = add_extras(final_size, &final_components,
@@ -1447,16 +1454,16 @@
       two_subtract_tail(first_end_x, first_start_x, minuend_x);
   double subtrahend_x_tail =
       two_subtract_tail(second_end_x, second_start_x, subtrahend_x);
   double minuend_y_tail =
       two_subtract_tail(first_end_y, first_start_y, minuend_y);
   double subtrahend_y_tail =
       two_subtract_tail(second_end_y, second_start_y, subtrahend_y);
-  if (!minuend_x_tail && !minuend_y_tail && !subtrahend_x_tail &&
-      !subtrahend_y_tail)
+  if (minuend_x_tail == 0.0 && minuend_y_tail == 0.0 &&
+      subtrahend_x_tail == 0.0 && subtrahend_y_tail == 0.0)
     return result;
   static const double second_upper_bound_coefficient =
       (9.0 + 64.0 * EPSILON) * EPSILON * EPSILON;
   static const double result_coefficient = (3.0 + 8.0 * EPSILON) * EPSILON;
   threshold = second_upper_bound_coefficient * upper_bound +
               result_coefficient * fabs(result);
   result += (minuend_x * subtrahend_y_tail + subtrahend_y * minuend_x_tail) -
@@ -1564,16 +1571,16 @@
       two_subtract_tail(first_end_x, first_start_x, minuend_x);
   double subtrahend_x_tail =
       two_subtract_tail(second_end_x, second_start_x, subtrahend_x);
   double minuend_y_tail =
       two_subtract_tail(first_end_y, first_start_y, minuend_y);
   double subtrahend_y_tail =
       two_subtract_tail(second_end_y, second_start_y, subtrahend_y);
-  if (!minuend_x_tail && !minuend_y_tail && !subtrahend_x_tail &&
-      !subtrahend_y_tail) {
+  if (minuend_x_tail == 0.0 && minuend_y_tail == 0.0 &&
+      subtrahend_x_tail == 0.0 && subtrahend_y_tail == 0.0) {
     size_t result_size = compress_components_single(4, first_components);
     copy_components(result_size, first_components, result);
     return result_size;
   }
   static const double second_upper_bound_coefficient =
       (9.0 + 64.0 * EPSILON) * EPSILON * EPSILON;
   static const double estimation_coefficient = (3.0 + 8.0 * EPSILON) * EPSILON;
@@ -1681,15 +1688,15 @@
                      "Components should be finite, but found: %R.", component);
         Py_DECREF(component);
       }
       PyMem_Free(components);
       return NULL;
     }
   ExpansionObject *result = (ExpansionObject *)(cls->tp_alloc(cls, 0));
-  if (result) {
+  if (result != NULL) {
     result->components = components;
     result->size = size;
   } else
     PyMem_Free(components);
   return result;
 }
 
@@ -1700,15 +1707,15 @@
   double *result_components =
       (double *)PyMem_Malloc((self->size + other->size) * sizeof(double));
   size_t result_size;
   if (add_components(self->size, self->components, other->size,
                      other->components, &result_size, &result_components) < 0)
     return NULL;
   result_size = compress_components(result_size, result_components);
-  if (!result_size) {
+  if (result_size == 0) {
     PyMem_Free(result_components);
     return NULL;
   }
   if (!PyMem_Resize(result_components, double, result_size))
     return (ExpansionObject *)PyErr_NoMemory();
   return construct_Expansion(&ExpansionType, result_size, result_components);
 }
@@ -1772,15 +1779,15 @@
                                             (ExpansionObject *)other)
                : Expansion_PyObject_add((ExpansionObject *)self, other);
   else
     return Expansion_PyObject_add((ExpansionObject *)other, self);
 }
 
 static int Expansion_bool(ExpansionObject *self) {
-  return !!self->components[self->size - 1];
+  return self->components[self->size - 1] != 0.0;
 }
 
 static void Expansion_dealloc(ExpansionObject *self) {
   PyMem_Free(self->components);
   Py_TYPE(self)->tp_free((PyObject *)self);
 }
 
@@ -1789,20 +1796,20 @@
          self->components[self->size - 1]);
   return self->components[self->size - 1];
 }
 
 static PyObject *Expansion_ceil(ExpansionObject *self,
                                 PyObject *Py_UNUSED(args)) {
   PyObject *result = components_to_PyLong(self->size, self->components);
-  if (!result) return NULL;
+  if (result == NULL) return NULL;
   double fraction =
       components_to_accumulated_fraction(self->size, self->components);
   assert(fabs(fraction) < 1.0);
   PyObject *fraction_ceil = PyLong_FromLong((long)ceil(fraction));
-  if (!fraction_ceil) {
+  if (fraction_ceil == NULL) {
     Py_DECREF(result);
     return NULL;
   }
   PyObject *tmp = result;
   result = PyNumber_InPlaceAdd(result, fraction_ceil);
   Py_DECREF(tmp);
   Py_DECREF(fraction_ceil);
@@ -1812,50 +1819,50 @@
 static PyObject *Expansion_float(ExpansionObject *self) {
   return PyFloat_FromDouble(Expansion_double(self));
 }
 
 static PyObject *Expansion_floor(ExpansionObject *self,
                                  PyObject *Py_UNUSED(args)) {
   PyObject *result = components_to_PyLong(self->size, self->components);
-  if (!result) return NULL;
+  if (result == NULL) return NULL;
   double fraction =
       components_to_accumulated_fraction(self->size, self->components);
   assert(fabs(fraction) < 1.0);
   PyObject *fraction_floor = PyLong_FromLong((long)floor(fraction));
-  if (!fraction_floor) {
+  if (fraction_floor == NULL) {
     Py_DECREF(result);
     return NULL;
   }
   PyObject *tmp = result;
   result = PyNumber_InPlaceAdd(result, fraction_floor);
   Py_DECREF(tmp);
   Py_DECREF(fraction_floor);
   return result;
 }
 
 static PyObject *Expansion_getnewargs(ExpansionObject *self,
                                       PyObject *Py_UNUSED(args)) {
-  PyObject *result = PyTuple_New(self->size);
-  if (!result) return NULL;
+  PyObject *result = PyTuple_New((Py_ssize_t)(self->size));
+  if (result == NULL) return NULL;
   for (size_t index = 0; index < self->size; ++index) {
     PyObject *component = PyFloat_FromDouble(self->components[index]);
-    if (!component) {
+    if (component == NULL) {
       Py_DECREF(component);
       return NULL;
     }
-    PyTuple_SET_ITEM(result, index, component);
+    PyTuple_SET_ITEM(result, (Py_ssize_t)(index), component);
   }
   return result;
 }
 
 static Py_hash_t Expansion_hash(ExpansionObject *self) {
-  PyObject *components = PyTuple_New(self->size);
-  if (!components) return -1;
+  PyObject *components = PyTuple_New((Py_ssize_t)(self->size));
+  if (components == NULL) return -1;
   for (size_t index = 0; index < self->size; ++index)
-    PyTuple_SET_ITEM(components, index,
+    PyTuple_SET_ITEM(components, (Py_ssize_t)(index),
                      PyFloat_FromDouble(self->components[index]));
   Py_hash_t result = PyObject_Hash(components);
   Py_DECREF(components);
   return result;
 }
 
 static ExpansionObject *Expansions_multiply(ExpansionObject *self,
@@ -1863,15 +1870,15 @@
   double *result_components;
   size_t result_size;
   if (multiply_components(self->size, self->components, other->size,
                           other->components, &result_size,
                           &result_components) < 0)
     return NULL;
   result_size = compress_components(result_size, result_components);
-  if (!result_size) {
+  if (result_size == 0) {
     PyMem_Free(result_components);
     return NULL;
   }
   if (!PyMem_Resize(result_components, double, result_size))
     return (ExpansionObject *)PyErr_NoMemory();
   return construct_Expansion(&ExpansionType, result_size, result_components);
 }
@@ -1880,15 +1887,15 @@
                                                   double other) {
   double *result_components;
   size_t result_size;
   if (scale_components(self->size, self->components, other, &result_size,
                        &result_components) < 0)
     return NULL;
   result_size = compress_components(result_size, result_components);
-  if (!result_size) {
+  if (result_size == 0) {
     PyMem_Free(result_components);
     return NULL;
   }
   if (!PyMem_Resize(result_components, double, result_size))
     return (ExpansionObject *)PyErr_NoMemory();
   return construct_Expansion(&ExpansionType, result_size, result_components);
 }
@@ -1951,27 +1958,27 @@
   Py_DECREF(tmp);
   return result;
 }
 
 static int normalize_fraction_components(PyObject **result_numerator,
                                          PyObject **result_denominator) {
   PyObject *gcd = _PyLong_GCD(*result_numerator, *result_denominator);
-  if (!gcd) return -1;
+  if (gcd == NULL) return -1;
   int is_gcd_unit = is_unit_Object(gcd);
   if (is_gcd_unit < 0) {
     Py_DECREF(gcd);
     return -1;
   } else if (!is_gcd_unit) {
     PyObject *numerator = PyNumber_FloorDivide(*result_numerator, gcd);
-    if (!numerator) {
+    if (numerator == NULL) {
       Py_DECREF(gcd);
       return -1;
     }
     PyObject *denominator = PyNumber_FloorDivide(*result_denominator, gcd);
-    if (!denominator) {
+    if (denominator == NULL) {
       Py_DECREF(numerator);
       Py_DECREF(gcd);
       return -1;
     }
     PyObject *tmp = *result_numerator;
     *result_numerator = numerator;
     Py_DECREF(tmp);
@@ -1986,18 +1993,18 @@
 static int fractions_components_add(PyObject *numerator, PyObject *denominator,
                                     PyObject *other_numerator,
                                     PyObject *other_denominator,
                                     PyObject **result_numerator,
                                     PyObject **result_denominator) {
   PyObject *first_result_numerator_component =
       PyNumber_Multiply(numerator, other_denominator);
-  if (!first_result_numerator_component) return -1;
+  if (first_result_numerator_component == NULL) return -1;
   PyObject *second_result_numerator_component =
       PyNumber_Multiply(other_numerator, denominator);
-  if (!second_result_numerator_component) {
+  if (second_result_numerator_component == NULL) {
     Py_DECREF(first_result_numerator_component);
     return -1;
   }
   *result_numerator = PyNumber_Add(first_result_numerator_component,
                                    second_result_numerator_component);
   Py_DECREF(second_result_numerator_component);
   Py_DECREF(first_result_numerator_component);
@@ -2012,18 +2019,19 @@
     Py_DECREF(*result_numerator);
     return -1;
   }
   return 0;
 }
 
 static PyObject *double_as_integer_ratio(double value) {
-  PyObject *as_integer_ratio_method_name = PyUnicode_FromString("as_integer_ratio");
-  if (!as_integer_ratio_method_name) return NULL;
+  PyObject *as_integer_ratio_method_name =
+      PyUnicode_FromString("as_integer_ratio");
+  if (as_integer_ratio_method_name == NULL) return NULL;
   PyObject *tmp = PyFloat_FromDouble(value);
-  PyObject* result =
+  PyObject *result =
 #if PY39_OR_MORE
       PyObject_CallMethodNoArgs(tmp, as_integer_ratio_method_name);
 #else
       PyObject_CallMethodObjArgs(tmp, as_integer_ratio_method_name, NULL)
 #endif
   ;
   Py_DECREF(tmp);
@@ -2076,58 +2084,58 @@
   size_t size = (size_t)raw_size;
   if (size == 1) {
     PyObject *argument = PyTuple_GET_ITEM(args, 0);
     if (PyObject_TypeCheck(argument, &ExpansionType)) {
       ExpansionObject *expansion_argument = (ExpansionObject *)argument;
       components =
           (double *)PyMem_Malloc(expansion_argument->size * sizeof(double));
-      if (!components) return NULL;
+      if (components == NULL) return NULL;
       copy_components(expansion_argument->size, expansion_argument->components,
                       components);
       size = expansion_argument->size;
     } else if (PyFloat_Check(argument)) {
       components = (double *)PyMem_Malloc(sizeof(double));
-      if (!components) return PyErr_NoMemory();
+      if (components == NULL) return PyErr_NoMemory();
       components[0] = PyFloat_AS_DOUBLE(argument);
       size = 1;
     } else if (PyLong_Check(argument)) {
       if (PyLong_to_components(argument, &size, &components) < 0) return NULL;
     } else if (PyObject_IsInstance(argument, Rational)) {
       if (Rational_to_components(argument, &size, &components) < 0) return NULL;
     } else {
       PyErr_Format(PyExc_TypeError,
                    "Argument should be of type %R, `Rational` or `float`, but "
                    "found: %R.",
                    &ExpansionType, Py_TYPE(argument));
       return NULL;
     }
-  } else if (size) {
+  } else if (size != 0) {
     components = (double *)PyMem_Malloc(size * sizeof(double));
-    if (!components) return PyErr_NoMemory();
+    if (components == NULL) return PyErr_NoMemory();
     for (size_t index = 0; index < size; ++index) {
       PyObject *item = PyTuple_GET_ITEM(args, index);
-      if (!item) {
+      if (item == NULL) {
         PyMem_Free(components);
         return NULL;
       }
       if (!PyFloat_Check(item)) {
         PyErr_Format(PyExc_TypeError,
                      "Components should be of type `float`, but found: %R.",
                      Py_TYPE(item));
         PyMem_Free(components);
         return NULL;
       }
       components[index] = PyFloat_AS_DOUBLE(item);
     }
     size = compress_components(size, components);
-    if (!size) return NULL;
+    if (size == 0) return NULL;
     if (!PyMem_Resize(components, double, size)) return PyErr_NoMemory();
   } else {
     components = (double *)PyMem_Malloc(sizeof(double));
-    if (!components) return PyErr_NoMemory();
+    if (components == NULL) return PyErr_NoMemory();
     components[0] = 0.0;
     size = 1;
   }
   return (PyObject *)construct_Expansion(cls, size, components);
 }
 
 static ExpansionObject *Expansion_negative(ExpansionObject *self) {
@@ -2147,35 +2155,36 @@
   return self->components[self->size - 1] < 0.0 ? Expansion_negative(self)
                                                 : Expansion_positive(self);
 }
 
 static PyObject *Expansion_repr(ExpansionObject *self) {
   PyObject *result;
   if (self->size > 1) {
-    PyObject *components_reprs = PyTuple_New(self->size);
-    if (!components_reprs) return NULL;
+    PyObject *components_reprs = PyTuple_New((Py_ssize_t)(self->size));
+    if (components_reprs == NULL) return NULL;
     for (size_t index = 0; index < self->size; ++index) {
       PyObject *item = PyFloat_FromDouble(self->components[index]);
-      if (!item) {
+      if (item == NULL) {
         Py_DECREF(components_reprs);
         return NULL;
       }
-      PyTuple_SET_ITEM(components_reprs, index, PyObject_Repr(item));
+      PyTuple_SET_ITEM(components_reprs, (Py_ssize_t)(index),
+                       PyObject_Repr(item));
       Py_DECREF(item);
     }
     PyObject *separator = PyUnicode_FromString(", ");
-    if (!separator) {
+    if (separator == NULL) {
       Py_DECREF(components_reprs);
       return NULL;
     }
     PyObject *joined_components_reprs =
         PyUnicode_Join(separator, components_reprs);
     Py_DECREF(separator);
     Py_DECREF(components_reprs);
-    if (!joined_components_reprs) return NULL;
+    if (joined_components_reprs == NULL) return NULL;
     result = PyUnicode_FromFormat("Expansion(%U)", joined_components_reprs);
     Py_DECREF(joined_components_reprs);
   } else {
     PyObject *head = PyFloat_FromDouble(self->components[0]);
     result = PyUnicode_FromFormat("Expansion(%R)", head);
     Py_DECREF(head);
   }
@@ -2298,15 +2307,15 @@
     return Expansion_Rational_richcompare(self, other, op);
   else
     Py_RETURN_NOTIMPLEMENTED;
 }
 
 static PyObject *Expansion_round_plain(ExpansionObject *self) {
   PyObject *result = components_to_PyLong(self->size, self->components);
-  if (!result) return NULL;
+  if (result == NULL) return NULL;
   size_t fractions_size;
   double *fractions_components;
   if (components_to_fractions(self->size, self->components, &fractions_size,
                               &fractions_components) < 0) {
     Py_DECREF(result);
     return NULL;
   }
@@ -2315,15 +2324,15 @@
       are_components_equal_to_double(fractions_size, fractions_components,
                                      -0.5)) {
     double fraction =
         components_to_accumulated_fraction(self->size, self->components);
     if ((fraction > 0.0 && Py_SIZE(result) < 0) ||
         (fraction < 0.0 && Py_SIZE(result) > 0)) {
       PyObject *sign = PyLong_FromLong(Py_SIZE(result) > 0 ? 1 : -1);
-      if (!sign) {
+      if (sign == NULL) {
         Py_DECREF(result);
         return NULL;
       }
       PyObject *tmp = result;
       result = PyNumber_InPlaceSubtract(result, sign);
       Py_DECREF(tmp);
       Py_DECREF(sign);
@@ -2331,15 +2340,15 @@
     const int is_truncation_odd = is_PyLong_odd(result);
     if (is_truncation_odd < 0) {
       Py_DECREF(result);
       return NULL;
     }
     if (is_truncation_odd) {
       PyObject *sign = PyLong_FromLong(Py_SIZE(result) > 0 ? 1 : -1);
-      if (!sign) {
+      if (sign == NULL) {
         Py_DECREF(result);
         return NULL;
       }
       PyObject *tmp = result;
       result = PyNumber_InPlaceAdd(result, sign);
       Py_DECREF(tmp);
       Py_DECREF(sign);
@@ -2349,68 +2358,68 @@
              is_double_lesser_than_components(0.5, fractions_size,
                                               fractions_components)) {
     PyObject *sign =
         PyLong_FromLong(is_double_lesser_than_components(0.0, fractions_size,
                                                          fractions_components)
                             ? 1
                             : -1);
-    if (!sign) {
+    if (sign == NULL) {
       Py_DECREF(result);
       return NULL;
     }
     PyObject *tmp = result;
     result = PyNumber_InPlaceAdd(result, sign);
     Py_DECREF(tmp);
     Py_DECREF(sign);
   }
   return result;
 }
 
 static PyObject *Expansion_round(ExpansionObject *self, PyObject *args) {
   PyObject *precision = NULL;
   if (!PyArg_ParseTuple(args, "|O", &precision)) return NULL;
-  if (!precision) return Expansion_round_plain(self);
+  if (precision == NULL) return Expansion_round_plain(self);
   const size_t size = self->size;
   double *const components = self->components;
   size_t result_size = size;
   double *result_components =
       (double *)PyMem_Malloc(result_size * sizeof(double));
-  if (!result_components) {
+  if (result_components == NULL) {
     Py_DECREF(precision);
     return PyErr_NoMemory();
   }
   PyObject *round_args = PyTuple_New(2);
-  if (!round_args) {
+  if (round_args == NULL) {
     Py_DECREF(precision);
     PyMem_Free(result_components);
     return NULL;
   }
   Py_INCREF(precision);
   PyTuple_SET_ITEM(round_args, 1, precision);
   for (size_t index = 0; index < self->size; ++index) {
     PyObject *component = PyFloat_FromDouble(components[index]);
-    if (!component) {
+    if (component == NULL) {
       Py_DECREF(round_args);
       PyMem_Free(result_components);
       return NULL;
     }
     PyTuple_SET_ITEM(round_args, 0, component);
     PyObject *rounded_component =
         PyObject_CallObject(PyFloat_round, round_args);
-    if (!rounded_component) {
+    if (rounded_component == NULL) {
       Py_DECREF(round_args);
       PyMem_Free(result_components);
       return NULL;
     }
     result_components[index] = PyFloat_AS_DOUBLE(rounded_component);
     Py_DECREF(rounded_component);
   }
   Py_DECREF(round_args);
   result_size = compress_components(result_size, result_components);
-  if (!result_size) {
+  if (result_size == 0) {
     PyMem_Free(result_components);
     return NULL;
   }
   if (!PyMem_Resize(result_components, double, result_size))
     return PyErr_NoMemory();
   return (PyObject *)construct_Expansion(&ExpansionType, result_size,
                                          result_components);
@@ -2659,20 +2668,20 @@
   }
   PyMem_Free(components);
   return construct_Expansion(&ExpansionType, result_size, result_components);
 }
 
 static ExpansionObject *Expansion_double_true_divide(ExpansionObject *self,
                                                      double other) {
-  if (!other) {
+  if (other == 0.0) {
     PyErr_Format(PyExc_ZeroDivisionError, "Divisor is zero.");
     return NULL;
   }
   double *other_components = (double *)PyMem_Malloc(sizeof(double));
-  if (!other_components) return (ExpansionObject *)PyErr_NoMemory();
+  if (other_components == NULL) return (ExpansionObject *)PyErr_NoMemory();
   other_components[0] = other;
   double *result_components;
   size_t result_size;
   if (divide_components(self->size, self->components, 1, other_components,
                         &result_size, &result_components) < 0) {
     PyMem_Free(other_components);
     return NULL;
@@ -2684,15 +2693,15 @@
 static ExpansionObject *double_Expansion_true_divide(double self,
                                                      ExpansionObject *other) {
   if (!Expansion_bool(other)) {
     PyErr_Format(PyExc_ZeroDivisionError, "Divisor is zero.");
     return NULL;
   }
   double *components = (double *)PyMem_Malloc(sizeof(double));
-  if (!components) return (ExpansionObject *)PyErr_NoMemory();
+  if (components == NULL) return (ExpansionObject *)PyErr_NoMemory();
   components[0] = self;
   double *result_components;
   size_t result_size;
   if (divide_components(1, components, other->size, other->components,
                         &result_size, &result_components) < 0) {
     PyMem_Free(components);
     return NULL;
@@ -2726,15 +2735,15 @@
                                                       (ExpansionObject *)other);
   Py_RETURN_NOTIMPLEMENTED;
 }
 
 static PyObject *Expansion_trunc(ExpansionObject *self,
                                  PyObject *Py_UNUSED(args)) {
   PyObject *result = components_to_PyLong(self->size, self->components);
-  if (!result) return NULL;
+  if (result == NULL) return NULL;
   double fraction =
       components_to_accumulated_fraction(self->size, self->components);
   if ((fraction < 0.0 && Py_SIZE(result) > 0) ||
       (fraction > 0.0 && Py_SIZE(result) < 0)) {
     PyObject *sign = PyLong_FromLong(Py_SIZE(result) > 0 ? 1 : -1);
     result = PyNumber_InPlaceSubtract(result, sign);
     Py_DECREF(sign);
@@ -2750,39 +2759,55 @@
     .nb_multiply = Expansion_multiply,
     .nb_negative = (unaryfunc)Expansion_negative,
     .nb_positive = (unaryfunc)Expansion_positive,
     .nb_subtract = Expansion_subtract,
     .nb_true_divide = Expansion_true_divide,
 };
 
-PyObject *Expansion_getimag(ExpansionObject *self, void *closure) {
+PyObject *Expansion_getimag(ExpansionObject *Py_UNUSED(self),
+                            void *Py_UNUSED(closure)) {
   return PyLong_FromLong(0);
 }
 
-PyObject *Expansion_getreal(ExpansionObject *self, void *closure) {
+PyObject *Expansion_getreal(ExpansionObject *self, void *Py_UNUSED(closure)) {
   return (PyObject *)Expansion_positive(self);
 }
 
+#ifdef __GNUC__
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wmissing-field-initializers"
+#endif
 static PyGetSetDef Expansion_getset[] = {
     {"real", (getter)Expansion_getreal, (setter)NULL,
      "The real part of the expansion.", NULL},
     {"imag", (getter)Expansion_getimag, (setter)NULL,
      "The imaginary part of the expansion.", NULL},
-    {NULL} /* Sentinel */
+    {NULL} /* sentinel */
 };
+#ifdef __GNUC__
+#pragma GCC diagnostic pop
+#endif
 
+#ifdef __GNUC__
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wmissing-field-initializers"
+#endif
 static PyMethodDef Expansion_methods[] = {
-    {"as_integer_ratio", (PyCFunction)Expansion_as_integer_ratio, METH_NOARGS, NULL},
+    {"as_integer_ratio", (PyCFunction)Expansion_as_integer_ratio, METH_NOARGS,
+     NULL},
     {"__ceil__", (PyCFunction)Expansion_ceil, METH_NOARGS, NULL},
     {"__floor__", (PyCFunction)Expansion_floor, METH_NOARGS, NULL},
     {"__getnewargs__", (PyCFunction)Expansion_getnewargs, METH_NOARGS, NULL},
     {"__round__", (PyCFunction)Expansion_round, METH_VARARGS, NULL},
     {"__trunc__", (PyCFunction)Expansion_trunc, METH_NOARGS, NULL},
     {NULL, NULL} /* sentinel */
 };
+#ifdef __GNUC__
+#pragma GCC diagnostic pop
+#endif
 
 static PyTypeObject ExpansionType = {
     PyVarObject_HEAD_INIT(NULL, 0).tp_as_number = &Expansion_as_number,
     .tp_basicsize = sizeof(ExpansionObject),
     .tp_dealloc = (destructor)Expansion_dealloc,
     .tp_doc = PyDoc_STR("Represents floating point number expansion."),
     .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE,
@@ -2838,15 +2863,15 @@
     return NULL;
   double components[16];
   size_t result_size = vectors_cross_product_impl(
       first_start_x, first_start_y, first_end_x, first_end_y, second_start_x,
       second_start_y, second_end_x, second_end_y, components);
   double *result_components =
       (double *)PyMem_Malloc(result_size * sizeof(double));
-  if (!result_components) return PyErr_NoMemory();
+  if (result_components == NULL) return PyErr_NoMemory();
   copy_components(result_size, components, result_components);
   return (PyObject *)construct_Expansion(&ExpansionType, result_size,
                                          result_components);
 }
 
 static PyObject *vectors_dot_product(PyObject *Py_UNUSED(self),
                                      PyObject *args) {
@@ -2858,20 +2883,24 @@
     return NULL;
   double components[16];
   size_t result_size = vectors_cross_product_impl(
       first_start_x, first_start_y, first_end_x, first_end_y, -second_start_y,
       second_start_x, -second_end_y, second_end_x, components);
   double *result_components =
       (double *)PyMem_Malloc(result_size * sizeof(double));
-  if (!result_components) return PyErr_NoMemory();
+  if (result_components == NULL) return PyErr_NoMemory();
   copy_components(result_size, components, result_components);
   return (PyObject *)construct_Expansion(&ExpansionType, result_size,
                                          result_components);
 }
 
+#ifdef __GNUC__
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wmissing-field-initializers"
+#endif
 static PyMethodDef _cshewchuk_methods[] = {
     {"incircle_test", incircle_test, METH_VARARGS,
      PyDoc_STR("incircle_test(point_x, point_y, first_x, first_y, second_x, "
                "second_y, third_x, third_y, /)\n--\n\n"
                "Computes location  of point relative to a circle formed by "
                "three others given their coordinates.")},
     {"kind", kind, METH_VARARGS,
@@ -2891,59 +2920,62 @@
                "coordinates.")},
     {"vectors_dot_product", vectors_dot_product, METH_VARARGS,
      PyDoc_STR("vectors_dot_product(first_start_x, first_start_y, first_end_x, "
                "first_end_y, second_start_x, second_start_y, second_end_x, "
                "second_end_y, /)\n--\n\n"
                "Computes dot product of two vectors given their endpoints "
                "coordinates.")},
-    {NULL, NULL},
+    {NULL, NULL}, /* sentinel */
 };
+#ifdef __GNUC__
+#pragma GCC diagnostic pop
+#endif
 
 static PyModuleDef _cshewchuk_module = {
     PyModuleDef_HEAD_INIT,
     .m_doc = PyDoc_STR("Robust floating point operations."),
     .m_methods = _cshewchuk_methods,
     .m_name = "shewchuk",
     .m_size = -1,
 };
 
 static int load_PyFloat_round() {
   PyFloat_round = PyDict_GetItemString(PyFloat_Type.tp_dict, "__round__");
-  return !PyFloat_round ? -1 : 0;
+  return PyFloat_round == NULL ? -1 : 0;
 }
 
 static int load_number_interfaces() {
   PyObject *numbers_module = PyImport_ImportModule("numbers");
-  if (!numbers_module) return -1;
+  if (numbers_module == NULL) return -1;
   Rational = PyObject_GetAttrString(numbers_module, "Rational");
-  if (!Rational) {
+  if (Rational == NULL) {
     Py_DECREF(numbers_module);
     return -1;
   }
   Real = PyObject_GetAttrString(numbers_module, "Real");
   Py_DECREF(numbers_module);
-  if (!Real) {
+  if (Real == NULL) {
     Py_DECREF(Rational);
     return -1;
   }
   return 0;
 }
 
 static int mark_as_real(PyObject *python_type) {
   PyObject *register_method_name = PyUnicode_FromString("register");
-  if (!register_method_name) return -1;
+  if (register_method_name == NULL) return -1;
   PyObject *tmp =
 #if PY39_OR_MORE
       PyObject_CallMethodOneArg(Real, register_method_name, python_type);
 #else
       PyObject_CallMethodObjArgs(Real, register_method_name, python_type, NULL)
 #endif
   ;
   Py_DECREF(register_method_name);
-  if (!tmp) return -1;
+  if (tmp == NULL) return -1;
   Py_DECREF(tmp);
   return 0;
 }
 
 PyMODINIT_FUNC PyInit__cshewchuk(void) {
   PyObject *result;
   if (PyType_Ready(&ExpansionType) < 0) return NULL;
```

### Comparing `shewchuk-6.7.0/tests/test_incircle_test.py` & `shewchuk-6.7.1/tests/test_incircle_test.py`

 * *Files identical despite different names*

### Comparing `shewchuk-6.7.0/tests/test_kind.py` & `shewchuk-6.7.1/tests/test_kind.py`

 * *Files identical despite different names*

### Comparing `shewchuk-6.7.0/tests/test_orientation.py` & `shewchuk-6.7.1/tests/test_orientation.py`

 * *Files identical despite different names*

### Comparing `shewchuk-6.7.0/tests/test_vectors_cross_product.py` & `shewchuk-6.7.1/tests/test_vectors_cross_product.py`

 * *Files identical despite different names*

### Comparing `shewchuk-6.7.0/tests/test_vectors_dot_product.py` & `shewchuk-6.7.1/tests/test_vectors_dot_product.py`

 * *Files identical despite different names*

