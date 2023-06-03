# Comparing `tmp/UBC-Solar-Simulation-0.5.6a0.tar.gz` & `tmp/UBC-Solar-Simulation-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UBC-Solar-Simulation-0.5.6a0.tar", last modified: Sat Feb 11 19:35:43 2023, max compression
+gzip compressed data, was "UBC-Solar-Simulation-0.5.7.tar", last modified: Sat Jun  3 18:33:35 2023, max compression
```

## Comparing `UBC-Solar-Simulation-0.5.6a0.tar` & `UBC-Solar-Simulation-0.5.7.tar`

### file list

```diff
@@ -1,83 +1,86 @@
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.629209 UBC-Solar-Simulation-0.5.6a0/
--rw-r--r--   0 joshuariefman   (501) staff       (20)     1066 2023-01-28 20:31:40.000000 UBC-Solar-Simulation-0.5.6a0/LICENSE
--rw-r--r--   0 joshuariefman   (501) staff       (20)      108 2023-02-11 19:35:08.000000 UBC-Solar-Simulation-0.5.6a0/MANIFEST.in
--rw-r--r--   0 joshuariefman   (501) staff       (20)      615 2023-02-11 19:35:43.629043 UBC-Solar-Simulation-0.5.6a0/PKG-INFO
--rw-r--r--   0 joshuariefman   (501) staff       (20)     3453 2023-01-28 20:31:40.000000 UBC-Solar-Simulation-0.5.6a0/README.md
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.606817 UBC-Solar-Simulation-0.5.6a0/UBC_Solar_Simulation.egg-info/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      615 2023-02-11 19:35:43.000000 UBC-Solar-Simulation-0.5.6a0/UBC_Solar_Simulation.egg-info/PKG-INFO
--rw-r--r--   0 joshuariefman   (501) staff       (20)     2035 2023-02-11 19:35:43.000000 UBC-Solar-Simulation-0.5.6a0/UBC_Solar_Simulation.egg-info/SOURCES.txt
--rw-r--r--   0 joshuariefman   (501) staff       (20)        1 2023-02-11 19:35:43.000000 UBC-Solar-Simulation-0.5.6a0/UBC_Solar_Simulation.egg-info/dependency_links.txt
--rw-r--r--   0 joshuariefman   (501) staff       (20)      145 2023-02-11 19:35:43.000000 UBC-Solar-Simulation-0.5.6a0/UBC_Solar_Simulation.egg-info/requires.txt
--rw-r--r--   0 joshuariefman   (501) staff       (20)       11 2023-02-11 19:35:43.000000 UBC-Solar-Simulation-0.5.6a0/UBC_Solar_Simulation.egg-info/top_level.txt
--rw-r--r--   0 joshuariefman   (501) staff       (20)       38 2023-02-11 19:35:43.629260 UBC-Solar-Simulation-0.5.6a0/setup.cfg
--rw-r--r--   0 joshuariefman   (501) staff       (20)     1468 2023-02-11 19:35:31.000000 UBC-Solar-Simulation-0.5.6a0/setup.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.606966 UBC-Solar-Simulation-0.5.6a0/simulation/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      882 2023-02-09 02:58:14.000000 UBC-Solar-Simulation-0.5.6a0/simulation/__init__.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.614302 UBC-Solar-Simulation-0.5.6a0/simulation/array/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      102 2023-01-28 20:43:42.000000 UBC-Solar-Simulation-0.5.6a0/simulation/array/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      189 2023-01-28 20:43:42.000000 UBC-Solar-Simulation-0.5.6a0/simulation/array/base_array.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)     2425 2023-01-28 20:43:42.000000 UBC-Solar-Simulation-0.5.6a0/simulation/array/basic_array.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.614860 UBC-Solar-Simulation-0.5.6a0/simulation/battery/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      114 2023-01-28 20:44:35.000000 UBC-Solar-Simulation-0.5.6a0/simulation/battery/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)     2446 2023-01-28 20:44:35.000000 UBC-Solar-Simulation-0.5.6a0/simulation/battery/base_battery.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)     5210 2023-01-28 20:44:35.000000 UBC-Solar-Simulation-0.5.6a0/simulation/battery/basic_battery.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.615098 UBC-Solar-Simulation-0.5.6a0/simulation/cache/
--rw-r--r--   0 joshuariefman   (501) staff       (20)        0 2023-02-09 03:10:21.000000 UBC-Solar-Simulation-0.5.6a0/simulation/cache/__init__.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.617725 UBC-Solar-Simulation-0.5.6a0/simulation/cache/route/
--rw-r--r--   0 joshuariefman   (501) staff       (20)       64 2023-02-07 23:16:14.000000 UBC-Solar-Simulation-0.5.6a0/simulation/cache/route/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)  1309540 2023-02-07 23:16:14.000000 UBC-Solar-Simulation-0.5.6a0/simulation/cache/route/route_data.npz
--rw-r--r--   0 joshuariefman   (501) staff       (20)     9396 2023-02-07 23:16:14.000000 UBC-Solar-Simulation-0.5.6a0/simulation/cache/route/route_data_FSGP.npz
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.618350 UBC-Solar-Simulation-0.5.6a0/simulation/cache/weather/
--rw-r--r--   0 joshuariefman   (501) staff       (20)       66 2023-02-07 23:16:14.000000 UBC-Solar-Simulation-0.5.6a0/simulation/cache/weather/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)    38842 2023-02-07 23:16:14.000000 UBC-Solar-Simulation-0.5.6a0/simulation/cache/weather/weather_data.npz
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.620067 UBC-Solar-Simulation-0.5.6a0/simulation/common/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      246 2023-01-28 20:42:02.000000 UBC-Solar-Simulation-0.5.6a0/simulation/common/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      523 2023-01-28 20:31:40.000000 UBC-Solar-Simulation-0.5.6a0/simulation/common/car.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      113 2023-01-28 20:31:40.000000 UBC-Solar-Simulation-0.5.6a0/simulation/common/constants.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      782 2023-01-28 20:31:40.000000 UBC-Solar-Simulation-0.5.6a0/simulation/common/consumer.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      121 2023-01-28 20:31:40.000000 UBC-Solar-Simulation-0.5.6a0/simulation/common/exceptions.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)    29628 2023-01-28 20:45:05.000000 UBC-Solar-Simulation-0.5.6a0/simulation/common/helpers.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      784 2023-01-28 20:31:40.000000 UBC-Solar-Simulation-0.5.6a0/simulation/common/producer.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      523 2023-01-28 20:31:40.000000 UBC-Solar-Simulation-0.5.6a0/simulation/common/storage.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.620472 UBC-Solar-Simulation-0.5.6a0/simulation/config/
--rw-r--r--   0 joshuariefman   (501) staff       (20)       67 2023-01-28 20:31:40.000000 UBC-Solar-Simulation-0.5.6a0/simulation/config/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      509 2023-01-28 20:31:40.000000 UBC-Solar-Simulation-0.5.6a0/simulation/config/settings_ASC.json
--rw-r--r--   0 joshuariefman   (501) staff       (20)      732 2023-01-28 20:31:40.000000 UBC-Solar-Simulation-0.5.6a0/simulation/config/settings_FSGP.json
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.620650 UBC-Solar-Simulation-0.5.6a0/simulation/data/
--rw-r--r--   0 joshuariefman   (501) staff       (20)        0 2023-02-07 23:16:14.000000 UBC-Solar-Simulation-0.5.6a0/simulation/data/__init__.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.621677 UBC-Solar-Simulation-0.5.6a0/simulation/environment/
--rw-r--r--   0 joshuariefman   (501) staff       (20)    15947 2023-02-11 19:31:57.000000 UBC-Solar-Simulation-0.5.6a0/simulation/environment/GIS.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)    13987 2023-01-28 20:45:36.000000 UBC-Solar-Simulation-0.5.6a0/simulation/environment/SolarCalculations.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)    22544 2023-02-11 19:26:14.000000 UBC-Solar-Simulation-0.5.6a0/simulation/environment/WeatherForecasts.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      183 2023-01-28 20:45:21.000000 UBC-Solar-Simulation-0.5.6a0/simulation/environment/__init__.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.622151 UBC-Solar-Simulation-0.5.6a0/simulation/examples/
--rw-r--r--   0 joshuariefman   (501) staff       (20)        0 2023-02-09 02:06:02.000000 UBC-Solar-Simulation-0.5.6a0/simulation/examples/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)     2926 2023-02-09 02:46:25.000000 UBC-Solar-Simulation-0.5.6a0/simulation/examples/fastest_time_given_distance.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)     2594 2023-02-08 08:32:26.000000 UBC-Solar-Simulation-0.5.6a0/simulation/examples/max_distance_from_speed_using_arrays.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.622875 UBC-Solar-Simulation-0.5.6a0/simulation/lvs/
--rw-r--r--   0 joshuariefman   (501) staff       (20)       90 2023-01-28 20:45:53.000000 UBC-Solar-Simulation-0.5.6a0/simulation/lvs/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      185 2023-01-28 20:45:59.000000 UBC-Solar-Simulation-0.5.6a0/simulation/lvs/base_lvs.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      197 2023-01-28 20:45:59.000000 UBC-Solar-Simulation-0.5.6a0/simulation/lvs/basic_lvs.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.625680 UBC-Solar-Simulation-0.5.6a0/simulation/main/
--rw-r--r--   0 joshuariefman   (501) staff       (20)     1453 2023-01-31 01:43:48.000000 UBC-Solar-Simulation-0.5.6a0/simulation/main/ExecuteSimulation.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)    17593 2023-01-28 20:46:46.000000 UBC-Solar-Simulation-0.5.6a0/simulation/main/MainSimulation.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      569 2023-01-28 20:31:40.000000 UBC-Solar-Simulation-0.5.6a0/simulation/main/SimulationResult.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)    17728 2023-02-09 03:13:17.000000 UBC-Solar-Simulation-0.5.6a0/simulation/main/TimeSimulation.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      174 2023-01-28 20:46:16.000000 UBC-Solar-Simulation-0.5.6a0/simulation/main/__init__.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.626263 UBC-Solar-Simulation-0.5.6a0/simulation/motor/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      102 2023-01-28 20:47:28.000000 UBC-Solar-Simulation-0.5.6a0/simulation/motor/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      123 2023-01-28 20:47:28.000000 UBC-Solar-Simulation-0.5.6a0/simulation/motor/base_motor.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)     9335 2023-01-28 20:48:36.000000 UBC-Solar-Simulation-0.5.6a0/simulation/motor/basic_motor.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.627326 UBC-Solar-Simulation-0.5.6a0/simulation/optimization/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      199 2023-02-07 23:16:14.000000 UBC-Solar-Simulation-0.5.6a0/simulation/optimization/__init__.py
--rwxr-xr-x   0 joshuariefman   (501) staff       (20)      396 2023-01-28 20:47:37.000000 UBC-Solar-Simulation-0.5.6a0/simulation/optimization/base_optimization.py
--rwxr-xr-x   0 joshuariefman   (501) staff       (20)      754 2023-01-28 20:47:37.000000 UBC-Solar-Simulation-0.5.6a0/simulation/optimization/bayesian.py
--rwxr-xr-x   0 joshuariefman   (501) staff       (20)      775 2023-01-28 20:47:41.000000 UBC-Solar-Simulation-0.5.6a0/simulation/optimization/random.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.628216 UBC-Solar-Simulation-0.5.6a0/simulation/regen/
--rw-r--r--   0 joshuariefman   (501) staff       (20)      102 2023-01-28 20:47:47.000000 UBC-Solar-Simulation-0.5.6a0/simulation/regen/__init__.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      123 2023-01-28 20:47:50.000000 UBC-Solar-Simulation-0.5.6a0/simulation/regen/base_regen.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)      237 2023-01-28 20:47:53.000000 UBC-Solar-Simulation-0.5.6a0/simulation/regen/basic_regen.py
-drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-02-11 19:35:43.628749 UBC-Solar-Simulation-0.5.6a0/simulation/utils/
--rwxr-xr-x   0 joshuariefman   (501) staff       (20)      827 2023-01-28 20:31:40.000000 UBC-Solar-Simulation-0.5.6a0/simulation/utils/InputBounds.py
--rwxr-xr-x   0 joshuariefman   (501) staff       (20)     3856 2023-01-28 20:47:59.000000 UBC-Solar-Simulation-0.5.6a0/simulation/utils/MapPlot.py
--rw-r--r--   0 joshuariefman   (501) staff       (20)       53 2023-02-07 23:16:14.000000 UBC-Solar-Simulation-0.5.6a0/simulation/utils/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.875714 UBC-Solar-Simulation-0.5.7/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     1066 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.7/LICENSE
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      179 2023-03-18 21:26:04.000000 UBC-Solar-Simulation-0.5.7/MANIFEST.in
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      613 2023-06-03 18:33:35.875554 UBC-Solar-Simulation-0.5.7/PKG-INFO
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     3672 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/README.md
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.856601 UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      613 2023-06-03 18:33:35.000000 UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/PKG-INFO
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     2093 2023-06-03 18:33:35.000000 UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/SOURCES.txt
+-rw-r--r--   0 joshuariefman   (501) staff       (20)        1 2023-06-03 18:33:35.000000 UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/dependency_links.txt
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      145 2023-06-03 18:33:35.000000 UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/requires.txt
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       11 2023-06-03 18:33:35.000000 UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/top_level.txt
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       38 2023-06-03 18:33:35.875765 UBC-Solar-Simulation-0.5.7/setup.cfg
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     1462 2023-06-03 18:33:32.000000 UBC-Solar-Simulation-0.5.7/setup.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.856947 UBC-Solar-Simulation-0.5.7/simulation/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      920 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.857659 UBC-Solar-Simulation-0.5.7/simulation/arrays/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      104 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/arrays/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      153 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/arrays/base_array.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     2515 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/arrays/basic_array.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.858392 UBC-Solar-Simulation-0.5.7/simulation/battery/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      114 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/battery/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     2446 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/battery/base_battery.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     6204 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/battery/basic_battery.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.858532 UBC-Solar-Simulation-0.5.7/simulation/cache/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)        0 2023-03-04 19:45:57.000000 UBC-Solar-Simulation-0.5.7/simulation/cache/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.861190 UBC-Solar-Simulation-0.5.7/simulation/cache/route/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       64 2023-03-18 21:22:15.000000 UBC-Solar-Simulation-0.5.7/simulation/cache/route/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)  1309540 2023-03-18 21:22:21.000000 UBC-Solar-Simulation-0.5.7/simulation/cache/route/route_data.npz
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     9396 2023-03-18 21:22:24.000000 UBC-Solar-Simulation-0.5.7/simulation/cache/route/route_data_FSGP.npz
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.864582 UBC-Solar-Simulation-0.5.7/simulation/cache/weather/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       66 2023-03-18 21:22:15.000000 UBC-Solar-Simulation-0.5.7/simulation/cache/weather/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)    38842 2023-03-18 21:22:31.000000 UBC-Solar-Simulation-0.5.7/simulation/cache/weather/weather_data.npz
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.869163 UBC-Solar-Simulation-0.5.7/simulation/common/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      308 2023-04-08 18:23:00.000000 UBC-Solar-Simulation-0.5.7/simulation/common/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      541 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/common/car.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      113 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.7/simulation/common/constants.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      786 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/common/consumer.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      121 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.7/simulation/common/exceptions.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)    27367 2023-06-03 18:19:19.000000 UBC-Solar-Simulation-0.5.7/simulation/common/helpers.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     1377 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/common/plotting.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      785 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/common/producer.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      569 2023-05-30 21:02:16.000000 UBC-Solar-Simulation-0.5.7/simulation/common/simulationState.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      523 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/common/storage.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     1345 2023-03-07 05:08:11.000000 UBC-Solar-Simulation-0.5.7/simulation/common/valuedProcess.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.869967 UBC-Solar-Simulation-0.5.7/simulation/config/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       67 2023-05-30 21:02:16.000000 UBC-Solar-Simulation-0.5.7/simulation/config/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      452 2023-03-04 19:45:57.000000 UBC-Solar-Simulation-0.5.7/simulation/config/initial_conditions.json
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      531 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/config/settings_ASC.json
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      732 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.7/simulation/config/settings_FSGP.json
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.870149 UBC-Solar-Simulation-0.5.7/simulation/data/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)        0 2023-03-04 19:45:57.000000 UBC-Solar-Simulation-0.5.7/simulation/data/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.870868 UBC-Solar-Simulation-0.5.7/simulation/environment/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)    24478 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/environment/GIS.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)    15475 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/environment/SolarCalculations.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)    21792 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/environment/WeatherForecasts.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      183 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/environment/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.871337 UBC-Solar-Simulation-0.5.7/simulation/library/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       51 2023-04-08 18:23:00.000000 UBC-Solar-Simulation-0.5.7/simulation/library/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)    11207 2023-05-27 21:34:34.000000 UBC-Solar-Simulation-0.5.7/simulation/library/libraries.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.871905 UBC-Solar-Simulation-0.5.7/simulation/lvs/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       90 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/lvs/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      149 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/lvs/base_lvs.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      197 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/lvs/basic_lvs.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.872768 UBC-Solar-Simulation-0.5.7/simulation/main/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     1199 2023-06-03 18:30:10.000000 UBC-Solar-Simulation-0.5.7/simulation/main/ExecuteSimulation.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)    20161 2023-06-03 18:19:19.000000 UBC-Solar-Simulation-0.5.7/simulation/main/Simulation.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      571 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/main/SimulationResult.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      111 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/main/__init__.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.873253 UBC-Solar-Simulation-0.5.7/simulation/motor/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      102 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/motor/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      123 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/motor/base_motor.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     9597 2023-05-23 22:13:50.000000 UBC-Solar-Simulation-0.5.7/simulation/motor/basic_motor.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.874182 UBC-Solar-Simulation-0.5.7/simulation/optimization/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      199 2023-03-25 17:45:46.000000 UBC-Solar-Simulation-0.5.7/simulation/optimization/__init__.py
+-rwxr-xr-x   0 joshuariefman   (501) staff       (20)      396 2023-03-25 17:45:27.000000 UBC-Solar-Simulation-0.5.7/simulation/optimization/base_optimization.py
+-rwxr-xr-x   0 joshuariefman   (501) staff       (20)      755 2023-03-18 21:26:04.000000 UBC-Solar-Simulation-0.5.7/simulation/optimization/bayesian.py
+-rwxr-xr-x   0 joshuariefman   (501) staff       (20)      775 2023-03-25 17:45:46.000000 UBC-Solar-Simulation-0.5.7/simulation/optimization/random.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.874829 UBC-Solar-Simulation-0.5.7/simulation/regen/
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      102 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/regen/__init__.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      123 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/regen/base_regen.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)      237 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/regen/basic_regen.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)     9413 2023-06-03 18:19:19.000000 UBC-Solar-Simulation-0.5.7/simulation/run_simulation.py
+drwxr-xr-x   0 joshuariefman   (501) staff       (20)        0 2023-06-03 18:33:35.875269 UBC-Solar-Simulation-0.5.7/simulation/utils/
+-rwxr-xr-x   0 joshuariefman   (501) staff       (20)      827 2023-02-11 21:13:29.000000 UBC-Solar-Simulation-0.5.7/simulation/utils/InputBounds.py
+-rwxr-xr-x   0 joshuariefman   (501) staff       (20)     3856 2023-03-18 21:20:02.000000 UBC-Solar-Simulation-0.5.7/simulation/utils/MapPlot.py
+-rw-r--r--   0 joshuariefman   (501) staff       (20)       53 2023-03-04 19:45:57.000000 UBC-Solar-Simulation-0.5.7/simulation/utils/__init__.py
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/LICENSE` & `UBC-Solar-Simulation-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.6a0/PKG-INFO` & `UBC-Solar-Simulation-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UBC-Solar-Simulation
-Version: 0.5.6a0
+Version: 0.5.7
 Summary: UBC Solar's simulation environment
 Home-page: https://github.com/UBC-Solar/Simulation
 Author: Fisher Xue, Mihir Nimgade, Chris Chang, David Widjaja, Justin Hua, Ilya Veksler, Renu Rajamagmesh, Joshua Riefman, Ritchie Xia, Erik Langille, Chris Aung, Ishaan Trivedi, Jason Liang
 Author-email: software@ubcsolar.com
 License: MIT
 Keywords: car,simulation,solar
 Platform: UNKNOWN
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/README.md` & `UBC-Solar-Simulation-0.5.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -67,30 +67,45 @@
     ```python
     import simulation
 
     # creates a battery object
     battery = simulation.BasicBattery(0.90)
     ```
 
-### Run an example simulation
+### Run Simulation
 
-To run an example simulation, you can either run the main Python script directly from your IDE or you can run it from your terminal. 
+To run Simulation, you can either run the main Python script directly from your IDE or you can run it from your terminal. 
 The following instructions are for running it from your terminal.
 
-Before running the following commands make sure you have navigated to the "Simulation" folder on your terminal or the commands will not work. Please note support those in `examples/archive` has discontinued.
+Before running the following commands make sure you have navigated to the "Simulation" folder on your terminal or the commands will not work. Please note support those in `examples` and `examples/archive` has discontinued.
 
 #### Ubuntu/MacOS
 
 ```bash
-python3 examples/max_distance_from_speed_using_arrays.py
+python3 simulation/run_simulation.py
 ```
 #### Windows
 
 ```bash
-python .\examples\max_distance_from_speed_using_arrays.py
+python .\simulation\run_simulation.py
+```
+
+### Arguments
+
+You can view a list of valid arguments and settings that Simulation can accept with the `-help` command.
+
+#### Ubuntu/MacOS
+
+```bash
+python3 simulation/run_simulation.py -help
+```
+#### Windows
+
+```bash
+python .\simulation\run_simulation.py -help
 ```
 
 ### Testing
 
 To run the pre-written tests and ensure the simulation package is functioning correctly, navigate to the "Simulation" folder on your terminal, and run:
 
 ``` bash
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/UBC_Solar_Simulation.egg-info/PKG-INFO` & `UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UBC-Solar-Simulation
-Version: 0.5.6a0
+Version: 0.5.7
 Summary: UBC Solar's simulation environment
 Home-page: https://github.com/UBC-Solar/Simulation
 Author: Fisher Xue, Mihir Nimgade, Chris Chang, David Widjaja, Justin Hua, Ilya Veksler, Renu Rajamagmesh, Joshua Riefman, Ritchie Xia, Erik Langille, Chris Aung, Ishaan Trivedi, Jason Liang
 Author-email: software@ubcsolar.com
 License: MIT
 Keywords: car,simulation,solar
 Platform: UNKNOWN
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/UBC_Solar_Simulation.egg-info/SOURCES.txt` & `UBC-Solar-Simulation-0.5.7/UBC_Solar_Simulation.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 setup.py
 UBC_Solar_Simulation.egg-info/PKG-INFO
 UBC_Solar_Simulation.egg-info/SOURCES.txt
 UBC_Solar_Simulation.egg-info/dependency_links.txt
 UBC_Solar_Simulation.egg-info/requires.txt
 UBC_Solar_Simulation.egg-info/top_level.txt
 simulation/__init__.py
-simulation/array/__init__.py
-simulation/array/base_array.py
-simulation/array/basic_array.py
+simulation/run_simulation.py
+simulation/arrays/__init__.py
+simulation/arrays/base_array.py
+simulation/arrays/basic_array.py
 simulation/battery/__init__.py
 simulation/battery/base_battery.py
 simulation/battery/basic_battery.py
 simulation/cache/__init__.py
 simulation/cache/route/__init__.py
 simulation/cache/route/route_data.npz
 simulation/cache/route/route_data_FSGP.npz
@@ -22,34 +23,36 @@
 simulation/cache/weather/weather_data.npz
 simulation/common/__init__.py
 simulation/common/car.py
 simulation/common/constants.py
 simulation/common/consumer.py
 simulation/common/exceptions.py
 simulation/common/helpers.py
+simulation/common/plotting.py
 simulation/common/producer.py
+simulation/common/simulationState.py
 simulation/common/storage.py
+simulation/common/valuedProcess.py
 simulation/config/__init__.py
+simulation/config/initial_conditions.json
 simulation/config/settings_ASC.json
 simulation/config/settings_FSGP.json
 simulation/data/__init__.py
 simulation/environment/GIS.py
 simulation/environment/SolarCalculations.py
 simulation/environment/WeatherForecasts.py
 simulation/environment/__init__.py
-simulation/examples/__init__.py
-simulation/examples/fastest_time_given_distance.py
-simulation/examples/max_distance_from_speed_using_arrays.py
+simulation/library/__init__.py
+simulation/library/libraries.py
 simulation/lvs/__init__.py
 simulation/lvs/base_lvs.py
 simulation/lvs/basic_lvs.py
 simulation/main/ExecuteSimulation.py
-simulation/main/MainSimulation.py
+simulation/main/Simulation.py
 simulation/main/SimulationResult.py
-simulation/main/TimeSimulation.py
 simulation/main/__init__.py
 simulation/motor/__init__.py
 simulation/motor/base_motor.py
 simulation/motor/basic_motor.py
 simulation/optimization/__init__.py
 simulation/optimization/base_optimization.py
 simulation/optimization/bayesian.py
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/setup.py` & `UBC-Solar-Simulation-0.5.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,9 +31,9 @@
       author='Fisher Xue, Mihir Nimgade, Chris Chang, David Widjaja, Justin Hua, Ilya Veksler, Renu Rajamagmesh, Joshua Riefman, Ritchie Xia, Erik Langille, Chris Aung, Ishaan Trivedi, Jason Liang',
       url='https://github.com/UBC-Solar/Simulation',
       author_email='software@ubcsolar.com',
       keywords="car, simulation, solar",
       license="MIT",
       long_description=long_description,
       long_description_content_type='text/markdown',
-      version="0.5.6-alpha"
+      version="0.5.7"
       )
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/__init__.py` & `UBC-Solar-Simulation-0.5.7/simulation/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from simulation.common import Consumer
 from simulation.common import Producer
 from simulation.common import Storage
 from simulation.common import BatteryEmptyError
 
-from simulation.array import BaseArray
+from simulation.arrays import BaseArray
 from simulation.battery import BaseBattery
 from simulation.lvs import BaseLVS
 from simulation.motor import BaseMotor
 from simulation.regen import BaseRegen
 
-from simulation.array import BasicArray
+from simulation.arrays import BasicArray
 from simulation.battery import BasicBattery
 from simulation.lvs import BasicLVS
 from simulation.motor import BasicMotor
 from simulation.regen import BasicRegen
 
 from simulation.environment.GIS import GIS
 from simulation.environment.SolarCalculations import SolarCalculations
 from simulation.environment.WeatherForecasts import WeatherForecasts
 
+from simulation.library import Libraries
+
 from simulation.main import Simulation
 
-__version__ = "0.5.5-alpha"
+__version__ = "0.5.6"
 
 print(f"Package 'simulation' imported. Version: {__version__}\n")
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/array/basic_array.py` & `UBC-Solar-Simulation-0.5.7/simulation/arrays/basic_array.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from simulation.array.base_array import BaseArray
+import numpy as np
+from simulation.arrays.base_array import BaseArray
 
 
 class BasicArray(BaseArray):
 
     # incident_sunlight:
     def __init__(self):
         super().__init__()
@@ -15,53 +16,60 @@
 
         # please do not use this.
         self.solar_irradiance = 1200
 
     @staticmethod
     def calculate_produced_power(solar_irradiance, panel_efficiency, panel_size):
         """
-        returns the power produced by a solar panel in watts
+
+        Returns the power produced by a solar panel in Watts
 
         :param solar_irradiance: (float) a value for global horizontal irradiance (GHI)
             in W/m2
         :param panel_efficiency: (float) the efficiency of the solar cells as a number
             between 0 and 1, in atmosphere and with sunlight.
         :param panel_size: (float) the area of the solar panels in m2
         
         :returns: the power produced by a solar panel in W
+        :rtype: float
+
         """
 
         produced_power = solar_irradiance * panel_efficiency * panel_size
 
         return produced_power
 
     def update(self, tick):
         """
-        updates solar array model for a single tick
 
-        :param tick: (float) the length of time for the tick (in seconds)
+        Updates solar array model for a single tick
+
+        :param float tick: the length of time for the tick (in seconds)
 
         note: do not use this please. Use calculate_produced_energy instead.
         """
 
         # Assume constant sunlight in this simple model.
         self.produced_energy = self.calculate_produced_power(self.solar_irradiance,
                                                              self.panel_efficiency, self.panel_size) * tick
 
     def calculate_produced_energy(self, solar_irradiance, tick):
         """
-        returns a numpy array with the energy produced by the solar panels across
+
+        Returns a numpy array with the energy produced by the solar panels across
         each the length of each tick
 
-        :param solar_irradiance: (float[N]) the global horizontal irradiance(GHI) at
+        :param np.ndarray solar_irradiance: (float[N]) the global horizontal irradiance(GHI) at
             each moment experienced by the vehicle, in W/m2
-        :param tick: (float) the duration of a time step in seconds
+        :param float tick: (float) the duration of a time step in seconds
 
-        returns: (float[N]) array of energy produced by the solar panels on the vehicle
+        :returns: (float[N]) array of energy produced by the solar panels on the vehicle
             in Joules
+        :rtype: np.ndarray
+
         """
 
         return solar_irradiance * self.panel_efficiency * self.panel_size * tick
 
     def __str__(self):
         return(f"BasicArray: incident_sunlight: {self.solar_irradiance}W/m^2\n"
                f"BasicArray: panel_size: {self.panel_size}m^2\n"
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/battery/base_battery.py` & `UBC-Solar-Simulation-0.5.7/simulation/battery/base_battery.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/battery/basic_battery.py` & `UBC-Solar-Simulation-0.5.7/simulation/battery/basic_battery.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,17 +18,19 @@
         discharge_capacity (float): instantaneous amount of charge extracted from battery (Ah)
         voltage (float): instantaneous voltage of the battery (V)
         stored_energy (float): instantaneous energy stored in the battery (Wh)
     """
 
     def __init__(self, state_of_charge):
         """
+
         Constructor for BasicBattery class.
 
-        :param state_of_charge: initial battery state of charge
+        :param float state_of_charge: initial battery state of charge
+
         """
 
         # ----- DayBreak battery constants -----
 
         self.max_voltage = 117.6
         self.min_voltage = 75.6
         self.max_current_capacity = 48.9
@@ -63,59 +65,65 @@
         # ----- DayBreak battery initialisation -----
 
         super().__init__(self.stored_energy, self.max_current_capacity, self.max_energy_capacity,
                          self.max_voltage, self.min_voltage, self.voltage, self.state_of_charge)
 
     def update(self, tick):
         """
+
         Updates battery variables according to energy changes.
 
-        :param tick: time interval (in seconds) for battery variable update (dt)
+        :param float tick: time interval (in seconds) for battery variable update (dt)
+
         """
 
         energy_discharged = self.max_energy_capacity - self.stored_energy
 
         self.discharge_capacity = self.calculate_discharge_capacity_from_energy(energy_discharged)
         self.state_of_charge = self.calculate_soc_from_discharge_capacity(self.discharge_capacity)
         self.voltage = self.calculate_voltage_from_discharge_capacity(self.discharge_capacity)
 
     def charge(self, energy):
         """
+
         Adds energy to the battery.
 
-        :param energy: energy (in joules) to be added to battery.
+        :param float energy: energy (in joules) to be added to battery.
+
         """
 
         # divide by 3600 to convert from joules to watt-hours
         super().charge(energy / 3600)
 
     def discharge(self, energy):
         """
+
         Takes energy from the battery.
 
         :param energy: energy (in joules) to be taken from battery.
         
         :return discharged_energy: energy (in joules) removed from the battery.
+
         """
 
         return super().discharge(energy / 3600)
 
     def update_array(self, cumulative_energy_array):
         """
         Performs energy calculations with NumPy arrays
 
         :param cumulative_energy_array: a NumPy array containing the cumulative energy changes at each time step
         experienced by the battery
 
-        :return soc_array: a NumPy array containing the battery state of charge at each time step
+        :return: soc_array – a NumPy array containing the battery state of charge at each time step
+
+        :return: voltage_array – a NumPy array containing the voltage of the battery at each time step
 
-        :return voltage_array: a NumPy array containing the voltage of the battery at each time step
+        :return: stored_energy_array– a NumPy array containing the energy stored in the battery at each time step
 
-        :return stored_energy_array: a NumPy array containing the energy stored in the battery at each time step
-        step
         """
 
         stored_energy_array = np.full_like(cumulative_energy_array, fill_value=self.stored_energy)
         stored_energy_array += cumulative_energy_array / 3600
         stored_energy_array = np.clip(stored_energy_array, a_min=0, a_max=self.max_energy_capacity)
 
         energy_discharged_array = np.full_like(cumulative_energy_array, fill_value=self.max_energy_capacity) - \
@@ -123,7 +131,31 @@
 
         discharge_capacity_array = self.calculate_discharge_capacity_from_energy(energy_discharged_array)
 
         soc_array = self.calculate_soc_from_discharge_capacity(discharge_capacity_array)
         voltage_array = self.calculate_voltage_from_discharge_capacity(discharge_capacity_array)
 
         return soc_array, voltage_array, stored_energy_array
+
+    def get_raw_soc(self, cumulative_energy_array):
+        """
+
+        Return the not truncated (SOC is allowed to go above 100% and below 0%) state of charge.
+
+        :param np.ndarray cumulative_energy_array: a NumPy array containing the cumulative energy changes at each time step
+        experienced by the battery
+
+        :return: a NumPy array containing the battery state of charge at each time step
+        :rtype: np.ndarray
+
+        """
+
+        stored_energy_array = np.full_like(cumulative_energy_array, fill_value=self.stored_energy)
+        stored_energy_array += cumulative_energy_array / 3600
+
+        energy_discharged_array = np.full_like(cumulative_energy_array, fill_value=self.max_energy_capacity) - stored_energy_array
+
+        discharge_capacity_array = self.calculate_discharge_capacity_from_energy(energy_discharged_array)
+
+        soc_array = self.calculate_soc_from_discharge_capacity(discharge_capacity_array)
+
+        return soc_array
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/cache/route/route_data.npz` & `UBC-Solar-Simulation-0.5.7/simulation/cache/route/route_data.npz`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/cache/route/route_data_FSGP.npz` & `UBC-Solar-Simulation-0.5.7/simulation/cache/route/route_data_FSGP.npz`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/cache/weather/weather_data.npz` & `UBC-Solar-Simulation-0.5.7/simulation/cache/weather/weather_data.npz`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/common/car.py` & `UBC-Solar-Simulation-0.5.7/simulation/common/car.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-
+import numpy as np
 
 class Car(ABC):
     def __init__(self, array, battery, lvs, motor):
         self.array = array
         self.battery = battery
         self.lvs = lvs
         self.motor = motor
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/common/consumer.py` & `UBC-Solar-Simulation-0.5.7/simulation/common/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from abc import ABC, abstractmethod
 
 
 class Consumer(ABC):
     """
+
     The base consumer model
 
     :param consumed_energy: (float) the initial state for consumed energy
+
     """
 
     def __init__(self, consumed_energy):
         self.consumed_energy = consumed_energy
 
     @abstractmethod
     def update(self, tick):
         """
+
         updates model for a single tick
 
         :param tick: (float) the length of time for the tick (in seconds)
+
         """
         raise NotImplementedError
 
     def get_consumed_energy(self):
         return self.consumed_energy
 
     def set_consumed_energy(self, value):
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/common/helpers.py` & `UBC-Solar-Simulation-0.5.7/simulation/common/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-import array as arr
-import ctypes
 import datetime
 import functools
+import logging
+
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import time as timer
+
 from bokeh.layouts import gridplot
 from bokeh.models import HoverTool
-from bokeh.palettes import Bokeh8
 from bokeh.plotting import figure, show, output_file
-from math import radians
-from math import radians
 from matplotlib import pyplot as plt
 from simulation.common import constants
-from sklearn.neighbors import BallTree
-from sklearn.neighbors import BallTree
 
 """
 Description: contains the simulation's helper functions.
 """
 
 
 def timeit(func):
+    """
+
+    Apply this decorator to functions in order to time and print how long they take to execute.
+
+    :param func: function to be timed
+
+    """
+
     @functools.wraps(func)
     def wrapper_timer(*args, **kwargs):
         print(f">>> Running {func.__name__!r}... \n")
         start = timer.perf_counter()
         value = func(*args, **kwargs)
         stop = timer.perf_counter()
         run_time = stop - start
@@ -35,24 +39,38 @@
 
     return wrapper_timer
 
 
 def date_from_unix_timestamp(unix_timestamp):
     """
 
-    Args:
-        unix_timestamp: A unix timestamp
+    Return a stringified UTC datetime from UNIX timestamped.
+
+    :param int unix_timestamp: A unix timestamp
 
-    Returns: A string of the UTC representation of the UNIX timestamp in the format Y-m-d H:M:S
+    :returns: A string of the UTC representation of the UNIX timestamp in the format Y-m-d H:M:S
+    :rtype: str
 
     """
+
     return datetime.datetime.utcfromtimestamp(unix_timestamp).strftime('%Y-%m-%d %H:%M:%S')
 
 
 def check_for_non_consecutive_zeros(array, verbose=False):
+    """
+
+    Checks if an array has non-consecutive zeroes as elements.
+
+    :param np.ndarray array: array to be examined
+    :param bool verbose: whether method should be verbose
+    :return: whether the array has non-consecutive zeroes
+    :rtype: bool
+
+    """
+
     zeroed_indices = np.where(array == 0)[0]
 
     if len(zeroed_indices) == 0:
         if verbose:
             print("No zeroes found in the array!")
         return -1
 
@@ -65,54 +83,81 @@
     else:
         if verbose:
             print("Non-consecutive zeroes found!")
         return True
 
 
 def reshape_and_repeat(input_array, reshape_length):
+    """
+
+    Reshape and repeat an input array to have a certain length while maintaining its elements.
+    Examples:
+        If you want a constant speed for the entire simulation, insert a single element
+        into the input_speed array.
+
+            input_speed = np.array([30]) <-- constant speed of 30km/h
+
+        If you want 50km/h in the first half of the simulation and 60km/h in the second half,
+        do the following:
+
+            input_speed = np.array([50, 60])
+
+        This logic will apply for all subsequent array lengths (3, 4, 5, etc.)
+    Keep in mind, however, that the condition len(input_array) <= reshape_length must be true
+
+    :param np.ndarray input_array: array to be modified
+    :param float reshape_length: length for input array to be modified to
+    :return: modified array
+    :rtype: np.ndarray
+
+    """
+
     if input_array.size >= reshape_length:
-        print(f"Input array of shape {input_array.shape} was not reshaped\n")
         return input_array
     else:
         quotient_remainder_tuple = divmod(reshape_length, input_array.size)
         temp = np.repeat(input_array, quotient_remainder_tuple[0])
         result = np.append(temp, np.repeat(
             temp[-1], quotient_remainder_tuple[1]))
 
-        print(
-            f"Reshaped input array from {input_array.shape} to {result.shape}\n")
         return result
 
 
 def generate_deceleration_array(initial_velocity, final_velocity, deceleration_interval):
     """
+
     Create an array where each element represents a step in the deceleration from initial_velocity to final_velocity.
 
-    :param initial_velocity: the velocity at which deceleration occurs for the first time (km/h)
-    :param final_velocity: the target velocity that is being decelerated to (km/h)
-    :param deceleration_interval: the time it will take to decelerate from initial velocity to final velocity (s)
+    :param float initial_velocity: the velocity at which deceleration occurs for the first time (km/h)
+    :param float final_velocity: the target velocity that is being decelerated to (km/h)
+    :param int deceleration_interval: the time it will take to decelerate from initial velocity to final velocity (s)
     :return: an array of the velocities between initial_velocity and final_velocity
+    :rtype: np.ndarray
+
     """
 
-    deceleration_instance_size = (
-        final_velocity - initial_velocity) / (deceleration_interval + 1)
-    return np.arange(initial_velocity, final_velocity, deceleration_instance_size)[1:(deceleration_interval+1)]
+    deceleration_instance_size = (final_velocity - initial_velocity) / (deceleration_interval + 1)
+    return np.arange(initial_velocity, final_velocity, deceleration_instance_size)[1:(deceleration_interval + 1)]
 
 
 def apply_deceleration(input_speed_array, deceleration_interval):
     """
+
     Replace instances of instant deceleration in a velocity array with uniform changes in velocity that are spread
     over the deceleration_interval.
 
     The distance travelled by the simulation will be reduced by a negligible amount.
 
-    :param input_speed_array: the velocity array (km/h)
-    :param deceleration_interval: the duration of the deceleration intervals (s)
+    :param np.ndarray input_speed_array: the velocity array (km/h)
+    :param int deceleration_interval: the duration of the deceleration intervals (s)
     :return: a speed array with uniform deceleration (km/h)
+    :rtype: np.ndarray
+
     """
+
     if input_speed_array is None:
         return np.array([])
     if deceleration_interval <= 0:
         return input_speed_array
 
     input_speed_array = input_speed_array.astype(float)
     # Prepending 0 to align acceleration_instances
@@ -132,61 +177,80 @@
             input_speed_array[idx -
                               deceleration_interval:idx] = deceleration_array
     return input_speed_array
 
 
 def is_valid_speed_array(deceleration_interval, idx, initial_velocity, input_speed_array):
     """
+
     Check that the specified speed array is valid in relation to the chosen deceleration interval.
 
-    :param deceleration_interval: the duration of the deceleration intervals (s)
-    :param idx: the index used to check our deceleration interval
-    :param initial_velocity: the velocity at the beginning of the deceleration period
-    :param input_speed_array: the speed array
+    :param int deceleration_interval: the duration of the deceleration intervals (s)
+    :param int idx: the index used to check our deceleration interval
+    :param float initial_velocity: the velocity at the beginning of the deceleration period
+    :param np.ndarray input_speed_array: the speed array
     :return: True if the array is valid, False if it is not
+    :rtype: bool
+
     """
     if deceleration_interval > len(input_speed_array) - 1:  # Check that the speed array isn't smaller than the
         # deceleration interval
         return False
 
     # Check that the speed is constant over the deceleration interval
     for i in range(0, deceleration_interval):
         if initial_velocity != input_speed_array[idx - i - 1]:
             return False
     return True
 
 
 def hour_from_unix_timestamp(unix_timestamp):
+    """
+
+    Return the hour of a UNIX timestamp.
+
+    :param float unix_timestamp: a UNIX timestamp
+    :return: hour of UTC datetime from unix timestamp
+    :rtype: int
+
+    """
+
     val = datetime.datetime.utcfromtimestamp(unix_timestamp)
     return val.hour
 
 
 def adjust_timestamps_to_local_times(timestamps, starting_drive_time, time_zones):
     """
+
     Takes in the timestamps of the vehicle's driving duration, starting drive time, and a list of time zones,
-        returns the local times at each point
+    returns the local times at each point
+
+    :param np.ndarray timestamps: (int[N]) timestamps starting from 0, in seconds
+    :param float starting_drive_time: (int[N]) local time that the car was start to be driven in UNIX time (Daylight Saving included)
+    :param np.ndarray time_zones: (int[N])
+    :returns: array of local times at each point
+    :rtype: np.ndarray
 
-    :param timestamps: (int[N]) timestamps starting from 0, in seconds
-    :param starting_drive_time: (int[N]) local time that the car was start to be driven in UNIX time (Daylight Saving included)
-    :param time_zones: (int[N])
     """
 
     return np.array(timestamps + starting_drive_time - (time_zones[0] - time_zones), dtype=np.uint64)
 
 
 def calculate_path_distances(coords):
     """
+
     The coordinates are spaced quite tightly together, and they capture the
     features of the road. So, the lines between every pair of adjacent
     coordinates can be treated like a straight line, and the distances can
     thus be obtained.
 
-    :param coords: A NumPy array [n][latitude, longitude]
-
+    :param np.ndarray coords: A NumPy array [n][latitude, longitude]
     :returns path_distances: a NumPy array [n-1][distances],
+    :rtype: np.ndarray
+
     """
 
     offset = np.roll(coords, (1, 1))
 
     # get the latitude and longitude differences, in radians
     diff = (coords - offset)[1:] * np.pi / 180
     diff_lat, diff_lng = np.split(diff, 2, axis=1)
@@ -208,141 +272,157 @@
     path_distances = constants.EARTH_RADIUS * np.sqrt(square_sum)
 
     return path_distances
 
 
 def get_array_directional_wind_speed(vehicle_bearings, wind_speeds, wind_directions):
     """
+
     Returns the array of wind speed in m/s, in the direction opposite to the
         bearing of the vehicle
 
-    vehicle_bearings: (float[N]) The azimuth angles that the vehicle in, in degrees
-    wind_speeds: (float[N]) The absolute speeds in m/s
-    wind_directions: (float[N]) The wind direction in the meteorlogical convention. To convert from
-        meteorlogical convention to azimuth angle, use (x + 180) % 360
+    :param np.ndarray vehicle_bearings: (float[N]) The azimuth angles that the vehicle in, in degrees
+    :param np.ndarray wind_speeds: (float[N]) The absolute speeds in m/s
+    :param np.ndarray wind_directions: (float[N]) The wind direction in the meteorlogical convention. To convert from meteorological convention to azimuth angle, use (x + 180) % 360
+    :returns: The wind speeds in the direction opposite to the bearing of the vehicle
+    :rtype: np.ndarray
 
-    Returns: The wind speeds in the direction opposite to the bearing of the vehicle
     """
 
     # wind direction is 90 degrees meteorlogical, so it is 270 degrees azimuthal. car is 90 degrees
     #   cos(90 - 90) = cos(0) = 1. Wind speed is moving opposite to the car,
     # car is 270 degrees, cos(90-270) = -1. Wind speed is in direction of the car.
     return wind_speeds * (np.cos(np.radians(wind_directions - vehicle_bearings)))
 
+
 def get_day_of_year_map(date):
     """
+
     Extracts day, month, year, from datetime object
+
+    :param datetime.date date: date to be decomposed
+
     """
     return get_day_of_year(date.day, date.month, date.year)
 
+
 def get_day_of_year(day, month, year):
     """
-        Calculates the day of the year, given the day, month and year.
 
-        day, month, year: self explanatory
+    Calculates the day of the year, given the day, month and year.
+    Day refers to a number representing the nth day of the year. So, Jan 1st will be the 1st day of the year
 
-        Day refers to a number representing the n'th day of the year. So, Jan 1st will be the 1st day of the year
-        """
+    :param int day: nth day of the year
+    :param int month: month
+    :param int year: year
+    :returns: day of year
+    :rtype: int
 
-    return (datetime.date(year, month, day) -
-            datetime.date(year, 1, 1)).days + 1
+    """
+
+    return (datetime.date(year, month, day) - datetime.date(year, 1, 1)).days + 1
 
 
 def calculate_declination_angle(day_of_year):
     """
+
     Calculates the Declination Angle of the Earth at a given day
     https://www.pveducation.org/pvcdrom/properties-of-sunlight/declination-angle
 
-    day_of_year: The number of the day of the current year, with January 1
-        being the first day of the year.
+    :param np.ndarray day_of_year: The number of the day of the current year, with January 1 being the first day of the year.
+    :returns: The declination angle of the Earth relative to the Sun, in degrees
+    :rtype: np.ndarray
 
-    Returns: The declination angle of the Earth relative to the Sun, in
-        degrees
     """
 
     declination_angle = -23.45 * np.cos(np.radians((np.float_(360) / 365) *
                                                    (day_of_year + 10)))
 
     return declination_angle
 
 
 # ----- Calculation of Apparent Solar Time -----
 
 def calculate_eot_correction(day_of_year):
     """
+
     Approximates and returns the correction factor between the apparent
     solar time and the mean solar time
 
-    day_of_year: The number of the day of the current year, with January 1
-        being the first day of the year.
+    :param np.ndarray day_of_year: The number of the day of the current year, with January 1 being the first day of the year.
+    :returns: The Equation of Time correction EoT in minutes, where apparent Solar Time = Mean Solar Time + EoT
+    :rtype: np.ndarray
 
-    Returns: The Equation of Time correction EoT in minutes, where
-        Apparent Solar Time = Mean Solar Time + EoT
     """
 
     b = np.radians((np.float_(360) / 364) * (day_of_year - 81))
 
     eot = 9.87 * np.sin(2 * b) - 7.83 * np.cos(b) - 1.5 * np.sin(b)
 
     return eot
 
 
 def calculate_LSTM(time_zone_utc):
     """
+
     Calculates and returns the LSTM, or Local Solar Time Meridian.
     https://www.pveducation.org/pvcdrom/properties-of-sunlight/solar-time
 
-    time_zone_utc: The UTC time zone of your area in hours of UTC offset.
+    :param np.ndarray time_zone_utc: The UTC time zone of your area in hours of UTC offset.
+    :returns: The Local Solar Time Meridian in degrees
+    :rtype: np.ndarray
 
-    Returns: The Local Solar Time Meridian in degrees
     """
 
     return 15 * time_zone_utc
 
 
 def local_time_to_apparent_solar_time(time_zone_utc, day_of_year, local_time,
                                       longitude):
     """
+
     Converts between the local time to the apparent solar time and returns the apparent
     solar time.
     https://www.pveducation.org/pvcdrom/properties-of-sunlight/solar-time
 
-    time_zone_utc: The UTC time zone of your area in hours of UTC offset.
-    day_of_year: The number of the day of the current year, with January 1
-        being the first day of the year.
-    local_time: The local time in hours from midnight (Adjust for Daylight Savings)
-    longitude: The longitude of a location on Earth
+    Note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the
+        calculation will end up just the same
 
-    note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the
-            calculation will end up just the same
+    :param np.ndarray time_zone_utc: The UTC time zone of your area in hours of UTC offset.
+    :param np.ndarray day_of_year: The number of the day of the current year, with January 1 being the first day of the year.
+    :param np.ndarray local_time: The local time in hours from midnight (Adjust for Daylight Savings)
+    :param np.ndarray longitude: The longitude of a location on Earth
+    :returns: The Apparent Solar Time of a location, in hours from midnight
+    :rtype: np.ndarray
 
-    Returns: The Apparent Solar Time of a location, in hours from midnight
     """
 
     lstm = calculate_LSTM(time_zone_utc)
     eot = calculate_eot_correction(day_of_year)
 
     # local solar time
     lst = local_time + np.float_(longitude - lstm) / 15 + np.float_(eot) / 60
 
     return lst
 
 
 def calculate_path_gradients(elevations, distances):
     """
-    Get the approximate gradients of every point on the path.
 
-    :param elevations: [N][elevations]
-    :param distances: [N-1][distances]
-
-    :returns gradients: [N-1][gradients]
+    Get the approximate gradients of every point on the path.
 
     Note:
         - gradient > 0 corresponds to uphill
         - gradient < 0 corresponds to downhill
+
+    :param np.ndarray elevations: [N][elevations]
+    :param np.ndarray distances: [N-1][distances]
+    :returns gradients: [N-1][gradients]
+    :rtype: np.ndarray
+
     """
 
     # subtract every next elevation with the previous elevation to
     # get the difference in elevation
     # [1 2 3 4 5]
     # [5 1 2 3 4] -
     # -------------
@@ -356,65 +436,75 @@
     # gradient < 0: downhill
 
     gradients = delta_elevations / distances
 
     return gradients
 
 
-def cull_dataset(coords):
+def cull_dataset(coords, cull_factor=625):  # DEPRECATED
     """
+
     As we currently have a limited number of API calls(60) every minute with the
         current Weather API, we must shrink the dataset significantly. As the
         OpenWeatherAPI models have a resolution of between 2.5 - 70 km, we will
         go for a resolution of 25km. Assuming we travel at 100km/h for 12 hours,
         1200 kilometres/25 = 48 API calls
 
     As the Google Maps API has a resolution of around 40m between points,
         we must cull at 625:1 (because 25,000m / 40m = 625)
-    """
 
-    return coords[::625]
+    :param int cull_factor: factor in which the input array should be culled, default is 625.
+    :param np.ndarray coords: array to be culled
+    :returns: culled array
+    :rtype: np.ndarray
+
+    """
+    logging.warning("Using deprecated function 'cull_dataset()'!")
+    return coords[::cull_factor]
 
 
 def compute_elevation_angle_math(declination_angle, hour_angle, latitude):
     """
+
     Gets the two terms to calculate and return elevation angle, given the
     declination angle, hour angle, and latitude.
 
     This method separates the math part of the calculation from its caller
     method to optimize for numba compilation.
 
-    declination_angle: The declination angle of the Earth relative to the Sun
-    hour_angle: The hour angle of the sun in the sky
+    :param np.ndarray latitude: array of latitudes
+    :param np.ndarray declination_angle: The declination angle of the Earth relative to the Sun
+    :param np.ndarray hour_angle: The hour angle of the sun in the sky
+    :returns: The elevation angle in degrees
+    :rtype: np.ndarray
 
-    Returns: The elevation angle in degrees
     """
-    term_1 = np.sin(np.radians(declination_angle)) * \
-        np.sin(np.radians(latitude))
-
-    term_2 = np.cos(np.radians(declination_angle)) * \
-        np.cos(np.radians(latitude)) * \
-        np.cos(np.radians(hour_angle))
 
+    term_1 = np.sin(np.radians(declination_angle)) * np.sin(np.radians(latitude))
+    term_2 = np.cos(np.radians(declination_angle)) * np.cos(np.radians(latitude)) * np.cos(np.radians(hour_angle))
     elevation_angle = np.arcsin(term_1 + term_2)
+
     return np.degrees(elevation_angle)
 
 
 def find_runs(x):
     """
+
     Method to identify runs of consecutive items in NumPy array
     Based on code from: user alimanfoo on https://gist.github.com/alimanfoo/c5977e87111abe8127453b21204c1065
 
     :returns a tuple of 3 NumPy arrays for (run_values, run_starts, run_lengths)
-    Args:
-        x: a 1D NumPy array3
-    Throws: ValueError if array dimension is greater than 1
+    :param x: a 1D NumPy array3
+    :raises: ValueError if array dimension is greater than 1
+
+    :returns: a tuple of 3 NumPy arrays for (run_values, run_starts, run_lengths)
+    :rtype: tuple
 
-    Returns: a tuple of 3 NumPy arrays for (run_values, run_starts, run_lengths)
     """
+
     x = np.asanyarray(x)
     if x.ndim != 1:
         raise ValueError('only 1D array supported')
     n = x.shape[0]
 
     # handle empty array
     if n == 0:
@@ -446,26 +536,25 @@
 
     return multi_index_run_values, multi_index_run_starts, multi_index_run_lengths
 
 
 def apply_race_timing_constraints(speed_kmh, start_hour, simulation_duration, race_type, timestamps, verbose):
     """
 
-    Args:
-        speed_kmh: A NumPy array representing the speed at each timestamp in km/h
-        start_hour: An integer representing the race's start hour
-        simulation_duration: An integer representing simulation duration in seconds
-        race_type: A string describing the race type. Must be one of "ASC" or "FSGP"
-        timestamps: A NumPy array representing the timestamps for the simulated race
-        verbose: A flag to show speed array modifications for debugging purposes
-
-    Returns: constrained_speed_kmh, a speed array with race timing constraints applied to it, not_charge,
-    a boolean array representing when the car can charge and when it cannot (1 = charge, 0 = not_charge)
+    Applies regulation timing constraints to a speed array.
 
-    Raises: ValueError is race_type is not one of "ASC" or "FSGP"
+    :param np.ndarray speed_kmh: A NumPy array representing the speed at each timestamp in km/h
+    :param int start_hour: An integer representing the race's start hour
+    :param int simulation_duration: An integer representing simulation duration in seconds
+    :param str race_type: A string describing the race type. Must be one of "ASC" or "FSGP"
+    :param np.ndarray timestamps: A NumPy array representing the timestamps for the simulated race
+    :param bool verbose: A flag to show speed array modifications for debugging purposes
+    :returns: constrained_speed_kmh, a speed array with race timing constraints applied to it, not_charge, a boolean array representing when the car can charge and when it cannot (1 = charge, 0 = not_charge)
+    :rtype: np.ndarray
+    :raises: ValueError is race_type is not one of "ASC" or "FSGP"
 
     """
 
     # (Charge from 7am-9am and 6pm-8pm) for ASC - 13 Hours of Race Day, 9 Hours of Driving
     # (Charge from 8am-9am and 6pm-8pm) for FSGP
 
     simulation_hours = np.arange(
@@ -494,35 +583,35 @@
 
     return constrained_speed_kmh, not_charge
 
 
 def plot_graph(timestamps, arrays_to_plot, array_labels, graph_title, save=True):
     """
 
-        This is a utility function to plot out any set of NumPy arrays you pass into it using the Bokeh library.
-        The precondition of this function is that the length of arrays_to_plot and array_labels are equal.
+    This is a utility function to plot out any set of NumPy arrays you pass into it using the Bokeh library.
+    The precondition of this function is that the length of arrays_to_plot and array_labels are equal.
 
-        This is because there be a 1:1 mapping of each entry of arrays_to_plot to array_labels such that:
-            arrays_to_plot[n] has label array_labels[n]
+    This is because there be a 1:1 mapping of each entry of arrays_to_plot to array_labels such that:
+        arrays_to_plot[n] has label array_labels[n]
 
-        Another precondition of this function is that each of the arrays within arrays_to_plot also have the
-        same length. This is each of them will share the same time axis.
+    Result:
+        Produces a 3 x ceil(len(arrays_to_plot) / 3) plot
+        If save is enabled, save html file
+
+    Another precondition of this function is that each of the arrays within arrays_to_plot also have the
+    same length. This is each of them will share the same time axis.
+
+    :param np.ndarray timestamps: An array of timestamps for the race
+    :param list arrays_to_plot: An array of NumPy arrays to plot
+    :param list array_labels: An array of strings for the individual plot titles
+    :param str graph_title: A string that serves as the plot's main title
+    :param bool save: Boolean flag to control whether to save an .html file
 
-        Args:
-            timestamps: An array of timestamps for the race
-            arrays_to_plot: An array of NumPy arrays to plot
-            array_labels: An array of strings for the individual plot titles
-            graph_title: A string that serves as the plot's main title
-            save: Boolean flag to contorl whether to save an .html file
-
-        Result:
-            Produces a 3 x ceil(len(arrays_to_plot) / 3) plot
-            If save is enabled, save html file
+    """
 
-        """
     compress_constant = int(timestamps.shape[0] / 5000)
 
     for index, array in enumerate(arrays_to_plot):
         arrays_to_plot[index] = array[::compress_constant]
 
     figures = list()
 
@@ -534,16 +623,20 @@
     ]
 
     for (index, data_array) in enumerate(arrays_to_plot):
         # create figures and put them in list
         figures.append(figure(title=array_labels[index], x_axis_label="Time (hr)",
                               y_axis_label=array_labels[index], x_axis_type="datetime"))
 
-        # add line renderers to each figure
-        colours = ('#EC1557', '#F05223', '#F6A91B', '#A5CD39', '#20B254', '#00AAAE', '#4998D3', '#892889', '#fa1b9a')
+        # add line renderers to each figur
+        colours = (
+            '#EC1557', '#F05223', '#F6A91B', '#A5CD39', '#20B254', '#00AAAE', '#4998D3', '#892889', '#fa1b9a',
+            '#F05223', '#EC1557', '#F05223', '#F6A91B', '#A5CD39', '#20B254', '#00AAAE', '#4998D3', '#892889',
+            '#fa1b9a', '#F05223', '#EC1557', '#F05223', '#F6A91B', '#A5CD39', '#20B254', '#00AAAE', '#4998D3',
+            '#892889', '#fa1b9a', '#F05223', '#EC1557', '#F05223', '#F6A91B', '#A5CD39', '#EC1557', '#F05223')
         figures[index].line(timestamps[::compress_constant] * 1000, data_array, line_color=colours[index],
                             line_width=2)
 
         figures[index].add_tools(hover_tool)
 
     grid = gridplot(figures, sizing_mode="scale_both",
                     ncols=3, plot_height=200, plot_width=300)
@@ -554,34 +647,36 @@
     show(grid)
 
     return
 
 
 def route_visualization(coords, visible=True):
     """
-    Takes in a list of coordinates and visualizes them using MapBox.
 
-    :Param coords: A NumPy array [n][latitude, longitude]
+    Takes in a list of coordinates and visualizes them using MapBox.
     Outputs a window that visualizes the route with given coordinates
+
+    :param np.ndarray coords: A NumPy array [n][latitude, longitude]
+
     """
 
     point_labels = [f"Point {str(i)}" for i in range(len(coords))]
     colours = [0 for _ in coords]
     sizes = [6 for _ in coords]
     latitudes = [c[0] for c in coords]
     longitudes = [c[1] for c in coords]
 
     zipped_data = list(zip(point_labels, latitudes,
-                       longitudes, colours, sizes))
+                           longitudes, colours, sizes))
 
     colour_hex = "#002145"
     solid_color_hex_continuous_scale = [colour_hex, colour_hex]
 
     dataframe = pd.DataFrame(zipped_data, columns=[
-                             "Point", "Latitude", "Longitude", "Colour", "Size"])
+        "Point", "Latitude", "Longitude", "Colour", "Size"])
 
     fig = px.scatter_mapbox(dataframe, lat="Latitude", lon="Longitude", color="Colour",
                             hover_name=point_labels, color_continuous_scale=solid_color_hex_continuous_scale,
                             size="Size", size_max=6, zoom=3, height=800)
 
     fig.update_layout(mapbox_style="stamen-terrain", mapbox_zoom=5, mapbox_center_lat=41,
                       margin={"r": 0, "t": 0, "l": 0, "b": 0})
@@ -589,50 +684,50 @@
     if visible:
         fig.show()
 
 
 def simple_plot_graph(data, title, visible=True):
     """
 
-    Args:
-        visible: A control flag specifying if the plot should be shown
-        data: A NumPy[n] array of data to plot
-        title: The graph title
+    Displays a graph of the data using Matplotlib
 
-    Result: Displays a graph of the data using Matplotlib
+    :param bool visible: A control flag specifying if the plot should be shown
+    :param np.ndarray data: A NumPy[n] array of data to plot
+    :param str title: The graph title
 
     """
     fig, ax = plt.subplots()
     x = np.arange(0, len(data))
     ax.plot(x, data)
     plt.title(title)
     if visible:
         plt.show()
 
 
 def calculate_race_completion_time(path_length, cumulative_distances):
     """
+
     This function uses the maximum path distance and cumulative distances travelled
     during the simulation to identify how long the car takes to finish travelling the route.
 
     This problem, although framed in the context of the Simulation, is just to find the array position of the first
     value that is greater or equal to a target value
 
-    Args:
-        path_length: The length of the path the vehicle travels on
-        cumulative_distances: A NumPy array representing the cumulative distanced travelled by the vehicle
+    :param float path_length: The length of the path the vehicle travels on
+    :param np.ndarray cumulative_distances: A NumPy array representing the cumulative distanced travelled by the vehicle
 
     Pre-Conditions:
         path_length and cumulative_distances may be in any length unit, but they must share the same length unit
         Each index of the cumulative_distances array represents one second of the simulation
 
-    Returns: The number of seconds the vehicle requires to travel the full path length.
-    If vehicle does not travel the full path length, returns 
+    :returns: The number of seconds the vehicle requires to travel the full path length. If vehicle does not travel the full path length, returns
+    :rtype: int
 
     """
+
     # Create a boolean array to encode whether the vehicle has completed or not completed the route at a given timestamp
     # This is based on the assumption that each index represents a single timestamp of one second
     crossed_finish_line = np.where(cumulative_distances >= path_length, 1, 0)
 
     # Based on the boolean encoding, identify the first index which the vehicle has completed the route
     completion_index = np.where(crossed_finish_line == 1)
 
@@ -640,147 +735,35 @@
         return completion_index[0][0]
     else:
         return len(cumulative_distances) + 1
 
 
 def plot_longitudes(coordinates):
     """
+
     Plots the longitudes of a set of coordinates. Meant to support Simulation development and verification of route data.
-    Args:
-        coordinates: A NumPy array (float[N][longitude, latitude]) representing a path of coordinates
 
-    Returns: Nothing, but plots the longitudes
+    :param np.ndarray coordinates: A NumPy array (float[N][longitude, latitude]) representing a path of coordinates
+    :returns: Nothing, but plots the longitudes
 
     """
     simple_plot_graph(coordinates[:, 0], "Longitudes")
 
 
 def plot_latitudes(coordinates):
     """
-    Plots the latitudes of a set of coordinates. Meant to support Simulation development and verification of route data.
-    Args:
-        coordinates: A NumPy array (float[N][longitude, latitude]) representing a path of coordinates
-
-    Returns: Nothing, but plots the latitudes
-
-    """
-    simple_plot_graph(coordinates[:, 1], "Latitudes")
-
-
-def generate_golang_io_pointers(input_array):
-    """
-    Generates I/O pointers for use in calling Golang functions using NumPy arrays as arguments
 
-    Args:
-        input_array: A Python list 0r NumPy Array that will serve as an input to a Golang function
+    Plots the latitudes of a set of coordinates. Meant to support Simulation development and verification of route data.
 
-    Returns:
-        - input_array_pointer: A pointer to input_array
-        - output_array_pointer: A pointer to the output_array return value
-        - output_array: The array that output_array_pointer points to.
-                        Will contain result if GoLang writes memory location specified by output_array_pointer
+    :param np.ndarray coordinates: A NumPy array (float[N][longitude, latitude]) representing a path of coordinates
+    :returns: Nothing, but plots the latitudes
 
     """
-    input_array_copy = arr.array('d', input_array)
-    input_array_pointer = (
-        ctypes.c_double * len(input_array_copy)).from_buffer(input_array_copy)
-
-    output_array = arr.array('d', [0] * len(input_array))
-    output_array_pointer = (
-        ctypes.c_double * len(output_array)).from_buffer(output_array)
-
-    return input_array_pointer, output_array_pointer, output_array
 
-
-def speeds_with_waypoints(path, distances, speeds, waypoints, verbose=False):
-    # First we need to find the closest path coordinates for each waypoint/checkpoint
-    path_rad = np.array([[radians(p[0]), radians(p[1])] for p in path])
-    tree = BallTree(path_rad, metric='haversine')
-    _, wp = tree.query([[radians(w[0]), radians(w[1])] for w in waypoints])
-    if verbose:
-        print(f"Waypoint indices in path array:\n{wp}\n")
-
-    delta = 0.05  # margin of error with double arithmetic
-    path_index = 0  # current path coordinate
-    # stores the interim distance travelled between two path coordinates
-    temp_distance_travelled = 0
-
-    # iterate through the speeds array for each second
-    i = 0
-    while i < len(speeds):
-        distance = speeds[i]
-
-        """
-        For each second, we will:
-            1) keep travelling past path coordinates until:
-                i) we don't have enough speed to reach the next path coordinate
-                ii) we reach a waypoint
-                    - replace the next 45 minutes of speeds with 0
-            2) come to a "fractional coordinate" that exists between 2 path coordinates
-                - add the temporary distance travelled between two path coordinates to a temp variable
-        """
-
-        total_distance_travelled = 0  # total distance travelled this second
-        waypoint_flag = 0  # flag used to indicate if we reached a waypoint
-
-        # if we can reach the next path coordinate
-        while distance + temp_distance_travelled > distances[path_index] - delta:
-            # update distance to be remainder of distance we can travel this second
-            distance = distance + temp_distance_travelled - \
-                distances[path_index]
-            # add the distance travelled to our total distance travelled this second
-            total_distance_travelled += distances[path_index] - \
-                temp_distance_travelled
-            # reset the temp_distance_travelled since we just reached a new path coordinate
-            temp_distance_travelled = 0
-            # increment values of path_index
-            path_index += 1
-
-            # If we reached the end of the coordinate list, exit
-            if path_index >= len(distances):
-                if verbose:
-                    print(f"Travelled {total_distance_travelled} m at second {i}\n"
-                          f"New coordinates: {path[path_index]}\n"
-                          "Race complete!\n")
-                return np.multiply(speeds, 3.6)
-
-            # If we have reached a waypoint/checkpoint, replace speeds with 0
-            if wp.size > 0 and path_index == wp[0]:
-                if verbose:
-                    print(
-                        f"Travelled {total_distance_travelled} m at second {i}\n" f"New coordinates: {path[path_index]}\n" "Reached a waypoint!\n")
-                # delete the waypoint we just reached from the wp array
-                wp = np.delete(wp, 0)
-                # update the current speed to be only what we travelled this second
-                speeds[i] = total_distance_travelled
-                # replace the speeds with 0's
-                speeds[i + 1: i + 1 + 45 * 60] = [0] * 45 * 60
-                i += 45 * 60 - 1
-                distance = 0  # shouldn't travel anymore in this second
-                waypoint_flag = 1
-                break
-
-            if waypoint_flag:
-                continue
-
-        # If I still have distance to travel but can't reach the next coordinate
-        if distance + temp_distance_travelled < distances[path_index] - delta:
-            # Update total distance travelled
-            total_distance_travelled += distance
-
-            # Add onto the temporary distance between two coordinates
-            temp_distance_travelled += distance
-
-            if verbose:
-                print(
-                    f"Travelled {total_distance_travelled} m at second {i}\n" f"Reached fractional coordinate.\n")
-
-        i += 1
-
-    return np.multiply(speeds, 3.6)
+    simple_plot_graph(coordinates[:, 1], "Latitudes")
 
 
 if __name__ == '__main__':
     # speed_array input
     speed_array = np.array([45, 87, 65, 89, 43, 54, 45, 23, 34, 20])
 
     expanded_speed_array = reshape_and_repeat(speed_array, 9 * 3600)
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/common/storage.py` & `UBC-Solar-Simulation-0.5.7/simulation/common/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from abc import ABC, abstractmethod
 
 
 class Storage(ABC):
     """
+
     The base storage model
 
-    :param stored_energy: (float) amount of energy stored in the storage module
+    :param float stored_energy: amount of energy stored in the storage module
+
     """
 
     def __init__(self, stored_energy=0):
         self.stored_energy = stored_energy
 
     @abstractmethod
     def update(self, tick):
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/config/settings_FSGP.json` & `UBC-Solar-Simulation-0.5.7/simulation/config/settings_FSGP.json`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/environment/SolarCalculations.py` & `UBC-Solar-Simulation-0.5.7/simulation/environment/SolarCalculations.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,83 @@
 #!/usr/bin/env python
 
-
 """
 A class to perform calculation and approximations for obtaining quantities
     such as solar time, solar position, and the various types of solar irradiance.
 """
 
 import datetime
 import numpy as np
-import sys
+
 from simulation.common import helpers
-from tqdm import tqdm
 
 
 class SolarCalculations:
 
-    def __init__(self):
+    def __init__(self, golang=True, library=None):
         """
+
         Initializes the instance of a SolarCalculations class
+
+        :param golang: Boolean that determines whether GoLang implementations will be used when applicable.
+        :param library: GoLang binaries library
+
         """
 
         # Solar Constant in W/m2
         self.S_0 = 1353
 
+        self.golang = golang
+        self.lib = library
+
     # ----- Calculation of solar position in the sky -----
 
     @staticmethod
     def calculate_hour_angle(time_zone_utc, day_of_year, local_time, longitude):
         """
+
         Calculates and returns the Hour Angle of the Sun in the sky.
         https://www.pveducation.org/pvcdrom/properties-of-sunlight/solar-time
-
-        time_zone_utc: The UTC time zone of your area in hours of UTC offset.
-        day_of_year: The number of the day of the current year, with January 1
-            being the first day of the year.
-        local_time: The local time in hours from midnight. (Adjust for Daylight Savings)
-        longitude: The longitude of a location on Earth
-
-        note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the
+        Note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the
                 calculation will end up just the same
+        :param np.ndarray time_zone_utc: The UTC time zone of your area in hours of UTC offset.
+        :param np.ndarray day_of_year: The number of the day of the current year, with January 1 being the first day of the year.
+        :param np.ndarray local_time: The local time in hours from midnight. (Adjust for Daylight Savings)
+        :param np.ndarray longitude: The longitude of a location on Earth
+        :returns: The Hour Angle in degrees.
+        :rtype: np.ndarray
 
-        Returns: The Hour Angle in degrees.
         """
 
         lst = helpers.local_time_to_apparent_solar_time(time_zone_utc / 3600, day_of_year,
                                                         local_time, longitude)
 
         hour_angle = 15 * (lst - 12)
 
         return hour_angle
 
     def calculate_elevation_angle(self, latitude, longitude, time_zone_utc, day_of_year,
                                   local_time):
         """
+
         Calculates the Elevation Angle of the Sun relative to a location on the Earth
         https://www.pveducation.org/pvcdrom/properties-of-sunlight/elevation-angle
-
-        latitude: The latitude of a location on Earth
-        longitude: The longitude of a location on Earth       
-        time_zone_utc: The UTC time zone of your area in hours of UTC offset. For example,
-            Vancouver has time_zone_utc = -7
-        day_of_year: The number of the day of the current year, with January 1
-            being the first day of the year.
-        local_time: The local time in hours from midnight. (Adjust for Daylight Savings)
-
-        note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the 
+        Note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the
                 calculation will end up just the same
 
-        Returns: The elevation angle in degrees
+        :param np.ndarray latitude: The latitude of a location on Earth
+        :param np.ndarray longitude: The longitude of a location on Earth
+        :param np.ndarray time_zone_utc: The UTC time zone of your area in hours of UTC offset. For example, Vancouver has time_zone_utc = -7
+        :param np.ndarray day_of_year: The number of the day of the current year, with January 1 being the first day of the year.
+        :param np.ndarray  local_time: The local time in hours from midnight. (Adjust for Daylight Savings)
+        :returns: The elevation angle in degrees
+        :rtype: np.ndarray
+
         """
+
         # Negative declination angles: Northern Hemisphere winter
         # 0 declination angle : Equinoxes (March 22, Sept 22)
         # Positive declination angle: Northern Hemisphere summer
         declination_angle = helpers.calculate_declination_angle(day_of_year)
 
         # Negative hour angles: Morning
         # 0 hour angle : Solar noon
@@ -85,53 +90,52 @@
 
         # mathy part is delegated to a helper function to optimize for numba compilation
         return helpers.compute_elevation_angle_math(declination_angle, hour_angle, latitude)
 
     def calculate_zenith_angle(self, latitude, longitude, time_zone_utc, day_of_year,
                                local_time):
         """
+
         Calculates the Zenith Angle of the Sun relative to a location on the Earth
         https://www.pveducation.org/pvcdrom/properties-of-sunlight/azimuth-angle
-
-        latitude: The latitude of a location on Earth
-        longitude: The longitude of a location on Earth       
-        time_zone_utc: The UTC time zone of your area in hours of UTC offset.
-        day_of_year: The number of the day of the current year, with January 1
-            being the first day of the year.
-        local_time: The local time in hours from midnight. (Adjust for Daylight Savings)
-
-        note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the 
+        Note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the
                 calculation will end up just the same
 
-        Returns: The zenith angle in degrees
+        :param latitude: The latitude of a location on Earth
+        :param longitude: The longitude of a location on Earth
+        :param time_zone_utc: The UTC time zone of your area in hours of UTC offset.
+        :param day_of_year: The number of the day of the current year, with January 1 being the first day of the year.
+        :param local_time: The local time in hours from midnight. (Adjust for Daylight Savings)
+        :return: The zenith angle in degrees
+        :rtype: float
+
         """
 
         elevation_angle = self.calculate_elevation_angle(latitude, longitude,
                                                          time_zone_utc, day_of_year, local_time)
 
         return 90 - elevation_angle
 
     def calculate_azimuth_angle(self, latitude, longitude, time_zone_utc, day_of_year,
                                 local_time):
         """
+
         Calculates the Azimuth Angle of the Sun relative to a location on the Earth.
         https://www.pveducation.org/pvcdrom/properties-of-sunlight/azimuth-angle
-
-        latitude: The latitude of a location on Earth
-        longitude: The longitude of a location on Earth       
-        time_zone_utc: The UTC time zone of your area in hours of UTC offset. For example,
-            Vancouver has time_zone_utc = -7
-        day_of_year: The number of the day of the current year, with January 1
-            being the first day of the year.
-        local_time: The local time in hours from midnight. (Adjust for Daylight Savings)
-
-        note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the 
+        Note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the
                 calculation will end up just the same
 
-        Returns: The azimuth angle in degrees
+        :param latitude: The latitude of a location on Earth
+        :param longitude: The longitude of a location on Earth
+        :param time_zone_utc: The UTC time zone of your area in hours of UTC offset. For example, Vancouver has time_zone_utc = -7
+        :param day_of_year: The number of the day of the current year, with January 1 being the first day of the year.
+        :param local_time: The local time in hours from midnight. (Adjust for Daylight Savings)
+        :returns: The azimuth angle in degrees
+        :rtype: np.ndarray
+
         """
 
         declination_angle = helpers.calculate_declination_angle(day_of_year)
         hour_angle = self.calculate_hour_angle(time_zone_utc, day_of_year,
                                                local_time, longitude)
 
         term_1 = np.sin(np.radians(declination_angle)) * \
@@ -159,30 +163,30 @@
     # ----- Calculation of sunrise and sunset times -----
 
     # ----- Calculation of modes of solar irradiance -----
 
     def calculate_DNI(self, latitude, longitude, time_zone_utc, day_of_year,
                       local_time, elevation):
         """
+
         Calculates the Direct Normal Irradiance from the Sun, relative to a location
         on the Earth (clearsky)
         https://www.pveducation.org/pvcdrom/properties-of-sunlight/calculation-of-solar-insolation
-
-        latitude: The latitude of a location on Earth
-        longitude: The longitude of a location on Earth       
-        time_zone_utc: The UTC time zone of your area in hours of UTC offset.
-        day_of_year: The number of the day of the current year, with January 1
-            being the first day of the year.
-        local_time: The local time in hours from midnight. (Adjust for Daylight Savings)
-        elevation: The local elevation of a location in metres
-
-        note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the 
+        Note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the
                 calculation will end up just the same
 
-        Returns: The Direct Normal Irradiance in W/m2
+        :param np.ndarray latitude: The latitude of a location on Earth
+        :param np.ndarray longitude: The longitude of a location on Earth
+        :param np.ndarray time_zone_utc: The UTC time zone of your area in hours of UTC offset.
+        :param np.ndarray day_of_year: The number of the day of the current year, with January 1 being the first day of the year.
+        :param np.ndarray local_time: The local time in hours from midnight. (Adjust for Daylight Savings)
+        :param np.ndarray elevation: The local elevation of a location in metres
+        :returns: The Direct Normal Irradiance in W/m2
+        :rtype: np.ndarray
+
         """
 
         zenith_angle = self.calculate_zenith_angle(latitude, longitude,
                                                    time_zone_utc, day_of_year, local_time)
         a = 0.14
 
         # air_mass = 1 / (math.cos(math.radians(zenith_angle)) + \
@@ -193,61 +197,59 @@
             DNI = self.S_0 * ((1 - a * elevation * 0.001) * np.power(np.power(0.7, air_mass),
                                                                      0.678) + a * elevation * 0.001)
         return np.where(zenith_angle > 90, 0, DNI)
 
     def calculate_DHI(self, latitude, longitude, time_zone_utc, day_of_year,
                       local_time, elevation):
         """
+
         Calculates the Diffuse Horizontal Irradiance from the Sun, relative to a location
         on the Earth (clearsky)
         https://www.pveducation.org/pvcdrom/properties-of-sunlight/calculation-of-solar-insolation
-
-        latitude: The latitude of a location on Earth
-        longitude: The longitude of a location on Earth
-        time_zone_utc: The UTC time zone of your area in hours of UTC offset.
-        day_of_year: The number of the day of the current year, with January 1
-            being the first day of the year.
-        local_time: The local time in hours from midnight
-        elevation: The local elevation of a location in metres
-
-        note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the
+        Note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the
                 calculation will end up just the same
 
-        Returns: The Diffuse Horizontal Irradiance in W/m2
+        :param np.ndarray latitude: The latitude of a location on Earth
+        :param np.ndarray longitude: The longitude of a location on Earth
+        :param np.ndarray time_zone_utc: The UTC time zone of your area in hours of UTC offset.
+        :param np.ndarray np.ndarray day_of_year: The number of the day of the current year, with January 1 being the first day of the year.
+        :param np.ndarray local_time: The local time in hours from midnight
+        :param np.ndarray elevation: The local elevation of a location in metres
+        :returns: The Diffuse Horizontal Irradiance in W/m2
+        :rtype: np.ndarray
+
         """
 
         DNI = self.calculate_DNI(latitude, longitude, time_zone_utc, day_of_year,
                                  local_time, elevation)
 
         DHI = 0.1 * DNI
 
         return DHI
 
     def calculate_GHI(self, latitude, longitude, time_zone_utc, day_of_year,
                       local_time, elevation, cloud_cover):
         """
+
         Calculates the Global Horizontal Irradiance from the Sun, relative to a location
         on the Earth
         https://www.pveducation.org/pvcdrom/properties-of-sunlight/calculation-of-solar-insolation
-
-        latitude: The latitude of a location on Earth
-        longitude: The longitude of a location on Earth
-        time_zone_utc: The UTC time zone of your area in hours of UTC offset, without
-            including the effects of Daylight Savings Time. For example, Vancouver
-             has time_zone_utc = -8 year-round.
-        day_of_year: The number of the day of the current year, with January 1
-            being the first day of the year.
-        local_time: The local time in hours from midnight.
-        elevation: The local elevation of a location in metres
-        cloud_cover: A NumPy array representing cloud cover as a percentage from 0 to 100
-
-        note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the
+        Note: If local time and time_zone_utc are both unadjusted for Daylight Savings, the
                 calculation will end up just the same
 
-        Returns: The Global Horizontal Irradiance in W/m^2
+        :param np.ndarray latitude: The latitude of a location on Earth
+        :param np.ndarray longitude: The longitude of a location on Earth
+        :param np.ndarray time_zone_utc: The UTC time zone of your area in hours of UTC offset, without including the effects of Daylight Savings Time. For example, Vancouver has time_zone_utc = -8 year-round.
+        :param np.ndarray day_of_year: The number of the day of the current year, with January 1 being the first day of the year.
+        :param np.ndarray local_time: The local time in hours from midnight.
+        :param np.ndarray elevation: The local elevation of a location in metres
+        :param np.ndarray cloud_cover: A NumPy array representing cloud cover as a percentage from 0 to 100
+        :returns: The Global Horizontal Irradiance in W/m^2
+        :rtype: np.ndarray
+
         """
 
         DHI = self.calculate_DHI(latitude, longitude, time_zone_utc, day_of_year,
                                  local_time, elevation)
 
         DNI = self.calculate_DNI(latitude, longitude, time_zone_utc, day_of_year,
                                  local_time, elevation)
@@ -258,61 +260,80 @@
         GHI = DNI * np.cos(np.radians(zenith_angle)) + DHI
 
         return self.apply_cloud_cover(GHI=GHI, cloud_cover=cloud_cover)
 
     @staticmethod
     def apply_cloud_cover(GHI, cloud_cover):
         """
+
         Applies a cloud cover model to the GHI data.
 
         Cloud cover adjustment follows the equation laid out here:
         http://www.shodor.org/os411/courses/_master/tools/calculators/solarrad/
 
-        Args:
-            GHI: Global Horizontal Index in W/m^2
-            cloud_cover: A NumPy array representing cloud cover as a percentage from 0 to 100
+        :param np.ndarray GHI: Global Horizontal Index in W/m^2
+        :param np.ndarray cloud_cover: A NumPy array representing cloud cover as a percentage from 0 to 100
 
-        Returns: GHI after considering cloud cover data
+        :returns: GHI after considering cloud cover data
+        :rtype: np.ndarray
 
         """
 
         assert np.logical_and(cloud_cover >= 0, cloud_cover <= 100).all()
 
         scaled_cloud_cover = cloud_cover / 100
 
         assert np.logical_and(scaled_cloud_cover >= 0,
                               scaled_cloud_cover <= 1).all()
 
         return GHI * (1 - (0.75 * np.power(scaled_cloud_cover, 3.4)))
 
     # ----- Calculation of modes of solar irradiance, but returning numpy arrays -----
+    def python_calculate_array_GHI_times(self, local_times):
+        date = list(map(datetime.datetime.utcfromtimestamp, local_times))
+        day_of_year = np.array(list(map(helpers.get_day_of_year_map, date)), dtype=np.float64)
+        local_time = np.array(list(map(SolarCalculations.dateConvert, date)))
+        return day_of_year, local_time
+
+    @staticmethod
+    def dateConvert(date):
+        """
+
+        Convert a date into local time.
+
+        :param datetime.date date: date to be converted
+        :return: a date converted into local time.
+        :rtype: int
+
+        """
+
+        return date.hour + (float(date.minute * 60 + date.second) / 3600)
+
     def calculate_array_GHI(self, coords, time_zones, local_times,
                             elevations, cloud_covers):
         """
+
         Calculates the Global Horizontal Irradiance from the Sun, relative to a location
         on the Earth, for arrays of coordinates, times, elevations and weathers
         https://www.pveducation.org/pvcdrom/properties-of-sunlight/calculation-of-solar-insolation
-
-        coords: (float[N][lat, lng]) array of latitudes and longitudes
-        time_zones: (int[N]) time zones at different locations in seconds relative to UTC
-        local_times: (int[N]) unix time that the vehicle will be at each location. 
-                        (Adjusted for Daylight Savings)
-        elevations: (float[N]) elevation from sea level in m
-        cloud_covers: (float[N]) percentage cloud cover in range of 0 to 1 
-
-        note: If local_times and time_zones are both unadjusted for Daylight Savings, the 
+        Note: If local_times and time_zones are both unadjusted for Daylight Savings, the
                 calculation will end up just the same
 
-        Returns: (float[N]) Global Horizontal Irradiance in W/m2
+        :param np.ndarray coords: (float[N][lat, lng]) array of latitudes and longitudes
+        :param np.ndarray time_zones: (int[N]) time zones at different locations in seconds relative to UTC
+        :param np.ndarray local_times: (int[N]) unix time that the vehicle will be at each location. (Adjusted for Daylight Savings)
+        :param np.ndarray elevations: (float[N]) elevation from sea level in m
+        :param np.ndarray cloud_covers: (float[N]) percentage cloud cover in range of 0 to 1
+        :returns: (float[N]) Global Horizontal Irradiance in W/m2
+        :rtype: np.ndarray
+
         """
 
-        date = list(map(
-            datetime.datetime.utcfromtimestamp, local_times))
-        day_of_year = np.array(
-            list(map(helpers.get_day_of_year_map, date)), dtype=np.float64)
-        local_time = np.array(list(map(lambda date: date.hour +
-                                       (float(date.minute * 60 + date.second) / 3600), date)))
+        if not self.golang:
+            day_of_year, local_time = self.python_calculate_array_GHI_times(local_times)
+        else:
+            day_of_year, local_time = self.lib.golang_calculate_array_GHI_times(local_times)
 
         ghi = self.calculate_GHI(coords[:, 0], coords[:, 1], time_zones,
                                  day_of_year, local_time, elevations, cloud_covers)
 
         return ghi
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/environment/WeatherForecasts.py` & `UBC-Solar-Simulation-0.5.7/simulation/environment/WeatherForecasts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 A class to extract local and path weather predictions such as wind_speed, 
     wind_direction, cloud_cover and weather type
 """
-import ctypes
 import json
 import numpy as np
 import os
-import pathlib
 import requests
 import sys
+
 from simulation.cache.weather import weather_directory
 from simulation.common import helpers
 from tqdm import tqdm
 
 
 class WeatherForecasts:
     """
@@ -29,46 +28,39 @@
         weather_forecast (NumPy array [N][T][9]): array that stores the complete weather forecast data. N represents the
             number of coordinates, T represents time length which differs depending on the `weather_data_frequency`
             argument ("current" -> T = 1 ; "hourly" -> T = 24 ; "daily" -> T = 8). The last 9 represents the number of
             weather forecast fields available. These are: (latitude, longitude, dt (UNIX time), timezone_offset
             (in seconds), dt + timezone_offset (local time), wind_speed, wind_direction, cloud_cover, description_id)
     """
 
-    def __init__(self, api_key, coords, duration, race_type, weather_data_frequency="daily", force_update=False):
+    def __init__(self, api_key, coords, duration, race_type, golang=False, library=None, weather_data_frequency="daily", force_update=False, origin_coord=None):
         """
+
         Initializes the instance of a WeatherForecast class
 
         :param api_key: A personal OpenWeatherAPI key to access weather forecasts
+        :param origin_coord: A NumPy array of a single [latitude, longitude]
         :param coords: A NumPy array of [latitude, longitude]
         :param weather_data_frequency: Influences what resolution weather data is requested, must be one of
             "current", "hourly", or "daily"
         :param duration: amount of time simulated (in hours)
         :param force_update: if true, weather cache data is updated by calling the OpenWeatherAPI
+        :param golang: boolean determining whether to use faster GoLang implementations when available
+
         """
         self.race_type = race_type
         self.api_key = api_key
         self.last_updated_time = -1
+        self.golang = golang
+        self.lib = library
 
-        # To compile the go file: go build -buildmode c-shared -o weather_in_time_loop.so weather_in_time_loop
-        # The following section is commented out to allow for cross-compatibility with UNIX
-        # If you are on Windows, you can use the faster Go implementation by setting golang=True and uncommenting
-
-        # Setup for Golang use in get_weather_forecast_in_time()
-        # go_directory = pathlib.Path(__file__).parent
-        #
-        # self.lib = ctypes.cdll.LoadLibrary(f"{go_directory}/weather_in_time_loop.so")
-        # self.lib.weather_in_time_loop.argtypes = [
-        #     ctypes.POINTER(ctypes.c_double),
-        #     ctypes.POINTER(ctypes.c_double),
-        #     ctypes.POINTER(ctypes.c_double),
-        #     ctypes.c_longlong,
-        #     ctypes.c_longlong
-        # ]
-
-        self.origin_coord = coords[0]
+        if origin_coord is not None:
+            self.origin_coord = np.array(origin_coord)
+        else:
+            self.origin_coord = coords[0]
         self.dest_coord = coords[-1]
 
         assert race_type in ["ASC", "FSGP"]
 
         if self.race_type == "ASC":
             self.coords = self.cull_dataset(coords, reduction_factor=625)
             weather_file = weather_directory / "weather_data.npz"
@@ -114,30 +106,32 @@
                 np.savez(f, weather_forecast=self.weather_forecast, origin_coord=self.origin_coord,
                          dest_coord=self.dest_coord)
 
         self.last_updated_time = self.weather_forecast[0, 0, 2]
 
     def get_coord_weather_forecast(self, coord, weather_data_frequency, duration):
         """
+
         Passes in a single coordinate, returns a weather forecast
         for the coordinate depending on the entered "weather_data_frequency"
         argument. This function is unlikely to ever be called directly.
 
-        :param coord: A single coordinate stored inside a NumPy array [latitude, longitude]
-        :param weather_data_frequency: Influences what resolution weather data is requested, must be one of
+        :param np.ndarray coord: A single coordinate stored inside a NumPy array [latitude, longitude]
+        :param str weather_data_frequency: Influences what resolution weather data is requested, must be one of
             "current", "hourly", or "daily"
-        :param duration: amount of time simulated (in hours)
+        :param int  duration: amount of time simulated (in hours)
 
         :returns weather_array: [N][9]
         - [N]: is 1 for "current", 24 for "hourly", 8 for "daily"
         - [9]: (latitude, longitude, dt (UNIX time), timezone_offset (in seconds), dt + timezone_offset (local time),
                wind_speed, wind_direction, cloud_cover, description_id)
-
+        :rtype: np.ndarray
         For reference to the API used:
         - https://openweathermap.org/api/one-call-api
+
         """
 
         # TODO: Who knows, maybe we want to run the simulation like a week into the future, when the weather forecast
         #   api only allows 24 hours of hourly forecast. I think it is good to pad the end of the weather_array with
         #   daily forecasts, after the hourly. Then in get_weather_forecast_in_time() the appropriate weather can be
         #   obtained by using the same shortest place method that you did with the cumulative distances.
 
@@ -211,29 +205,31 @@
             weather_array[i][7] = weather_data_dict["clouds"]
             weather_array[i][8] = weather_data_dict["weather"][0]["id"]
 
         return weather_array
 
     def update_path_weather_forecast(self, coords, weather_data_frequency, duration):
         """
+
         Passes in a list of coordinates, returns the hourly weather forecast
         for each of the coordinates
-        
-        :param coords: A NumPy array of [coord_index][2]
+
+        :param np.ndarray coords: A NumPy array of [coord_index][2]
         - [2] => [latitude, longitude]
-        :param weather_data_frequency: Influences what resolution weather data is requested, must be one of
+        :param str weather_data_frequency: Influences what resolution weather data is requested, must be one of
             "current", "hourly", or "daily"
-        :param duration: duration of weather requested, in hours
+        :param int duration: duration of weather requested, in hours
 
         :returns
         - A NumPy array [coord_index][N][9]
         - [coord_index]: the index of the coordinates passed into the function
         - [N]: is 1 for "current", 24 for "hourly", 8 for "daily"
         - [9]: (latitude, longitude, dt (UNIX time), timezone_offset (in seconds), dt + timezone_offset (local time),
                wind_speed, wind_direction, cloud_cover, description_id)
+
         """
 
         if int(duration) > 48 and weather_data_frequency == "hourly":
             time_length = {"current": 1, "hourly": 54, "daily": 8}
         else:
             time_length = {"current": 1, "hourly": 48, "daily": 8}
 
@@ -248,36 +244,31 @@
         print()
 
         return weather_forecast
 
     def calculate_closest_weather_indices(self, cumulative_distances):
         """
 
-        Args:
-            cumulative_distances: NumPy Array representing cumulative distances theoretically achievable for a given input speed array
-
-        Returns:
+        :param np.ndarray cumulative_distances: NumPy Array representing cumulative distances theoretically achievable for a given input speed array
+        :returns: array of the closest weather indices.
+        :rtype: np.ndarray
 
         """
-        current_coordinate_index = 0
-        result = []
-
-        # TODO: can rewrite this to use self.gis.path[closest_gis_indices]
 
         """
         IMPORTANT: we only have weather coordinates for a discrete set of coordinates. However, the car could be at any
         coordinate in between these available weather coordinates. We need to figure out what coordinate the car is at
         at each timestep and then we can figure out the full weather forecast at each timestep.
-        
+
         For example, imagine the car is at some coordinate (10, 20). Further imagine that we have a week's worth of
         weather forecasts for the following five coordinates: (5, 4), (11, 19), (20, 30), (40, 30), (0, 60). Which
         set of weather forecasts should we choose? Well, we should choose the (11, 19) one since our coordinate
         (10, 20) is closest to (11, 19). This is what the following code is accomplishing. However, it is not dealing
         with the coordinates directly but rather is dealing with the distances between the coordinates. 
-        
+
         Furthermore, once we have chosen a week's worth of weather forecasts for a specific coordinate, we must isolate
         a single weather forecast depending on what time the car is at the coordinate (10, 20). That is the job of the
         `get_weather_forecast_in_time()` method.
         """
 
         # if racing FSGP, there is no need for distance calculations. We will return only the origin coordinate
         # This characterizes the weather at every point along the FSGP tracks
@@ -297,14 +288,29 @@
         # makes every even-index element negative, this allows the use of np.diff() to calculate the sum of consecutive
         # elements
         cumulative_weather_path_distances[::2] *= -1
 
         # contains the average distance between two consecutive elements in the cumulative_weather_path_distances array
         average_distances = np.abs(np.diff(cumulative_weather_path_distances) / 2)
 
+        if not self.golang:
+            return self.python_calculate_closest_weather_indices(cumulative_distances, average_distances)
+        else:
+            return self.lib.golang_calculate_closest_weather_indices(cumulative_distances, average_distances)
+
+    def python_calculate_closest_weather_indices(self, cumulative_distances, average_distances):
+        """
+
+        Python implementation of calculate_closest_weather_indices. See parent function for documentation details.
+
+        """
+
+        current_coordinate_index = 0
+        result = []
+
         for distance in np.nditer(cumulative_distances):
 
             # makes sure the current_coordinate_index does not exceed its maximum value
             if current_coordinate_index > len(average_distances) - 1:
                 current_coordinate_index = len(average_distances) - 1
 
             if distance > average_distances[current_coordinate_index]:
@@ -312,148 +318,132 @@
                 if current_coordinate_index > len(average_distances) - 1:
                     current_coordinate_index = len(average_distances) - 1
 
             result.append(current_coordinate_index)
 
         return np.array(result)
 
-    def golang_calculate_closest_timestamp_indices(self, unix_timestamps, dt_local_array):
-        """
-        GoLang implementation to find the indices of the closest timestamps in dt_local_array and package them into a NumPy Array
-
-        Args:
-            unix_timestamps: NumPy Array (float[N]) unix timestamps of the vehicle's journey
-            dt_local_array: NumPy Array (float[N]) local times, represented as unix timestamps
-
-        Returns: NumPy Array (int[N]) containing closest timestamp indices used by get_weather_forecast_in_time
-
-        """
-        unix_timestamps_pointer, closest_time_stamp_indices_pointer, \
-        closest_time_stamp_indices = helpers.generate_golang_io_pointers(unix_timestamps)
-
-        dt_local_arr_pointer, _, _ = helpers.generate_golang_io_pointers(dt_local_array)
-
-        self.lib.weather_in_time_loop(
-            unix_timestamps_pointer,
-            closest_time_stamp_indices_pointer,
-            dt_local_arr_pointer,
-            len(dt_local_array),
-            len(unix_timestamps))
-
-        return np.array(closest_time_stamp_indices, 'i')
-
     @staticmethod
-    @helpers.timeit
     def python_calculate_closest_timestamp_indices(unix_timestamps, dt_local_array):
         """
 
         Python implementation to find the indices of the closest timestamps in dt_local_array and package them into a NumPy Array
 
-        Args:
-            unix_timestamps: NumPy Array (float[N]) of unix timestamps of the vehicle's journey
-            dt_local_array: NumPy Array (float[N]) of local times, represented as unix timestamps
-
-        Returns: NumPy Array of (int[N]) containing closest timestamp indices used by get_weather_forecast_in_time
+        :param np.ndarray unix_timestamps: NumPy Array (float[N]) of unix timestamps of the vehicle's journey
+        :param np.ndarray dt_local_array: NumPy Array (float[N]) of local times, represented as unix timestamps
+        :returns: NumPy Array of (int[N]) containing closest timestamp indices used by get_weather_forecast_in_time
+        :rtype: np.ndarray
 
         """
         closest_time_stamp_indices = []
         for unix_timestamp in unix_timestamps:
             unix_timestamp_array = np.full_like(dt_local_array, fill_value=unix_timestamp)
             differences = np.abs(unix_timestamp_array - dt_local_array)
             minimum_index = np.argmin(differences)
             closest_time_stamp_indices.append(minimum_index)
 
         return np.asarray(closest_time_stamp_indices, dtype=np.int32)
 
-    @helpers.timeit
-    def get_weather_forecast_in_time(self, indices, unix_timestamps, golang=False):
+    def get_weather_forecast_in_time(self, indices, unix_timestamps):
         """
+
         Takes in an array of indices of the weather_forecast array, and an array of timestamps. Uses those to figure out
         what the weather forecast is at each time step being simulated.
 
         we only have weather at discrete timestamps. The car however can be in any timestamp in
         between. Therefore, we must be able to choose the weather timestamp that is closest to the one that the car is in
         so that we can more accurately determine the weather experienced by the car at that timestamp.
 
         For example, imagine the car is at some coordinate (x,y) at timestamp 100. Imagine we know the weather forecast
         at (x,y) for five different timestamps: 0, 30, 60, 90, and 120. Which weather forecast should we
         choose? Clearly, we should choose the weather forecast at 90 since it is the closest to 100. That's what the
         below code is accomplishing.
 
-        :param indices: (int[N]) coordinate indices of self.weather_forecast
-        :param unix_timestamps: (int[N]) unix timestamps of the vehicle's journey
-        :param golang: Boolean specifying whether a GoLang implementation of get_weather_forecast_in_time should be used
-                   If false, a slower Python implementation is used.
-
-        :returns
-        - A NumPy array of size [N][9]
-        - [9]: (latitude, longitude, unix_time, timezone_offset, unix_time_corrected, wind_speed, wind_direction,
-                    cloud_cover, precipitation, description):
+        :param np.ndarray indices: (int[N]) coordinate indices of self.weather_forecast
+        :param np.ndarray unix_timestamps: (int[N]) unix timestamps of the vehicle's journey
+        :returns:
+            - A NumPy array of size [N][9]
+            - [9] (latitude, longitude, unix_time, timezone_offset, unix_time_corrected, wind_speed, wind_direction,
+                        cloud_cover, precipitation, description):
+        :rtype: np.ndarray
 
         """
 
         # each element is the weather forecast for all available times at that coordinate
         full_weather_forecast_at_coords = self.weather_forecast[indices]
         dt_local_array = full_weather_forecast_at_coords[0, :, 4]
 
-        if golang:
-            closest_timestamp_indices = self.golang_calculate_closest_timestamp_indices(unix_timestamps, dt_local_array)
+        if self.golang:
+            closest_timestamp_indices = self.lib.golang_calculate_closest_timestamp_indices(unix_timestamps, dt_local_array)
         else:
             closest_timestamp_indices = self.python_calculate_closest_timestamp_indices(unix_timestamps, dt_local_array)
 
         temp_0 = np.arange(0, full_weather_forecast_at_coords.shape[0])
 
         # if you're wondering why or how this works, don't ask because I don't know, it just does
         # this is what duct-taping looks like in software engineering
         result = full_weather_forecast_at_coords[tuple((temp_0, closest_timestamp_indices))]
 
         return result
 
     @staticmethod
     def cull_dataset(coords, reduction_factor):
         """
+        
         As we currently have a limited number of API calls(60) every minute with the
-            current Weather API, we must shrink the dataset significantly. As the
-            OpenWeatherAPI models have a resolution of between 2.5 - 70 km, we will
-            go for a resolution of 25km. Assuming we travel at 100km/h for 12 hours,
-            1200 kilometres/25 = 48 API calls
+        current Weather API, we must shrink the dataset significantly. As the
+        OpenWeatherAPI models have a resolution of between 2.5 - 70 km, we will
+        go for a resolution of 25km. Assuming we travel at 100km/h for 12 hours,
+        1200 kilometres/25 = 48 API calls
 
         As the Google Maps API has a resolution of around 40m between points,
-            for ASC, we must cull at 625:1 (because 25,000m / 40m = 625)
+        for ASC, we must cull at 625:1 (because 25,000m / 40m = 625)
+        
+        :param np.ndarray coords: array to be reduced
+        :param int reduction_factor: the factor in which the array will be reduced
+        :return: reduced array
+        :rtype: np.ndarray
+        
         """
 
         return coords[::reduction_factor]
 
     @staticmethod
     def get_array_directional_wind_speed(vehicle_bearings, wind_speeds, wind_directions):
         """
+
         Returns the array of wind speed in m/s, in the direction opposite to the 
             bearing of the vehicle
 
 
-        vehicle_bearings: (float[N]) The azimuth angles that the vehicle in, in degrees
-        wind_speeds: (float[N]) The absolute speeds in m/s
-        wind_directions: (float[N]) The wind direction in the meteorlogical convention. To convert from
-            meteorlogical convention to azimuth angle, use (x + 180) % 360
-
-        Returns: The wind speeds in the direction opposite to the bearing of the vehicle
+        :param np.ndarray vehicle_bearings: (float[N]) The azimuth angles that the vehicle in, in degrees
+        :param np.ndarray wind_speeds: (float[N]) The absolute speeds in m/s
+        :param np.ndarray wind_directions: (float[N]) The wind direction in the meteorlogical convention. To convert from meteorlogical convention to azimuth angle, use (x + 180) % 360
+        :returns: The wind speeds in the direction opposite to the bearing of the vehicle
+        :rtype: np.ndarray
+        
         """
 
         # wind direction is 90 degrees meteorological, so it is 270 degrees azimuthal. car is 90 degrees
         #   cos(90 - 90) = cos(0) = 1. Wind speed is moving opposite to the car,
         # car is 270 degrees, cos(90-270) = -1. Wind speed is in direction of the car.
         return wind_speeds * (np.cos(np.radians(wind_directions - vehicle_bearings)))
 
     @staticmethod
     def get_weather_advisory(weather_id):
         """
+
         Returns a string indicating the type of weather to expect, from the standardized
             weather code passed as a parameter
 
         https://openweathermap.org/weather-conditions#Weather-Condition-Codes-2
+        :param int weather_id: Weather ID
+        :return: type of weather advisory
+        :rtype: str
+
         """
 
         if 200 <= weather_id < 300:
             return "Thunderstorm"
         elif 300 <= weather_id < 500:
             return "Drizzle"
         elif 500 <= weather_id < 600:
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/main/ExecuteSimulation.py` & `UBC-Solar-Simulation-0.5.7/simulation/main/ExecuteSimulation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 import numpy as np
+import json
 
-from simulation.common import helpers
-from simulation.main import TimeSimulation
-from simulation.optimization.bayesian import BayesianOptimization
-from simulation.utils.InputBounds import InputBounds
+from simulation.main.Simulation import Simulation, SimulationReturnType
+from simulation.common.simulationState import SimulationState
 from simulation.main.SimulationResult import SimulationResult
+from simulation.config import settings_directory
+
 
 """
 Description: Export Simulation data as a SimulationResults object. 
 """
 
 
-@helpers.timeit
-def main() -> SimulationResult:
-    """
-    Returns a SimulationResult object with the purpose of exporting simulation data.
-    TODO: Add functionality to modify data up to a point in the simulation to allow the simulation to run on real data.
+def GetSimulationData(golang=True):
     """
 
-    simulation_model = TimeSimulation(race_type="ASC")
-
-    bounds = InputBounds()
-    bounds.add_bounds(8, 20, 60)
-    optimization = BayesianOptimization(bounds, simulation_model.run_model)
+    Returns a SimulationResult object with the purpose of exporting simulation data.
 
-    # The number of times simulation runs is init_points + n_iter + 1
-    results = optimization.maximize(init_points=0, n_iter=0, kappa=10)
-    optimized = simulation_model.run_model(speed=np.fromiter(results, dtype=float),
-                                           plot_results=False, verbose=False, route_visualization=False,
-                                           return_results_object=True)
+    """
 
-    return optimized
+    input_speed = np.array([30])
 
+    with open(settings_directory / "initial_conditions.json") as f:
+        args = json.load(f)
 
-def GetSimulationData() -> SimulationResult:
-    """
-    Returns a SimulationResult object with the purpose of exporting simulation data.
-    """
-    return main()
+    return_type = SimulationReturnType.simulation_results
+    initialSimulationConditions = SimulationState(args)
+    simulation_model = Simulation(initialSimulationConditions, return_type, race_type="ASC", golang=golang)
+
+    results = simulation_model.run_model(speed=input_speed, plot_results=False, verbose=False, route_visualization=False)
+    map_coordinates = simulation_model.gis.path
+    return results, map_coordinates
 
 
 if __name__ == "__main__":
-    main()
+    results, map_coordinates = GetSimulationData()
+    print(map_coordinates[100])
+    print(results.time_taken)
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/main/MainSimulation.py` & `UBC-Solar-Simulation-0.5.7/simulation/main/Simulation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,127 +1,173 @@
-import datetime
 import json
-import numpy as np
+import sys
+import logging
 import os
-import simulation as simulation
-from bayes_opt import BayesianOptimization
-from bokeh.layouts import gridplot
-from bokeh.models import HoverTool
-from bokeh.palettes import Bokeh8
-from bokeh.plotting import figure, show, output_file
+import numpy as np
+import simulation
+
+from tqdm import tqdm
+from enum import Enum
 from dotenv import load_dotenv
 from simulation.common import helpers
-from simulation.common.helpers import adjust_timestamps_to_local_times, get_array_directional_wind_speed
 from simulation.config import settings_directory
 from simulation.main.SimulationResult import SimulationResult
+from simulation.common.plotting import Graph, Plotting
 
 
-class Simulation:
+class SimulationReturnType(Enum):
+    """
 
-    def __init__(self, race_type):
-        """
-        Instantiates a simple model of the car.
+    This enum exists to discretize different data types run_model should return.
+
+    """
+
+    time_taken = 0
+    distance_travelled = 1
+    simulation_results = 2
 
-        :param race_type: a string that describes the race type to simulate (ASC or FSGP)
 
-        Depending on the race type, the following initialisation parameters are read from the corresponding
-        settings json file located in the config folder.
+class Simulation:
+    """
 
-        google_api_key: API key to access GoogleMaps API. Stored in a .env file. Please ask Chris for this!
-        weather_api_key: API key to access OpenWeather API. Stored in a .env file. Please ask Chris for this!
+    Attributes:
+        google_api_key: API key to access GoogleMaps API. Stored in a .env file. Please ask Simulation Lead for this!
+        weather_api_key: API key to access OpenWeather API. Stored in a .env file. Please ask Simulation Lead for this!
         origin_coord: array containing latitude and longitude of route start point
         dest_coord: array containing latitude and longitude of route end point
         waypoints: array containing latitude and longitude pairs of route waypoints
         tick: length of simulation's discrete time step (in seconds)
         simulation_duration: length of simulated time (in seconds)
         start_hour: describes the hour to start the simulation (typically either 7 or 9, these
         represent 7am and 9am respectively)
+
+    """
+
+    def __init__(self, initial_conditions, return_type, race_type, golang=True):
         """
 
+        Instantiates a simple model of the car.
+
+        :param race_type: a string that describes the race type to simulate (ASC or FSGP)
+        :param initial_conditions: a SimulationState object that provides initial conditions for the simulation
+        :param return_type: discretely defines what kind of data run_model should return.
+        :param golang: boolean which controls whether GoLang implementations are used when available
+
+        """
+
+        # ----- Return type -----
+
+        assert return_type in SimulationReturnType, "return_type must be of SimulationReturnType enum."
+
+        self.return_type = return_type
+
+        # ----- Race type -----
+
         assert race_type in ["ASC", "FSGP"]
 
+        self.race_type = race_type
+
         if race_type == "ASC":
             settings_path = settings_directory / "settings_ASC.json"
         else:
             settings_path = settings_directory / "settings_FSGP.json"
 
         with open(settings_path) as f:
             args = json.load(f)
 
-        self.initial_battery_charge = args['initial_battery_charge']
-
-        # LVS power loss is pretty small, so it is neglected
-        self.lvs_power_loss = args['lvs_power_loss']
+        # ----- Load from settings_*.json -----
 
-        # ----- Time constants -----
+        self.lvs_power_loss = args['lvs_power_loss']  # LVS power loss is pretty small, so it is neglected
 
         self.tick = args['tick']
-        self.simulation_duration = args['simulation_duration']
-        self.start_hour = args['start_hour']
 
-        # ----- API keys -----
+        if self.race_type == "ASC":
+            race_length = args['race_length']  # Race length in days, arbitrary as ASC doesn't have a time limit
+            self.simulation_duration = race_length * 24 * 60 * 60
+        elif self.race_type == "FSGP":
+            self.simulation_duration = args['simulation_duration']
 
-        load_dotenv()
+        # ----- Load from initial_conditions
+
+        self.initial_battery_charge = initial_conditions.initial_battery_charge
 
-        self.weather_api_key = os.environ.get("OPENWEATHER_API_KEY")
-        self.google_api_key = os.environ.get("GOOGLE_MAPS_API_KEY")
+        self.start_hour = initial_conditions.start_hour
 
-        # ----- Route constants -----
+        self.origin_coord = initial_conditions.origin_coord
+        self.dest_coord = initial_conditions.dest_coord
+        self.current_coord = initial_conditions.current_coord
+        self.waypoints = initial_conditions.waypoints
 
-        self.origin_coord = args['origin_coord']
-        self.dest_coord = args['dest_coord']
-        self.waypoints = args['waypoints']
+        gis_force_update = initial_conditions.gis_force_update
+        weather_force_update = initial_conditions.weather_force_update
 
         # ----- Route Length -----
 
         self.route_length = 0  # Tentatively set to 0
 
-        # ----- Race type -----
+        # ----- API keys -----
 
-        self.race_type = race_type
+        load_dotenv()
 
-        # ----- Force update flags -----
+        self.weather_api_key = os.getenv('OPENWEATHER_API_KEY')
+        self.google_api_key = os.getenv('GOOGLE_MAPS_API_KEY')
 
-        gis_force_update = args['gis_force_update']
-        weather_force_update = args['weather_force_update']
+        # ----- GoLang library initialisation -----
+        self.golang = golang
+        self.library = simulation.Libraries(raiseExceptionOnFail=False)
+
+        if self.golang and self.library.found_compatible_binaries() is False:
+            # If compatible GoLang binaries weren't found, disable GoLang usage.
+            self.golang = False
+            logging.warning("GoLang binaries not found --> GoLang usage has been disabled. "
+                            "To use GoLang implementations, see COMPILING_HOWTO about "
+                            "compiling GoLang for your operating system.")
 
         # ----- Component initialisation -----
 
         self.basic_array = simulation.BasicArray()
 
         self.basic_battery = simulation.BasicBattery(self.initial_battery_charge)
 
         self.basic_lvs = simulation.BasicLVS(self.lvs_power_loss * self.tick)
 
         self.basic_motor = simulation.BasicMotor()
 
         self.gis = simulation.GIS(self.google_api_key, self.origin_coord, self.dest_coord, self.waypoints,
-                                  self.race_type, force_update=gis_force_update)
+                                  self.race_type, library=self.library, force_update=gis_force_update,
+                                  current_coord=self.current_coord, golang=golang)
+
         self.route_coords = self.gis.get_path()
 
         self.vehicle_bearings = self.gis.calculate_current_heading_array()
+
         self.weather = simulation.WeatherForecasts(self.weather_api_key, self.route_coords,
                                                    self.simulation_duration / 3600,
                                                    self.race_type,
+                                                   library=self.library,
                                                    weather_data_frequency="daily",
-                                                   force_update=weather_force_update)
+                                                   force_update=weather_force_update,
+                                                   origin_coord=self.gis.launch_point,
+                                                   golang=golang)
 
         weather_hour = helpers.hour_from_unix_timestamp(self.weather.last_updated_time)
         self.time_of_initialization = self.weather.last_updated_time + 3600 * (24 + self.start_hour - weather_hour)
 
-        self.solar_calculations = simulation.SolarCalculations()
+        self.solar_calculations = simulation.SolarCalculations(library=self.library)
 
         self.local_times = 0
 
         self.timestamps = np.arange(0, self.simulation_duration + self.tick, self.tick)
 
-    @helpers.timeit
+        self.plotting = Plotting()
+
     def run_model(self, speed=np.array([20, 20, 20, 20, 20, 20, 20, 20]), plot_results=True, verbose=False,
                   route_visualization=False, **kwargs):
         """
+
         Updates the model in tick increments for the entire simulation duration. Returns
         a final battery charge and a distance travelled for this duration, given an
         initial charge, and a target speed. Also requires the current time and location.
         This is where the magic happens.
 
         Note: if the speed remains constant throughout this update, and knowing the starting
             time, the cumulative distance at every time can be known. From the cumulative
@@ -145,24 +191,42 @@
             speed = np.fromiter(kwargs.values(), dtype=float)
 
             # Don't plot results since this code is run by the optimizer
             plot_results = False
             verbose = False
 
         # ----- Reshape speed array -----
-
-        print(f"Input speeds: {speed}\n")
+        if not kwargs:
+            print(f"Input speeds: {speed}\n")
 
         speed_kmh = helpers.reshape_and_repeat(speed, self.simulation_duration)
         speed_kmh = np.insert(speed_kmh, 0, 0)
         speed_kmh = helpers.apply_deceleration(speed_kmh, 20)
 
-        # ------ Run calculations and get result and modified speed array -------
+        speed_kmh, not_charge = helpers.apply_race_timing_constraints(speed_kmh=speed_kmh, start_hour=self.start_hour,
+                                                                      simulation_duration=self.simulation_duration,
+                                                                      race_type=self.race_type,
+                                                                      timestamps=self.timestamps,
+                                                                      verbose=verbose)
 
-        result = self.__run_simulation_calculations(speed_kmh, verbose=verbose)
+        if self.race_type == "ASC":
+            speed_kmh_without_checkpoints = speed_kmh
+            speed_kmh = self.gis.speeds_with_waypoints(self.gis.path, self.gis.path_distances, speed_kmh / 3.6,
+                                                       self.waypoints, verbose=False)[:self.simulation_duration + 1]
+            if verbose:
+                self.plotting.add_graph_to_queue(Graph([speed_kmh_without_checkpoints, speed_kmh],
+                                                       ["Speed before waypoints", " Speed after waypoints"],
+                                                       "Before and After waypoints"))
+
+        speed_kmh = helpers.apply_deceleration(speed_kmh, 20)
+        raw_speed = speed_kmh
+
+        # ------ Run calculations and get result and modified speed array -------
+        with tqdm(total=20, file=sys.stdout, desc="Running Simulation Calculations") as pbar:
+            result = self.__run_simulation_calculations(speed_kmh, not_charge, pbar, verbose=verbose)
 
         # ------- Parse results ---------
         simulation_arrays = result.arrays
         speed_kmh = simulation_arrays[0]
         distances = simulation_arrays[1]
         state_of_charge = simulation_arrays[2]
         delta_energy = simulation_arrays[3]
@@ -170,226 +234,248 @@
         wind_speeds = simulation_arrays[5]
         gis_route_elevations_at_each_tick = simulation_arrays[6]
         cloud_covers = simulation_arrays[7]
 
         distance_travelled = result.distance_travelled
         time_taken = result.time_taken
         final_soc = result.final_soc
+        raw_soc = self.basic_battery.get_raw_soc(np.cumsum(delta_energy))
 
-        print(f"Simulation successful!\n"
-              f"Time taken: {time_taken}\n"
-              f"Route length: {self.route_length:.2f}km\n"
-              f"Maximum distance traversable: {distance_travelled:.2f}km\n"
-              f"Average speed: {np.average(speed_kmh):.2f}km/h\n"
-              f"Final battery SOC: {final_soc:.2f}%\n")
+        if not kwargs:
+            print(f"Simulation successful!\n"
+                  f"Time taken: {time_taken}\n"
+                  f"Route length: {self.route_length:.2f}km\n"
+                  f"Maximum distance traversable: {distance_travelled:.2f}km\n"
+                  f"Average speed: {np.average(speed_kmh):.2f}km/h\n"
+                  f"Final battery SOC: {final_soc:.2f}%\n")
 
         # ----- Plotting -----
 
         if plot_results:
             arrays_to_plot = [speed_kmh, distances, state_of_charge, delta_energy,
                               solar_irradiances, wind_speeds, gis_route_elevations_at_each_tick,
-                              cloud_covers]
+                              cloud_covers, raw_soc, raw_speed]
             y_label = ["Speed (km/h)", "Distance (km)", "SOC (%)", "Delta energy (J)",
-                       "Solar irradiance (W/m^2)", "Wind speeds (km/h)", "Elevation (m)", "Cloud cover (%)"]
+                       "Solar irradiance (W/m^2)", "Wind speeds (km/h)", "Elevation (m)", "Cloud cover (%)",
+                       "Raw SOC (%)", "Raw Speed (km/h)"]
 
-            helpers.plot_graph(timestamps=self.timestamps,
-                               arrays_to_plot=arrays_to_plot,
-                               array_labels=y_label,
-                               graph_title="Simulation Result")
+            self.plotting.add_graph_to_queue(Graph(arrays_to_plot, y_label, "Results"))
+            self.plotting.plot_graphs(self.timestamps)
 
         if self.race_type == "FSGP":
-            # Do this so I'm not plotting the entire 300 laps which will look the same as one lap anyway.
             helpers.route_visualization(self.gis.single_lap_path, visible=route_visualization)
         elif self.race_type == "ASC":
             helpers.route_visualization(self.gis.path, visible=route_visualization)
 
-        return distance_travelled
+        if self.return_type is SimulationReturnType.distance_travelled:
+            return distance_travelled
+        if self.return_type is SimulationReturnType.time_taken:
+            return -1 * time_taken
+        if self.return_type is SimulationReturnType.simulation_results:
+            return result
+        else:
+            raise TypeError("Return type not found.")
 
-    def __run_simulation_calculations(self, speed_kmh, verbose=False):
+    def __run_simulation_calculations(self, speed_kmh, not_charge, pbar, verbose=False):
         """
+
         Helper method to perform all calculations used in run_model. Returns a SimulationResult object 
         containing members that specify total distance travelled and time taken at the end of the simulation
         and final battery state of charge. This is where most of the main simulation logic happens.
 
         :param speed_kmh: array that specifies the solar car's driving speed (in km/h) at each time step
+        :param not_charge: array that specifies when the car is charging for calculations
+        :param pbar: progress bar used to track Simulation progress
+
         """
 
+        # ----- Tick array -----
+
         tick_array = np.diff(self.timestamps)
         tick_array = np.insert(tick_array, 0, 0)
 
-        speed_kmh, not_charge = helpers.apply_race_timing_constraints(speed_kmh=speed_kmh, start_hour=self.start_hour,
-                                                                      simulation_duration=self.simulation_duration,
-                                                                      race_type=self.race_type,
-                                                                      timestamps=self.timestamps,
-                                                                      verbose=verbose)
-
-        if self.race_type == "ASC":
-            speed_kmh_without_checkpoints = speed_kmh
-            speed_kmh = helpers.speeds_with_waypoints(self.gis.path, self.gis.path_distances, speed_kmh / 3.6,
-                                                      self.waypoints, verbose=False)[:self.simulation_duration + 1]
-            if verbose:
-                helpers.plot_graph(self.timestamps, [speed_kmh_without_checkpoints, speed_kmh],
-                                   ["Speed before waypoints", " Speed after waypoints"],
-                                   "Before and After waypoints")
-
-        speed_kmh = helpers.apply_deceleration(speed_kmh, 20)
+        pbar.update(1)
 
         # ----- Expected distance estimate -----
 
         # Array of cumulative distances theoretically achievable via the speed array
-
         distances = tick_array * speed_kmh / 3.6
         cumulative_distances = np.cumsum(distances)
 
         temp = cumulative_distances
+        pbar.update(1)
 
         # ----- Weather and location calculations -----
 
         """ closest_gis_indices is a 1:1 mapping between each point which has within it a timestamp and cumulative
                 distance from a starting point, to its closest point on a map.
 
             closest_weather_indices is a 1:1 mapping between a weather condition, and its closest point on a map.
         """
 
         closest_gis_indices = self.gis.calculate_closest_gis_indices(cumulative_distances)
 
+        pbar.update(1)
+
         closest_weather_indices = self.weather.calculate_closest_weather_indices(cumulative_distances)
 
+        pbar.update(1)
+
         path_distances = self.gis.path_distances
         cumulative_distances = np.cumsum(path_distances)  # [cumulative_distances] = meters
 
+        pbar.update(1)
+
         max_route_distance = cumulative_distances[-1]
 
         self.route_length = max_route_distance / 1000.0  # store the route length in kilometers
 
+        pbar.update(1)
+
         # Array of elevations at every route point
         gis_route_elevations = self.gis.get_path_elevations()
 
         gis_route_elevations_at_each_tick = gis_route_elevations[closest_gis_indices]
 
+        pbar.update(1)
+
         # Get the azimuth angle of the vehicle at every location
         gis_vehicle_bearings = self.vehicle_bearings[closest_gis_indices]
 
+        pbar.update(1)
+
         # Get array of path gradients
         gradients = self.gis.get_gradients(closest_gis_indices)
 
+        pbar.update(1)
+
         # ----- Timing Calculations -----
 
         # Get time zones at each point on the GIS path
         time_zones = self.gis.get_time_zones(closest_gis_indices)
 
         # Local times in UNIX timestamps
-        local_times = adjust_timestamps_to_local_times(self.timestamps, self.time_of_initialization, time_zones)
+        local_times = helpers.adjust_timestamps_to_local_times(self.timestamps, self.time_of_initialization, time_zones)
+
+        pbar.update(1)
 
         # Get the weather at every location
         weather_forecasts = self.weather.get_weather_forecast_in_time(closest_weather_indices, local_times)
         roll_by_tick = 3600 * (24 + self.start_hour - helpers.hour_from_unix_timestamp(weather_forecasts[0, 2]))
         weather_forecasts = np.roll(weather_forecasts, -roll_by_tick, 0)
+
+        pbar.update(2)
+
         absolute_wind_speeds = weather_forecasts[:, 5]
         wind_directions = weather_forecasts[:, 6]
         cloud_covers = weather_forecasts[:, 7]
 
+        pbar.update(1)
+
         # Get the wind speeds at every location
-        wind_speeds = get_array_directional_wind_speed(gis_vehicle_bearings, absolute_wind_speeds,
+        wind_speeds = helpers.get_array_directional_wind_speed(gis_vehicle_bearings, absolute_wind_speeds,
                                                        wind_directions)
 
+        pbar.update(1)
+
         # Get an array of solar irradiance at every coordinate and time
         solar_irradiances = self.solar_calculations.calculate_array_GHI(self.route_coords[closest_gis_indices],
                                                                         time_zones, local_times,
                                                                         gis_route_elevations_at_each_tick,
                                                                         cloud_covers)
 
+        pbar.update(2)
         # TLDR: we have now obtained solar irradiances, wind speeds, and gradients at each tick
 
         # ----- Energy Calculations -----
 
         self.basic_lvs.update(self.tick)
 
         lvs_consumed_energy = self.basic_lvs.get_consumed_energy()
         motor_consumed_energy = self.basic_motor.calculate_energy_in(speed_kmh, gradients, wind_speeds, self.tick)
         array_produced_energy = self.basic_array.calculate_produced_energy(solar_irradiances, self.tick)
 
         motor_consumed_energy = np.logical_and(motor_consumed_energy, not_charge) * motor_consumed_energy
 
+        pbar.update(1)
+
         consumed_energy = motor_consumed_energy + lvs_consumed_energy
         produced_energy = array_produced_energy
 
         # net energy added to the battery
         delta_energy = produced_energy - consumed_energy
 
+        pbar.update(1)
+
         # ----- Array initialisation -----
 
         # used to calculate the time the car was in motion
         tick_array = np.full_like(self.timestamps, fill_value=self.tick, dtype='f4')
         tick_array[0] = 0
 
         # ----- Array calculations -----
 
         cumulative_delta_energy = np.cumsum(delta_energy)
         battery_variables_array = self.basic_battery.update_array(cumulative_delta_energy)
 
+        pbar.update(1)
+
         # stores the battery SOC at each time step
         state_of_charge = battery_variables_array[0]
         state_of_charge[np.abs(state_of_charge) < 1e-03] = 0
 
+        speed_kmh = np.logical_and(not_charge, state_of_charge) * speed_kmh
+
         if verbose:
+            indices_and_environment_graph = Graph([temp, closest_gis_indices, closest_weather_indices, gradients,
+                                                   time_zones, gis_vehicle_bearings],
+                                                  ["speed dist (m)", "gis ind", "weather ind", "gradients (m)",
+                                                   "time zones",
+                                                   "vehicle bearings"], "Indices and Environment variables")
+            self.plotting.add_graph_to_queue(indices_and_environment_graph)
+
+            speed_boolean_graph = Graph([speed_kmh, state_of_charge],
+                                        ["Speed (km/h)", "SOC", "Speed & SOC", "Speed & not_charge"],
+                                        "Speed Boolean Operations")
+            self.plotting.add_graph_to_queue(speed_boolean_graph)
 
-            helpers.plot_graph(timestamps=self.timestamps,
-                               arrays_to_plot=[temp, closest_gis_indices, closest_weather_indices, gradients,
-                                               time_zones, gis_vehicle_bearings],
-                               array_labels=["speed dist (m)", "gis ind", "weather ind", "gradients (m)", "time zones",
-                                             "vehicle bearings"],
-                               graph_title="Indices and Environment variables")
-            arrays_to_plot = [speed_kmh, state_of_charge]
-
-            for arr in [state_of_charge, not_charge]:
-                speed_kmh = np.logical_and(speed_kmh, arr) * speed_kmh
-                arrays_to_plot.append(speed_kmh)
-
-            helpers.plot_graph(timestamps=self.timestamps,
-                               arrays_to_plot=arrays_to_plot,
-                               array_labels=["Speed (km/h)", "SOC", "Speed & SOC", "Speed & not_charge"],
-                               graph_title="Speed Boolean Operations")
-        else:
-            speed_kmh = np.logical_and(not_charge, state_of_charge) * speed_kmh
+        pbar.update(1)
 
         time_in_motion = np.logical_and(tick_array, speed_kmh) * self.tick
 
         final_soc = state_of_charge[-1] * 100 + 0.
 
         distance = speed_kmh * (time_in_motion / 3600)
         distances = np.cumsum(distance)
 
         # Car cannot exceed Max distance, and it is not in motion after exceeded
         distances = distances.clip(0, max_route_distance / 1000)
 
-        try:
-            max_dist_index = np.where(distances == max_route_distance / 1000)[0][0]
-        except IndexError:
-            max_dist_index = len(time_in_motion)
-
-        time_in_motion = np.array(
-            (list(time_in_motion[0:max_dist_index])) + list(np.zeros_like(time_in_motion[max_dist_index:])))
-
-        time_taken = np.sum(time_in_motion)
-        time_taken = str(datetime.timedelta(seconds=int(time_taken)))
-
         results = SimulationResult()
 
         results.arrays = [
             speed_kmh,
             distances,
             state_of_charge,
             delta_energy,
             solar_irradiances,
             wind_speeds,
             gis_route_elevations_at_each_tick,
             cloud_covers
         ]
+
         results.distance_travelled = distances[-1]
-        results.time_taken = time_taken
+
+        pbar.update(1)
+
+        if results.distance_travelled >= self.route_length:
+            results.time_taken = helpers.calculate_race_completion_time(
+                self.route_length, distances)
+        else:
+            results.time_taken = self.simulation_duration
+
         results.final_soc = final_soc
 
         self.time_zones = time_zones
         self.local_times = local_times
 
         return results
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/main/SimulationResult.py` & `UBC-Solar-Simulation-0.5.7/simulation/main/SimulationResult.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 class SimulationResult:
     def __init__(self, arrays=None, distance_travelled=None, time_taken=None, final_soc=None):
         """
+
         Instantiates a SimulationResult object. This is used in the MainSimulation class when
         running a simulation. This object simply stores desired simulation results while the
         simulation is running its calculations to better encapsulate the information
+
         """
         self.arrays = arrays
         self.distance_travelled = distance_travelled
         self.time_taken = time_taken
         self.final_soc = final_soc
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/motor/basic_motor.py` & `UBC-Solar-Simulation-0.5.7/simulation/motor/basic_motor.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,17 +31,20 @@
         self.e_mc = 0.98  # motor controller efficiency, subject to change
         self.e_m = 0.9  # motor efficiency, subject to change
 
         # print("torque experienced by motor: {} Nm".format(self.constant_torque))
 
     def calculate_power_out(self):
         """
+
         Calculates the power transferred to the wheel by the motor and the motor controller
     
-        returns: the power transferred to the wheel in W
+        :returns: the power transferred to the wheel in W
+        :rtype: float
+
         """
         power_in = self.dc_v * self.dc_i
         power_controller = power_in * self.e_mc
 
         # alternatively, power_controller = sqrt(3) / 2 * Vrms * Irms
         power_out = power_controller * self.e_m
 
@@ -50,31 +53,35 @@
 
         return power_out
 
     # For the motor, the energy consumed by the motor/motor controller depends on the voltage and
     #   current supplied by the battery to the motor controller
     def update_motor_input(self, dc_v, dc_i):
         """
+
         For the motor, the energy consumed by the motor/motor controller depends on the voltage 
             and current supplied by the battery to the motor controller
+
         """
 
         self.dc_v = dc_v
         self.dc_i = dc_i
 
     def calculate_power_in(self, required_speed_kmh, gradient, wind_speed):
         """
+
         For a given road gradient, calculate the power that must be inputted into
             the motor to maintain a required speed
 
-        :param required_speed_kmh: required speed in km/h
-        :param gradient: road gradient, where > 0 means uphill and < 0 means downhill
-        :param wind_speed: speed of wind in m/s, where > 0 means against the direction of the vehicle.
+        :param np.ndarray required_speed_kmh: required speed in km/h
+        :param np.ndarray gradient: road gradient, where > 0 means uphill and < 0 means downhill
+        :param np.ndarray wind_speed: speed of wind in m/s, where > 0 means against the direction of the vehicle.
+        :returns: power required to travel at a speed and gradient in W
+        :rtype: np.ndarray
 
-        returns: power required to travel at a speed and gradient in W
         """
 
         required_speed_ms = required_speed_kmh / 3.6
         required_angular_speed_rads = required_speed_ms / self.tire_radius
 
         drag_force = 0.5 * self.air_density * (
                 (required_speed_ms + wind_speed) ** 2) * self.drag_coefficient * self.vehicle_frontal_area
@@ -85,35 +92,39 @@
 
         motor_input_power = motor_output_power / self.e_m
 
         self.input_power = motor_input_power / self.e_mc
 
     def update(self, tick):
         """
+
         For the motor, the update tick calculates a value for the energy expended in a period
             of time.
         
-        :param tick: length of 1 update cycle in seconds
+        :param int tick: length of 1 update cycle in seconds
+
         """
 
         self.consumed_energy = self.input_power * tick
 
     @staticmethod
     def calculate_motor_efficiency(motor_angular_speed, motor_output_energy, tick):
         """
+
         Calculates a NumPy array of motor efficiency from NumPy array of operating angular speeds and NumPy array
             of output power. Based on data obtained from NGM SC-M150 Datasheet and modelling done in MATLAB
 
         r squared value: 0.873
 
-        :param motor_angular_speed: (float[N]) angular speed motor operates in rad/s
-        :param motor_output_energy: (float[N]) energy motor outputs to the wheel in J
-        :param tick: length of 1 update cycle in seconds
-
+        :param np.ndarray motor_angular_speed: (float[N]) angular speed motor operates in rad/s
+        :param np.ndarray motor_output_energy: (float[N]) energy motor outputs to the wheel in J
+        :param int tick: length of 1 update cycle in seconds
         :returns e_m: (float[N]) efficiency of the motor
+        :rtype: np.ndarray
+
         """
 
         # Power = Energy / Time
         motor_output_power = motor_output_energy * tick
         rads_rpm_conversion_factor = 30 / math.pi
 
         revolutions_per_minute = motor_angular_speed * rads_rpm_conversion_factor
@@ -129,25 +140,26 @@
         e_m[e_m > 1] = 1
 
         return e_m
 
     @staticmethod
     def calculate_motor_controller_efficiency(motor_angular_speed, motor_output_energy, tick):
         """
+
         Calculates a NumPy array of motor controller efficiency from NumPy array of operating angular speeds and
         NumPy array of output power. Based on data obtained from the WaveSculptor Motor Controller Datasheet efficiency
         curve for a 90 V DC Bus and modelling done in MATLAB.
 
         r squared value: 0.7431
 
-        :param motor_angular_speed: (float[N]) angular speed motor operates in rad/s
-        :param motor_output_energy: (float[N]) energy motor outputs to the wheel in J
-        :param tick: length of 1 update cycle in seconds
-
+        :param np.ndarray motor_angular_speed: (float[N]) angular speed motor operates in rad/s
+        :param np.ndarray motor_output_energy: (float[N]) energy motor outputs to the wheel in J
+        :param int tick: length of 1 update cycle in seconds
         :returns e_mc (float[N]) efficiency of the motor controller
+        :rtype: np.ndarray
 
         """
 
         # Ignore nan warning. Set nan value to 0
         np.seterr(divide='ignore', invalid='ignore')
 
         # Power = Energy / Time
@@ -172,23 +184,25 @@
         e_mc[e_mc < 0.9] = 0.9
         e_mc[e_mc > 1] = 1
 
         return e_mc
 
     def calculate_energy_in(self, required_speed_kmh, gradients, wind_speeds, tick):
         """
+
         Create a function which takes in array of elevation, array of wind speed, required
             speed, returns the consumed energy.
 
-        :param required_speed_kmh: (float[N]) required speed array in km/h
-        :param gradients: (float[N]) gradient at parts of the road
-        :param wind_speeds: (float[N]) speeds of wind in m/s, where > 0 means against the direction of the vehicle
-        :param tick: (int) length of 1 update cycle in seconds
+        :param np.ndarray required_speed_kmh: (float[N]) required speed array in km/h
+        :param np.ndarray gradients: (float[N]) gradient at parts of the road
+        :param np.ndarray wind_speeds: (float[N]) speeds of wind in m/s, where > 0 means against the direction of the vehicle
+        :param int tick: length of 1 update cycle in seconds
+        :returns: (float[N]) energy expended by the motor at every tick
+        :rtype: np.ndarray
 
-        returns: (float[N]) energy expended by the motor at every tick
         """
 
         required_speed_ms = required_speed_kmh / 3.6
 
         required_angular_speed_rads = required_speed_ms / self.tire_radius
         required_angular_speed_rads_array = np.ones(len(gradients)) * required_angular_speed_rads
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/optimization/bayesian.py` & `UBC-Solar-Simulation-0.5.7/simulation/optimization/bayesian.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 
 
 class BayesianOptimization(BaseOptimization):
     def __init__(self, bounds: InputBounds, f):
         BaseOptimization.__init__(self, bounds, f)
         self.optimizer = bayes_opt.BayesianOptimization(self.func, self.bounds.get_bound_dict(), verbose=2)
 
-    def maximize(self, init_points=5, n_iter=3, acq="ucb", kappa=10):
+    def maximize(self, init_points=5, n_iter=25, acq="ucb", kappa=10):
         self.optimizer.maximize(init_points=init_points, n_iter=n_iter, acq=acq, kappa=kappa)
         self.result = self.optimizer.max
         self.bestinput = list(self.result["params"].values())
         self.target = self.result["target"]
         return self.bestinput
```

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/optimization/random.py` & `UBC-Solar-Simulation-0.5.7/simulation/optimization/random.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/utils/InputBounds.py` & `UBC-Solar-Simulation-0.5.7/simulation/utils/InputBounds.py`

 * *Files identical despite different names*

### Comparing `UBC-Solar-Simulation-0.5.6a0/simulation/utils/MapPlot.py` & `UBC-Solar-Simulation-0.5.7/simulation/utils/MapPlot.py`

 * *Files identical despite different names*

