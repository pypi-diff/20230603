# Comparing `tmp/pyresidfp-0.6.7.tar.gz` & `tmp/pyresidfp-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresidfp-0.6.7.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pyresidfp-0.7.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pyresidfp-0.6.7.tar` & `pyresidfp-0.7.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
--rw-r--r--   0        0        0     3943 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/CMakeLists.txt
--rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/COPYING
--rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/README.md
--rw-r--r--   0        0        0     2365 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     4256 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/PythonSid.cpp
--rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/PythonSid.h
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/config.h.in
--rw-r--r--   0        0        0     1436 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp/__init__.py
--rw-r--r--   0        0        0     8720 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp/_pyresidfp/__init__.pyi
--rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp/_version.py
--rw-r--r--   0        0        0     4092 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp/musical_scale.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp/py.typed
--rw-r--r--   0        0        0     2863 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp/registers.py
--rw-r--r--   0        0        0    11360 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp/sound_interface_device.py
--rw-r--r--   0        0        0     9187 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/pyresidfp.cpp
--rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/AUTHORS
--rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/COPYING
--rw-r--r--   0        0        0     3317 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Dac.cpp
--rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Dac.h
--rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/EnvelopeGenerator.cpp
--rw-r--r--   0        0        0    10947 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/EnvelopeGenerator.h
--rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/ExternalFilter.cpp
--rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/ExternalFilter.h
--rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Filter.cpp
--rw-r--r--   0        0        0     3861 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Filter.h
--rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Filter6581.cpp
--rw-r--r--   0        0        0    15048 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Filter6581.h
--rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Filter8580.cpp
--rw-r--r--   0        0        0    13323 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Filter8580.h
--rw-r--r--   0        0        0     2343 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/FilterModelConfig.cpp
--rw-r--r--   0        0        0     5094 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/FilterModelConfig.h
--rw-r--r--   0        0        0     8172 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/FilterModelConfig6581.cpp
--rw-r--r--   0        0        0     3023 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/FilterModelConfig6581.h
--rw-r--r--   0        0        0     6999 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/FilterModelConfig8580.cpp
--rw-r--r--   0        0        0     1830 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/FilterModelConfig8580.h
--rw-r--r--   0        0        0      965 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Integrator6581.cpp
--rw-r--r--   0        0        0     9200 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Integrator6581.h
--rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Integrator8580.cpp
--rw-r--r--   0        0        0     3550 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Integrator8580.h
--rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/OpAmp.cpp
--rw-r--r--   0        0        0     2977 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/OpAmp.h
--rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Potentiometer.h
--rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/README
--rw-r--r--   0        0        0    13759 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/SID.cpp
--rw-r--r--   0        0        0     9686 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/SID.h
--rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Spline.cpp
--rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Spline.h
--rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/Voice.h
--rw-r--r--   0        0        0     6862 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/WaveformCalculator.cpp
--rw-r--r--   0        0        0     4123 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/WaveformCalculator.h
--rw-r--r--   0        0        0    12362 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/WaveformGenerator.cpp
--rw-r--r--   0        0        0    11756 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/WaveformGenerator.h
--rw-r--r--   0        0        0     1829 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/array.h
--rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/resample/Resampler.h
--rw-r--r--   0        0        0    11494 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/resample/SincResampler.cpp
--rw-r--r--   0        0        0     3779 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/resample/SincResampler.h
--rw-r--r--   0        0        0     2688 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/resample/TwoPassSincResampler.h
--rw-r--r--   0        0        0     2161 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/resample/ZeroOrderResampler.h
--rw-r--r--   0        0        0     1910 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/siddefs-fp.h.in
--rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/residfp/version.cc
--rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/sidcxx11.h
--rw-r--r--   0        0        0     1138 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/src/sidcxx14.h
--rw-r--r--   0        0        0     1201 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/tests/test_basic.py
--rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/tests/test_versions.py
--rw-r--r--   0        0        0     3121 2022-11-09 12:37:21.000000 pyresidfp-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0     4158 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/CMakeLists.txt
+-rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/COPYING
+-rw-r--r--   0        0        0     2045 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/README.md
+-rw-r--r--   0        0        0     2365 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4256 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/PythonSid.cpp
+-rw-r--r--   0        0        0     2305 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/PythonSid.h
+-rw-r--r--   0        0        0      517 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/config.h.in
+-rw-r--r--   0        0        0     1436 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/pyresidfp/__init__.py
+-rw-r--r--   0        0        0     8720 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/pyresidfp/_pyresidfp/__init__.pyi
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/pyresidfp/_version.py
+-rw-r--r--   0        0        0     4092 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/pyresidfp/musical_scale.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/pyresidfp/py.typed
+-rw-r--r--   0        0        0     2863 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/pyresidfp/registers.py
+-rw-r--r--   0        0        0    11360 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/pyresidfp/sound_interface_device.py
+-rw-r--r--   0        0        0     9187 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/pyresidfp.cpp
+-rw-r--r--   0        0        0      251 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/AUTHORS
+-rw-r--r--   0        0        0    18092 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/COPYING
+-rw-r--r--   0        0        0     3317 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Dac.cpp
+-rw-r--r--   0        0        0     3264 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Dac.h
+-rw-r--r--   0        0        0     4050 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/EnvelopeGenerator.cpp
+-rw-r--r--   0        0        0    10947 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/EnvelopeGenerator.h
+-rw-r--r--   0        0        0     2013 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/ExternalFilter.cpp
+-rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/ExternalFilter.h
+-rw-r--r--   0        0        0     2113 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Filter.cpp
+-rw-r--r--   0        0        0     3861 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Filter.h
+-rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Filter6581.cpp
+-rw-r--r--   0        0        0    15048 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Filter6581.h
+-rw-r--r--   0        0        0     2265 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Filter8580.cpp
+-rw-r--r--   0        0        0    13323 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Filter8580.h
+-rw-r--r--   0        0        0     2474 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/FilterModelConfig.cpp
+-rw-r--r--   0        0        0     5021 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/FilterModelConfig.h
+-rw-r--r--   0        0        0    10415 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/FilterModelConfig6581.cpp
+-rw-r--r--   0        0        0     3023 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/FilterModelConfig6581.h
+-rw-r--r--   0        0        0     8941 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/FilterModelConfig8580.cpp
+-rw-r--r--   0        0        0     1830 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/FilterModelConfig8580.h
+-rw-r--r--   0        0        0      965 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Integrator6581.cpp
+-rw-r--r--   0        0        0     9205 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Integrator6581.h
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Integrator8580.cpp
+-rw-r--r--   0        0        0     3530 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Integrator8580.h
+-rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/OpAmp.cpp
+-rw-r--r--   0        0        0     3097 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/OpAmp.h
+-rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Potentiometer.h
+-rw-r--r--   0        0        0     1024 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/README
+-rw-r--r--   0        0        0    13918 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/SID.cpp
+-rw-r--r--   0        0        0     9686 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/SID.h
+-rw-r--r--   0        0        0     3350 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Spline.cpp
+-rw-r--r--   0        0        0     1901 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Spline.h
+-rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/Voice.h
+-rw-r--r--   0        0        0     5924 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/WaveformCalculator.cpp
+-rw-r--r--   0        0        0     4297 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/WaveformCalculator.h
+-rw-r--r--   0        0        0    12119 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/WaveformGenerator.cpp
+-rw-r--r--   0        0        0    12098 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/WaveformGenerator.h
+-rw-r--r--   0        0        0     2001 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/array.h
+-rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/resample/Resampler.h
+-rw-r--r--   0        0        0    11494 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/resample/SincResampler.cpp
+-rw-r--r--   0        0        0     3779 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/resample/SincResampler.h
+-rw-r--r--   0        0        0     2688 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/resample/TwoPassSincResampler.h
+-rw-r--r--   0        0        0     2161 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/resample/ZeroOrderResampler.h
+-rw-r--r--   0        0        0     1910 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/siddefs-fp.h.in
+-rw-r--r--   0        0        0     1054 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/residfp/version.cc
+-rw-r--r--   0        0        0     1469 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/src/sidcxx11.h
+-rw-r--r--   0        0        0     1201 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/tests/test_basic.py
+-rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/tests/test_versions.py
+-rw-r--r--   0        0        0     3121 2022-11-09 12:37:21.000000 pyresidfp-0.7.0/PKG-INFO
```

### Comparing `pyresidfp-0.6.7/CMakeLists.txt` & `pyresidfp-0.7.0/CMakeLists.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 string(REGEX REPLACE "^([0-9]+\.[0-9]+(\.[0-9]+)?)(\.[^.]*)*$" "\\1" TRUNCATED_PROJECT_VERSION ${SKBUILD_PROJECT_VERSION})
 
 project(${SKBUILD_PROJECT_NAME} VERSION ${TRUNCATED_PROJECT_VERSION} LANGUAGES CXX)
 
 set(PYBIND11_NEWPYTHON ON)
 find_package(pybind11 CONFIG REQUIRED)
+find_package(OpenMP)
 
 include(CheckCXXSourceCompiles)
 include(CheckIncludeFileCXX)
 include(CheckIPOSupported)
 
 enable_testing()
 
@@ -31,25 +32,26 @@
 
 check_cxx_source_compiles("
 int main(void) { if (__builtin_expect(0, 0)) return 1; return 0; }
 " HAVE_BUILTIN_EXPECT)
 
 check_ipo_supported(RESULT IPO_SUPPORTED OUTPUT IPO_ERROR)
 
-set(CMAKE_CXX_STANDARD 14)
+set(CMAKE_CXX_STANDARD 17)
 set(CMAKE_CXX_EXTENSIONS OFF)
 set(PACKAGE_VERSION ${PROJECT_VERSION})
 option(ENABLE_INLINING "Enable inlining" ON)
 if(ENABLE_INLINING)
   set(RESID_INLINE inline)
   set(RESID_INLINING 1)
 endif()
 set(RESID_BRANCH_HINTS 1)
 set(HAVE_CXX11 $<COMPILE_FEATURES:cxx_std_11>)
 set(HAVE_CXX14 $<COMPILE_FEATURES:cxx_std_14>)
+set(HAVE_CXX17 $<COMPILE_FEATURES:cxx_std_17>)
 
 configure_file(src/residfp/siddefs-fp.h.in siddefs-fp.h)
 configure_file(src/config.h.in config.h)
 
 set(HEADER_FILES
         ${CMAKE_CURRENT_BINARY_DIR}/siddefs-fp.h
         ${CMAKE_CURRENT_BINARY_DIR}/config.h
@@ -73,15 +75,14 @@
         src/residfp/Potentiometer.h
         src/residfp/SID.h
         src/residfp/Spline.h
         src/residfp/Voice.h
         src/residfp/WaveformCalculator.h
         src/residfp/WaveformGenerator.h
         src/sidcxx11.h
-        src/sidcxx14.h
         src/PythonSid.h)
 set(SOURCE_FILES
         src/residfp/resample/SincResampler.cpp
         src/residfp/Dac.cpp
         src/residfp/EnvelopeGenerator.cpp
         src/residfp/ExternalFilter.cpp
         src/residfp/Filter.cpp
@@ -104,15 +105,23 @@
 pybind11_add_module(_pyresidfp MODULE
         ${HEADER_FILES} ${SOURCE_FILES})
 target_include_directories(_pyresidfp
         PRIVATE ${CMAKE_CURRENT_BINARY_DIR} ${CMAKE_CURRENT_SOURCE_DIR}
         src/residfp src/residfp/resample)
 target_compile_definitions(_pyresidfp PRIVATE HAVE_CONFIG_H)
 target_compile_definitions(_pyresidfp PRIVATE PROJECT_VERSION="${SKBUILD_PROJECT_VERSION}")
-set_property(TARGET _pyresidfp PROPERTY CXX_STANDARD 14)
+set_property(TARGET _pyresidfp PROPERTY CXX_STANDARD 17)
+
+if(OpenMP_CXX_FOUND)
+  message(STATUS "OpenMP found")
+  target_link_libraries(_pyresidfp PUBLIC OpenMP::OpenMP_CXX)
+else()
+  message(STATUS "OpenMP not found")
+endif()
+
 
 if (IPO_SUPPORTED)
   message(STATUS "IPO / LTO enabled")
   set_property(TARGET _pyresidfp PROPERTY INTERPROCEDURAL_OPTIMIZATION TRUE)
 else()
   message(STATUS "IPO / LTO not supported: <${IPO_ERROR}>")
 endif()
```

### Comparing `pyresidfp-0.6.7/COPYING` & `pyresidfp-0.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/README.md` & `pyresidfp-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/pyproject.toml` & `pyresidfp-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/PythonSid.cpp` & `pyresidfp-0.7.0/src/PythonSid.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/PythonSid.h` & `pyresidfp-0.7.0/src/PythonSid.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/pyresidfp/__init__.py` & `pyresidfp-0.7.0/src/pyresidfp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/pyresidfp/_pyresidfp/__init__.pyi` & `pyresidfp-0.7.0/src/pyresidfp/_pyresidfp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/pyresidfp/musical_scale.py` & `pyresidfp-0.7.0/src/pyresidfp/musical_scale.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/pyresidfp/registers.py` & `pyresidfp-0.7.0/src/pyresidfp/registers.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/pyresidfp/sound_interface_device.py` & `pyresidfp-0.7.0/src/pyresidfp/sound_interface_device.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/pyresidfp.cpp` & `pyresidfp-0.7.0/src/pyresidfp.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/COPYING` & `pyresidfp-0.7.0/src/residfp/COPYING`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/Dac.cpp` & `pyresidfp-0.7.0/src/residfp/Dac.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/Dac.h` & `pyresidfp-0.7.0/src/residfp/Dac.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/EnvelopeGenerator.cpp` & `pyresidfp-0.7.0/src/residfp/EnvelopeGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/EnvelopeGenerator.h` & `pyresidfp-0.7.0/src/residfp/EnvelopeGenerator.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/ExternalFilter.cpp` & `pyresidfp-0.7.0/src/residfp/ExternalFilter.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/ExternalFilter.h` & `pyresidfp-0.7.0/src/residfp/ExternalFilter.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/Filter.cpp` & `pyresidfp-0.7.0/src/residfp/Filter.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/Filter.h` & `pyresidfp-0.7.0/src/residfp/Filter.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/Filter6581.cpp` & `pyresidfp-0.7.0/src/residfp/Filter6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/Filter6581.h` & `pyresidfp-0.7.0/src/residfp/Filter6581.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/Filter8580.cpp` & `pyresidfp-0.7.0/src/residfp/Filter8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/Filter8580.h` & `pyresidfp-0.7.0/src/residfp/Filter8580.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/FilterModelConfig.cpp` & `pyresidfp-0.7.0/src/residfp/FilterModelConfig.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -54,26 +54,29 @@
 {
     // Convert op-amp voltage transfer to 16 bit values.
 
     std::vector<Spline::Point> scaled_voltage(opamp_size);
 
     for (int i = 0; i < opamp_size; i++)
     {
-        scaled_voltage[i].x = N16 * (opamp_voltage[i].x - opamp_voltage[i].y + denorm) / 2.;
+        scaled_voltage[i].x = N16 * (opamp_voltage[i].x - opamp_voltage[i].y) / 2.;
+        // We add 32768 to get a positive number in the range [0-65535]
+        scaled_voltage[i].x += static_cast<double>(1u << 15);
+
         scaled_voltage[i].y = N16 * (opamp_voltage[i].x - vmin);
     }
 
     // Create lookup table mapping capacitor voltage to op-amp input voltage:
 
     Spline s(scaled_voltage);
 
     for (int x = 0; x < (1 << 16); x++)
     {
         const Spline::Point out = s.evaluate(x);
-        // If Vmax > max opamp_voltage the first elements may be negative
+        // When interpolating outside range the first elements may be negative
         double tmp = out.x > 0. ? out.x : 0.;
         assert(tmp < 65535.5);
         opamp_rev[x] = static_cast<unsigned short>(tmp + 0.5);
     }
 }
 
 } // namespace reSIDfp
```

### Comparing `pyresidfp-0.6.7/src/residfp/FilterModelConfig.h` & `pyresidfp-0.7.0/src/residfp/FilterModelConfig.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * This file is part of libsidplayfp, a SID player engine.
  *
- * Copyright 2011-2022 Leandro Nini <drfiemost@users.sourceforge.net>
+ * Copyright 2011-2023 Leandro Nini <drfiemost@users.sourceforge.net>
  * Copyright 2007-2010 Antti Lankila
  * Copyright 2004,2010 Dag Lem
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 2 of the License, or
  * (at your option) any later version.
@@ -133,15 +133,14 @@
      * The "zero" output level of the voices.
      */
     int getNormalizedVoiceDC() const { return static_cast<int>(N16 * (voice_DC_voltage - vmin)); }
 
     inline unsigned short getOpampRev(int i) const { return opamp_rev[i]; }
     inline double getVddt() const { return Vddt; }
     inline double getVth() const { return Vth; }
-    inline double getVoiceDCVoltage() const { return voice_DC_voltage; }
 
     // helper functions
     inline unsigned short getNormalizedValue(double value) const
     {
         const double tmp = N16 * (value - vmin);
         assert(tmp > -0.5 && tmp < 65535.5);
         return static_cast<unsigned short>(tmp + 0.5);
```

### Comparing `pyresidfp-0.6.7/src/residfp/FilterModelConfig6581.h` & `pyresidfp-0.7.0/src/residfp/FilterModelConfig6581.h`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 #include "FilterModelConfig.h"
 
 #include <memory>
 
 #include "Dac.h"
 
-#include "src/sidcxx14.h"
+#include "src/sidcxx11.h"
 
 namespace reSIDfp
 {
 
 class Integrator6581;
 
 /**
```

### Comparing `pyresidfp-0.6.7/src/residfp/FilterModelConfig8580.h` & `pyresidfp-0.7.0/src/residfp/FilterModelConfig8580.h`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #ifndef FILTERMODELCONFIG8580_H
 #define FILTERMODELCONFIG8580_H
 
 #include "FilterModelConfig.h"
 
 #include <memory>
 
-#include "src/sidcxx14.h"
+#include "src/sidcxx11.h"
 
 namespace reSIDfp
 {
 
 class Integrator8580;
 
 /**
```

### Comparing `pyresidfp-0.6.7/src/residfp/Integrator6581.cpp` & `pyresidfp-0.7.0/src/residfp/Integrator6581.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/Integrator6581.h` & `pyresidfp-0.7.0/src/residfp/Integrator6581.h`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
  *
  *     Ids = I0*W/L*e^(Vgst/(Ut/k))   , Vgst < 0               (subthreshold mode)
  *
  * where
  *     I0 = (2 * uCox * Ut^2) / k
  *
  * The remaining problem with the textbook model is that the transition
- * from subthreshold the triode/saturation is not continuous.
+ * from subthreshold to triode/saturation is not continuous.
  *
  * Realizing that the subthreshold and triode/saturation modes may both
  * be defined by independent (and equal) terms of Vgs and Vds,
  * respectively, the corresponding terms can be blended into (equal)
  * continuous functions suitable for table lookup.
  *
  * The EKV model (Enz, Krummenacher and Vittoz) essentially performs this
@@ -232,23 +232,23 @@
     const int n_I_snake = nSnake * (static_cast<int>(Vgst_2 - Vgdt_2) >> 15);
 
     // VCR gate voltage.       // Scaled by m*2^16
     // Vg = Vddt - sqrt(((Vddt - Vw)^2 + Vgdt^2)/2)
     const int nVg = static_cast<int>(fmc->getVcr_nVg((nVddt_Vw_2 + (Vgdt_2 >> 1)) >> 16));
 #ifdef SLOPE_FACTOR
     const double nVp = static_cast<double>(nVg - nVt) / n; // Pinch-off voltage
-    const int kVg = static_cast<int>(nVp + 0.5) - nVmin;
+    const int kVgt = static_cast<int>(nVp + 0.5) - nVmin;
 #else
-    const int kVg = (nVg - nVt) - nVmin;
+    const int kVgt = (nVg - nVt) - nVmin;
 #endif
 
     // VCR voltages for EKV model table lookup.
-    const int kVgt_Vs = (vx < kVg) ? kVg - vx : 0;
+    const int kVgt_Vs = (vx < kVgt) ? kVgt - vx : 0;
     assert(kVgt_Vs < (1 << 16));
-    const int kVgt_Vd = (vi < kVg) ? kVg - vi : 0;
+    const int kVgt_Vd = (vi < kVgt) ? kVgt - vi : 0;
     assert(kVgt_Vd < (1 << 16));
 
     // VCR current, scaled by m*2^15*2^15 = m*2^30
     const unsigned int If = static_cast<unsigned int>(fmc->getVcr_n_Ids_term(kVgt_Vs)) << 15;
     const unsigned int Ir = static_cast<unsigned int>(fmc->getVcr_n_Ids_term(kVgt_Vd)) << 15;
 #ifdef SLOPE_FACTOR
     const double iVcr = static_cast<double>(If - Ir);
```

### Comparing `pyresidfp-0.6.7/src/residfp/Integrator8580.cpp` & `pyresidfp-0.7.0/src/residfp/Integrator8580.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/Integrator8580.h` & `pyresidfp-0.7.0/src/residfp/Integrator8580.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * This file is part of libsidplayfp, a SID player engine.
  *
- * Copyright 2011-2022 Leandro Nini <drfiemost@users.sourceforge.net>
+ * Copyright 2011-2023 Leandro Nini <drfiemost@users.sourceforge.net>
  * Copyright 2007-2010 Antti Lankila
  * Copyright 2004, 2010 Dag Lem <resid@nimrod.no>
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 2 of the License, or
  * (at your option) any later version.
@@ -85,15 +85,15 @@
      * Set FC gate voltage multiplier.
      */
     void setV(double v)
     {
         // Gate voltage is controlled by the switched capacitor voltage divider
         // Ua = Ue * v = 4.76v  1<v<2
         assert(v > 1.0 && v < 2.0);
-        const double Vg = fmc->getVoiceDCVoltage() * v;
+        const double Vg = 4.76 * v;
         const double Vgt = Vg - fmc->getVth();
 
         // Vg - Vth, normalized so that translated values can be subtracted:
         // Vgt - x = (Vgt - t) - (x - t)
         nVgt = fmc->getNormalizedValue(Vgt);
     }
```

### Comparing `pyresidfp-0.6.7/src/residfp/OpAmp.cpp` & `pyresidfp-0.7.0/src/residfp/OpAmp.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/OpAmp.h` & `pyresidfp-0.7.0/src/residfp/OpAmp.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * This file is part of libsidplayfp, a SID player engine.
  *
- * Copyright 2011-2015 Leandro Nini <drfiemost@users.sourceforge.net>
+ * Copyright 2011-2023 Leandro Nini <drfiemost@users.sourceforge.net>
  * Copyright 2007-2010 Antti Lankila
  * Copyright 2004,2010 Dag Lem
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 2 of the License, or
  * (at your option) any later version.
@@ -46,14 +46,16 @@
  *
  *     IR1f + IR2r = 0
  *
  * Substituting the triode mode transistor model K*W/L*(Vgst^2 - Vgdt^2)
  * for the currents, we get:
  *
  *     n*((Vddt - vx)^2 - (Vddt - vi)^2) + (Vddt - vx)^2 - (Vddt - vo)^2 = 0
+ * 
+ * where n is the ratio between R1 and R2.
  *
  * Our root function f can thus be written as:
  *
  *     f = (n + 1)*(Vddt - vx)^2 - n*(Vddt - vi)^2 - (Vddt - vo)^2 = 0
  *
  * Using substitution constants
  *
@@ -79,35 +81,41 @@
     std::unique_ptr<Spline> const opamp;
 
 public:
     /**
      * Opamp input -> output voltage conversion
      *
      * @param opamp opamp mapping table as pairs of points (in -> out)
-     * @param opamplength length of the opamp array
-     * @param kVddt transistor dt parameter (in volts)
+     * @param Vddt transistor dt parameter (in volts)
+     * @param vmin
+     * @param vmax
      */
-    OpAmp(const std::vector<Spline::Point> &opamp, double Vddt) :
+    OpAmp(const std::vector<Spline::Point> &opamp, double Vddt,
+            double vmin, double vmax
+    ) :
         x(0.),
         Vddt(Vddt),
-        vmin(opamp.front().x),
-        vmax(opamp.back().x),
+        vmin(vmin),
+        vmax(vmax),
         opamp(new Spline(opamp)) {}
 
+    /**
+     * Reset root position
+     */
     void reset() const
     {
         x = vmin;
     }
 
     /**
      * Solve the opamp equation for input vi in loading context n
      *
      * @param n the ratio of input/output loading
-     * @param vi input
-     * @return vo
+     * @param vi input voltage
+     * @return vo output voltage
      */
     double solve(double n, double vi) const;
 };
 
 } // namespace reSIDfp
 
 #endif
```

### Comparing `pyresidfp-0.6.7/src/residfp/Potentiometer.h` & `pyresidfp-0.7.0/src/residfp/Potentiometer.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/README` & `pyresidfp-0.7.0/src/residfp/README`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/SID.cpp` & `pyresidfp-0.7.0/src/residfp/SID.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -222,15 +222,16 @@
     default:
         throw SIDError("Unknown chip type");
     }
 
     this->model = model;
 
     // calculate waveform-related tables
-    matrix_t* tables = WaveformCalculator::getInstance()->buildTable(model);
+    matrix_t* wavetables = WaveformCalculator::getInstance()->getWaveTable();
+    matrix_t* pulldowntables = WaveformCalculator::getInstance()->buildPulldownTable(model);
 
     // calculate envelope DAC table
     {
         Dac dacBuilder(ENV_DAC_BITS);
         dacBuilder.kinkedDac(model);
 
         for (unsigned int i = 0; i < (1 << ENV_DAC_BITS); i++)
@@ -257,15 +258,16 @@
 
     // set voice tables
     for (int i = 0; i < 3; i++)
     {
         voice[i]->setEnvDAC(envDAC);
         voice[i]->setWavDAC(oscDAC);
         voice[i]->wave()->setModel(is6581);
-        voice[i]->wave()->setWaveformModels(tables);
+        voice[i]->wave()->setWaveformModels(wavetables);
+        voice[i]->wave()->setPulldownModels(pulldowntables);
     }
 }
 
 void SID::reset()
 {
     for (int i = 0; i < 3; i++)
     {
```

### Comparing `pyresidfp-0.6.7/src/residfp/SID.h` & `pyresidfp-0.7.0/src/residfp/SID.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/Spline.cpp` & `pyresidfp-0.7.0/src/residfp/Spline.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/Spline.h` & `pyresidfp-0.7.0/src/residfp/Spline.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/Voice.h` & `pyresidfp-0.7.0/src/residfp/Voice.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/WaveformCalculator.h` & `pyresidfp-0.7.0/src/residfp/WaveformCalculator.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * This file is part of libsidplayfp, a SID player engine.
  *
- * Copyright 2011-2016 Leandro Nini <drfiemost@users.sourceforge.net>
+ * Copyright 2011-2023 Leandro Nini <drfiemost@users.sourceforge.net>
  * Copyright 2007-2010 Antti Lankila
  *
  * This program is free software; you can redistribute it and/or modify
  * it under the terms of the GNU General Public License as published by
  * the Free Software Foundation; either version 2 of the License, or
  * (at your option) any later version.
  *
@@ -33,20 +33,18 @@
 {
 
 /**
  * Combined waveform model parameters.
  */
 typedef struct
 {
-    float bias;
+    float threshold;
     float pulsestrength;
-    float topbit;
     float distance1;
     float distance2;
-    float stmix;
 } CombinedWaveformConfig;
 
 /**
  * Combined waveform calculator for WaveformGenerator.
  * By combining waveforms, the bits of each waveform are effectively short
  * circuited. A zero bit in one waveform will result in a zero output bit
  * (thus the infamous claim that the waveforms are AND'ed).
@@ -100,29 +98,39 @@
  */
 class WaveformCalculator
 {
 private:
     typedef std::map<const CombinedWaveformConfig*, matrix_t> cw_cache_t;
 
 private:
-    cw_cache_t CACHE;
+    matrix_t wftable;
 
-    WaveformCalculator() DEFAULT;
+    cw_cache_t PULLDOWN_CACHE;
+
+private:
+    WaveformCalculator();
 
 public:
     /**
      * Get the singleton instance.
      */
     static WaveformCalculator* getInstance();
 
     /**
-     * Build waveform tables for use by WaveformGenerator.
+     * Get the waveform table for use by WaveformGenerator.
      *
-     * @param model Chip model to use
      * @return Waveform table
      */
-    matrix_t* buildTable(ChipModel model);
+    matrix_t* getWaveTable() { return &wftable; }
+
+    /**
+     * Build pulldown table for use by WaveformGenerator.
+     *
+     * @param model Chip model to use
+     * @return Pulldown table
+     */
+    matrix_t* buildPulldownTable(ChipModel model);
 };
 
 } // namespace reSIDfp
 
 #endif
```

### Comparing `pyresidfp-0.6.7/src/residfp/WaveformGenerator.cpp` & `pyresidfp-0.7.0/src/residfp/WaveformGenerator.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -75,14 +75,26 @@
 const unsigned int SHIFT_REGISTER_FADE_6581R3  =   15000;
 // ~2.15s
 const unsigned int SHIFT_REGISTER_RESET_6581R4 = 2150000;
 // ~2.8s
 const unsigned int SHIFT_REGISTER_RESET_8580R5 =  986000;
 const unsigned int SHIFT_REGISTER_FADE_8580R5  =  314300;
 
+const unsigned int shift_mask =
+    ~(
+        (1u <<  2) |  // Bit 20
+        (1u <<  4) |  // Bit 18
+        (1u <<  8) |  // Bit 14
+        (1u << 11) |  // Bit 11
+        (1u << 13) |  // Bit  9
+        (1u << 17) |  // Bit  5
+        (1u << 20) |  // Bit  2
+        (1u << 22)    // Bit  0
+    );
+
 /*
  * This is what happens when the lfsr is clocked:
  *
  * cycle 0: bit 19 of the accumulator goes from low to high, the noise register acts normally,
  *          the output may pulldown a bit;
  *
  * cycle 1: first phase of the shift, the bits are interconnected and the output of each bit
@@ -116,147 +128,105 @@
     // New noise waveform output.
     set_noise_output();
 }
 
 unsigned int WaveformGenerator::get_noise_writeback()
 {
   return
-    ~(
-        (1 <<  2) |  // Bit 20
-        (1 <<  4) |  // Bit 18
-        (1 <<  8) |  // Bit 14
-        (1 << 11) |  // Bit 11
-        (1 << 13) |  // Bit  9
-        (1 << 17) |  // Bit  5
-        (1 << 20) |  // Bit  2
-        (1 << 22)    // Bit  0
-    ) |
-    ((waveform_output & (1 << 11)) >>  9) |  // Bit 11 -> bit 20
-    ((waveform_output & (1 << 10)) >>  6) |  // Bit 10 -> bit 18
-    ((waveform_output & (1 <<  9)) >>  1) |  // Bit  9 -> bit 14
-    ((waveform_output & (1 <<  8)) <<  3) |  // Bit  8 -> bit 11
-    ((waveform_output & (1 <<  7)) <<  6) |  // Bit  7 -> bit  9
-    ((waveform_output & (1 <<  6)) << 11) |  // Bit  6 -> bit  5
-    ((waveform_output & (1 <<  5)) << 15) |  // Bit  5 -> bit  2
-    ((waveform_output & (1 <<  4)) << 18);   // Bit  4 -> bit  0
+    ((waveform_output & (1u << 11)) >>  9) |  // Bit 11 -> bit 20
+    ((waveform_output & (1u << 10)) >>  6) |  // Bit 10 -> bit 18
+    ((waveform_output & (1u <<  9)) >>  1) |  // Bit  9 -> bit 14
+    ((waveform_output & (1u <<  8)) <<  3) |  // Bit  8 -> bit 11
+    ((waveform_output & (1u <<  7)) <<  6) |  // Bit  7 -> bit  9
+    ((waveform_output & (1u <<  6)) << 11) |  // Bit  6 -> bit  5
+    ((waveform_output & (1u <<  5)) << 15) |  // Bit  5 -> bit  2
+    ((waveform_output & (1u <<  4)) << 18);   // Bit  4 -> bit  0
 }
 
 void WaveformGenerator::write_shift_register()
 {
     if (unlikely(waveform > 0x8) && likely(!test) && likely(shift_pipeline != 1))
     {
         // Write changes to the shift register output caused by combined waveforms
         // back into the shift register. This happens only when the register is clocked
         // (see $D1+$81_wave_test [1]) or when the test bit is falling.
         // A bit once set to zero cannot be changed, hence the and'ing.
         //
         // [1] ftp://ftp.untergrund.net/users/nata/sid_test/$D1+$81_wave_test.7z
-        //
-        // FIXME: Write test program to check the effect of 1 bits and whether
-        // neighboring bits are affected.
 
 #ifdef NO_WB_NOI_PUL
         if (waveform == 0xc)
             return;
 #endif
-        shift_register &= get_noise_writeback();
+        shift_register &= shift_mask | get_noise_writeback();
 
         noise_output &= waveform_output;
         set_no_noise_or_noise_output();
     }
 }
 
 void WaveformGenerator::set_noise_output()
 {
     noise_output =
-        ((shift_register & (1 <<  2)) <<  9) |  // Bit 20 -> bit 11
-        ((shift_register & (1 <<  4)) <<  6) |  // Bit 18 -> bit 10
-        ((shift_register & (1 <<  8)) <<  1) |  // Bit 14 -> bit  9
-        ((shift_register & (1 << 11)) >>  3) |  // Bit 11 -> bit  8
-        ((shift_register & (1 << 13)) >>  6) |  // Bit  9 -> bit  7
-        ((shift_register & (1 << 17)) >> 11) |  // Bit  5 -> bit  6
-        ((shift_register & (1 << 20)) >> 15) |  // Bit  2 -> bit  5
-        ((shift_register & (1 << 22)) >> 18);   // Bit  0 -> bit  4
+        ((shift_register & (1u <<  2)) <<  9) |  // Bit 20 -> bit 11
+        ((shift_register & (1u <<  4)) <<  6) |  // Bit 18 -> bit 10
+        ((shift_register & (1u <<  8)) <<  1) |  // Bit 14 -> bit  9
+        ((shift_register & (1u << 11)) >>  3) |  // Bit 11 -> bit  8
+        ((shift_register & (1u << 13)) >>  6) |  // Bit  9 -> bit  7
+        ((shift_register & (1u << 17)) >> 11) |  // Bit  5 -> bit  6
+        ((shift_register & (1u << 20)) >> 15) |  // Bit  2 -> bit  5
+        ((shift_register & (1u << 22)) >> 18);   // Bit  0 -> bit  4
 
     set_no_noise_or_noise_output();
 }
 
 void WaveformGenerator::setWaveformModels(matrix_t* models)
 {
     model_wave = models;
 }
 
+void WaveformGenerator::setPulldownModels(matrix_t* models)
+{
+    model_pulldown = models;
+}
+
 void WaveformGenerator::synchronize(WaveformGenerator* syncDest, const WaveformGenerator* syncSource) const
 {
     // A special case occurs when a sync source is synced itself on the same
     // cycle as when its MSB is set high. In this case the destination will
     // not be synced. This has been verified by sampling OSC3.
     if (unlikely(msb_rising) && syncDest->sync && !(sync && syncSource->msb_rising))
     {
         syncDest->accumulator = 0;
     }
 }
 
 bool do_pre_writeback(unsigned int waveform_prev, unsigned int waveform, bool is6581)
 {
     // no writeback without combined waveforms
-    if (likely(waveform_prev <= 0x8))
-        return false;
-    // no writeback when changing to noise
-    if (waveform == 8)
+    if (waveform <= 8)
         return false;
     // What's happening here?
     if (is6581 &&
             ((((waveform_prev & 0x3) == 0x1) && ((waveform & 0x3) == 0x2))
             || (((waveform_prev & 0x3) == 0x2) && ((waveform & 0x3) == 0x1))))
         return false;
     if (waveform_prev == 0xc)
-    {
-        if (is6581)
-            return false;
-        else if ((waveform != 0x9) && (waveform != 0xe))
-            return false;
-    }
+        return false;
 #ifdef NO_WB_NOI_PUL
     if (waveform == 0xc)
         return false;
 #endif
     // ok do the writeback
     return true;
 }
 
-/*
- * When noise and pulse are combined all the bits are
- * connected and the four lower ones are grounded.
- * This causes the adjacent bits to be pulled down,
- * with different strength depending on model.
- *
- * This is just a rough attempt at modelling the effect.
- */
- 
-static unsigned int noise_pulse6581(unsigned int noise)
-{
-    return (noise < 0xf00) ? 0x000 : noise & (noise << 1) & (noise << 2);
-}
-
-static unsigned int noise_pulse8580(unsigned int noise)
-{
-    return (noise < 0xfc0) ? noise & (noise << 1) : 0xfc0;
-}
-
 void WaveformGenerator::set_no_noise_or_noise_output()
 {
     no_noise_or_noise_output = no_noise | noise_output;
-
-    // pulse+noise
-    if (unlikely((waveform & 0xc) == 0xc))
-        no_noise_or_noise_output = is6581
-            ? noise_pulse6581(no_noise_or_noise_output)
-            : noise_pulse8580(no_noise_or_noise_output);
-
 }
 
 void WaveformGenerator::writeCONTROL_REG(unsigned char control)
 {
     const unsigned int waveform_prev = waveform;
     const bool test_prev = test;
 
@@ -265,16 +235,39 @@
     sync = (control & 0x02) != 0;
 
     // Substitution of accumulator MSB when sawtooth = 0, ring_mod = 1.
     ring_msb_mask = ((~control >> 5) & (control >> 2) & 0x1) << 23;
 
     if (waveform != waveform_prev)
     {
-        // Set up waveform table.
-        wave = (*model_wave)[waveform & 0x7];
+        // Set up waveform tables
+        wave = (*model_wave)[waveform & 0x3];
+        // We assume tha combinations including noise
+        // behave the same as without
+        switch (waveform & 0x7)
+        {
+        case 3:
+            pulldown = (*model_pulldown)[0];
+            break;
+        case 4:
+            pulldown = (waveform & 0x8) ? (*model_pulldown)[4] : nullptr;
+            break;
+        case 5:
+            pulldown = (*model_pulldown)[1];
+            break;
+        case 6:
+            pulldown = (*model_pulldown)[2];
+            break;
+        case 7:
+            pulldown = (*model_pulldown)[3];
+            break;
+        default:
+            pulldown = nullptr;
+            break;
+        }
 
         // no_noise and no_pulse are used in set_waveform_output() as bitmasks to
         // only let the noise or pulse influence the output when the noise or pulse
         // waveforms are selected.
         no_noise = (waveform & 0x8) != 0 ? 0x000 : 0xfff;
         set_no_noise_or_noise_output();
         no_pulse = (waveform & 0x4) != 0 ? 0x000 : 0xfff;
@@ -302,19 +295,19 @@
         }
         else
         {
             // When the test bit is falling, the second phase of the shift is
             // completed by enabling SRAM write.
 
             // During first phase of the shift the bits are interconnected
-            // and the output of each bit is latched into the following.
+            // and the output of each bit is loaded into the following.
             // The output may overwrite the latched value.
             if (do_pre_writeback(waveform_prev, waveform, is6581))
             {
-                shift_register &= get_noise_writeback();
+                shift_register = (shift_register & shift_mask) | get_noise_writeback();
             }
 
             // bit0 = (bit22 | test) ^ bit17 = 1 ^ bit17 = ~bit17
             clock_shift_register((~shift_register << 17) & (1 << 22));
         }
     }
 }
@@ -346,14 +339,15 @@
     waveform = 0;
     osc3 = 0;
 
     test = false;
     sync = false;
 
     wave = model_wave ? (*model_wave)[0] : nullptr;
+    pulldown = nullptr;
 
     ring_msb_mask = 0;
     no_noise = 0xfff;
     no_pulse = 0xfff;
     pulse_output = 0xfff;
 
     shift_register_reset = 0;
```

### Comparing `pyresidfp-0.6.7/src/residfp/WaveformGenerator.h` & `pyresidfp-0.7.0/src/residfp/WaveformGenerator.h`

 * *Files 7% similar despite different names*

```diff
@@ -83,16 +83,18 @@
  *
  * The low 4 waveform bits are zero (grounded).
  */
 class WaveformGenerator
 {
 private:
     matrix_t* model_wave;
+    matrix_t* model_pulldown;
 
     short* wave;
+    short* pulldown;
 
     // PWout = (PWn/40.95)%
     unsigned int pw;
 
     unsigned int shift_register;
 
     /// Emulation of pipeline causing bit 19 to clock the shift register.
@@ -152,14 +154,15 @@
 
     void waveBitfade();
 
     void shiftregBitfade();
 
 public:
     void setWaveformModels(matrix_t* models);
+    void setPulldownModels(matrix_t* models);
 
     /**
      * Set the chip model.
      * Must be called before any operation.
      *
      * @param is6581 true if MOS6581, false if CSG8580
      */
@@ -181,15 +184,17 @@
     void synchronize(WaveformGenerator* syncDest, const WaveformGenerator* syncSource) const;
 
     /**
      * Constructor.
      */
     WaveformGenerator() :
         model_wave(nullptr),
+        model_pulldown(nullptr),
         wave(nullptr),
+        pulldown(nullptr),
         pw(0),
         shift_register(0),
         shift_pipeline(0),
         ring_msb_mask(0),
         no_noise(0),
         noise_output(0),
         no_noise_or_noise_output(0),
@@ -322,15 +327,15 @@
         {
             // Pipeline: Detect rising bit, shift phase 1, shift phase 2.
             shift_pipeline = 2;
         }
         else if (unlikely(shift_pipeline != 0) && --shift_pipeline == 0)
         {
             // bit0 = (bit22 | test) ^ bit17
-            clock_shift_register(((shift_register << 22) ^ (shift_register << 17)) & (1 << 22));
+            clock_shift_register(((shift_register << 22) ^ (shift_register << 17)) & (1u << 22));
         }
     }
 }
 
 RESID_INLINE
 unsigned int WaveformGenerator::output(const WaveformGenerator* ringModulator)
 {
@@ -338,20 +343,25 @@
     if (likely(waveform != 0))
     {
         const unsigned int ix = (accumulator ^ (~ringModulator->accumulator & ring_msb_mask)) >> 12;
 
         // The bit masks no_pulse and no_noise are used to achieve branch-free
         // calculation of the output value.
         waveform_output = wave[ix] & (no_pulse | pulse_output) & no_noise_or_noise_output;
+        if (pulldown != nullptr)
+            waveform_output = pulldown[waveform_output];
 
         // Triangle/Sawtooth output is delayed half cycle on 8580.
-        // This will appear as a one cycle delay on OSC3 as it is latched first phase of the clock.
+        // This will appear as a one cycle delay on OSC3 as it is latched
+        // in the first phase of the clock.
         if ((waveform & 3) && !is6581)
         {
             osc3 = tri_saw_pipeline & (no_pulse | pulse_output) & no_noise_or_noise_output;
+            if (pulldown != nullptr)
+                osc3 = pulldown[osc3];
             tri_saw_pipeline = wave[ix];
         }
         else
         {
             osc3 = waveform_output;
         }
```

### Comparing `pyresidfp-0.6.7/src/residfp/array.h` & `pyresidfp-0.7.0/src/residfp/array.h`

 * *Files 14% similar despite different names*

```diff
@@ -17,21 +17,34 @@
  *  along with this program; if not, write to the Free Software
  *  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
  */
 
 #ifndef ARRAY_H
 #define ARRAY_H
 
+
+#ifdef HAVE_CONFIG_H
+#  include "config.h"
+#endif
+
+#ifdef HAVE_CXX11
+#  include <atomic>
+#endif
+
 /**
  * Counter.
  */
 class counter
 {
 private:
-    unsigned int c;
+#ifndef HAVE_CXX11
+    volatile unsigned int c;
+#else
+    std::atomic<unsigned int> c;
+#endif
 
 public:
     counter() : c(1) {}
     void increase() { ++c; }
     unsigned int decrease() { return --c; }
 };
```

### Comparing `pyresidfp-0.6.7/src/residfp/resample/Resampler.h` & `pyresidfp-0.7.0/src/residfp/resample/Resampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/resample/SincResampler.cpp` & `pyresidfp-0.7.0/src/residfp/resample/SincResampler.cpp`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/resample/SincResampler.h` & `pyresidfp-0.7.0/src/residfp/resample/SincResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/resample/TwoPassSincResampler.h` & `pyresidfp-0.7.0/src/residfp/resample/TwoPassSincResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/resample/ZeroOrderResampler.h` & `pyresidfp-0.7.0/src/residfp/resample/ZeroOrderResampler.h`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/siddefs-fp.h.in` & `pyresidfp-0.7.0/src/residfp/siddefs-fp.h.in`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/residfp/version.cc` & `pyresidfp-0.7.0/src/residfp/version.cc`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/src/sidcxx11.h` & `pyresidfp-0.7.0/src/sidcxx11.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * This file is part of libsidplayfp, a SID player engine.
  *
- *  Copyright 2014-2015 Leandro Nini
+ *  Copyright 2014-2022 Leandro Nini
  *
  *  This program is free software; you can redistribute it and/or modify
  *  it under the terms of the GNU General Public License as published by
  *  the Free Software Foundation; either version 2 of the License, or
  *  (at your option) any later version.
  *
  *  This program is distributed in the hope that it will be useful,
@@ -14,21 +14,36 @@
  *  GNU General Public License for more details.
  *
  *  You should have received a copy of the GNU General Public License
  *  along with this program; if not, write to the Free Software
  *  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
  */
 
-#ifndef SIDCXX11_H
-#define SIDCXX11_H
+#ifndef SIDCXX_H
+#define SIDCXX_H
 
 #ifdef HAVE_CONFIG_H
 #  include "config.h"
 #endif
 
+
+#ifdef HAVE_CXX17
+#  define HAVE_CXX14
+#  define MAYBE_UNUSED [[ maybe_unused ]]
+#else
+#  define MAYBE_UNUSED
+#endif
+
+#ifdef HAVE_CXX14
+#  define HAVE_CXX11
+#  define MAKE_UNIQUE(type, ...) std::make_unique<type>(__VA_ARGS__)
+#else
+#  define MAKE_UNIQUE(type, ...) std::unique_ptr<type>(new type(__VA_ARGS__))
+#endif
+
 #ifndef HAVE_CXX11
 #  define nullptr    0
 #  define override
 #  define final
 #  define unique_ptr auto_ptr
 #  define DEFAULT {}
 #  define DELETE {}
```

### Comparing `pyresidfp-0.6.7/tests/test_basic.py` & `pyresidfp-0.7.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyresidfp-0.6.7/PKG-INFO` & `pyresidfp-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyresidfp
-Version: 0.6.7
+Version: 0.7.0
 Summary: Emulates the SID sound-chip
 Author-Email: Sebastian Klemke <pypi@nerdheim.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

