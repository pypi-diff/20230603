# Comparing `tmp/miniosl-0.0.2.tar.gz` & `tmp/miniosl-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniosl-0.0.2.tar", last modified: Mon May 29 08:24:09 2023, max compression
+gzip compressed data, was "miniosl-0.0.3a1.tar", last modified: Sat Jun  3 06:34:50 2023, max compression
```

## Comparing `miniosl-0.0.2.tar` & `miniosl-0.0.3a1.tar`

### file list

```diff
@@ -1,194 +1,286 @@
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.218136 miniosl-0.0.2/
--rw-r--r--   0 tk         (501) staff       (20)      514 2023-05-25 08:23:14.000000 miniosl-0.0.2/AUTHORS.osl
--rw-r--r--   0 tk         (501) staff       (20)     3417 2023-05-25 08:23:00.000000 miniosl-0.0.2/LICENSE.osl
--rw-r--r--   0 tk         (501) staff       (20)      145 2023-05-29 08:17:53.000000 miniosl-0.0.2/MANIFEST.in
--rw-r--r--   0 tk         (501) staff       (20)      734 2023-05-29 08:24:09.218017 miniosl-0.0.2/PKG-INFO
--rw-r--r--   0 tk         (501) staff       (20)      444 2023-05-29 07:49:18.000000 miniosl-0.0.2/README.md
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.201587 miniosl-0.0.2/miniosl/
--rw-r--r--   0 tk         (501) staff       (20)       56 2023-05-27 00:20:16.000000 miniosl-0.0.2/miniosl/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)    10645 2023-05-29 00:28:30.000000 miniosl-0.0.2/miniosl/state.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.202153 miniosl-0.0.2/miniosl.egg-info/
--rw-r--r--   0 tk         (501) staff       (20)      734 2023-05-29 08:24:09.000000 miniosl-0.0.2/miniosl.egg-info/PKG-INFO
--rw-r--r--   0 tk         (501) staff       (20)     6845 2023-05-29 08:24:09.000000 miniosl-0.0.2/miniosl.egg-info/SOURCES.txt
--rw-r--r--   0 tk         (501) staff       (20)        1 2023-05-29 08:24:09.000000 miniosl-0.0.2/miniosl.egg-info/dependency_links.txt
--rw-r--r--   0 tk         (501) staff       (20)        1 2023-05-25 07:14:23.000000 miniosl-0.0.2/miniosl.egg-info/not-zip-safe
--rw-r--r--   0 tk         (501) staff       (20)       18 2023-05-29 08:24:09.000000 miniosl-0.0.2/miniosl.egg-info/top_level.txt
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.202252 miniosl-0.0.2/minioslcc/
--rw-r--r--   0 tk         (501) staff       (20)     1644 2023-05-29 08:23:12.000000 miniosl-0.0.2/minioslcc/CMakeLists.txt
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.202607 miniosl-0.0.2/minioslcc/acutest/
--rw-r--r--   0 tk         (501) staff       (20)     1565 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/acutest/CMakeLists.txt
--rw-r--r--   0 tk         (501) staff       (20)     1096 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/acutest/LICENSE.md
--rw-r--r--   0 tk         (501) staff       (20)    15576 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/acutest/README.md
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.202848 miniosl-0.0.2/minioslcc/acutest/examples/
--rw-r--r--   0 tk         (501) staff       (20)      178 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/acutest/examples/CMakeLists.txt
--rw-r--r--   0 tk         (501) staff       (20)     3147 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/acutest/examples/cpp-example.cc
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.202971 miniosl-0.0.2/minioslcc/acutest/include/
--rw-r--r--   0 tk         (501) staff       (20)    61302 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/acutest/include/acutest.h
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.203953 miniosl-0.0.2/minioslcc/pybind11/
--rw-r--r--   0 tk         (501) staff       (20)     2196 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/.cmake-format.yaml
--rw-r--r--   0 tk         (501) staff       (20)     3600 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 tk         (501) staff       (20)    12031 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/CMakeLists.txt
--rw-r--r--   0 tk         (501) staff       (20)     1684 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/LICENSE
--rw-r--r--   0 tk         (501) staff       (20)      235 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/MANIFEST.in
--rw-r--r--   0 tk         (501) staff       (20)     7686 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/README.rst
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.204152 miniosl-0.0.2/minioslcc/pybind11/docs/
--rw-r--r--   0 tk         (501) staff       (20)     2856 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/docs/benchmark.py
--rw-r--r--   0 tk         (501) staff       (20)    11574 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/docs/conf.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.199725 miniosl-0.0.2/minioslcc/pybind11/include/
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.206612 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/
--rw-r--r--   0 tk         (501) staff       (20)    24334 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/attr.h
--rw-r--r--   0 tk         (501) staff       (20)     7069 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 tk         (501) staff       (20)    67312 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/cast.h
--rw-r--r--   0 tk         (501) staff       (20)     8458 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 tk         (501) staff       (20)      120 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/common.h
--rw-r--r--   0 tk         (501) staff       (20)     2096 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.207432 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/
--rw-r--r--   0 tk         (501) staff       (20)    28518 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 tk         (501) staff       (20)    53462 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 tk         (501) staff       (20)     5962 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 tk         (501) staff       (20)    17859 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 tk         (501) staff       (20)    28221 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 tk         (501) staff       (20)    48364 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 tk         (501) staff       (20)     1625 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.207660 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/eigen/
--rw-r--r--   0 tk         (501) staff       (20)    31450 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 tk         (501) staff       (20)    18140 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 tk         (501) staff       (20)      316 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 tk         (501) staff       (20)    13459 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/embed.h
--rw-r--r--   0 tk         (501) staff       (20)     4731 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/eval.h
--rw-r--r--   0 tk         (501) staff       (20)     5002 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/functional.h
--rw-r--r--   0 tk         (501) staff       (20)     8262 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/gil.h
--rw-r--r--   0 tk         (501) staff       (20)     8862 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 tk         (501) staff       (20)    79416 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 tk         (501) staff       (20)     9103 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/operators.h
--rw-r--r--   0 tk         (501) staff       (20)     2734 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/options.h
--rw-r--r--   0 tk         (501) staff       (20)   126708 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 tk         (501) staff       (20)    94641 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.207764 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/stl/
--rw-r--r--   0 tk         (501) staff       (20)     4185 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 tk         (501) staff       (20)    15399 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/stl.h
--rw-r--r--   0 tk         (501) staff       (20)    29897 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 tk         (501) staff       (20)     1929 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/include/pybind11/type_caster_pyobject_ptr.h
--rw-r--r--   0 tk         (501) staff       (20)     2765 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/noxfile.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.208255 miniosl-0.0.2/minioslcc/pybind11/pybind11/
--rw-r--r--   0 tk         (501) staff       (20)      429 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/pybind11/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)     1544 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/pybind11/__main__.py
--rw-r--r--   0 tk         (501) staff       (20)      233 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/pybind11/_version.py
--rw-r--r--   0 tk         (501) staff       (20)     1207 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/pybind11/commands.py
--rw-r--r--   0 tk         (501) staff       (20)    17462 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 tk         (501) staff       (20)     1452 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/setup.cfg
--rw-r--r--   0 tk         (501) staff       (20)     4877 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/setup.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.213519 miniosl-0.0.2/minioslcc/pybind11/tests/
--rw-r--r--   0 tk         (501) staff       (20)    21801 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 tk         (501) staff       (20)     5619 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/conftest.py
--rw-r--r--   0 tk         (501) staff       (20)    11736 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/constructor_stats.h
--rw-r--r--   0 tk         (501) staff       (20)      926 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/env.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.213622 miniosl-0.0.2/minioslcc/pybind11/tests/extra_python_package/
--rw-r--r--   0 tk         (501) staff       (20)     8345 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.213714 miniosl-0.0.2/minioslcc/pybind11/tests/extra_setuptools/
--rw-r--r--   0 tk         (501) staff       (20)     4153 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 tk         (501) staff       (20)     2847 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/local_bindings.h
--rw-r--r--   0 tk         (501) staff       (20)     5743 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/object.h
--rw-r--r--   0 tk         (501) staff       (20)     2685 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 tk         (501) staff       (20)      536 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_async.py
--rw-r--r--   0 tk         (501) staff       (20)     4848 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_buffers.py
--rw-r--r--   0 tk         (501) staff       (20)    17243 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 tk         (501) staff       (20)     6549 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_call_policies.py
--rw-r--r--   0 tk         (501) staff       (20)     6796 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_callbacks.py
--rw-r--r--   0 tk         (501) staff       (20)     5691 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_chrono.py
--rw-r--r--   0 tk         (501) staff       (20)    14757 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_class.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.213904 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/
--rw-r--r--   0 tk         (501) staff       (20)     2639 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.213998 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 tk         (501) staff       (20)     1171 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.214094 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 tk         (501) staff       (20)     1293 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.214186 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 tk         (501) staff       (20)     1685 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.214288 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 tk         (501) staff       (20)     1353 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.214402 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 tk         (501) staff       (20)     1163 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.214502 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 tk         (501) staff       (20)     1368 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 tk         (501) staff       (20)      198 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 tk         (501) staff       (20)      593 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_const_name.py
--rw-r--r--   0 tk         (501) staff       (20)     1551 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 tk         (501) staff       (20)     4796 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_copy_move.py
--rw-r--r--   0 tk         (501) staff       (20)     3992 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 tk         (501) staff       (20)     1091 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0 tk         (501) staff       (20)     2423 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 tk         (501) staff       (20)    29028 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_eigen_matrix.py
--rw-r--r--   0 tk         (501) staff       (20)     9414 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_eigen_tensor.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.214784 miniosl-0.0.2/minioslcc/pybind11/tests/test_embed/
--rw-r--r--   0 tk         (501) staff       (20)     1798 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 tk         (501) staff       (20)      237 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 tk         (501) staff       (20)      275 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_embed/test_trampoline.py
--rw-r--r--   0 tk         (501) staff       (20)     8939 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_enum.py
--rw-r--r--   0 tk         (501) staff       (20)     1143 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_eval.py
--rw-r--r--   0 tk         (501) staff       (20)      119 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_eval_call.py
--rw-r--r--   0 tk         (501) staff       (20)      399 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_exceptions.h
--rw-r--r--   0 tk         (501) staff       (20)    13176 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_exceptions.py
--rw-r--r--   0 tk         (501) staff       (20)    16491 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 tk         (501) staff       (20)     8507 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 tk         (501) staff       (20)     7144 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_iostream.py
--rw-r--r--   0 tk         (501) staff       (20)    13600 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 tk         (501) staff       (20)     8054 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 tk         (501) staff       (20)    18346 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 tk         (501) staff       (20)     3963 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_modules.py
--rw-r--r--   0 tk         (501) staff       (20)    11874 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 tk         (501) staff       (20)    20414 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 tk         (501) staff       (20)    14272 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 tk         (501) staff       (20)     9658 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 tk         (501) staff       (20)     1847 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 tk         (501) staff       (20)     4332 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 tk         (501) staff       (20)     2720 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_pickling.py
--rw-r--r--   0 tk         (501) staff       (20)    23629 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_pytypes.py
--rw-r--r--   0 tk         (501) staff       (20)     8039 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 tk         (501) staff       (20)     9530 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 tk         (501) staff       (20)    12239 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_stl.py
--rw-r--r--   0 tk         (501) staff       (20)     9804 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 tk         (501) staff       (20)      741 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 tk         (501) staff       (20)      826 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_thread.py
--rw-r--r--   0 tk         (501) staff       (20)     3260 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_type_caster_pyobject_ptr.py
--rw-r--r--   0 tk         (501) staff       (20)      148 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_union.py
--rw-r--r--   0 tk         (501) staff       (20)     1141 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_unnamed_namespace_a.py
--rw-r--r--   0 tk         (501) staff       (20)      143 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_unnamed_namespace_b.py
--rw-r--r--   0 tk         (501) staff       (20)      329 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_vector_unique_ptr_member.py
--rw-r--r--   0 tk         (501) staff       (20)    12913 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tests/test_virtual_functions.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.216286 miniosl-0.0.2/minioslcc/pybind11/tools/
--rw-r--r--   0 tk         (501) staff       (20)     2449 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 tk         (501) staff       (20)     3105 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 tk         (501) staff       (20)    11190 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 tk         (501) staff       (20)      817 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/JoinPaths.cmake
--rw-r--r--   0 tk         (501) staff       (20)      952 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 tk         (501) staff       (20)     1117 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 tk         (501) staff       (20)     1031 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/libsize.py
--rwxr-xr-x   0 tk         (501) staff       (20)     1311 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/make_changelog.py
--rw-r--r--   0 tk         (501) staff       (20)      196 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 tk         (501) staff       (20)    14179 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 tk         (501) staff       (20)     6930 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 tk         (501) staff       (20)     8960 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 tk         (501) staff       (20)     8361 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 tk         (501) staff       (20)     2104 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/setup_global.py.in
--rw-r--r--   0 tk         (501) staff       (20)     1234 2023-05-29 07:56:23.000000 miniosl-0.0.2/minioslcc/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.217234 miniosl-0.0.2/minioslcc/src/
--rw-r--r--   0 tk         (501) staff       (20)    34523 2023-05-29 07:46:14.000000 miniosl-0.0.2/minioslcc/src/checkmate.cc
--rw-r--r--   0 tk         (501) staff       (20)     5505 2023-05-29 07:46:14.000000 miniosl-0.0.2/minioslcc/src/checkmate.h
--rw-r--r--   0 tk         (501) staff       (20)     8259 2023-05-29 07:46:14.000000 miniosl-0.0.2/minioslcc/src/miniosl.cc
--rw-r--r--   0 tk         (501) staff       (20)    31524 2023-05-29 07:46:14.000000 miniosl-0.0.2/minioslcc/src/more.cc
--rw-r--r--   0 tk         (501) staff       (20)    33411 2023-05-29 07:46:14.000000 miniosl-0.0.2/minioslcc/src/more.h
--rw-r--r--   0 tk         (501) staff       (20)    18572 2023-05-29 07:46:14.000000 miniosl-0.0.2/minioslcc/src/record.cc
--rw-r--r--   0 tk         (501) staff       (20)     3711 2023-05-29 07:46:14.000000 miniosl-0.0.2/minioslcc/src/record.h
--rw-r--r--   0 tk         (501) staff       (20)    57215 2023-05-29 07:46:14.000000 miniosl-0.0.2/minioslcc/src/state.cc
--rw-r--r--   0 tk         (501) staff       (20)    89290 2023-05-29 07:46:14.000000 miniosl-0.0.2/minioslcc/src/state.h
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.217574 miniosl-0.0.2/minioslcc/test/
--rw-r--r--   0 tk         (501) staff       (20)   195761 2023-05-29 07:46:14.000000 miniosl-0.0.2/minioslcc/test/minitest.cc
--rw-r--r--   0 tk         (501) staff       (20)    14060 2023-05-29 07:46:14.000000 miniosl-0.0.2/minioslcc/test/minitest_file.cc
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.217751 miniosl-0.0.2/minioslcc/util/
--rw-r--r--   0 tk         (501) staff       (20)      803 2023-05-29 07:46:14.000000 miniosl-0.0.2/minioslcc/util/csa-to-sfen.cc
--rw-r--r--   0 tk         (501) staff       (20)     2840 2023-05-29 07:46:14.000000 miniosl-0.0.2/minioslcc/util/validate-sfen.cc
--rw-r--r--   0 tk         (501) staff       (20)       38 2023-05-29 08:24:09.218165 miniosl-0.0.2/setup.cfg
--rw-r--r--   0 tk         (501) staff       (20)     8480 2023-05-29 07:46:14.000000 miniosl-0.0.2/setup.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-05-29 08:24:09.217844 miniosl-0.0.2/tests/
--rw-r--r--   0 tk         (501) staff       (20)     1603 2023-05-27 00:52:11.000000 miniosl-0.0.2/tests/test_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.529977 miniosl-0.0.3a1/
+-rw-r--r--   0 root         (0) root         (0)      514 2023-05-25 08:34:27.000000 miniosl-0.0.3a1/AUTHORS.osl
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-05-25 08:34:27.000000 miniosl-0.0.3a1/LICENSE.osl
+-rw-r--r--   0 root         (0) root         (0)      145 2023-05-29 15:00:54.000000 miniosl-0.0.3a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      798 2023-06-03 06:34:50.529977 miniosl-0.0.3a1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      450 2023-06-02 03:31:21.000000 miniosl-0.0.3a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/miniosl/
+-rw-r--r--   0 root         (0) root         (0)      281 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/miniosl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7276 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/miniosl/drawing.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/miniosl/record.py
+-rw-r--r--   0 root         (0) root         (0)     4858 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/miniosl/state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/miniosl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      798 2023-06-03 06:34:50.000000 miniosl-0.0.3a1/miniosl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10153 2023-06-03 06:34:50.000000 miniosl-0.0.3a1/miniosl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 06:34:50.000000 miniosl-0.0.3a1/miniosl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 07:26:17.000000 miniosl-0.0.3a1/miniosl.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-03 06:34:50.000000 miniosl-0.0.3a1/miniosl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/
+-rw-r--r--   0 root         (0) root         (0)     1816 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/acutest/
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/acutest/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/acutest/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)    15576 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/acutest/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/acutest/examples/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/acutest/examples/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3147 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/acutest/examples/cpp-example.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/acutest/include/
+-rw-r--r--   0 root         (0) root         (0)    61302 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/acutest/include/acutest.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/gbuild/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/3.22.1/
+-rw-r--r--   0 root         (0) root         (0)     5466 2023-05-25 08:35:29.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake
+-rw-r--r--   0 root         (0) root         (0)      402 2023-05-25 08:35:29.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/3.22.1/CMakeSystem.cmake
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-25 08:35:38.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 root         (0) root         (0)     2949 2023-05-29 15:01:08.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/Makefile.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/csa-to-sfen.dir/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-29 15:01:08.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/csa-to-sfen.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-29 15:01:08.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/csa-to-sfen.dir/cmake_clean.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/minioslcc.dir/
+-rw-r--r--   0 root         (0) root         (0)      673 2023-05-25 08:35:38.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/minioslcc.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-29 15:01:08.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/minioslcc.dir/cmake_clean.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/minioslcc20.dir/
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-05-29 15:01:08.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/minioslcc20.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      609 2023-05-29 15:01:08.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/minioslcc20.dir/cmake_clean.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/minitest.dir/
+-rw-r--r--   0 root         (0) root         (0)      677 2023-05-29 15:01:08.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/minitest.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      303 2023-05-29 15:01:08.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/minitest.dir/cmake_clean.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/minitest_file.dir/
+-rw-r--r--   0 root         (0) root         (0)      702 2023-05-29 15:01:08.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/minitest_file.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      338 2023-05-29 15:01:08.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/minitest_file.dir/cmake_clean.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/validate-sfen.dir/
+-rw-r--r--   0 root         (0) root         (0)      702 2023-05-29 15:01:08.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/validate-sfen.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      338 2023-05-29 15:01:08.000000 miniosl-0.0.3a1/minioslcc/gbuild/CMakeFiles/validate-sfen.dir/cmake_clean.cmake
+-rw-r--r--   0 root         (0) root         (0)      899 2023-05-29 15:01:08.000000 miniosl-0.0.3a1/minioslcc/gbuild/CTestTestfile.cmake
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-25 08:35:38.000000 miniosl-0.0.3a1/minioslcc/gbuild/cmake_install.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/gbuild/pybind11/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.509977 miniosl-0.0.3a1/minioslcc/gbuild/pybind11/CMakeFiles/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-25 08:35:38.000000 miniosl-0.0.3a1/minioslcc/gbuild/pybind11/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-05-25 08:35:38.000000 miniosl-0.0.3a1/minioslcc/gbuild/pybind11/cmake_install.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.513977 miniosl-0.0.3a1/minioslcc/pybind11/
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/.cmake-format.yaml
+-rw-r--r--   0 root         (0) root         (0)     3600 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    12031 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      235 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7686 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.513977 miniosl-0.0.3a1/minioslcc/pybind11/docs/
+-rw-r--r--   0 root         (0) root         (0)     2856 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/docs/benchmark.py
+-rw-r--r--   0 root         (0) root         (0)    11574 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/docs/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.505977 miniosl-0.0.3a1/minioslcc/pybind11/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.513977 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/
+-rw-r--r--   0 root         (0) root         (0)    24334 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 root         (0) root         (0)     7069 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 root         (0) root         (0)    67312 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 root         (0) root         (0)     8458 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 root         (0) root         (0)      120 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/common.h
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.513977 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/
+-rw-r--r--   0 root         (0) root         (0)    28518 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 root         (0) root         (0)    53462 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 root         (0) root         (0)     5962 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 root         (0) root         (0)    17859 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 root         (0) root         (0)    28221 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 root         (0) root         (0)    48364 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.513977 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 root         (0) root         (0)    31450 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 root         (0) root         (0)    18140 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 root         (0) root         (0)    13459 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 root         (0) root         (0)     5002 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 root         (0) root         (0)     8262 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 root         (0) root         (0)     8862 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 root         (0) root         (0)    79416 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 root         (0) root         (0)     9103 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/options.h
+-rw-r--r--   0 root         (0) root         (0)   126708 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 root         (0) root         (0)    94641 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.513977 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/stl/
+-rw-r--r--   0 root         (0) root         (0)     4185 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 root         (0) root         (0)    15399 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 root         (0) root         (0)    29897 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/noxfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.517977 miniosl-0.0.3a1/minioslcc/pybind11/pybind11/
+-rw-r--r--   0 root         (0) root         (0)      429 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/pybind11/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/pybind11/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/pybind11/_version.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/pybind11/commands.py
+-rw-r--r--   0 root         (0) root         (0)    17462 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4877 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.521977 miniosl-0.0.3a1/minioslcc/pybind11/tests/
+-rw-r--r--   0 root         (0) root         (0)    21801 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5619 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    11736 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 root         (0) root         (0)      926 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.521977 miniosl-0.0.3a1/minioslcc/pybind11/tests/extra_python_package/
+-rw-r--r--   0 root         (0) root         (0)     8345 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.521977 miniosl-0.0.3a1/minioslcc/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/local_bindings.h
+-rw-r--r--   0 root         (0) root         (0)     5743 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/object.h
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 root         (0) root         (0)      536 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_async.py
+-rw-r--r--   0 root         (0) root         (0)     4848 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_buffers.py
+-rw-r--r--   0 root         (0) root         (0)    17243 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 root         (0) root         (0)     6549 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 root         (0) root         (0)     6796 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 root         (0) root         (0)     5691 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_chrono.py
+-rw-r--r--   0 root         (0) root         (0)    14757 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.521977 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.521977 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 root         (0) root         (0)     1171 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.521977 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.521977 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.521977 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.521977 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.521977 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 root         (0) root         (0)      593 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_const_name.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 root         (0) root         (0)     4796 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 root         (0) root         (0)     3992 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 root         (0) root         (0)    29028 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_eigen_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     9414 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_eigen_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.521977 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_embed/
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 root         (0) root         (0)      275 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0 root         (0) root         (0)     8939 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_eval.py
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_exceptions.h
+-rw-r--r--   0 root         (0) root         (0)    13176 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    16491 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 root         (0) root         (0)     8507 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_iostream.py
+-rw-r--r--   0 root         (0) root         (0)    13600 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 root         (0) root         (0)     8054 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 root         (0) root         (0)    18346 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     3963 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_modules.py
+-rw-r--r--   0 root         (0) root         (0)    11874 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 root         (0) root         (0)    20414 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 root         (0) root         (0)    14272 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 root         (0) root         (0)     9658 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 root         (0) root         (0)     4332 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_pickling.py
+-rw-r--r--   0 root         (0) root         (0)    23629 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 root         (0) root         (0)     8039 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 root         (0) root         (0)     9530 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 root         (0) root         (0)    12239 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_stl.py
+-rw-r--r--   0 root         (0) root         (0)     9804 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 root         (0) root         (0)      741 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 root         (0) root         (0)      826 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_thread.py
+-rw-r--r--   0 root         (0) root         (0)     3260 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_type_caster_pyobject_ptr.py
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_union.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_unnamed_namespace_a.py
+-rw-r--r--   0 root         (0) root         (0)      143 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_unnamed_namespace_b.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_vector_unique_ptr_member.py
+-rw-r--r--   0 root         (0) root         (0)    12913 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tests/test_virtual_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.525977 miniosl-0.0.3a1/minioslcc/pybind11/tools/
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 root         (0) root         (0)     3105 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 root         (0) root         (0)    11190 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 root         (0) root         (0)      817 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/JoinPaths.cmake
+-rw-r--r--   0 root         (0) root         (0)      952 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/libsize.py
+-rwxr-xr-x   0 root         (0) root         (0)     1311 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/make_changelog.py
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 root         (0) root         (0)    14179 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 root         (0) root         (0)     6930 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 root         (0) root         (0)     8960 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 root         (0) root         (0)     8361 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-05-25 08:34:56.000000 miniosl-0.0.3a1/minioslcc/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.525977 miniosl-0.0.3a1/minioslcc/rbuild/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.525977 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.525977 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/3.22.1/
+-rw-r--r--   0 root         (0) root         (0)     5466 2023-05-25 08:37:30.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake
+-rw-r--r--   0 root         (0) root         (0)      402 2023-05-25 08:37:30.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/3.22.1/CMakeSystem.cmake
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-25 08:37:47.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 root         (0) root         (0)     2949 2023-06-02 03:33:02.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/Makefile.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.525977 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/csa-to-sfen.dir/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-02 03:33:02.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/csa-to-sfen.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-02 03:33:02.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/csa-to-sfen.dir/cmake_clean.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.525977 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/minioslcc.dir/
+-rw-r--r--   0 root         (0) root         (0)      673 2023-05-25 08:37:47.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/minioslcc.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-02 03:33:02.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/minioslcc.dir/cmake_clean.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.525977 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/minioslcc20.dir/
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-06-02 03:33:02.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/minioslcc20.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      609 2023-06-02 03:33:02.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/minioslcc20.dir/cmake_clean.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.525977 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/minitest.dir/
+-rw-r--r--   0 root         (0) root         (0)      677 2023-06-02 03:33:02.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/minitest.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-02 03:33:02.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/minitest.dir/cmake_clean.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.525977 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/minitest_file.dir/
+-rw-r--r--   0 root         (0) root         (0)      702 2023-06-02 03:33:02.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/minitest_file.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-02 03:33:02.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/minitest_file.dir/cmake_clean.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.525977 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/validate-sfen.dir/
+-rw-r--r--   0 root         (0) root         (0)      702 2023-06-02 03:33:02.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/validate-sfen.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-02 03:33:02.000000 miniosl-0.0.3a1/minioslcc/rbuild/CMakeFiles/validate-sfen.dir/cmake_clean.cmake
+-rw-r--r--   0 root         (0) root         (0)      899 2023-06-02 03:33:02.000000 miniosl-0.0.3a1/minioslcc/rbuild/CTestTestfile.cmake
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-05-25 08:37:47.000000 miniosl-0.0.3a1/minioslcc/rbuild/cmake_install.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.525977 miniosl-0.0.3a1/minioslcc/rbuild/pybind11/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.525977 miniosl-0.0.3a1/minioslcc/rbuild/pybind11/CMakeFiles/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-25 08:37:47.000000 miniosl-0.0.3a1/minioslcc/rbuild/pybind11/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-05-25 08:37:47.000000 miniosl-0.0.3a1/minioslcc/rbuild/pybind11/cmake_install.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.525977 miniosl-0.0.3a1/minioslcc/src/
+-rw-r--r--   0 root         (0) root         (0)    35834 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/src/checkmate.cc
+-rw-r--r--   0 root         (0) root         (0)     5573 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/src/checkmate.h
+-rw-r--r--   0 root         (0) root         (0)    11645 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/src/miniosl.cc
+-rw-r--r--   0 root         (0) root         (0)    29878 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/src/more.cc
+-rw-r--r--   0 root         (0) root         (0)    33294 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/src/more.h
+-rw-r--r--   0 root         (0) root         (0)    38838 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/src/record.cc
+-rw-r--r--   0 root         (0) root         (0)     6064 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/src/record.h
+-rw-r--r--   0 root         (0) root         (0)    57189 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/src/state.cc
+-rw-r--r--   0 root         (0) root         (0)    89652 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/src/state.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.525977 miniosl-0.0.3a1/minioslcc/tbuild/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.529977 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.529977 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/3.26.3/
+-rw-r--r--   0 root         (0) root         (0)     5469 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/3.26.3/CMakeCXXCompiler.cmake
+-rw-r--r--   0 root         (0) root         (0)      402 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/3.26.3/CMakeSystem.cmake
+-rw-r--r--   0 root         (0) root         (0)    31003 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/CMakeConfigureLog.yaml
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 root         (0) root         (0)    11253 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/Makefile.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.529977 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/minioslcc.dir/
+-rw-r--r--   0 root         (0) root         (0)      616 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/minioslcc.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/minioslcc.dir/cmake_clean.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.529977 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/minioslcc20.dir/
+-rw-r--r--   0 root         (0) root         (0)      929 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/minioslcc20.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      513 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/minioslcc20.dir/cmake_clean.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.529977 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/minitest.dir/
+-rw-r--r--   0 root         (0) root         (0)      617 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/minitest.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      301 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/minitest.dir/cmake_clean.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.529977 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/minitest_file.dir/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/minitest_file.dir/DependInfo.cmake
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/CMakeFiles/minitest_file.dir/cmake_clean.cmake
+-rw-r--r--   0 root         (0) root         (0)      899 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/CTestTestfile.cmake
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/cmake_install.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.529977 miniosl-0.0.3a1/minioslcc/tbuild/pybind11/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.529977 miniosl-0.0.3a1/minioslcc/tbuild/pybind11/CMakeFiles/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/pybind11/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-05-27 07:30:00.000000 miniosl-0.0.3a1/minioslcc/tbuild/pybind11/cmake_install.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.529977 miniosl-0.0.3a1/minioslcc/test/
+-rw-r--r--   0 root         (0) root         (0)   209279 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/test/minitest.cc
+-rw-r--r--   0 root         (0) root         (0)    14899 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/test/minitest_file.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.529977 miniosl-0.0.3a1/minioslcc/util/
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/util/compress-sfen.cc
+-rw-r--r--   0 root         (0) root         (0)      994 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/util/csa-to-sfen.cc
+-rw-r--r--   0 root         (0) root         (0)     3202 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/minioslcc/util/validate-sfen.cc
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 06:34:50.529977 miniosl-0.0.3a1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8554 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 06:34:50.529977 miniosl-0.0.3a1/tests/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/tests/test_record.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2023-06-03 06:28:32.000000 miniosl-0.0.3a1/tests/test_state.py
```

### Comparing `miniosl-0.0.2/AUTHORS.osl` & `miniosl-0.0.3a1/AUTHORS.osl`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/LICENSE.osl` & `miniosl-0.0.3a1/LICENSE.osl`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/PKG-INFO` & `miniosl-0.0.3a1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: miniosl
-Version: 0.0.2
+Version: 0.0.3a1
 Summary: A python interface to miniosl (shogi library)
 Author: Tomoyuki Kaneko
 Author-email: kaneko@graco.c.u-tokyo.ac.jp
+Project-URL: Source, https://github.com/tkaneko/miniosl
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.osl
 License-File: AUTHORS.osl
 
 # miniOSL
 
 Python interface to [OSL (open shogi library)](https://gps.tanaka.ecc.u-tokyo.ac.jp/gpsshogi/index.php?GPSshogi) refurbished by C++20 and by pybind11.
 
 WIP.
 
-## demo
+## demo@colab
 
 https://colab.research.google.com/drive/1orT32kOR58owC0SfhPdC0yodFdn8h2nX?usp=share_link
 
 ## pip wheel
 
 - https://pypi.org/project/miniosl/
```

### Comparing `miniosl-0.0.2/miniosl.egg-info/PKG-INFO` & `miniosl-0.0.3a1/miniosl.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: miniosl
-Version: 0.0.2
+Version: 0.0.3a1
 Summary: A python interface to miniosl (shogi library)
 Author: Tomoyuki Kaneko
 Author-email: kaneko@graco.c.u-tokyo.ac.jp
+Project-URL: Source, https://github.com/tkaneko/miniosl
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.osl
 License-File: AUTHORS.osl
 
 # miniOSL
 
 Python interface to [OSL (open shogi library)](https://gps.tanaka.ecc.u-tokyo.ac.jp/gpsshogi/index.php?GPSshogi) refurbished by C++20 and by pybind11.
 
 WIP.
 
-## demo
+## demo@colab
 
 https://colab.research.google.com/drive/1orT32kOR58owC0SfhPdC0yodFdn8h2nX?usp=share_link
 
 ## pip wheel
 
 - https://pypi.org/project/miniosl/
```

### Comparing `miniosl-0.0.2/minioslcc/CMakeLists.txt` & `miniosl-0.0.3a1/minioslcc/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,18 @@
   add_executable(csa-to-sfen util/csa-to-sfen.cc)  
   target_include_directories(csa-to-sfen PRIVATE src)
   target_link_libraries(csa-to-sfen PRIVATE minioslcc20)
 
   add_executable(validate-sfen util/validate-sfen.cc)  
   target_include_directories(validate-sfen PRIVATE src)
   target_link_libraries(validate-sfen PRIVATE minioslcc20)
+
+  add_executable(compress-sfen util/compress-sfen.cc)  
+  target_include_directories(compress-sfen PRIVATE src)
+  target_link_libraries(compress-sfen PRIVATE minioslcc20)
 endif()
 
 option(BUILD_TEST "build test executable" OFF)
 
 if(BUILD_TEST)
   enable_testing()
```

### Comparing `miniosl-0.0.2/minioslcc/acutest/CMakeLists.txt` & `miniosl-0.0.3a1/minioslcc/acutest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/acutest/LICENSE.md` & `miniosl-0.0.3a1/minioslcc/acutest/LICENSE.md`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/acutest/README.md` & `miniosl-0.0.3a1/minioslcc/acutest/README.md`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/acutest/examples/cpp-example.cc` & `miniosl-0.0.3a1/minioslcc/acutest/examples/cpp-example.cc`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/acutest/include/acutest.h` & `miniosl-0.0.3a1/minioslcc/acutest/include/acutest.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/.cmake-format.yaml` & `miniosl-0.0.3a1/minioslcc/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/.pre-commit-config.yaml` & `miniosl-0.0.3a1/minioslcc/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/CMakeLists.txt` & `miniosl-0.0.3a1/minioslcc/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/LICENSE` & `miniosl-0.0.3a1/minioslcc/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/README.rst` & `miniosl-0.0.3a1/minioslcc/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/docs/benchmark.py` & `miniosl-0.0.3a1/minioslcc/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/docs/conf.py` & `miniosl-0.0.3a1/minioslcc/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/attr.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/buffer_info.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/cast.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/chrono.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/complex.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/class.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/common.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/descr.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/init.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/internals.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/type_caster_base.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/detail/typeid.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/eigen/matrix.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/eigen/tensor.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/embed.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/eval.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/functional.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/gil.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/iostream.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/numpy.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/operators.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/options.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/pybind11.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/pytypes.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/stl/filesystem.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/stl.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/stl_bind.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/include/pybind11/type_caster_pyobject_ptr.h` & `miniosl-0.0.3a1/minioslcc/pybind11/include/pybind11/type_caster_pyobject_ptr.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/noxfile.py` & `miniosl-0.0.3a1/minioslcc/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/pybind11/__main__.py` & `miniosl-0.0.3a1/minioslcc/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/pybind11/commands.py` & `miniosl-0.0.3a1/minioslcc/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/pybind11/setup_helpers.py` & `miniosl-0.0.3a1/minioslcc/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/setup.cfg` & `miniosl-0.0.3a1/minioslcc/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/setup.py` & `miniosl-0.0.3a1/minioslcc/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/CMakeLists.txt` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/conftest.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/constructor_stats.h` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/env.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/extra_python_package/test_files.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/extra_setuptools/test_setuphelper.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/local_bindings.h` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/object.h` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/pybind11_tests.h` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_async.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_buffers.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_builtin_casters.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_call_policies.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_callbacks.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_chrono.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_class.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/CMakeLists.txt` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_const_name.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_constants_and_functions.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_copy_move.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_custom_type_casters.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_custom_type_setup.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_docstring_options.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_eigen_matrix.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_eigen_matrix.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_eigen_tensor.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_eigen_tensor.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_embed/CMakeLists.txt` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_enum.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_eval.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_exceptions.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_factory_constructors.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_gil_scoped.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_iostream.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_kwargs_and_defaults.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_local_bindings.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_methods_and_attributes.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_modules.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_multiple_inheritance.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_numpy_array.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_numpy_dtypes.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_numpy_vectorize.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_opaque_types.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_operator_overloading.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_pickling.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_pytypes.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_sequences_and_iterators.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_smart_ptr.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_stl.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_stl_binders.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_tagbased_polymorphic.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_thread.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_type_caster_pyobject_ptr.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_type_caster_pyobject_ptr.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_unnamed_namespace_a.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_unnamed_namespace_a.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tests/test_virtual_functions.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tools/FindCatch.cmake` & `miniosl-0.0.3a1/minioslcc/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tools/FindEigen3.cmake` & `miniosl-0.0.3a1/minioslcc/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tools/FindPythonLibsNew.cmake` & `miniosl-0.0.3a1/minioslcc/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tools/JoinPaths.cmake` & `miniosl-0.0.3a1/minioslcc/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tools/cmake_uninstall.cmake.in` & `miniosl-0.0.3a1/minioslcc/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tools/codespell_ignore_lines_from_errors.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tools/libsize.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tools/make_changelog.py` & `miniosl-0.0.3a1/minioslcc/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tools/pybind11Common.cmake` & `miniosl-0.0.3a1/minioslcc/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tools/pybind11Config.cmake.in` & `miniosl-0.0.3a1/minioslcc/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tools/pybind11NewTools.cmake` & `miniosl-0.0.3a1/minioslcc/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tools/pybind11Tools.cmake` & `miniosl-0.0.3a1/minioslcc/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tools/setup_global.py.in` & `miniosl-0.0.3a1/minioslcc/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/pybind11/tools/setup_main.py.in` & `miniosl-0.0.3a1/minioslcc/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `miniosl-0.0.2/minioslcc/src/checkmate.cc` & `miniosl-0.0.3a1/minioslcc/src/checkmate.cc`

 * *Files 2% similar despite different names*

```diff
@@ -926,12 +926,49 @@
 
 namespace osl
 {
   template void move_generator::AddEffect::generate<BLACK>(const EffectState&,Square,MoveStore&,bool&);
   template void move_generator::AddEffect::generate<WHITE>(const EffectState&,Square,MoveStore&,bool&);
 } // namespace osl
 
+bool osl::win_if_declare(const EffectState& state) {
+  const auto Turn = state.turn();
+
+  //手番, 持時間は省略
+  assert(Turn == state.turn());
+  const Square my_king_sq = state.kingSquare(Turn);
+
+  if (my_king_sq.isPieceStand() || state.hasEffectAt(alt(Turn), my_king_sq))
+    return false;
+
+  if (! promote_area_y(Turn, my_king_sq.y()))
+    return false;
+  
+  // 敵陣に自分の駒が10枚以上 (自玉を除いて) あるか
+  // 駒の点数を勘定する.  (対象: 敵陣の駒 + 持駒)
+  // 大駒を5点として, 先手は28点, 後手なら27点必要
+  int pieces_in_area = 0;
+  int score_in_area = -1; // 自玉の分を予め引いておく
+
+  for (int n: state.piecesOnBoard(Turn).toRange()) {
+    auto p = state.pieceOf(n);
+    if (p.square().isPromoteArea(Turn)) {
+      ++pieces_in_area;
+      score_in_area += 1 + 4 * is_major(p.ptype());
+    }
+  }
+  if (pieces_in_area < 11)
+    return false;
+
+  int score_stand = 5 * state.countPiecesOnStand(Turn, ROOK) + 5 * state.countPiecesOnStand(Turn, BISHOP)
+    + state.countPiecesOnStand(Turn, GOLD)   + state.countPiecesOnStand(Turn, SILVER)
+    + state.countPiecesOnStand(Turn, KNIGHT) + state.countPiecesOnStand(Turn, LANCE)
+    + state.countPiecesOnStand(Turn, PAWN);
+
+  return score_in_area + score_stand >= 27 + (Turn==BLACK);
+}
+
 // ;;; Local Variables:
 // ;;; mode:c++
 // ;;; c-basic-offset:2
 // ;;; End:
```

### Comparing `miniosl-0.0.2/minioslcc/src/checkmate.h` & `miniosl-0.0.3a1/minioslcc/src/checkmate.h`

 * *Files 2% similar despite different names*

```diff
@@ -163,9 +163,14 @@
         bool dummy;
         generate<P>(state,target,action,dummy);
       }
     };
   }
 }
 
+namespace osl
+{
+  bool win_if_declare(const EffectState& state);
+}
+
 #endif
 /* CHECKMATE_H */
```

### Comparing `miniosl-0.0.2/minioslcc/src/miniosl.cc` & `miniosl-0.0.3a1/minioslcc/src/miniosl.cc`

 * *Files 25% similar despite different names*

```diff
@@ -2,43 +2,29 @@
 #include <pybind11/stl.h>
 #include <pybind11/numpy.h>
 #include "state.h"
 #include "record.h"
 #include "more.h"
 #include <sstream>
 #include <iostream>
+#include <fstream>
 
 namespace py = pybind11;
 
 namespace mini {
   using namespace osl;
-  Move to_move(const EffectState& state, std::string move) {
-    try {
-      return usi::to_move(move, state);
-    }
-    catch (std::exception& e) {
-    }
-    try {
-      return csa::to_move(move, state);
-    }
-    catch (std::exception& e) {
-    }
-    return Move::PASS(state.turn());
-  }
-  py::array_t<int8_t> to_np(const EffectState& state) {
-    auto feature = py::array_t<int8_t>(9*9);
-    auto buffer = feature.request();
-    auto ptr = static_cast<int8_t*>(buffer.ptr);
-    for (int y: board_y_range())
-      for (int x: board_x_range())
-        ptr[(y-1)*9+(x-1)] = state.pieceAt(Square(x,y)).ptypeO();
-    return feature;
-  }
+  Move to_move(const EffectState& state, std::string move);
+  py::array_t<int8_t> to_np(const EffectState& state);
+  py::array_t<int8_t> to_np_hand(const EffectState& state);
+  py::array_t<int8_t> to_np_cover(const EffectState& state);
+  py::array_t<uint64_t> to_np_pack(const EffectState& state);
+  std::pair<MiniRecord, int> unpack_record(py::array_t<uint64_t> code_seq);
 }
 
+
 PYBIND11_MODULE(minioslcc, m) {
   m.doc() = "shogi utilities derived from osl";
   // classes
   typedef osl::EffectState state_t;
   py::class_<state_t>(m, "CCState", py::dynamic_attr(),
                                   "shogi state = board position + pieces in hand (mochigoma)")
     .def(py::init())
@@ -56,15 +42,18 @@
     }, "genenerate full moves")
     .def("genmove_check", [](const state_t &s) {
       osl::MoveVector moves;
       s.generateCheck(moves);
       return moves;
     }, "generate check moves only")
     .def("make_move", [](state_t &s, std::string input) {
-      s.makeMove(mini::to_move(s, input));
+      auto move = mini::to_move(s, input);
+      if (! move.isNormal() || ! s.isLegal(move))
+        throw std::runtime_error("move error "+input);
+      s.makeMove(move);
     })
     .def("make_move", &state_t::makeMove)
     .def("to_usi", [](const state_t &s) { return osl::to_usi(s); })
     .def("to_csa", [](const state_t &s) { return osl::to_csa(s); })
     .def("__repr__", [](const state_t &s) {
       return "<CCState '" + osl::to_usi(s) + "'>";
     })
@@ -80,14 +69,21 @@
     .def("piece", &state_t::pieceOf, py::arg("id"))
     .def("in_check", py::overload_cast<>(&state_t::inCheck, py::const_))
     .def("in_checkmate", py::overload_cast<>(&state_t::inCheckmate, py::const_))
     .def("king_square", [](const state_t& s, osl::Player P) { return s.kingSquare(P); })
     .def("to_move", &mini::to_move, "parse and return move")
     .def("is_legal", &state_t::isLegal)
     .def("to_np", &mini::to_np, "pieces on board as numpy array")
+    .def("to_np_hand", &mini::to_np_hand, "pieces on board as numpy array")
+    .def("to_np_cover", &mini::to_np_cover, "pieces on board as numpy array")
+    .def("to_np_pack", &mini::to_np_pack, "pack into 256bits")
+    .def("encode_move", [](const state_t& s, osl::Move m) { return osl::bitpack::encode12(s, m); },
+         "compress move into 12bits uint")
+    .def("decode_move", [](const state_t& s, uint32_t c) { return osl::bitpack::decode_move12(s, c); },
+         "uncompress move from 12bits uint")
   ;
   py::class_<osl::Square>(m, "Square", py::dynamic_attr())
     .def(py::init<int,int>())
     .def("x", &osl::Square::x)
     .def("y", &osl::Square::y)
     .def("to_xy", [](osl::Square sq) { return std::make_pair<int,int>(sq.x(), sq.y()); })
     .def("to_usi", [](osl::Square sq) { return osl::to_psn(sq); })
@@ -109,52 +105,63 @@
     .def("to_csa", [](osl::Move m) { return osl::to_csa(m); })
     .def("__repr__", [](osl::Move m) { return "<Move '"+osl::to_psn(m) + "'>"; })
     .def("__str__", [](osl::Move m) { return osl::to_csa(m); })
     ;
   py::class_<osl::Piece>(m, "Piece", py::dynamic_attr())
     .def("square", &osl::Piece::square)
     .def("ptype", &osl::Piece::ptype)
-    .def("owner", &osl::Piece::owner)
+    .def("color", &osl::Piece::owner)
     .def("is_piece", &osl::Piece::isPiece)
     .def("__repr__", [](osl::Piece p) {
       std::stringstream ss;
       ss << p;
       return "<Piece '"+ss.str()+ "'>";
     })
     ;
   py::class_<osl::MiniRecord>(m, "MiniRecord", py::dynamic_attr())
     .def_readonly("initial_state", &osl::MiniRecord::initial_state)
     .def_readonly("moves", &osl::MiniRecord::moves)
+    .def_readonly("result", &osl::MiniRecord::result)
+    .def_readonly("final_move", &osl::MiniRecord::final_move)
+    .def("has_winner", &osl::MiniRecord::has_winner)
+    .def("to_usi", py::overload_cast<const osl::MiniRecord&>(&osl::to_usi))
+    .def("pack_record", [](const osl::MiniRecord& r){
+      std::vector<uint64_t> code; osl::bitpack::append_binary_record(r, code);
+      return code;
+    }, "encode in uint64 array")
     .def("__len__", [](const osl::MiniRecord& r) { return r.moves.size(); })
     .def("__repr__", [](const osl::MiniRecord& r) {
       return "<MiniRecord '"+osl::to_usi(r.initial_state)
         + " " + std::to_string(r.moves.size()) + " moves'>"; })
     ;
   // functions
   m.def("csa_board", [](std::string input){
     try { return osl::csa::read_board(input); }
     catch (std::exception& e) { std::cerr << e.what() << '\n'; } return state_t();
   }, "parse and return State");
   m.def("usi_board", [](std::string input){
-    state_t state;
-    try {
-      std::vector<osl::Move> moves;
-      osl::usi::parse(input, state, moves);
-    } catch (std::exception& e) { std::cerr << e.what() << '\n'; }
-    return state;
+    auto record = osl::usi::read_record(input); return record.initial_state;
   }, "parse and return State");
-  m.def("csa_record", py::overload_cast<std::string>(&osl::csa::read_record), "read a game record");
-  m.def("usi_record", &osl::usi::read_record, "read a game record");
+  m.def("csa_record", py::overload_cast<std::string>(&osl::csa::read_record), "read str as a game record");
+  m.def("csa_file", [](std::string filepath){
+    return osl::csa::read_record(std::filesystem::path(filepath)); }, "load a game record");
+  m.def("usi_record", &osl::usi::read_record, "read str as a game record");
+  m.def("usi_file", [](std::string filepath, int id=0){
+    std::ifstream is(filepath);
+    std::string line;
+    for (int i=0; i<id; ++i) getline(is, line);
+    getline(is, line);
+    return osl::usi::read_record(line); }, py::arg("arg"), py::arg("id")=0, "load a game record");
+  m.def("unpack_record", &mini::unpack_record, "read record from np.array encoded by MiniRecord.pack_record");
   m.def("to_csa", py::overload_cast<osl::Ptype>(&osl::to_csa));
   m.def("to_csa", py::overload_cast<osl::Player>(&osl::to_csa));
   m.def("to_ja", py::overload_cast<osl::Square>(&osl::to_ki2));
   m.def("to_ja", py::overload_cast<osl::Ptype>(&osl::to_ki2));
   m.def("to_ja", py::overload_cast<osl::Move, const state_t&, osl::Square>(&osl::to_ki2),
         py::arg("move"), py::arg("state"), py::arg("prev_to")=osl::Square());
-  m.def("piece_stand_order", []() { return std::vector<osl::Ptype>{osl::PieceStand::order.begin(), osl::PieceStand::order.end()}; });
   
   // enums
   py::enum_<osl::Player>(m, "Player", py::arithmetic())
     .value("black", osl::BLACK).value("white", osl::WHITE)
     .export_values();
   py::enum_<osl::Ptype>(m, "Ptype", py::arithmetic(), "piece type")
     .value("pawn",   osl::PAWN).value("lance",  osl::LANCE).value("knight", osl::KNIGHT)
@@ -170,17 +177,87 @@
     .value("L",  osl::L).value("R",  osl::R)
     .value("DL", osl::DL).value("D",  osl::D).value("DR", osl::DR)
     .value("UUL", osl::UUL).value("UUR", osl::UUR)
     .value("Long_UL", osl::Long_UL).value("Long_U",  osl::Long_U).value("Long_UR", osl::Long_UR)
     .value("Long_L",  osl::Long_L).value("Long_R",  osl::Long_R)
     .value("Long_DL", osl::Long_DL).value("Long_D",  osl::Long_D).value("Long_DR", osl::Long_DR)
     .export_values();
+  py::enum_<osl::GameResult>(m, "GameResult")
+    .value("BlackWin", osl::BlackWin).value("WhiteWin", osl::WhiteWin)
+    .value("Draw", osl::Draw).value("Interim", osl::Interim)
+    .export_values();
 
   // data
   m.attr("ptype_move_direction") = &osl::ptype_move_direction;
   m.attr("ptype_piece_id") = &osl::ptype_piece_id;
   m.attr("ptype_csa_names") = &osl::ptype_csa_names;
   m.attr("ptype_en_names") = &osl::ptype_en_names;
+  m.attr("piece_stand_order") = &osl::piece_stand_order;
   
   // "mapping of ptype to bitset of movable directions"
 
 }
+
+osl::Move mini::to_move(const EffectState& state, std::string move) {
+  try {
+    return usi::to_move(move, state);
+  }
+  catch (std::exception& e) {
+  }
+  try {
+    return csa::to_move(move, state);
+  }
+  catch (std::exception& e) {
+  }
+  return Move::PASS(state.turn());
+}
+
+py::array_t<int8_t> mini::to_np(const EffectState& state) {
+  auto feature = py::array_t<int8_t>(9*9);
+  auto buffer = feature.request();
+  auto ptr = static_cast<int8_t*>(buffer.ptr);
+  for (int y: board_y_range())
+    for (int x: board_x_range())
+      ptr[(y-1)*9+(x-1)] = state.pieceAt(Square(x,y)).ptypeO();
+  return feature;
+}
+
+py::array_t<int8_t> mini::to_np_hand(const EffectState& state) {
+  const int N = piece_stand_order.size();
+  auto feature = py::array_t<int8_t>(N*2);
+  auto buffer = feature.request();
+  auto ptr = static_cast<int8_t*>(buffer.ptr);
+  for (auto pl: players)
+    for (auto n: std::views::iota(0,N))
+      ptr[n + 5*idx(pl)] = state.countPiecesOnStand(pl, piece_stand_order[n]);
+  return feature;
+}
+
+py::array_t<int8_t> mini::to_np_cover(const EffectState& state) {
+  auto feature = py::array_t<int8_t>(9*9*2);
+  auto buffer = feature.request();
+  auto ptr = static_cast<int8_t*>(buffer.ptr);
+  for (auto pl: players)
+    for (int y: board_y_range())
+      for (int x: board_x_range())
+        ptr[(y-1)*9+(x-1)+81*idx(pl)] = state.countEffect(pl, Square(x,y));
+  return feature;
+}
+
+py::array_t<uint64_t> mini::to_np_pack(const EffectState& state) {
+  auto packed = py::array_t<uint64_t>(4);
+  auto buffer = packed.request();
+  auto ptr = static_cast<uint64_t*>(buffer.ptr);
+  osl::PackedState ps {state};
+  auto bs = ps.to_bitset();
+  for (int i: std::views::iota(0,4))
+    ptr[i] = bs.binary[i];
+  return packed;
+}
+
+std::pair<osl::MiniRecord, int> mini::unpack_record(py::array_t<uint64_t> code_seq) {
+  auto buf = code_seq.request();
+  auto ptr = static_cast<const uint64_t*>(buf.ptr);
+  MiniRecord record;
+  auto n = bitpack::read_binary_record(ptr, record);
+  return std::make_pair(record, n);
+}
```

### Comparing `miniosl-0.0.2/minioslcc/src/more.cc` & `miniosl-0.0.3a1/minioslcc/src/more.cc`

 * *Files 5% similar despite different names*

```diff
@@ -5,69 +5,14 @@
 #include <stdexcept>
 #include <cassert>
 #include <string>
 #include <array>
 
 /* ------------------------------------------------------------------------- */
 
-osl::Player osl::csa::to_player(char c) {
-  if(c=='+') 
-    return BLACK;
-  if(c=='-') 
-    return WHITE;
-  throw ParseError("not a csa PlayerCharacter "+std::string(1,c));
-}
-
-osl::Square osl::csa::to_square(const std::string& s) {
-  int x=s.at(0)-'0';
-  int y=s.at(1)-'0';
-  if(x==0 && y==0) 
-    return Square::STAND();
-  return Square(x,y);
-}
-
-osl::Ptype osl::csa::to_ptype(const std::string& s) {
-  auto p = std::ranges::find(ptype_csa_names, s);
-  if (p == ptype_csa_names.end())
-    throw ParseError("unknown std::string in csa::to_ptype "+s);
-  return Ptype(p-ptype_csa_names.begin());    
-}
-
-osl::Move osl::csa::to_move(const std::string& s,const SimpleState& state) {
-  if (s == "%KACHI")
-    return Move::DeclareWin();
-  if (s == "%TORYO")
-    return Move::INVALID();
-  if (s == "%PASS")		// FIXME: not in CSA protocol
-    return Move::PASS(state.turn());
-
-  Player pl=csa::to_player(s.at(0));
-  Square fromPos=csa::to_square(s.substr(1,2));
-  Square toPos=csa::to_square(s.substr(3,2));
-  Ptype ptype=csa::to_ptype(s.substr(5,2));
-  if(fromPos==Square::STAND()){
-    if (is_promoted(ptype))
-      throw ParseError("drop with promote ?! in csa::to_move "+s);
-    return Move(toPos,ptype,pl);
-  }
-  else{
-    Piece p0=state.pieceAt(fromPos);
-    Piece p1=state.pieceAt(toPos);
-    Ptype capturePtype=p1.ptype();
-    bool isPromote=(p0.ptype()!=ptype);
-    if (! ((p0.ptype()==ptype)||(p0.ptype()==unpromote(ptype))))
-      throw ParseError("illegal promotion in csa::to_move "+s);
-    return Move(fromPos,toPos,ptype, capturePtype,isPromote,pl);
-  }
-}
-
-/* ------------------------------------------------------------------------- */
-
-
-
 namespace osl 
 {
   namespace move_generator
   {
     namespace drop
     {
       // skeltons
```

### Comparing `miniosl-0.0.2/minioslcc/src/more.h` & `miniosl-0.0.3a1/minioslcc/src/more.h`

 * *Files 1% similar despite different names*

```diff
@@ -29,26 +29,24 @@
    * -  ROOK     : 2; 0
    *
    * == を軽くするために carry off の状態を基本とする
    */
   class PieceStand
   {
   public:
-    /** 持駒の表示で良く使われる順番. KINGや成駒は -1 */
-    static const CArray<Ptype,7> order;
     static constexpr uint32_t carryMask = 0x48822224;
   private:
     static const CArray<unsigned char,Ptype_MAX+1> shift;
     static const CArray<unsigned char,Ptype_MAX+1> mask;
     mutable uint32_t flags;
   public:
     explicit PieceStand(unsigned int value=0) : flags(value)
     {
     }
-    explicit PieceStand(Player, const SimpleState&);
+    explicit PieceStand(Player, const BaseState&);
     PieceStand(int pawnCount, int lanceCount, 
 	       int knightCount, int silverCount,
 	       int goldCount, int bishopCount,
 	       int rookCount, int kingCount) 
       : flags(0)
     {
       add(PAWN, pawnCount);
```

### Comparing `miniosl-0.0.2/minioslcc/src/state.cc` & `miniosl-0.0.3a1/minioslcc/src/state.cc`

 * *Files 2% similar despite different names*

```diff
@@ -94,22 +94,22 @@
 bool osl::Move::isConsistent() const {
   if (! isValid())
     return false;
   const Square from=this->from(), to=this->to();
   const Ptype ptype=this->ptype();
   const Player turn = player();
     
+  if (is_basic(ptype) && isPromotion())
+    return false;
+
   if (from.isPieceStand()) {  // 打つ手
     // 動けない場所ではないか?
-    return legal_drop_at(turn,ptype,to);
+    return is_basic(ptype) && legal_drop_at(turn,ptype,to) && !isCapture();
   }
   
-  if (is_basic(ptype) && isPromotion())
-    return false;
-
   const PtypeO old_ptypeo = oldPtypeO();
   const auto effect = ptype_effect(old_ptypeo, to_offset32(to,from));
   if (!is_definite(effect)) { // その offsetの動きがptypeに関してvalidか?
     if (to_offset(effect) == Offset_ZERO) 
       return false;
   }
   if (isPromotion()) { // promoteしている時にpromote可能か
@@ -134,19 +134,19 @@
   return Move(from().rotate180(), to().rotate180(), ptype(),
 	      capturePtype(), isPromotion(), alt(player()));
 }
 
 std::ostream& osl::operator<<(std::ostream& os,const Move move)
 {
   if (move == Move::DeclareWin())
-    return os << "MOVE_DECLARE_WIN";
+    return os << "Move_Declare_WIN";
   if (move.isInvalid())
-    return os << "MOVE_INVALID";
+    return os << "Move_Resign";
   if (move.isPass())
-    return os << "MOVE_PASS";
+    return os << "Move_Pass";
   const Player turn = move.player();
   if (move.isValid()) {
     if (move.from().isPieceStand())  {
       os << "Drop(" << move.to() << "," << move.ptype() << "," << turn << ")";
     }
     else {
       const Ptype capture_ptype=move.capturePtype();
@@ -176,28 +176,25 @@
 }
 
 
 namespace osl
 {
   static_assert(sizeof(unsigned int)*/*CHARBITS*/8>=32, "PieceStand");
 
-  const CArray<Ptype,7> PieceStand::order
-  = {{ ROOK, BISHOP, GOLD, SILVER, KNIGHT, LANCE, PAWN, }};
-
   const CArray<unsigned char,Ptype_MAX+1> PieceStand::shift
   = {{ 0,0,0,0,0,0,0,0, 28, 24, 18, 14, 10, 6, 3, 0, }};
   const CArray<unsigned char,Ptype_MAX+1> PieceStand::mask
   = {{ 0,0,0,0,0,0,0,0, (1<<2)-1, (1<<3)-1, (1<<5)-1, (1<<3)-1, (1<<3)-1, (1<<3)-1, (1<<2)-1, (1<<2)-1 }};
 }
 
 osl::PieceStand::
-PieceStand(Player pl, const SimpleState& state)
+PieceStand(Player pl, const BaseState& state)
   : flags(0)
 {
-  for (Ptype ptype: PieceStand::order)
+  for (Ptype ptype: piece_stand_order)
     add(ptype, state.countPiecesOnStand(pl, ptype));
 }
 
 bool osl::PieceStand::canAdd(Ptype type) const
 {
   const auto [l, r] = ptype_piece_id[Int(type)];
   const int max = l-r;
@@ -234,56 +231,56 @@
   std::cerr << original << " - " << other << " = " << *this << "\n";
   return false;
 }
 
 std::ostream& osl::operator<<(std::ostream& os, osl::PieceStand stand)
 {
   os << "(stand";
-  for (Ptype ptype: PieceStand::order)
+  for (Ptype ptype: piece_stand_order)
   {
     os << ' ' << stand.get(ptype);
   }
   return os << ")";
 }
 #endif
 
 std::ostream& osl::
 PieceStandIO::writeNumbers(std::ostream& os, const PieceStand& stand)
 {
-  for (Ptype ptype: PieceStand::order) {
+  for (Ptype ptype: piece_stand_order) {
     os << stand.get(ptype) << " ";
   }
   return os;
 }
 std::istream& osl::
 PieceStandIO::readNumbers(std::istream& is, PieceStand& stand)
 {
   stand  = PieceStand();
-  for (Ptype ptype: PieceStand::order) {
+  for (Ptype ptype: piece_stand_order) {
     int val;
     if (is >> val) 
       stand.add(ptype, val);
   }
   return is;
 }
 
 // pieceTable
 
 // 
 
-osl::SimpleState::SimpleState() {
-  init();
+osl::BaseState::BaseState() {
+  initEmpty();
 }
 
-osl::SimpleState::SimpleState(Handicap h) {
+osl::BaseState::BaseState(Handicap h) {
   init(h);
 }
 
-void osl::SimpleState::initPawnMask(){
-  for (Ptype ptype: PieceStand::order) {
+void osl::BaseState::initFinalize(){
+  for (Ptype ptype: piece_stand_order) {
     stand_count[BLACK][basic_idx(ptype)] = countPiecesOnStandBit(BLACK, ptype);
     stand_count[WHITE][basic_idx(ptype)] = countPiecesOnStandBit(WHITE, ptype);
   }
 
   pawnMask[0] = XNone;
   pawnMask[1] = XNone;
   for (int num: to_range(PAWN)) {
@@ -296,15 +293,15 @@
       }
       set_x(pawnMask[idx(player)], pos);
     }
   }
   assert(isConsistent());
 }
 
-void osl::SimpleState::init() {
+void osl::BaseState::initEmpty() {
   player_to_move=BLACK;
   for (int ipos=0;ipos<Square::SIZE;ipos++) {
     setBoard(Square::nth(ipos),Piece::EDGE());
   }
   for (int y: board_y_range())
     for (int x: board_x_range()) {
       setBoard(Square(x,y),Piece::EMPTY());
@@ -319,16 +316,16 @@
   pawnMask[1] = XNone;
   for (int num: all_piece_id()){
     pieces[num]=Piece(WHITE,piece_id_ptype[num],num,Square::STAND());
   }
 }
   
 
-void osl::SimpleState::init(Handicap h) {
-  init();
+void osl::BaseState::init(Handicap h) {
+  initEmpty();
   if (h != HIRATE) {
     std::cerr << "unsupported handicap\n";
     throw std::runtime_error("unsupported handicap");
   }
   // 歩
   for (int x=9;x>0;x--) {
     setPiece(BLACK,Square(x,7),PAWN);
@@ -360,21 +357,21 @@
   //
   setPiece(BLACK,Square(8,8),BISHOP);
   setPiece(WHITE,Square(2,2),BISHOP);
   //
   setPiece(BLACK,Square(2,8),ROOK);
   setPiece(WHITE,Square(8,2),ROOK);
 
-  initPawnMask();
+  initFinalize();
 }
   
 
-osl::SimpleState::~SimpleState() {}
+osl::BaseState::~BaseState() {}
 
-void osl::SimpleState::setPiece(Player player,Square pos,Ptype ptype) {
+void osl::BaseState::setPiece(Player player,Square pos,Ptype ptype) {
   for (int num: all_piece_id()) {
     if (!used_mask.test(num) && piece_id_ptype[num]==unpromote(ptype)
 	&& (ptype!=KING || 
 	    num==king_piece_id(player))) {
       used_mask.set(num);
       Piece p(player,ptype,num,pos);
       pieces[num] = p;
@@ -384,34 +381,34 @@
 	setBoard(pos,p);
 	if (ptype==PAWN)
 	  set_x(pawnMask[player], pos);
       }
       return;
     }
   }
-  std::cerr << "osl::SimpleState::setPiece! maybe too many pieces " 
+  std::cerr << "osl::BaseState::setPiece! maybe too many pieces " 
 	    << ptype << " " << pos << " " << player << "\n";
   abort();
 }
 
-void osl::SimpleState::setPieceAll(Player player) {
+void osl::BaseState::setPieceAll(Player player) {
   for (int num: all_piece_id()) {
     if (!used_mask.test(num)) {
       used_mask.set(num);
       stand_mask[player].set(num);
       Player pplayer = player;
       /* 片玉しかない問題のため */
       if (num==king_piece_id(alt(player)))
 	pplayer=alt(player);
       pieces[num] = Piece(pplayer,piece_id_ptype[num],num,Square::STAND());
     }
   }
 }
   
-bool osl::SimpleState::isConsistent() const {
+bool osl::BaseState::isConsistent() const {
   // board上の要素のconsistency
   for (int y: board_y_range()) {
     for (int x: board_x_range()) {
       const Square pos(x,y);
       const Piece p0=pieceAt(pos);
       if (p0.isPiece()) {
 	if (p0.square()!=pos)
@@ -450,15 +447,15 @@
       if (p0.isEmpty() && piece_id_ptype[num0] == KING)
 	continue;
       if (p0.id()!=num0 || ptype!=piece_id_ptype[num0] || ! p0.square().isPieceStand())
 	return false;
     }
   }
   // mask
-  for (Ptype ptype: PieceStand::order) {
+  for (Ptype ptype: piece_stand_order) {
     if (countPiecesOnStand(BLACK, ptype) != countPiecesOnStandBit(BLACK, ptype)
         || countPiecesOnStand(WHITE, ptype) != countPiecesOnStandBit(WHITE, ptype))
       return false;
   }
   // pawnMask;
   {
     CArray<BitXmask,2> pawnMask1 = {XNone, XNone};
@@ -489,28 +486,28 @@
     if (! knight.isPromoted() && knight.isOnBoard()
 	&& knight.square().blackView(knight.owner()).y() == 1)
       return false;
   }
   return true;
 }
 
-const osl::SimpleState osl::SimpleState::rotate180() const
+const osl::BaseState osl::BaseState::rotate180() const
 {
-  SimpleState ret;
+  BaseState ret;
   for (int i: all_piece_id()) {
     if(!usedMask().test(i)) continue;
     const Piece p = pieceOf(i);
     ret.setPiece(alt(p.owner()), p.square().rotate180(), p.ptype());
   }
   ret.setTurn(alt(turn()));
-  ret.initPawnMask();
+  ret.initFinalize();
   return ret;
 }
 
-bool osl::operator==(const SimpleState& st1,const SimpleState& st2)
+bool osl::operator==(const BaseState& st1,const BaseState& st2)
 {
   assert(st1.isConsistent());
   assert(st2.isConsistent());
   if (st1.turn()!=st2.turn()) 
     return false;
   if (st1.pawnMask[0]!=st2.pawnMask[0]) return false;
   if (st1.pawnMask[1]!=st2.pawnMask[1]) return false;
@@ -529,25 +526,25 @@
   namespace 
   {
     void showStand(std::ostream& os, Player player, PieceStand stand) {
       if (! stand.any())
 	return;
       
       os << "P" << to_csa(player);
-      for (Ptype ptype: PieceStand::order) {
+      for (Ptype ptype: piece_stand_order) {
 	for (unsigned int j=0; j<stand.get(ptype); ++j) {
 	  os << "00" << to_csa(ptype);
 	}
       }
       os << "\n";
     }
   } // anonymous namespace
 } // namespace osl
 
-std::ostream& osl::operator<<(std::ostream& os,const SimpleState& state)
+std::ostream& osl::operator<<(std::ostream& os,const BaseState& state)
 {
   for (int y: board_y_range()) {
     os << 'P' << y;  
     for (int x: board_x_range()) {
       os << to_csa(state.pieceOnBoard(Square(x,y)));
     }
     os << std::endl;
@@ -685,15 +682,15 @@
   return King8Info(canMoveMask);
 }
 
 
 // numSimpleEffect.tcc
 template<osl::Player P, osl::EffectOp OP>
 void  osl::effect::
-EffectSummary::doEffect(const SimpleState& state,PtypeO ptypeo,Square pos,int num)
+EffectSummary::doEffect(const BaseState& state,PtypeO ptypeo,Square pos,int num)
 {
   assert(P == owner(ptypeo));
   switch((int)ptypeo){
   case newPtypeO(P,PAWN):   doEffectBy<P,PAWN,OP>(state,pos,num); break;
   case newPtypeO(P,LANCE):  doEffectBy<P,LANCE,OP>(state,pos,num); break;
   case newPtypeO(P,KNIGHT): doEffectBy<P,KNIGHT,OP>(state,pos,num); break;
   case newPtypeO(P,SILVER): doEffectBy<P,SILVER,OP>(state,pos,num); break;
@@ -710,15 +707,15 @@
   default: assert(0);
   }
   return;
 }
 
 template<osl::Player P, osl::Ptype T, osl::EffectOp OP>
 void  osl::effect::
-EffectSummary::doEffectBy(const SimpleState& state,Square pos,int num)
+EffectSummary::doEffectBy(const BaseState& state,Square pos,int num)
 {
   if constexpr (T==LANCE || T==BISHOP || T==PBISHOP || T==ROOK || T==PROOK)
     setSourceChange(EffectPieceMask::makeLong<P>(num));
   else
     setSourceChange(EffectPieceMask::make<P>(num));
 
   doEffectShort<P,T,UL,OP>(state,pos,num);
@@ -739,15 +736,15 @@
   doEffectLong<P,T,Long_DL,OP>(state,pos,num);
   doEffectLong<P,T,Long_D,OP>(state,pos,num);
   doEffectLong<P,T,Long_DR,OP>(state,pos,num);
 }
 
 template<osl::Player P, osl::Ptype T, osl::Direction Dir, osl::EffectOp OP>
 void  osl::effect::EffectSummary::
-doEffectShort(const SimpleState& state,Square pos,int num) {
+doEffectShort(const BaseState& state,Square pos,int num) {
   if constexpr (! bittest(ptype_move_direction[idx(T)], Dir))
     return;
         
   const Square target = pos + to_offset(P,Dir);
   e_squares[target].increment<OP>(EffectPieceMask::make<P>(num));
 
   board_modified[P].setNeighbor<Dir,P>(pos);
@@ -760,15 +757,15 @@
         e_pieces[P].reset(num1);
     }
     e_pieces_modified[P].set(num1);
   }
 }
 template<osl::Player P, osl::Ptype T, osl::Direction Dir, osl::EffectOp OP>
 void  osl::effect::EffectSummary::
-doEffectLong(const SimpleState& state,Square pos,int num) {
+doEffectLong(const BaseState& state,Square pos,int num) {
   if constexpr (! bittest(ptype_move_direction[idx(T)], change_view(P,Dir)))
     return;
 
   int index_b=BoardMask::index(pos);
   constexpr Offset offset=to_offset(BLACK,Dir);
   assert(offset != Offset_ZERO);
   auto effect=EffectPieceMask::makeLong<P>(num);
@@ -819,15 +816,15 @@
         break;
       }
     }
   }
 }
 template<osl::EffectOp OP>
 void osl::effect::
-EffectSummary::doBlockAt(const SimpleState& state,Square pos,int piece_num) {
+EffectSummary::doBlockAt(const BaseState& state,Square pos,int piece_num) {
   setSourceChange(e_squares[pos]);
 
   for (int src_id: long_to_piece_id_range(e_squares[pos].selectLong())) {
     assert(32<=src_id && src_id<=39);
     auto p_src=state.pieceOf(src_id);
     auto pl_src=p_src.owner();
     auto effect=EffectPieceMask::makeLong(pl_src,src_id);
@@ -872,15 +869,15 @@
       }
     }
   }
 }
 
 // numSimpleEffect.cc
 void osl::effect::
-EffectSummary::init(const SimpleState& state)
+EffectSummary::init(const BaseState& state)
 {
   std::fill(e_squares.begin(), e_squares.end(),EffectPieceMask());
   pp_long_state.clear();
   long_piece_reach.clear();
   
   for (int num: all_piece_id()) {
     if (state.isOnBoard(num)) {
@@ -975,30 +972,30 @@
     return false;
   if (!(st1.pin_or_open == st2.pin_or_open)) 
     return false;
   if (!(st1.king_visibility == st2.king_visibility)) 
     return false;
   if (!(st1.king8infos == st2.king8infos)) 
     return false;
-  return (static_cast<const SimpleState&>(st1)
-	  == static_cast<const SimpleState&>(st2));
+  return (static_cast<const BaseState&>(st1)
+	  == static_cast<const BaseState&>(st2));
 }
 
 template<osl::Player P>
 void osl::EffectState::makeKing8Info()
 {
   king8infos[P] = King8Info{0};
   if (kingSquare<P>().isPieceStand())
     return;
   king8infos[P]=to_king8info<alt(P)>(*this,kingSquare<P>());
 }
 
 osl::
-EffectState::EffectState(const SimpleState& st) 
-  : SimpleState(st),effects(st)
+EffectState::EffectState(const BaseState& st) 
+  : BaseState(st),effects(st)
 {
   pieces_onboard[0].resetAll();
   pieces_onboard[1].resetAll();
   promoted.resetAll();
   effects.e_pieces[0].resetAll();
   effects.e_pieces[1].resetAll();
   effects.e_pieces_modified[0].resetAll();
@@ -1261,15 +1258,15 @@
   stand_mask[P] ^= PieceMask(num_one_hot);
   stand_count[P][basic_idx(ptype)]--;
   pieces_onboard[P] ^= PieceMask(num_one_hot);
   return num;
 }
 
 bool osl::EffectState::isConsistent() const {
-  if (!SimpleState::isConsistent()) 
+  if (!BaseState::isConsistent()) 
     return false;
   EffectSummary effects1(*this);
   if (!(effects1==effects)) 
     return false;
   for (Player p: players) {
     if (kingSquare(p).isPieceStand())
       continue;
@@ -1330,14 +1327,17 @@
         return false;      
     }
   }
   return true;
 }
 
 bool osl::EffectState::isLegalLight(Move move) const {
+  if (move == Move::DeclareWin())
+    return win_if_declare(*this);
+
   assert(this->turn() == move.player());
   assert(move.isConsistent());
 
   const Square to=move.to(), from=move.from();
   if (from.isPieceStand()) { // 打つ手 isAlmostValidDrop(move);
     const Ptype ptype=move.ptype();
     // ターゲットが空白か そもそもその駒を持っているか? 二歩?
@@ -1491,15 +1491,16 @@
     if (move.hasIgnoredUnpromote())
       moves.push_back(move.unpromote());
   }
 }
 
 osl::Move osl::EffectState::tryCheckmate1ply() const {
   auto best_move=Move::PASS(turn());
-  ImmediateCheckmate::hasCheckmateMove(turn(),*this,best_move);
+  if (! inCheck())
+    ImmediateCheckmate::hasCheckmateMove(turn(),*this,best_move);
   return best_move;
 }
 
 void osl::EffectState::
 findEffect(Player P, Square target, PieceVector& out) const
 {
   effect_action::StorePiece store(&out);
```

### Comparing `miniosl-0.0.2/minioslcc/src/state.h` & `miniosl-0.0.3a1/minioslcc/src/state.h`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,17 @@
   constexpr Ptype piece_ptype[] = { 
     PPAWN, PLANCE, PKNIGHT, PSILVER, PBISHOP, PROOK,
       KING, GOLD, PAWN, LANCE, KNIGHT, SILVER, BISHOP, ROOK,
   };
   constexpr Ptype basic_ptype[] = { 
     KING, GOLD, PAWN, LANCE, KNIGHT, SILVER, BISHOP, ROOK,
   };
+  /** 持駒の表示で良く使われる順番 */
+  constexpr std::array<Ptype,7> piece_stand_order = { ROOK, BISHOP, GOLD, SILVER, KNIGHT, LANCE, PAWN, };
+
   constexpr int Int(Ptype ptype) { return static_cast<int>(ptype); }
   constexpr int Ptype_MIN=0, Ptype_Basic_MIN=Int(KING),
     Ptype_Piece_MIN=2, Ptype_MAX=15, Ptype_SIZE=16;
   constexpr int idx(Ptype ptype) { return Int(ptype); }
   constexpr mask_t one_hot(Ptype ptype) { return one_hot(idx(ptype)); }
   constexpr int basic_idx(Ptype ptype) { return Int(ptype) - Ptype_Basic_MIN; }
   constexpr bool is_valid(Ptype ptype) {
@@ -173,15 +176,19 @@
   constexpr bool can_promote(PtypeO ptypeO) { return can_promote(ptype(ptypeO)); }
   /**
    * ptypeOが promote済みかどうか
    */
   constexpr bool is_promoted(PtypeO ptypeO) { return is_promoted(ptype(ptypeO)); }
   
   std::ostream& operator<<(std::ostream& os,const PtypeO ptypeO);
-  
+
+  /** Direction.
+   * steps achievable by a legal move only, i.e., no DDL or DDR.
+   * still, subtraction (sq - to_offset(UUL)) yields inverse step.
+   */
   enum class Direction{
     UL=0, U=1, UR=2,
     L=3, R=4,
     DL=5, D=6, DR=7,
     UUL=8, UUR=9,
     Long_UL=10, Long_U=11, Long_UR=12,
     Long_L=13, Long_R=14,
@@ -287,14 +294,19 @@
       KING, GOLD, PAWN, LANCE, KNIGHT, SILVER, BISHOP, ROOK,
     }};
   constexpr std::array<std::pair<int,int>, Ptype_SIZE> ptype_piece_id = {{
       {0, 0}, {0, 0},
       {0, 18}, {26, 30}, {18, 22}, {22, 26}, {36, 38}, {38, 40}, 
       {30, 32}, {26, 30}, {0, 18}, {32, 36}, {18, 22}, {22, 26}, {36, 38}, {38, 40}, 
     }};
+  constexpr int ptype_piece_count(Ptype ptype) {
+    auto r = ptype_piece_id[idx(ptype)];
+    return r.second-r.first;
+  }
+  
   template <Direction d>
   constexpr int ptype_set() {
     auto good = std::views::iota(Ptype_Piece_MIN, Ptype_MAX+1) // all_piece_ptype()
       | std::views::filter([](int p){
         return bittest(ptype_move_direction[p], d) || bittest(ptype_move_direction[p], to_long(d)); })
       | std::views::transform([](int p){ return one_hot(p); });
     return std::reduce(good.begin(), good.end()); // fold@c++23
@@ -731,15 +743,14 @@
 
   inline bool operator<(Piece l, Piece r) { return l.intValue() < r.intValue(); }
   std::ostream& operator<<(std::ostream& os,const Piece piece);
 }
 
 namespace osl
 {
-  class SimpleState;
   /**
    * 圧縮していない moveの表現 .
    * - invalid: isNormal 以外の演算はできない
    * - declare_win: isNormal 以外の演算はできない
    * - pass: from, to, ptype, oldPtype はとれる．player()はとれない．
    * 
    * Pieceとpromotepをそろえる  -> 変える． 
@@ -758,16 +769,16 @@
   public:
     static constexpr int BitOffsetPromote=Piece::BitOffsetMovePromote;  // 23
   private:
     int move;
     explicit Move(int value) : move(value) {
     }
     enum { 
-      INVALID_VALUE = (1<<8), DECLARE_WIN = (2<<8),
-      BLACK_PASS = 0, WHITE_PASS = (-1)<<28, 
+      Resign_VALUE = (1<<8), Declare_WIN = (2<<8),
+      Black_PASS = 0, White_PASS = (-1)<<28, 
     };
   public:
     int intValue() const { return move; }
     /** 一局面辺りの合法手の最大値 
      * 重複して手を生成することがある場合は，600では不足かもしれない
      */
     static const unsigned int MaxUniqMoves=600;
@@ -779,27 +790,27 @@
  	       + (from.uintValue()<<8)
 	       + (static_cast<unsigned int>(capture_ptype)<<16)
 	       + (static_cast<unsigned int>(is_promote)<<BitOffsetPromote)
 	       + (static_cast<unsigned int>(ptype)<<24)
 	       + (Int(player)<<28));
     }
   public:
-    Move() : move(INVALID_VALUE)
+    Move() : move(Resign_VALUE)
     {
     }
-    /** INVALID でも PASS でもない. isValid()かどうかは分からない．*/
+    /** Resign でも PASS でもない. isValid()かどうかは分からない．*/
     bool isNormal() const { 
-      // PASS や INVALID は to() が 00
+      // PASS や Resign は to() が 00
       return move & 0x00ff; 
     }
     bool isPass() const { return (move & 0xffff) == 0; }
     static const Move makeDirect(int value) { return Move(value); }
     static const Move PASS(Player P) { return Move(Int(P)<<28); }
-    static const Move INVALID() { return Move(INVALID_VALUE); }
-    static const Move DeclareWin() { return Move(DECLARE_WIN); }
+    static const Move Resign() { return Move(Resign_VALUE); }
+    static const Move DeclareWin() { return Move(Declare_WIN); }
     /**
      * 移動
      */
     Move(Square from, Square to, Ptype ptype,
 	 Ptype capture_ptype, bool is_promote, Player player)
     {
       init(from, to, ptype, capture_ptype, is_promote, player);
@@ -876,15 +887,15 @@
     Player player() const {
       assert(! isInvalid());
       return Player{move>>28};
     }
     bool isValid() const;
     /** state に apply 可能でない場合にtrue */
     bool isInvalid() const { 
-      return static_cast<unsigned int>(move-1) < DECLARE_WIN; 
+      return static_cast<unsigned int>(move-1) < Declare_WIN; 
     }
     bool isValidOrPass() const { return isPass() || isValid(); }
     /** おおむね合法手 */
     bool isConsistent() const;
     /**
      * no capture moveからcapture moveを作る
      */
@@ -1324,29 +1335,29 @@
 namespace osl
 {
   enum Handicap{
     HIRATE,
     //    KYOUOCHI,
     //    KAKUOCHI,
   };
-  class SimpleState;
-  std::ostream& operator<<(std::ostream& os,const SimpleState& state);
+  class BaseState;
+  std::ostream& operator<<(std::ostream& os,const BaseState& state);
   /**
    * 盤上の駒のみを比較する（持ち駒は見ない）.
    * なお、駒番に非依存な局面比較をしたい場合は、osl::record::CompactBoardや
    * osl::hash::HashKeyを用いる.
    */
-  bool operator==(const SimpleState& st1,const SimpleState& st2);
+  bool operator==(const BaseState& st1,const BaseState& st2);
   
-  class alignas(32) SimpleState
+  class alignas(32) BaseState
   {
   private:
-    friend std::ostream& operator<<(std::ostream& os,const SimpleState& state);
-    friend bool operator==(const SimpleState& st1,const SimpleState& st2);
-    typedef SimpleState state_t;
+    friend std::ostream& operator<<(std::ostream& os,const BaseState& state);
+    friend bool operator==(const BaseState& st1,const BaseState& st2);
+    typedef BaseState state_t;
   public:
     static const bool hasPawnMask=true;
   protected:
     CArray<Piece,Square::SIZE> board;
     /**
      * 全てのpieceが登録されている
      */
@@ -1356,24 +1367,23 @@
     CArray<CArray<char,basic_idx(Ptype(Ptype_SIZE))>,2> stand_count;
 
     /** 手番 */
     Player player_to_move;
     PieceMask used_mask;
   public:
     // 生成に関するもの
-    explicit SimpleState();
-    explicit SimpleState(Handicap h);
+    explicit BaseState();
+    explicit BaseState(Handicap h);
     // public継承させるので，virtual destructorを定義する．
-    virtual ~SimpleState();
-    /** 盤面が空の状態に初期化 */
-    void init();
-    /** ハンディに応じた初期状態に初期化 */
+    virtual ~BaseState();
+    /** set predefined initial state */
     void init(Handicap h);
-    // private:
-    void initPawnMask();
+    /** make empty board ready for manual initialization via setPiece() */
+    void initEmpty();
+    void initFinalize();
   public:
     const Piece pieceOf(int num) const { return pieces[num]; }
     inline auto all_pieces() const {
       return std::views::iota(0, Piece::SIZE)
         | std::views::transform([this](int n) { return this->pieceOf(n); });
     }
     inline auto long_pieces() const {
@@ -1456,15 +1466,15 @@
       for (; pieceAt(sq).isEmpty(); sq+=offset) {
         if (!pieceExistsAtTo && sq==to) 
           return true;
       }
       return sq==to;
       
     }
-    const SimpleState rotate180() const;
+    const BaseState rotate180() const;
   };  
 
 } // namespace osl
 
 // boardMask.h
 namespace osl 
 {
@@ -1745,51 +1755,51 @@
        * @param OP(template) - 利きを足すか，減らすか
        * @param state - 盤面(動かした後)
        * @param ptypeo - 駒の種類
        * @param pos - 駒の位置
        * @param num - 駒番号
        */
       template<Player P,EffectOp OP>
-        void doEffect(const SimpleState& state,PtypeO ptypeo,Square pos,int num);
+        void doEffect(const BaseState& state,PtypeO ptypeo,Square pos,int num);
 
       /**
        * ある駒が持つ利きを更新する.
        * @param OP(template) - 利きを足すか，減らすか
        * @param state - 盤面(動かした後)
        * @param p - 駒
        */
       template<EffectOp OP>
-        void doEffect(const SimpleState& state,Piece p) {
+        void doEffect(const BaseState& state,Piece p) {
         if (p.owner() == BLACK)
           doEffect<BLACK,OP>(state,p.ptypeO(),p.square(),p.id());
         else
           doEffect<WHITE,OP>(state,p.ptypeO(),p.square(),p.id());
       }
       /**
        * 盤面のデータを元に初期化する.
        * @param state - 盤面
        */
-      void init(const SimpleState& state);
+      void init(const BaseState& state);
       /**
        * コンストラクタ.
        */
-      EffectSummary(const SimpleState& state) { init(state); }
+      EffectSummary(const BaseState& state) { init(state); }
       /**
        * ある位置の利きデータを取り出す.
        * @param pos - 位置
        */
       EffectPieceMask effectAt(Square pos) const { return e_squares[pos]; }
       /**
        * posに駒を設置/削除して長い利きをブロック/延長する際の利きデータの更新.
        * @param OP(template) - 利きを足すか，減らすか
        * @param state - 局面の状態 posに駒を置く前でも後でもよい
        * @param pos - 変化する位置
        */
       template<EffectOp OP>
-        void doBlockAt(const SimpleState& state,Square pos,int piece_num);
+        void doBlockAt(const BaseState& state,Square pos,int piece_num);
       friend bool operator==(const EffectSummary& et1,const EffectSummary& et2);
       /*
        *
        */
       const BoardMask changedEffects(Player pl) const { return board_modified[pl]; }
       void setSourceChange(EffectPieceMask const& effect) { source_pieces_modified |= effect; }
       void clearPast() {
@@ -1809,38 +1819,38 @@
        * @param T(template) - ある位置にある駒の種類
        * @param D(template) - 駒の所有者の立場から見た方向
        * @param OP(template) - 利きを足すか，減らすか
        * @param pos - 駒の位置
        * @param num - 駒番号
        */
       template<Player P,Ptype T,Direction Dir,EffectOp OP>
-        void doEffectShort(const SimpleState& state,Square pos,int num);
+        void doEffectShort(const BaseState& state,Square pos,int num);
       /**
        * ある位置からある方向に長い利きがある時に，その方向の利きを更新する.
        * @param P(template) - ある位置にある駒の所有者
        * @param T(template) - ある位置にある駒の種類
        * @param Dir(template) - 黒の立場から見た方向
        * @param OP(template) - 利きを足すか，減らすか
        * @param state - 盤面(動かした後)
        * @param pos - 駒の位置
        * @param num - 駒番号
        */
       template<Player P,Ptype T,Direction Dir,EffectOp OP>
-        void doEffectLong(const SimpleState& state,Square pos,int num);
+        void doEffectLong(const BaseState& state,Square pos,int num);
       /**
        * ある種類の駒が持つ利きを更新する.
        * @param P(template) - ある位置にある駒の所有者
        * @param T(template) - ある位置にある駒の種類
        * @param OP(template) - 利きを足すか，減らすか
        * @param state - 盤面(動かした後)
        * @param pos - 駒の位置
        * @param num - 駒番号
        */ 
      template<Player P,Ptype T,EffectOp OP>
-        void doEffectBy(const SimpleState& state,Square pos,int num);      
+        void doEffectBy(const BaseState& state,Square pos,int num);      
     };
 
     inline bool operator!=(const EffectSummary& et1,const EffectSummary& et2)
     {
       return !(et1==et2);
     }
 
@@ -1871,15 +1881,15 @@
   bool operator==(const EffectState& st1, const EffectState& st2);
 
   /**
    * 利きを持つ局面
    * - effects (EffectSummary) 利き
    * - pieces_onboard (PieceMask) 盤上にある駒
    */
-  class EffectState : public SimpleState
+  class EffectState : public BaseState
   {
     EffectSummary effects;
     CArray<PieceMask,2> pieces_onboard;
     /** 成駒一覧 */
     PieceMask promoted;
     CArray<PieceMask,2> pin_or_open;
     CArray<KingVisibility,2> king_visibility;
@@ -1887,15 +1897,15 @@
 
     friend bool operator==(const EffectState& st1,const EffectState& st2);
     typedef EffectState state_t;
   public:
     // ----------------------------------------------------------------------
     // 0. 将棋以外の操作
     // ----------------------------------------------------------------------
-    explicit EffectState(const SimpleState& st=SimpleState(HIRATE));
+    explicit EffectState(const BaseState& st=BaseState(HIRATE));
     ~EffectState();
     /** 主要部分を高速にコピーする. 盤の外はコピーされない*/
     void copyFrom(const EffectState& src);
     bool isConsistent() const;
 
     // ----------------------------------------------------------------------
     // 1. 盤面全体の情報
```

### Comparing `miniosl-0.0.2/minioslcc/test/minitest.cc` & `miniosl-0.0.3a1/minioslcc/test/minitest.cc`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 #include "state.h"
 #include "more.h"
 #include "record.h"
 #include "checkmate.h"
 #include <iostream>
 #include <bitset>
 #include <algorithm>
+#include <filesystem>
+#include <fstream>
 
 #define TEST_CHECK_EQUAL(a,b) TEST_CHECK((a) == (b))
 #define TEST_ASSERT_EQUAL(a,b) TEST_ASSERT((a) == (b))
 
 using namespace osl;
 
 template <class Container, class T>
@@ -241,15 +243,15 @@
   p+=make_offset(-2,2);
   TEST_CHECK(p==Square(4,9));
   p-=make_offset(-5,3);
   TEST_CHECK(p==Square(9,6));
 }
 
 bool max_of_two(PieceStand l, PieceStand r, PieceStand m) {
-  for (auto ptype: PieceStand::order) {
+  for (auto ptype: piece_stand_order) {
     if (std::max(l.get(ptype), r.get(ptype)) != m.get(ptype))
       return false;
   }
   return true;
 }
 
 void test_piece_stand() {
@@ -392,15 +394,15 @@
     p1.subAtmostOnePiece(pRook);
     p1.subAtmostOnePiece(pKing);
 
     TEST_CHECK_EQUAL(PieceStand(0,0,0,0,0,0,0,0),p1);
   }
   {
     PieceStand src;
-    for (auto ptype: PieceStand::order) {
+    for (auto ptype: piece_stand_order) {
         src.add(ptype, random() % 3);
     }
     std::stringstream ss;
     PieceStandIO::writeNumbers(ss, src);
     PieceStand dst;
     PieceStandIO::readNumbers(ss, dst);
     
@@ -582,14 +584,38 @@
     const Move m69(Square(6,9), SILVER, WHITE);
     TEST_CHECK_EQUAL(m41.rotate180(), m69);
 
     TEST_CHECK_EQUAL(Move::PASS(BLACK).rotate180(), Move::PASS(WHITE));
   }
 }
 
+void test_csa() {
+  {
+    EffectState state;
+    Move move = csa::to_move("+7776FU", state);
+    TEST_CHECK(move.isNormal());
+    TEST_CHECK(! move.isInvalid());
+    TEST_CHECK(! move.isPass());
+    TEST_CHECK(move.from() == Square(7,7));
+    TEST_CHECK(move.to() == Square(7,6));
+    TEST_CHECK(move.ptype() == PAWN);
+    TEST_CHECK(! move.isCapture());
+    TEST_CHECK(! move.ignoreUnpromote());
+    TEST_CHECK(! move.hasIgnoredUnpromote());
+
+    try {
+      move = csa::to_move("+7775FU", state);
+      TEST_CHECK(! move.isNormal());
+    }
+    catch (std::runtime_error& e) {
+    }
+  }
+}
+
+
 void test_offset()
 {
   TEST_CHECK(to_offset(BLACK, UL) != Offset_ZERO);
   for (int dx: std::views::iota(-8,9))
     for (int dy: std::views::iota(-8,9)) 
       for (auto ptypeo: all_ptypeO_range()) {
         auto offset32 = to_offset32(dx,dy);
@@ -826,15 +852,15 @@
 			 moves(king8));
     TEST_CHECK_EQUAL((one_hot(UL)),libertyCount(king8));
   }
 }
 
 void test_state() {
   {
-    SimpleState state;
+    BaseState state;
     TEST_ASSERT(state.isConsistent());
   }
   {
     EffectState state;
     TEST_ASSERT(state.isConsistent());
   }
 }
@@ -1188,15 +1214,15 @@
                                    "P8 *  *  *  *  *  *  *  *  * \n"
                                    "P9 * +OU * -GI *  *  *  * -NG\n"
                                    "P+00HI00KI00KE00KY00FU00FU00FU00FU00FU00FU\n"
                                    "P-00KI00KY00FU00FU\n"
                                    "P-00AL\n"
                                    "+\n");
     TEST_CHECK(state.isConsistent());
-    testEffectedState(state,Move::INVALID());
+    testEffectedState(state,Move::Resign());
     { // simple move
       EffectState state1=state;
       TEST_CHECK(state1.isConsistent());
       Move move(Square(8,3),Square(8,2),PROOK,Ptype_EMPTY,false,BLACK);
       state1.makeMove(move);
       TEST_ASSERT(state1.isConsistent());
       testEffectedState(state1,move);
@@ -1845,15 +1871,15 @@
   }
   {
     EffectState state;
     const std::string hirate = "lnsgkgsnl/1r5b1/ppppppppp/9/9/9/PPPPPPPPP/1B5R1/LNSGKGSNL";
 
     EffectState state2;
     usi::parse_board(hirate, state2);
-    TEST_CHECK_EQUAL(static_cast<const SimpleState&>(state), state2);
+    TEST_CHECK_EQUAL(static_cast<const BaseState&>(state), state2);
   }
   {
     EffectState state;
     const std::string hirate = "8l/1l+R2P3/p2pBG1pp/kps1p4/Nn1P2G2/P1P1P2PP/1PS6/1KSG3+r1/LN2+p3L";
 
     EffectState state2;
     TEST_CHECK((usi::parse_board(hirate, state2), true));
@@ -1872,15 +1898,15 @@
                                      "P9+KY+KE+GI+KI+OU+KI+GI+KE+KY\n"
                                      "-\n"));
 
       const std::string s763426 = "startpos moves 7g7f 3c3d 2g2f";
 
       EffectState state2;
       usi::parse(s763426, state2);
-      TEST_CHECK_EQUAL(static_cast<const SimpleState&>(state), state2);
+      TEST_CHECK_EQUAL(static_cast<const BaseState&>(state), state2);
     }
     {
       EffectState state(csa::read_board(
                                      "P1-KY-KE-GI-KI-OU-KI-GI-KE-KY\n"
                                      "P2 * -HI *  *  *  *  *  *  * \n"
                                      "P3 *  *  * -FU-FU-FU-FU-FU-FU\n"
                                      "P4 *  *  *  *  *  *  *  *  * \n"
@@ -1893,20 +1919,20 @@
                                      "P-00KA00FU00FU00FU\n"
                                      "-\n"));
 
       const std::string stest = "sfen lnsgkgsnl/1r7/3pppppp/9/9/9/PPPPPPP2/1B5R1/LN1GKGSNL w S2Pb3p 1";
 
       EffectState state2;
       usi::parse(stest, state2);
-      TEST_CHECK_EQUAL(static_cast<const SimpleState&>(state), state2);
+      TEST_CHECK_EQUAL(static_cast<const BaseState&>(state), state2);
 
       const std::string stest3 = "sfen lnsgkgsnl/1r7/3pppppp/9/9/9/PPPPPPP2/1B5R1/LN1GKGSNL w S2Pb3p";
       EffectState state3;
       usi::parse(stest3, state3);
-      TEST_CHECK_EQUAL(static_cast<const SimpleState&>(state), state3);
+      TEST_CHECK_EQUAL(static_cast<const BaseState&>(state), state3);
     }
   }
   {
     EffectState state;
 
     TEST_EXCEPTION(usi::parse_board("lnsgkgsna/1r5b1/ppppppppp/9/9/9/PPPPPPPPP/1B5R1/LNSGKGSNL", state), // invalid ascii character a
                    osl::usi::ParseError);
@@ -1966,15 +1992,15 @@
                                      "P9+OU * +KI *  *  *  *  * +KY\n"
                                      "P+00KA00GI00GI00KE00KE00FU00FU\n"
                                      "P-00HI00KI00KI00FU\n"
                                      "+"));
       TEST_CHECK_EQUAL(str, to_usi(state));
       EffectState test;
       usi::parse(str, test);
-      TEST_CHECK_EQUAL(static_cast<const SimpleState&>(state), test);
+      TEST_CHECK_EQUAL(static_cast<const BaseState&>(state), test);
     }
     {
       std::string str = "sfen lnsg4l/2k2R+P2/pppp1s2p/9/4p1P2/2P2p+n2/PP1P4P/2KSG1p2/LN1G4L w BG2Prbsnp 1";
       EffectState state(csa::read_board(
                                      "P1-KY-KE-GI-KI *  *  *  * -KY\n"
                                      "P2 *  * -OU *  * +HI+TO *  * \n"
                                      "P3-FU-FU-FU-FU * -GI *  * -FU\n"
@@ -1986,30 +2012,28 @@
                                      "P9+KY+KE * +KI *  *  *  * +KY\n"
                                      "P+00KA00KI00FU00FU\n"
                                      "P-00HI00KA00GI00KE00FU\n"
                                      "-\n"));
       TEST_CHECK_EQUAL(str, to_usi(state));
       EffectState test;
       usi::parse(str, test);
-      TEST_CHECK_EQUAL(static_cast<const SimpleState&>(state), test);
+      TEST_CHECK_EQUAL(static_cast<const BaseState&>(state), test);
     }
   }
   {
     {
       const std::string sfen = "position sfen lnsgkgsnl/9/ppppppppp/9/9/9/PPPPPPPPP/1B5R1/LNSGKGSNL w - 1 moves 5a6b 2g2f 6b7b 2f2e 7b8b 2e2d 2c2d 2h2d";
-      EffectState state;
-      std::vector<Move> moves;
-      TEST_CHECK((usi::parse(sfen, state, moves), true)); // no throw
-
-      for (Ptype ptype: PieceStand::order) {
+      auto record = usi::read_record(sfen);
+      auto state = record.initial_state;
+      for (Ptype ptype: piece_stand_order) {
         TEST_CHECK_EQUAL(0, state.countPiecesOnStand(BLACK, ptype));
         TEST_CHECK_EQUAL(0, state.countPiecesOnStand(WHITE, ptype));
       }
 
-      for (Move move: moves) {
+      for (Move move: record.moves) {
         MoveVector all;
         state.generateLegal(all);
         TEST_CHECK(is_member(all, move));
         state.makeMove(move);
 
         for (int i = 0; i < Piece::SIZE; ++i) {
           if (! state.usedMask().test(i)) {
@@ -4357,29 +4381,307 @@
     auto moves = generate_check_move(state);
     // open move
     TEST_CHECK(is_member(moves, Move(Square(1,5),Square(1,7),LANCE,ROOK,false,WHITE)));
     TEST_CHECK(!is_member(moves, Move(Square(1,5),Square(1,7),PLANCE,ROOK,true,WHITE)));
   }
 }
 
+std::pair<int,int> find2(const auto& array) {
+  int a=0, b=0;
+  while (array[a] == 0) ++a;
+  b=a+1;
+  while (array[b] == 0) ++b;
+  return std::make_pair(a,b);
+}
+
+void test_combination_id() {
+  using osl::bitpack::detail::combination_id;
+  
+  TEST_CHECK(combination_id(0,1) == 0);
+  TEST_CHECK(combination_id(0,2) == 1);
+  TEST_CHECK(combination_id(1,2) == 2);
+
+  TEST_CHECK(combination_id(7,8) == 36-1); // 9C2
+  TEST_CHECK(combination_id(36,37) == 38*37/2-1); // 38C2
+
+  for (int a: std::views::iota(0,37))
+    for (int b: std::views::iota(a+1,38)) {
+      auto [c, d] = bitpack::detail::unpack2(combination_id(a,b));
+      TEST_ASSERT(a == c && b == d);
+    }
+
+  TEST_CHECK(combination_id(0,1,2) == 0);
+  TEST_CHECK(combination_id(0,1,3) == 1);
+  TEST_CHECK(combination_id(0,2,3) == 2);
+  TEST_CHECK(combination_id(1,2,3) == 3);
+
+  TEST_CHECK(combination_id(7,8,9) == 10*9*8/6-1); // 10C3
+
+  TEST_CHECK(combination_id(0,1,2,3) == 0);
+  TEST_CHECK(combination_id(0,1,2,4) == 1);
+  TEST_CHECK(combination_id(0,1,3,4) == 2);
+  TEST_CHECK(combination_id(0,2,3,4) == 3);
+  TEST_CHECK(combination_id(1,2,3,4) == 4);
+
+  TEST_CHECK(combination_id(6,7,8,9) == 10*9*8*7/24-1); // 10C4
+  TEST_CHECK(combination_id(30,31,32,33) == 34*33*32*31/24-1); // 34C4
+
+  for (int a: std::views::iota(0,34))
+    for (int b: std::views::iota(a+1,34)) 
+      for (int c: std::views::iota(b+1,34)) 
+        for (int d: std::views::iota(c+1,34)) {
+          auto [p, q, r, s] = bitpack::detail::unpack4(combination_id(a,b,c,d));
+          TEST_ASSERT(a == p && b == q && c == r && d == s);
+        }
+}
+
+void test_pack_position() {
+  {
+    PackedState ps;
+    auto bs = ps.to_bitset();
+    PackedState ps2;
+    ps2.restore(bs);
+    TEST_CHECK(to_usi(ps.state) == to_usi(ps2.state));
+  }
+  {
+    auto sfen = "sfen l2g3nl/5k3/2npppsgp/p2s2p2/5P1pP/PrPPS1R2/4P1P2/2G1K1G2/LNS4NL b B3Pbp 1";
+    EffectState state = usi::to_state(sfen);
+    
+    PackedState ps = {state};
+    auto bs = ps.to_bitset();
+    PackedState ps2;
+    ps2.restore(bs);
+
+    TEST_CHECK(sfen == to_usi(ps2.state));
+  }
+}
+
+void test_win_if_declare()
+{
+  {
+    const EffectState state;
+    TEST_CHECK( !win_if_declare(state) );
+  }
+  {
+    auto state=csa::read_board("P1 *  * +RY *  * +KI * -KE * \n"
+                               "P2+OU+TO+UM+UM+TO * -KI-OU * \n"
+                               "P3-FU+FU+FU+FU+FU-GI-GI *  * \n"
+                               "P4 *  *  *  * -FU-FU-FU-FU * \n"
+                               "P5 *  * -RY-NY-GI *  *  *  * \n"
+                               "P6 *  *  *  *  * +FU+FU+FU * \n"
+                               "P7 *  *  *  *  * +KI+KE * -NY\n"
+                               "P8 *  *  *  *  * +KI+GI *  * \n"
+                               "P9 *  *  *  * -NY *  *  *  * \n"
+                               "P+00FU00FU00FU00FU00KY00KE00KE\n"
+                               "+\n");
+    TEST_CHECK( win_if_declare(state) );
+  }
+  {
+    auto state=csa::read_board("P1 *  *  *  * +NY *  *  *  * \n"
+                               "P2 *  *  *  *  * -KI-GI *  * \n"
+                               "P3 *  *  *  *  * -KI-KE * +NY\n"
+                               "P4 *  *  *  *  * -FU-FU-FU * \n"
+                               "P5 *  * +RY+NY+GI *  *  *  * \n"
+                               "P6 *  *  *  * +FU+FU+FU+FU * \n"
+                               "P7+FU-FU-FU-FU-FU+GI+GI *  * \n"
+                               "P8-OU-TO-UM-UM-TO * +KI+OU * \n"
+                               "P9 *  * -RY *  * -KI * +KE * \n"
+                               "P-00FU00FU00FU00FU00KY00KE00KE\n"
+                               "-\n");
+    TEST_CHECK( win_if_declare(state) );
+  }
+  {
+    auto state=csa::read_board("P1 *  * +RY *  * +KI * -KE * \n"
+                               "P2+OU+TO+UM+UM+TO * -KI-OU * \n"
+                               "P3-FU+FU+FU+FU * -GI-GI *  * \n"
+                               "P4 *  *  *  * -FU-FU-FU-FU * \n"
+                               "P5 *  * -RY-NY-GI *  *  *  * \n"
+                               "P6 *  *  *  *  * +FU+FU+FU * \n"
+                               "P7 *  *  *  *  * +KI+KE * -NY\n"
+                               "P8 *  *  *  *  * +KI+GI *  * \n"
+                               "P9 *  *  *  * -NY *  *  *  * \n"
+                               "P+00FU00FU00FU00FU00KY00KE00KE\n"
+                               "P-00FU\n"
+                               "+\n");
+    TEST_CHECK( !win_if_declare(state) );
+  }
+  {
+    auto state=csa::read_board("P1 *  *  *  * +NY *  *  *  * \n"
+                               "P2 *  *  *  *  * -KI-GI *  * \n"
+                               "P3 *  *  *  *  * -KI-KE * +NY\n"
+                               "P4 *  *  *  *  * -FU-FU-FU * \n"
+                               "P5 *  * +RY+NY+GI *  *  *  * \n"
+                               "P6 *  *  *  * +FU+FU+FU+FU * \n"
+                               "P7+FU-FU-FU-FU * +GI+GI *  * \n"
+                               "P8-OU-TO-UM-UM-TO * +KI+OU * \n"
+                               "P9 *  * -RY *  * -KI * +KE * \n"
+                               "P+00FU\n"
+                               "P-00FU00FU00FU00FU00KY00KE00KE\n"
+                               "-\n");
+    TEST_CHECK( !win_if_declare(state) );
+  }
+  {
+    auto state=csa::read_board("P1 *  * +RY *  * +KI * -KE * \n"
+                               "P2+OU+TO+UM+TO+TO * -KI-OU * \n"
+                               "P3-FU+FU+FU+FU+FU-GI-GI *  * \n"
+                               "P4 *  *  *  * -FU-FU-FU-FU * \n"
+                               "P5 *  * -RY-NY-GI *  *  *  * \n"
+                               "P6 *  *  *  *  * +FU+FU+FU * \n"
+                               "P7+UM *  *  *  * +KI+KE * -NY\n"
+                               "P8 *  *  *  *  * +KI+GI *  * \n"
+                               "P9 *  *  *  * -NY *  *  *  * \n"
+                               "P+00FU00FU00FU00KY00KE00KE\n"
+                               "+\n");
+    TEST_CHECK( !win_if_declare(state) );
+  }
+  {
+    auto state=csa::read_board("P1 *  *  *  * +NY *  *  *  * \n"
+                               "P2 *  *  *  *  * -KI-GI *  * \n"
+                               "P3-UM *  *  *  * -KI-KE * +NY\n"
+                               "P4 *  *  *  *  * -FU-FU-FU * \n"
+                               "P5 *  * +RY+NY+GI *  *  *  * \n"
+                               "P6 *  *  *  * +FU+FU+FU+FU * \n"
+                               "P7+FU-FU-FU-FU-FU+GI+GI *  * \n"
+                               "P8-OU-TO-UM-TO-TO * +KI+OU * \n"
+                               "P9 *  * -RY *  * -KI * +KE * \n"
+                               "P-00FU00FU00FU00KY00KE00KE\n"
+                               "-\n");
+    TEST_CHECK( !win_if_declare(state) );
+  }
+  {
+    auto state=csa::read_board("P1 *  * +RY *  * +KI * -KE * \n"
+                               "P2+OU+TO+UM+UM+TO * -KI-OU * \n"
+                               "P3-FU+FU+FU+FU+FU-GI-GI *  * \n"
+                               "P4 *  *  *  * -FU-FU-FU-FU * \n"
+                               "P5 *  * -RY-NY-GI *  *  *  * \n"
+                               "P6 *  *  *  *  * +FU+FU+FU * \n"
+                               "P7 *  *  *  *  * +KI+KE * -NY\n"
+                               "P8 *  *  *  *  * +KI+GI *  * \n"
+                               "P9 *  *  *  * -NY *  *  *  * \n"
+                               "P+00FU00FU00FU00FU00KY00KE00KE\n"
+                               "+\n");
+    bool kachi = win_if_declare(state);
+    TEST_CHECK(kachi);
+  }
+  {
+    auto state=csa::read_board("P1 *  *  *  * +NY *  *  *  * \n"
+                               "P2 *  *  *  *  * -KI-GI *  * \n"
+                               "P3 *  *  *  *  * -KI-KE * +NY\n"
+                               "P4 *  *  *  *  * -FU-FU-FU * \n"
+                               "P5 *  * +RY+NY+GI *  *  *  * \n"
+                               "P6 *  *  *  * +FU+FU+FU+FU * \n"
+                               "P7+FU-FU-FU-FU-FU+GI+GI *  * \n"
+                               "P8-OU-TO-UM-UM-TO * +KI+OU * \n"
+                               "P9 *  * -RY *  * -KI * +KE * \n"
+                               "P-00FU00FU00FU00FU00KY00KE00KE\n"
+                               "-\n");
+    bool kachi = win_if_declare(state);
+    TEST_CHECK(kachi);
+  }
+  {
+    auto state=csa::read_board("P1 *  * +RY *  * +KI * -KE * \n"
+                               "P2+OU+TO+UM+UM+TO * -KI-OU * \n"
+                               "P3-FU+FU+FU+FU * -GI-GI *  * \n"
+                               "P4 *  *  *  * -FU-FU-FU-FU * \n"
+                               "P5 *  * -RY-NY-GI *  *  *  * \n"
+                               "P6 *  *  *  *  * +FU+FU+FU * \n"
+                               "P7 *  *  *  *  * +KI+KE * -NY\n"
+                               "P8 *  *  *  *  * +KI+GI *  * \n"
+                               "P9 *  *  *  * -NY *  *  *  * \n"
+                               "P+00FU00FU00FU00FU00KY00KE00KE\n"
+                               "P-00FU\n"
+                               "+\n");
+    bool kachi = win_if_declare(state);
+    TEST_CHECK(!kachi);
+    // TEST_CHECK(drops == 1);
+  }
+  {
+    auto state=csa::read_board("P1 *  *  *  * +NY *  *  *  * \n"
+                               "P2 *  *  *  *  * -KI-GI *  * \n"
+                               "P3 *  *  *  *  * -KI-KE * +NY\n"
+                               "P4 *  *  *  *  * -FU-FU-FU * \n"
+                               "P5 *  * +RY+NY+GI *  *  *  * \n"
+                               "P6 *  *  *  * +FU+FU+FU+FU * \n"
+                               "P7+FU-FU-FU-FU * +GI+GI *  * \n"
+                               "P8-OU-TO-UM-UM-TO * +KI+OU * \n"
+                               "P9 *  * -RY *  * -KI * +KE * \n"
+                               "P+00FU\n"
+                               "P-00FU00FU00FU00FU00KY00KE00KE\n"
+                               "-\n");
+    bool kachi = win_if_declare(state);
+    TEST_CHECK(!kachi);
+    // TEST_CHECK(drops == 1);
+  }
+  {
+    auto state=csa::read_board("P1 *  * +RY *  * +KI * -KE * \n"
+                               "P2+OU+TO+UM+TO+TO * -KI-OU * \n"
+                               "P3-FU+FU+FU+FU+FU-GI-GI *  * \n"
+                               "P4 *  *  *  * -FU-FU-FU-FU * \n"
+                               "P5 *  * -RY-NY-GI *  *  *  * \n"
+                               "P6 *  *  *  *  * +FU+FU+FU * \n"
+                               "P7+UM *  *  *  * +KI+KE * -NY\n"
+                               "P8 *  *  *  *  * +KI+GI *  * \n"
+                               "P9 *  *  *  * -NY *  *  *  * \n"
+                               "P+00FU00FU00FU00KY00KE00KE\n"
+                               "+\n");
+    bool kachi = win_if_declare(state);
+    TEST_CHECK(!kachi);
+    // TEST_CHECK(drops == 41);
+  }
+  {
+    auto state=csa::read_board("P1 *  *  *  * +NY *  *  *  * \n"
+                               "P2 *  *  *  *  * -KI-GI *  * \n"
+                               "P3-UM *  *  *  * -KI-KE * +NY\n"
+                               "P4 *  *  *  *  * -FU-FU-FU * \n"
+                               "P5 *  * +RY+NY+GI *  *  *  * \n"
+                               "P6 *  *  *  * +FU+FU+FU+FU * \n"
+                               "P7+FU-FU-FU-FU-FU+GI+GI *  * \n"
+                               "P8-OU-TO-UM-TO-TO * +KI+OU * \n"
+                               "P9 *  * -RY *  * -KI * +KE * \n"
+                               "P-00FU00FU00FU00KY00KE00KE\n"
+                               "-\n");
+    bool kachi = win_if_declare(state);
+    TEST_CHECK(!kachi);
+    // TEST_CHECK(drops == 41);
+  }
+}
 
+void test_compress_record()
+{
+  std::string sfen = "startpos moves 2g2f 8c8d 2f2e 8d8e 9g9f 4a3b 3i3h 7a7b 6i7h 5a5b 4g4f 9c9d 3h4g 7c7d 1g1f 7d7e 2e2d 2c2d 2h2d 8e8f 8g8f P*2c 2d7d 8b8f 5i5h 7b7c 7d7e 2c2d P*8g 8f8b 7e3e 3b2c 3e3f 2d2e 7g7f 5b4b 1f1e 3c3d 4i3h 7c6d 8h2b+ 3a2b 4f4e 2b3c 4g5f 8a7c 6g6f P*8f 8g8f 8b8f P*8g 8f8a 3f4f 6a6b 7i6h 5c5d 6h6g 4b3b 3g3f 5d5e 5f4g 6d5c 2i3g 6c6d 7f7e 8a8d 5h4h B*2d 3f3e 2d3e 4f3f P*8h 7h8h 1c1d 1e1d 1a1d 1i1d 2c1d P*2b 3c2b 4e4d 4c4d 8h7h 6d6e P*1b 1d2d L*7d P*7b 1b1a+ 2b1a 8i7g 4d4e 7d7c+ 7b7c 7g6e L*4f 6e5c 4f4g 4h5h 3e1g+ 3g4e 2d3e P*4d 8d4d P*3c 2a3c B*2a 3b2a 4e3c+ S*3b S*2d 4g4h+ 5h6h 4h5h 6g5h P*6g 7h6g B*1e 2d1e 3b3c 3f3g 1g1f L*1g N*4f 1g1f 4f5h+ 6h5h 6b5c B*6b 4d4c N*2d S*2c P*4d 5c4d B*5b 1a2b 5b4c+ 4d4c R*4a B*3a 4a4c+ 3c2d 1e2d N*4f 5h4g 3e3f 3g3f N*3e 2d3e L*1d S*3b 2a1a G*2a 1a1b 4c2c 2b2c N*2d 1b1c 3b2c+ 1c2c 3e3d 2c2d G*2c";
+  auto record = usi::read_record(sfen);
+  // record.moves.resize(2);
+  std::vector<uint64_t> code_seq;
+  int count = bitpack::append_binary_record(record, code_seq);
+  TEST_ASSERT(count > 0);
+  MiniRecord r2;
+  const uint64_t *ptr = &*code_seq.begin();
+  int read_count = bitpack::read_binary_record(ptr, r2);
+  TEST_ASSERT(count == read_count);
+  TEST_ASSERT(record == r2);
+}
 
 TEST_LIST = {
   { "player", test_player },
   { "ptype", test_ptype },
   { "direction", test_direction },
   { "square", test_square },
   { "piece_stand", test_piece_stand },
   { "move", test_move },
+  { "csa", test_csa },
   { "offset", test_offset },
   { "king8", test_king8 },
   { "state", test_state },
   { "effect_state", test_effect_state },
   { "effect_state2", test_effect_state2 },
   { "usi", test_usi },
   { "ki2", test_ki2 },
   { "classifier", test_classify },
   { "checkmate", test_checkmate },
   { "addeffect", test_addeffect },
   { "movegen", test_movegen },
+  { "combination_id", test_combination_id },
+  { "pack_position", test_pack_position },
+  { "win_if_declare", test_win_if_declare },
+  { "compress_record", test_compress_record },
   { nullptr, nullptr }
 };
```

### Comparing `miniosl-0.0.2/minioslcc/test/minitest_file.cc` & `miniosl-0.0.3a1/minioslcc/test/minitest_file.cc`

 * *Files 3% similar despite different names*

```diff
@@ -413,17 +413,47 @@
       }
       // TEST_CHECK(state.isConsistent());
       state.makeMove(move);
     }
   }
 }
 
+void test_pack_position()
+{
+  auto csa = make_path();
+  int count = 0;
+  
+  for (auto& file: std::filesystem::directory_iterator{csa}) {
+    if (! file.is_regular_file() || file.path().extension() != ".csa")
+      continue;
+    if (++count > limit/2)
+      break;
+
+    auto record=csa::read_record(file);
+    auto state(record.initial_state);
+    PackedState ps2;
+    int cnt = 0;
+    for (auto move:record.moves) {      
+      PackedState ps{state, move, record.result};
+      auto bs = ps.to_bitset();
+      ps2.restore(bs);
+      
+      TEST_ASSERT(to_usi(ps.state) == to_usi(ps2.state));
+      TEST_ASSERT(move == ps2.next);
+      TEST_MSG("%s v.s. %s", to_usi(move).c_str(), to_usi(ps2.next).c_str());
+      TEST_ASSERT(ps2.result == record.result);
+      state.makeMove(move);
+    }
+  }
+}
+
 
 TEST_LIST = {
   { "path", test_path },
   { "check", test_check },
   { "capture", test_capture },
   { "copy", test_copy },
   { "piece_stand", test_piece_stand },
   { "changed_effect", test_changed_effect },
+  { "pack_position", test_pack_position },
   { nullptr, nullptr }
 };
```

### Comparing `miniosl-0.0.2/minioslcc/util/csa-to-sfen.cc` & `miniosl-0.0.3a1/minioslcc/util/csa-to-sfen.cc`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,27 @@
   if (argc > 1) {
     std::cout << "search csa files in the current directory and write to sfen.txt\n";
     return std::string(argv[1]) == "--help" ? 0 : 1;
   }
   
   auto csa_folder = std::filesystem::path(".");
   std::ofstream os("sfen.txt");
-  int count=0;
+  int count=0, zero_skip_count=0;
   for (auto& file: std::filesystem::directory_iterator{csa_folder}) {
     if (! file.is_regular_file() || file.path().extension() != ".csa")
       continue;
     try {
       auto record=osl::csa::read_record(file);
+      if (record.moves.empty()) {
+        ++zero_skip_count;
+        continue;
+      }
       os << to_usi(record) << '\n';
       ++count;
     }
     catch (std::exception& e) {
       std::cerr << "skip " << file << '\n' << e.what() << '\n';
     }
   }
-  std::cout << "wrote " << count << " files\n";
+  std::cout << "wrote " << count << " records\n";
+  std::cerr << "skip " << zero_skip_count << " records with zero moves" << '\n';  
 }
```

### Comparing `miniosl-0.0.2/minioslcc/util/validate-sfen.cc` & `miniosl-0.0.3a1/minioslcc/util/validate-sfen.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+// validate-sfen.cc
 #include "record.h"
 #include <filesystem>
 #include <fstream>
 #include <iostream>
 #include <stdexcept>
 #include <ranges>
 
@@ -27,14 +28,15 @@
 }
 
 void check_consistency(const osl::MiniRecord& record) {
   auto state = record.initial_state;
   bool made_check = false, made_checkmate = false;
   osl::MoveVector all, check;
   int cnt = 0;
+  osl::PackedState ps2;
   for (auto move: record.moves) {
     if (made_checkmate)
       throw std::logic_error("checkmate inconsistent");
     if (state.inCheck(alt(state.turn())))
       throw std::runtime_error("check escape fail");
     if (state.inCheck() != made_check)
       throw std::logic_error("check inconsistent");
@@ -50,18 +52,26 @@
       if (std::ranges::find(check, move) == check.end()) {
         if (! move.ignoreUnpromote())
           throw std::runtime_error("movegen check "+to_usi(move)+" "+std::to_string(cnt));
         //std::cerr << "ignore unpromote in check\n";
       }
     }
     test_checkmate1ply(state);
+
+    osl::PackedState ps{state, move};
+    auto bs = ps.to_bitset();
+    ps2.restore(bs);
+      
+    if (ps.state != ps2.state || move != ps2.next)
+      throw std::runtime_error("pack position consistency"+to_usi(state)+" "+to_usi(move)+" "+to_usi(ps2.next)
+                               +" "+std::to_string(cnt));
     
     state.makeMove(move);
     if (!state.isConsistent())
-      throw std::runtime_error("internal consistency"+to_usi(move)+" "+std::to_string(cnt));
+      throw std::runtime_error("internal consistency "+to_usi(move)+" "+std::to_string(cnt));
     made_checkmate = state.inCheckmate();
     
     ++cnt;
   }
 }
 
 int main(int argc, char *argv[]) {
```

### Comparing `miniosl-0.0.2/setup.py` & `miniosl-0.0.3a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,31 +164,34 @@
         )
         subprocess.run(
             ["cmake", "--build", ".", *build_args], cwd=build_temp, check=True
         )
 
 
 # follow https://packaging.python.org/en/latest/guides/making-a-pypi-friendly-readme/        
-this_directory = Path(__file__).parent        
+this_directory = Path(__file__).parent
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="miniosl",
-    version="0.0.2",
+    version="0.0.3a1",
     author="Tomoyuki Kaneko",
     author_email="kaneko@graco.c.u-tokyo.ac.jp",
     description="A python interface to miniosl (shogi library)",
-    long_description = (this_directory / "README.md").read_text(),
+    long_description=(this_directory / "README.md").read_text(),
     long_description_content_type='text/markdown',
     packages=[
         'miniosl',
         'minioslcc',
     ],
     ext_modules=[CMakeExtension(
         name="minioslcc",
         sourcedir="minioslcc"
     )],
+    project_urls={
+        'Source': 'https://github.com/tkaneko/miniosl',
+    },
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     python_requires=">=3.10",
 )
```

### Comparing `miniosl-0.0.2/tests/test_state.py` & `miniosl-0.0.3a1/tests/test_state.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,138 @@
 import miniosl
 import minioslcc
+import numpy as np
+import pytest
+
 
 def test_state():
     board = miniosl.State()
     svg = board.to_svg()
+    assert svg
+    png = board.to_png()
+    assert png
     b2 = miniosl.State('sfen lnsgkgsnl/1r5b1/pppppp1pp/6p2/9/P8/1PPPPPPPP/1B5R1/LNSGKGSNL b - 1')
+    assert b2
 
 
 def test_make_move():
     board = miniosl.State()
     board.make_move('7g7f')
-    assert board.last_to().to_xy() == (7,6)
+    assert board.last_to().to_xy() == (7, 6)
     svg = board.to_svg()
     board.make_move('-3334FU')
-    assert board.last_to().to_xy() == (3,4)
+    assert board.last_to().to_xy() == (3, 4)
     svg = board.to_svg()
     svg = board.to_svg(decorate=True)
+    assert svg
 
 
 def test_genmove():
     board = miniosl.State()
     moves = board.genmove()
-    assert '7g7f' in [ m.to_usi() for m in moves]
-    assert '+7776FU' in [ m.to_csa() for m in moves]
+    assert '7g7f' in [m.to_usi() for m in moves]
+    assert '+7776FU' in [m.to_csa() for m in moves]
     assert len(moves) == 30
     copy = board.clone()
     board.make_move('+7776FU')
     moves = board.genmove()
-    assert '+7776FU' not in [ m.to_csa() for m in moves]
+    assert '+7776FU' not in [m.to_csa() for m in moves]
     moves = copy.genmove()
-    assert '+7776FU' in [ m.to_csa() for m in moves]
+    assert '+7776FU' in [m.to_csa() for m in moves]
     board.unmake_move()
     moves = board.genmove()
-    assert '7g7f' in [ m.to_usi() for m in moves]
-    
-    
-    
-def test_initial_csa():
+    assert '7g7f' in [m.to_usi() for m in moves]
+
+
+def test_to_np():
+    board = miniosl.State()
+    feature = board.to_np()
+    assert isinstance(feature, np.ndarray)
+    assert feature.shape == (9, 9)
+
+
+def test_to_np_hand():
+    board = miniosl.State()
+    feature = board.to_np_hand()
+    assert isinstance(feature, np.ndarray)
+    assert feature.shape == (2, 7)
+
+
+def test_to_np_cover():
+    board = miniosl.State()
+    feature = board.to_np_cover()
+    assert isinstance(feature, np.ndarray)
+    assert feature.shape == (2, 9, 9)
+
+
+def test_np_pack():
+    board = miniosl.State()
+    binary = board.to_np_pack()
+    assert isinstance(binary, np.ndarray)
+    assert binary.shape == (4,)
+    assert binary.dtype == np.uint64
+
+
+def test_board_csa():
     board = minioslcc.CCState()
     csa = board.to_csa()
-    for r,line in enumerate(csa.split('\n')):
+    for r, line in enumerate(csa.split('\n')):
         if r < 9:
             assert len(line) == 2+3*9
             assert line[0:2] == 'P'+str(r+1)
         else:
             assert line == '+' or line == '-' or len(line) < 1
 
 
 def test_replay():
     board = miniosl.State()
     board.make_move('+7776FU')
     board.make_move('-3334FU')
 
+
 def test_bitset():
     mobility = miniosl.ptype_move_direction[miniosl.knight]
     one_hot = 2**int(miniosl.UUR)
     assert (mobility & one_hot) != 0
+
+
+def test_encode_move():
+    board = miniosl.State()
+    board.make_move('+7776FU')
+    board.make_move('-3334FU')
+    board.make_move('+8822UM')
+    board.make_move('-3122GI')
+    moves = board.genmove()
+    for move in moves:
+        print(move)
+        code = board.encode_move(move)
+        print(code)
+        assert 0 < code < 2**12
+
+
+def test_illegal_move():
+    board = miniosl.State()
+    move = board.to_move('+7775FU')
+    assert not move.is_normal()
+
+    move = board.to_move('7g7f')
+    assert move.is_normal()
+
+    move = board.to_move('7g7c')
+    assert not move.is_normal()
+
+
+def test_illegal_make_move():
+    board = miniosl.State()
+    move = board.to_move('+7776FU')
+    assert move.is_normal()
+    board.make_move(move)
+
+    # turn mismatch
+    with pytest.raises(ValueError):
+        board.make_move(move)
+
+    board.make_move('-3334FU')
+
+    # piece mismatch
+    with pytest.raises(ValueError):
+        board.make_move(move)
```

