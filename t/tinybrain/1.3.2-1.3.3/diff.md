# Comparing `tmp/tinybrain-1.3.2.tar.gz` & `tmp/tinybrain-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybrain-1.3.2.tar", last modified: Thu May 11 21:47:16 2023, max compression
+gzip compressed data, was "tinybrain-1.3.3.tar", last modified: Sat Jun  3 00:09:23 2023, max compression
```

## Comparing `tinybrain-1.3.2.tar` & `tinybrain-1.3.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-05-11 21:47:16.019880 tinybrain-1.3.2/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-05-11 21:47:16.010887 tinybrain-1.3.2/.github/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-05-11 21:47:16.016823 tinybrain-1.3.2/.github/workflows/
--rw-r--r--   0 wms        (501) staff       (20)      947 2023-05-06 23:45:33.000000 tinybrain-1.3.2/.github/workflows/build_wheel.yml
--rw-r--r--   0 wms        (501) staff       (20)      878 2022-08-26 19:08:36.000000 tinybrain-1.3.2/.github/workflows/run_tests.yml
--rw-r--r--   0 wms        (501) staff       (20)       97 2023-05-11 21:47:14.000000 tinybrain-1.3.2/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     4490 2023-05-11 21:47:14.000000 tinybrain-1.3.2/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    35149 2021-01-20 17:58:46.000000 tinybrain-1.3.2/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)    10797 2023-05-11 21:47:16.020150 tinybrain-1.3.2/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     8879 2022-03-05 06:53:04.000000 tinybrain-1.3.2/README.md
--rw-r--r--   0 wms        (501) staff       (20)    21512 2022-08-26 19:05:33.000000 tinybrain-1.3.2/automated_test.py
--rwxr-xr-x   0 wms        (501) staff       (20)      709 2022-02-07 19:05:06.000000 tinybrain-1.3.2/build_linux.sh
--rw-r--r--   0 wms        (501) staff       (20)     1204 2021-03-17 20:30:55.000000 tinybrain-1.3.2/manylinux1.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     1235 2021-03-17 20:30:55.000000 tinybrain-1.3.2/manylinux2010.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     1558 2022-02-07 19:05:11.000000 tinybrain-1.3.2/manylinux2014.Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)     4337 2022-03-05 06:53:04.000000 tinybrain-1.3.2/perf.py
--rw-r--r--   0 wms        (501) staff       (20)       90 2022-02-07 19:58:32.000000 tinybrain-1.3.2/pyproject.toml
--rw-r--r--   0 wms        (501) staff       (20)        6 2021-12-02 23:06:40.000000 tinybrain-1.3.2/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)        6 2023-05-11 20:23:25.000000 tinybrain-1.3.2/requirements_dev.txt
--rw-r--r--   0 wms        (501) staff       (20)      924 2023-05-11 21:47:16.020960 tinybrain-1.3.2/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)     1141 2023-05-11 20:23:17.000000 tinybrain-1.3.2/setup.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-05-11 21:47:16.018256 tinybrain-1.3.2/tinybrain/
--rw-r--r--   0 wms        (501) staff       (20)      183 2023-05-11 20:31:27.000000 tinybrain-1.3.2/tinybrain/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    26011 2022-03-05 06:53:04.000000 tinybrain-1.3.2/tinybrain/accelerated.hpp
--rw-r--r--   0 wms        (501) staff       (20)    26323 2022-03-05 06:53:04.000000 tinybrain-1.3.2/tinybrain/accelerated.pyx
--rw-r--r--   0 wms        (501) staff       (20)    15412 2022-08-26 19:05:33.000000 tinybrain-1.3.2/tinybrain/downsample.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-05-11 21:47:16.019717 tinybrain-1.3.2/tinybrain.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)    10797 2023-05-11 21:47:14.000000 tinybrain-1.3.2/tinybrain.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      616 2023-05-11 21:47:16.000000 tinybrain-1.3.2/tinybrain.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2023-05-11 21:47:14.000000 tinybrain-1.3.2/tinybrain.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2021-01-20 17:59:34.000000 tinybrain-1.3.2/tinybrain.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2023-05-11 21:47:14.000000 tinybrain-1.3.2/tinybrain.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)        6 2023-05-11 21:47:14.000000 tinybrain-1.3.2/tinybrain.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       10 2023-05-11 21:47:14.000000 tinybrain-1.3.2/tinybrain.egg-info/top_level.txt
--rw-r--r--   0 wms        (501) staff       (20)      208 2023-05-11 20:22:50.000000 tinybrain-1.3.2/tox.ini
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-03 00:09:23.762244 tinybrain-1.3.3/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-03 00:09:23.752266 tinybrain-1.3.3/.github/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-03 00:09:23.758597 tinybrain-1.3.3/.github/workflows/
+-rw-r--r--   0 wms        (501) staff       (20)      947 2023-05-06 23:45:33.000000 tinybrain-1.3.3/.github/workflows/build_wheel.yml
+-rw-r--r--   0 wms        (501) staff       (20)      878 2022-08-26 19:08:36.000000 tinybrain-1.3.3/.github/workflows/run_tests.yml
+-rw-r--r--   0 wms        (501) staff       (20)       97 2023-06-03 00:09:22.000000 tinybrain-1.3.3/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     4721 2023-06-03 00:09:22.000000 tinybrain-1.3.3/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    35149 2021-01-20 17:58:46.000000 tinybrain-1.3.3/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)    10797 2023-06-03 00:09:23.762505 tinybrain-1.3.3/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     8879 2022-03-05 06:53:04.000000 tinybrain-1.3.3/README.md
+-rw-r--r--   0 wms        (501) staff       (20)    21512 2022-08-26 19:05:33.000000 tinybrain-1.3.3/automated_test.py
+-rwxr-xr-x   0 wms        (501) staff       (20)      709 2022-02-07 19:05:06.000000 tinybrain-1.3.3/build_linux.sh
+-rw-r--r--   0 wms        (501) staff       (20)     1204 2021-03-17 20:30:55.000000 tinybrain-1.3.3/manylinux1.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     1235 2021-03-17 20:30:55.000000 tinybrain-1.3.3/manylinux2010.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     1558 2022-02-07 19:05:11.000000 tinybrain-1.3.3/manylinux2014.Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)     4337 2022-03-05 06:53:04.000000 tinybrain-1.3.3/perf.py
+-rw-r--r--   0 wms        (501) staff       (20)       90 2022-02-07 19:58:32.000000 tinybrain-1.3.3/pyproject.toml
+-rw-r--r--   0 wms        (501) staff       (20)        6 2021-12-02 23:06:40.000000 tinybrain-1.3.3/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)        6 2023-05-11 20:23:25.000000 tinybrain-1.3.3/requirements_dev.txt
+-rw-r--r--   0 wms        (501) staff       (20)      924 2023-06-03 00:09:23.763731 tinybrain-1.3.3/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)     1141 2023-05-11 20:23:17.000000 tinybrain-1.3.3/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-03 00:09:23.760348 tinybrain-1.3.3/tinybrain/
+-rw-r--r--   0 wms        (501) staff       (20)      183 2023-06-02 23:47:47.000000 tinybrain-1.3.3/tinybrain/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    25889 2023-06-02 23:52:33.000000 tinybrain-1.3.3/tinybrain/accelerated.hpp
+-rw-r--r--   0 wms        (501) staff       (20)    26323 2022-03-05 06:53:04.000000 tinybrain-1.3.3/tinybrain/accelerated.pyx
+-rw-r--r--   0 wms        (501) staff       (20)    15497 2023-06-01 19:36:31.000000 tinybrain-1.3.3/tinybrain/downsample.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2023-06-03 00:09:23.762006 tinybrain-1.3.3/tinybrain.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)    10797 2023-06-03 00:09:22.000000 tinybrain-1.3.3/tinybrain.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      616 2023-06-03 00:09:23.000000 tinybrain-1.3.3/tinybrain.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2023-06-03 00:09:22.000000 tinybrain-1.3.3/tinybrain.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2021-01-20 17:59:34.000000 tinybrain-1.3.3/tinybrain.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2023-06-03 00:09:22.000000 tinybrain-1.3.3/tinybrain.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)        6 2023-06-03 00:09:22.000000 tinybrain-1.3.3/tinybrain.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       10 2023-06-03 00:09:22.000000 tinybrain-1.3.3/tinybrain.egg-info/top_level.txt
+-rw-r--r--   0 wms        (501) staff       (20)      208 2023-05-11 20:22:50.000000 tinybrain-1.3.3/tox.ini
```

### Comparing `tinybrain-1.3.2/.github/workflows/build_wheel.yml` & `tinybrain-1.3.3/.github/workflows/build_wheel.yml`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.2/.github/workflows/run_tests.yml` & `tinybrain-1.3.3/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.2/ChangeLog` & `tinybrain-1.3.3/ChangeLog`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+1.3.3
+-----
+
+* release(1.3.3): fix sparse mode 2x2x2 seg ds and throw error
+* fix: throw error if sparse mode isn't supported
+* refactor: remove unused variable oyoff
+* fix: incorrect sparse check value in 2x2x2 mode downsampling
+
 1.3.2
 -----
 
 * release(1.3.2): updates build system for py311
 * build: update for python311
 
 1.3.1
```

### Comparing `tinybrain-1.3.2/LICENSE` & `tinybrain-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.2/PKG-INFO` & `tinybrain-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybrain
-Version: 1.3.2
+Version: 1.3.3
 Summary: Image pyramid generation specialized for connectomics data types and procedures.
 Home-page: https://github.com/seung-lab/tinybrain/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/seung-lab/tinybrain.svg?branch=master)](https://travis-ci.org/seung-lab/tinybrain) [![PyPI version](https://badge.fury.io/py/tinybrain.svg)](https://badge.fury.io/py/tinybrain)
```

### Comparing `tinybrain-1.3.2/README.md` & `tinybrain-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.2/automated_test.py` & `tinybrain-1.3.3/automated_test.py`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.2/build_linux.sh` & `tinybrain-1.3.3/build_linux.sh`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.2/manylinux1.Dockerfile` & `tinybrain-1.3.3/manylinux1.Dockerfile`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.2/manylinux2010.Dockerfile` & `tinybrain-1.3.3/manylinux2010.Dockerfile`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.2/manylinux2014.Dockerfile` & `tinybrain-1.3.3/manylinux2014.Dockerfile`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.2/perf.py` & `tinybrain-1.3.3/perf.py`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.2/setup.cfg` & `tinybrain-1.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.2/setup.py` & `tinybrain-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.2/tinybrain/accelerated.hpp` & `tinybrain-1.3.3/tinybrain/accelerated.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,15 @@
   const size_t odd_y = static_cast<size_t>(sy & 0x01);
 
   if (out == NULL) {
     out = new T[ovoxels]();
   }
 
   size_t x, ox, y, oy;
-  size_t zoff, ozoff, oyoff;
+  size_t zoff, ozoff;
 
   for (size_t w = 0; w < sw; w++) {
     for (size_t z = 0; z < sz; z++) {
       zoff = sxy * (z + sz * w);
       ozoff = osxy * (z + sz * w);
 
       for (y = 0, oy = 0; y < sy - odd_y; y += 2, oy++) {
@@ -359,15 +359,14 @@
           );
         }
       }
 
       if (odd_y) {
         y = sy - 1;
         oy = osy - 1;
-        oyoff = (osx * oy + ozoff);
 
         for (x = 0, ox = 0; x < sx - odd_x; x += 2, ox++) {
           out[ox + osx * oy + ozoff] = static_cast<T>(
             (
                 static_cast<T2>(channel[x + sx * y + zoff]) 
               + static_cast<T2>(channel[(x+1) + sx * y + zoff])
             ) / 2
@@ -526,15 +525,15 @@
   const size_t odd_z = static_cast<size_t>(sz & 0x01);
 
   if (out == NULL) {
     out = new T[ovoxels]();
   }
 
   size_t x, ox, y, oy, z, oz;
-  size_t zoff, ozoff, oyoff;
+  size_t zoff, ozoff;
 
   for (size_t w = 0; w < sw; w++) {
     for (z = 0, oz = 0; z < sz - odd_z; z += 2, oz++) {
       zoff = sxy * (z + sz * w);
       ozoff = osxy * (oz + osz * w);
 
       for (y = 0, oy = 0; y < sy - odd_y; y += 2, oy++) {
@@ -566,15 +565,14 @@
           );
         }
       }
 
       if (odd_y) {
         y = sy - 1;
         oy = osy - 1;
-        oyoff = (osx * oy + ozoff);
 
         for (x = 0, ox = 0; x < sx - odd_x; x += 2, ox++) {
           out[ox + osx * oy + ozoff] = static_cast<T>(
             (
                 static_cast<T2>(channel[x + sx * y + zoff]) 
               + static_cast<T2>(channel[(x+1) + sx * y + zoff])
               + static_cast<T2>(channel[x + sx * y + zoff + sxy]) 
@@ -618,15 +616,14 @@
           );
         }
       }
 
       if (odd_y) {
         y = sy - 1;
         oy = osy - 1;
-        oyoff = (osx * oy + ozoff);
 
         for (x = 0, ox = 0; x < sx - odd_x; x += 2, ox++) {
           out[ox + osx * oy + ozoff] = static_cast<T>(
             (
                 static_cast<T2>(channel[x + sx * y + zoff]) 
               + static_cast<T2>(channel[(x+1) + sx * y + zoff])
             ) / 2
@@ -938,15 +935,15 @@
         size_t o_loc = (x >> 1) + osx * (y >> 1) + osxy * (z >> 1);
         // These two if statements could be removed, but they add a very small
         // cost on random data (< 10%) and can speed up connectomics data by ~4x
         if (vals[0] == vals[1] && vals[0] == vals[2] && vals[0] == vals[3] && (!sparse || vals[0] != 0)) {
           oimg[o_loc] = vals[0];
           continue;
         }
-        else if (vals[4] == vals[5] && vals[4] == vals[6] && vals[4] == vals[7] && (!sparse || vals[0] != 0)) {
+        else if (vals[4] == vals[5] && vals[4] == vals[6] && vals[4] == vals[7] && (!sparse || vals[4] != 0)) {
           oimg[o_loc] = vals[4];
           continue;
         }
 
         max_ct = 0;
         max_val = 0;
         for (short int t = 0; t < 8; t++) {
```

### Comparing `tinybrain-1.3.2/tinybrain/accelerated.pyx` & `tinybrain-1.3.3/tinybrain/accelerated.pyx`

 * *Files identical despite different names*

### Comparing `tinybrain-1.3.2/tinybrain/downsample.py` & `tinybrain-1.3.3/tinybrain/downsample.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,16 @@
   """
   if (
     img.dtype in (np.uint8, np.uint16, np.float32, np.float64)
     or num_mips == 1 # _average_pooling_2x2_single_mip_py supports all primative types
   ):
     img = np.asfortranarray(img)
     if (tuple(factor) in ( (2,2), (2,2,1), (2,2,1,1) )):
+      if sparse:
+        raise ValueError("sparse mode is not implemented for 2x2.")
       return tinybrain.accelerated.average_pooling_2x2(img, num_mips)
     elif (tuple(factor) in ( (2,2,2), (2,2,2,1) )):
       return tinybrain.accelerated.average_pooling_2x2x2(img, num_mips, sparse)
 
   results = []
   if np.dtype(img.dtype).itemsize < 4:
     dtype = img.dtype
```

### Comparing `tinybrain-1.3.2/tinybrain.egg-info/PKG-INFO` & `tinybrain-1.3.3/tinybrain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybrain
-Version: 1.3.2
+Version: 1.3.3
 Summary: Image pyramid generation specialized for connectomics data types and procedures.
 Home-page: https://github.com/seung-lab/tinybrain/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/seung-lab/tinybrain.svg?branch=master)](https://travis-ci.org/seung-lab/tinybrain) [![PyPI version](https://badge.fury.io/py/tinybrain.svg)](https://badge.fury.io/py/tinybrain)
```

### Comparing `tinybrain-1.3.2/tinybrain.egg-info/SOURCES.txt` & `tinybrain-1.3.3/tinybrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

