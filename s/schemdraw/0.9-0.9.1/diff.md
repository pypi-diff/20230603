# Comparing `tmp/schemdraw-0.9.tar.gz` & `tmp/schemdraw-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/schemdraw-0.9.tar", last modified: Sat Jan 30 21:04:36 2021, max compression
+gzip compressed data, was "dist/schemdraw-0.9.1.tar", last modified: Sat Jan 30 21:48:25 2021, max compression
```

## Comparing `schemdraw-0.9.tar` & `schemdraw-0.9.1.tar`

### file list

```diff
@@ -1,205 +1,209 @@
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.829222 schemdraw-0.9/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7470 2021-01-30 20:15:18.000000 schemdraw-0.9/CHANGES.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1065 2021-01-23 23:03:29.000000 schemdraw-0.9/LICENSE.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      227 2020-12-18 16:01:07.000000 schemdraw-0.9/MANIFEST.in
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1931 2021-01-30 21:04:36.829222 schemdraw-0.9/PKG-INFO
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      859 2021-01-23 23:03:29.000000 schemdraw-0.9/README.txt
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.740222 schemdraw-0.9/docs/
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.741222 schemdraw-0.9/docs/.ipynb_checkpoints/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2245 2021-01-17 23:40:04.000000 schemdraw-0.9/docs/.ipynb_checkpoints/conf-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1323 2021-01-03 15:49:00.000000 schemdraw-0.9/docs/.ipynb_checkpoints/index-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      634 2020-12-18 16:01:07.000000 schemdraw-0.9/docs/Makefile
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       50 2020-12-18 16:01:07.000000 schemdraw-0.9/docs/changes.rst
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.742222 schemdraw-0.9/docs/classes/
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.743222 schemdraw-0.9/docs/classes/.ipynb_checkpoints/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      711 2021-01-04 00:41:11.000000 schemdraw-0.9/docs/classes/.ipynb_checkpoints/drawing-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      103 2021-01-03 15:41:27.000000 schemdraw-0.9/docs/classes/.ipynb_checkpoints/dsp-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1154 2021-01-03 16:52:24.000000 schemdraw-0.9/docs/classes/.ipynb_checkpoints/electrical-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       79 2021-01-03 15:41:45.000000 schemdraw-0.9/docs/classes/.ipynb_checkpoints/flow-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      130 2021-01-03 16:28:37.000000 schemdraw-0.9/docs/classes/.ipynb_checkpoints/index-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      137 2021-01-03 15:54:26.000000 schemdraw-0.9/docs/classes/.ipynb_checkpoints/logic-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      139 2021-01-03 16:32:08.000000 schemdraw-0.9/docs/classes/.ipynb_checkpoints/segments-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      711 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/classes/drawing.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      103 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/classes/dsp.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1154 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/classes/electrical.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       79 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/classes/flow.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      130 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/classes/index.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      137 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/classes/logic.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      139 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/classes/segments.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2245 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/conf.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.744222 schemdraw-0.9/docs/elements/
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.747222 schemdraw-0.9/docs/elements/.ipynb_checkpoints/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1896 2021-01-03 15:55:31.000000 schemdraw-0.9/docs/elements/.ipynb_checkpoints/compound-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6481 2021-01-16 16:53:47.000000 schemdraw-0.9/docs/elements/.ipynb_checkpoints/connectors-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2022 2021-01-03 16:41:09.000000 schemdraw-0.9/docs/elements/.ipynb_checkpoints/dsp-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    16806 2021-01-18 01:42:55.000000 schemdraw-0.9/docs/elements/.ipynb_checkpoints/electrical-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1965 2021-01-03 16:37:53.000000 schemdraw-0.9/docs/elements/.ipynb_checkpoints/flow-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3781 2021-01-18 01:53:40.000000 schemdraw-0.9/docs/elements/.ipynb_checkpoints/intcircuits-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2561 2021-01-18 00:35:20.000000 schemdraw-0.9/docs/elements/.ipynb_checkpoints/logic-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1896 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/elements/compound.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6481 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/elements/connectors.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2022 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/elements/dsp.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    16806 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/elements/electrical.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1965 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/elements/flow.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3781 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/elements/intcircuits.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2561 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/elements/logic.rst
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.748222 schemdraw-0.9/docs/gallery/
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.750222 schemdraw-0.9/docs/gallery/.ipynb_checkpoints/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7948 2021-01-18 00:40:49.000000 schemdraw-0.9/docs/gallery/.ipynb_checkpoints/analog-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3389 2021-01-03 17:47:44.000000 schemdraw-0.9/docs/gallery/.ipynb_checkpoints/flowcharting-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    12307 2021-01-11 03:47:59.000000 schemdraw-0.9/docs/gallery/.ipynb_checkpoints/ic-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      291 2021-01-03 18:05:51.000000 schemdraw-0.9/docs/gallery/.ipynb_checkpoints/index-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5395 2021-01-11 00:28:42.000000 schemdraw-0.9/docs/gallery/.ipynb_checkpoints/logicgate-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6198 2021-01-03 17:50:13.000000 schemdraw-0.9/docs/gallery/.ipynb_checkpoints/opamp-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7011 2021-01-03 18:01:04.000000 schemdraw-0.9/docs/gallery/.ipynb_checkpoints/signalproc-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8505 2021-01-03 17:43:39.000000 schemdraw-0.9/docs/gallery/.ipynb_checkpoints/solidstate-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1525 2021-01-03 17:51:32.000000 schemdraw-0.9/docs/gallery/.ipynb_checkpoints/styles-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7948 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/gallery/analog.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3389 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/gallery/flowcharting.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    12307 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/gallery/ic.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      291 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/gallery/index.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5395 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/gallery/logicgate.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6198 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/gallery/opamp.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7011 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/gallery/signalproc.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8505 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/gallery/solidstate.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1525 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/gallery/styles.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1323 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/index.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      795 2020-12-18 16:01:07.000000 schemdraw-0.9/docs/make.bat
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       36 2020-12-20 00:36:24.000000 schemdraw-0.9/docs/requirements.txt
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.751222 schemdraw-0.9/docs/usage/
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.751222 schemdraw-0.9/docs/usage/.ipynb_checkpoints/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     9234 2021-01-30 18:41:01.000000 schemdraw-0.9/docs/usage/.ipynb_checkpoints/customizing-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    18483 2021-01-18 00:01:53.000000 schemdraw-0.9/docs/usage/.ipynb_checkpoints/placement-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6053 2021-01-03 18:56:20.000000 schemdraw-0.9/docs/usage/.ipynb_checkpoints/start-checkpoint.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8988 2021-01-30 19:45:23.000000 schemdraw-0.9/docs/usage/customizing.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    18483 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/usage/placement.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6053 2021-01-23 23:03:29.000000 schemdraw-0.9/docs/usage/start.rst
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      205 2020-12-18 16:01:07.000000 schemdraw-0.9/readthedocs.yml
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.754222 schemdraw-0.9/schemdraw/
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.758222 schemdraw-0.9/schemdraw/.ipynb_checkpoints/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      233 2021-01-30 20:20:05.000000 schemdraw-0.9/schemdraw/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      201 2020-12-19 23:20:49.000000 schemdraw-0.9/schemdraw/.ipynb_checkpoints/adddocs-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    17217 2021-01-30 20:31:00.000000 schemdraw-0.9/schemdraw/.ipynb_checkpoints/schemdraw-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    27824 2021-01-29 03:15:40.000000 schemdraw-0.9/schemdraw/.ipynb_checkpoints/segments-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1863 2021-01-29 02:53:20.000000 schemdraw-0.9/schemdraw/.ipynb_checkpoints/transform-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1302 2021-01-29 02:39:57.000000 schemdraw-0.9/schemdraw/.ipynb_checkpoints/types-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3148 2021-01-29 02:40:50.000000 schemdraw-0.9/schemdraw/.ipynb_checkpoints/util-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      233 2021-01-30 20:20:05.000000 schemdraw-0.9/schemdraw/__init__.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.759222 schemdraw-0.9/schemdraw/backends/
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.761222 schemdraw-0.9/schemdraw/backends/.ipynb_checkpoints/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     9078 2021-01-30 18:54:32.000000 schemdraw-0.9/schemdraw/backends/.ipynb_checkpoints/mpl-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    12837 2021-01-30 18:36:50.000000 schemdraw-0.9/schemdraw/backends/.ipynb_checkpoints/svg-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2264 2021-01-26 16:37:30.000000 schemdraw-0.9/schemdraw/backends/.ipynb_checkpoints/svgdisplay-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    12697 2021-01-30 16:01:59.000000 schemdraw-0.9/schemdraw/backends/.ipynb_checkpoints/svgtext-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2020-12-18 16:01:07.000000 schemdraw-0.9/schemdraw/backends/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     9078 2021-01-30 18:54:32.000000 schemdraw-0.9/schemdraw/backends/mpl.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    12837 2021-01-30 18:36:50.000000 schemdraw-0.9/schemdraw/backends/svg.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    12697 2021-01-30 16:01:59.000000 schemdraw-0.9/schemdraw/backends/svgtext.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.762222 schemdraw-0.9/schemdraw/dsp/
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.762222 schemdraw-0.9/schemdraw/dsp/.ipynb_checkpoints/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7985 2021-01-17 03:22:02.000000 schemdraw-0.9/schemdraw/dsp/.ipynb_checkpoints/dsp-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      737 2020-12-18 16:01:07.000000 schemdraw-0.9/schemdraw/dsp/.ipynb_checkpoints/legacy-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      584 2020-12-18 16:01:07.000000 schemdraw-0.9/schemdraw/dsp/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7985 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/dsp/dsp.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      737 2020-12-18 16:01:07.000000 schemdraw-0.9/schemdraw/dsp/legacy.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.765222 schemdraw-0.9/schemdraw/elements/
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.768222 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3071 2021-01-16 17:28:40.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6768 2021-01-16 17:40:44.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/cables-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8383 2021-01-29 03:17:37.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/compound-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    15861 2021-01-29 02:43:01.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/connectors-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    32010 2021-01-29 03:19:57.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/elements-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    29518 2021-01-29 03:23:47.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/intcircuits-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6595 2021-01-03 19:50:38.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/legacy-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    11628 2021-01-29 03:24:22.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/lines-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5973 2021-01-17 02:33:05.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/misc-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4750 2021-01-17 02:39:43.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/oneterm-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1718 2021-01-17 02:42:30.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/opamp-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    13606 2021-01-16 17:13:48.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/outlets-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7164 2021-01-17 02:47:44.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/sources-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10413 2021-01-17 02:53:32.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/switches-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8256 2021-01-18 00:20:54.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/transistors-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    19636 2021-01-29 03:25:25.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/twoterm-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3899 2021-01-17 02:59:00.000000 schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/xform-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3071 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/elements/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6768 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/elements/cables.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8383 2021-01-30 00:05:53.000000 schemdraw-0.9/schemdraw/elements/compound.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    15861 2021-01-30 00:05:53.000000 schemdraw-0.9/schemdraw/elements/connectors.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    32010 2021-01-30 00:05:53.000000 schemdraw-0.9/schemdraw/elements/elements.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    29518 2021-01-30 00:05:53.000000 schemdraw-0.9/schemdraw/elements/intcircuits.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6595 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/elements/legacy.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    11628 2021-01-30 00:05:53.000000 schemdraw-0.9/schemdraw/elements/lines.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5973 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/elements/misc.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4750 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/elements/oneterm.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1718 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/elements/opamp.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    13606 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/elements/outlets.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7164 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/elements/sources.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10413 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/elements/switches.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8256 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/elements/transistors.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    19636 2021-01-30 00:05:53.000000 schemdraw-0.9/schemdraw/elements/twoterm.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3899 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/elements/xform.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.774222 schemdraw-0.9/schemdraw/flow/
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.774222 schemdraw-0.9/schemdraw/flow/.ipynb_checkpoints/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6172 2021-01-17 03:24:58.000000 schemdraw-0.9/schemdraw/flow/.ipynb_checkpoints/flow-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      467 2020-12-18 16:01:07.000000 schemdraw-0.9/schemdraw/flow/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6172 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/flow/flow.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      668 2020-12-18 16:01:07.000000 schemdraw-0.9/schemdraw/flow/legacy.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.774222 schemdraw-0.9/schemdraw/logic/
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.774222 schemdraw-0.9/schemdraw/logic/.ipynb_checkpoints/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1133 2020-12-18 16:01:07.000000 schemdraw-0.9/schemdraw/logic/.ipynb_checkpoints/legacy-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    11429 2021-01-17 03:32:50.000000 schemdraw-0.9/schemdraw/logic/.ipynb_checkpoints/logic-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      522 2020-12-18 16:01:07.000000 schemdraw-0.9/schemdraw/logic/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1133 2020-12-18 16:01:07.000000 schemdraw-0.9/schemdraw/logic/legacy.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    11429 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/logic/logic.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.775222 schemdraw-0.9/schemdraw/parsing/
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.775222 schemdraw-0.9/schemdraw/parsing/.ipynb_checkpoints/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4789 2020-12-18 16:01:07.000000 schemdraw-0.9/schemdraw/parsing/.ipynb_checkpoints/buchheim-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5488 2021-01-02 23:58:50.000000 schemdraw-0.9/schemdraw/parsing/.ipynb_checkpoints/logic_parser-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       36 2020-12-18 16:01:07.000000 schemdraw-0.9/schemdraw/parsing/__init__.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4789 2020-12-18 16:01:07.000000 schemdraw-0.9/schemdraw/parsing/buchheim.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5488 2021-01-23 23:03:29.000000 schemdraw-0.9/schemdraw/parsing/logic_parser.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    17217 2021-01-30 20:31:00.000000 schemdraw-0.9/schemdraw/schemdraw.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    27824 2021-01-30 00:05:53.000000 schemdraw-0.9/schemdraw/segments.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1863 2021-01-30 00:05:53.000000 schemdraw-0.9/schemdraw/transform.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1274 2021-01-29 02:49:18.000000 schemdraw-0.9/schemdraw/types.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3148 2021-01-30 00:05:53.000000 schemdraw-0.9/schemdraw/util.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.756222 schemdraw-0.9/schemdraw.egg-info/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1931 2021-01-30 21:04:36.000000 schemdraw-0.9/schemdraw.egg-info/PKG-INFO
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6740 2021-01-30 21:04:36.000000 schemdraw-0.9/schemdraw.egg-info/SOURCES.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2021-01-30 21:04:36.000000 schemdraw-0.9/schemdraw.egg-info/dependency_links.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       10 2021-01-30 21:04:36.000000 schemdraw-0.9/schemdraw.egg-info/top_level.txt
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)       38 2021-01-30 21:04:36.829222 schemdraw-0.9/setup.cfg
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1369 2021-01-30 20:40:52.000000 schemdraw-0.9/setup.py
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.799222 schemdraw-0.9/test/
-drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:04:36.829222 schemdraw-0.9/test/.ipynb_checkpoints/
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1405449 2020-12-31 02:39:29.000000 schemdraw-0.9/test/.ipynb_checkpoints/gallery_legacy-checkpoint.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      353 2021-01-26 20:08:36.000000 schemdraw-0.9/test/.ipynb_checkpoints/schematic-checkpoint.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   131190 2021-01-30 19:37:27.000000 schemdraw-0.9/test/.ipynb_checkpoints/test_backend-checkpoint.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1742566 2020-12-31 02:57:33.000000 schemdraw-0.9/test/.ipynb_checkpoints/test_cases_legacy-checkpoint.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   195091 2021-01-30 19:37:36.000000 schemdraw-0.9/test/.ipynb_checkpoints/test_dsp-checkpoint.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1876417 2021-01-30 19:37:56.000000 schemdraw-0.9/test/.ipynb_checkpoints/test_elements-checkpoint.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   387409 2021-01-30 19:38:21.000000 schemdraw-0.9/test/.ipynb_checkpoints/test_elements2-checkpoint.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    51822 2021-01-30 19:38:41.000000 schemdraw-0.9/test/.ipynb_checkpoints/test_flow-checkpoint.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1857556 2021-01-30 19:40:15.000000 schemdraw-0.9/test/.ipynb_checkpoints/test_gallery-checkpoint.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1597000 2021-01-30 19:39:24.000000 schemdraw-0.9/test/.ipynb_checkpoints/test_gallery_kwargs-checkpoint.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   279222 2021-01-30 19:40:38.000000 schemdraw-0.9/test/.ipynb_checkpoints/test_intcircuits-checkpoint.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   339678 2021-01-30 19:41:03.000000 schemdraw-0.9/test/.ipynb_checkpoints/test_logic-checkpoint.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   130781 2021-01-30 19:41:15.000000 schemdraw-0.9/test/.ipynb_checkpoints/test_parselogic-checkpoint.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   652834 2021-01-30 19:41:53.000000 schemdraw-0.9/test/.ipynb_checkpoints/test_placement-checkpoint.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   137708 2021-01-30 19:42:18.000000 schemdraw-0.9/test/.ipynb_checkpoints/test_styles-checkpoint.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      297 2021-01-23 23:03:29.000000 schemdraw-0.9/test/headless.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      685 2021-01-30 20:07:01.000000 schemdraw-0.9/test/savetest.png
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)      353 2021-01-26 20:33:49.000000 schemdraw-0.9/test/schematic.py
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1122 2021-01-30 20:07:01.000000 schemdraw-0.9/test/testMPL.png
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   131190 2021-01-30 19:37:27.000000 schemdraw-0.9/test/test_backend.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   195091 2021-01-30 19:37:36.000000 schemdraw-0.9/test/test_dsp.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1876417 2021-01-30 19:37:56.000000 schemdraw-0.9/test/test_elements.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   387409 2021-01-30 19:38:21.000000 schemdraw-0.9/test/test_elements2.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)    51822 2021-01-30 19:38:41.000000 schemdraw-0.9/test/test_flow.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1857556 2021-01-30 19:40:15.000000 schemdraw-0.9/test/test_gallery.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1597000 2021-01-30 19:39:24.000000 schemdraw-0.9/test/test_gallery_kwargs.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   279222 2021-01-30 19:40:38.000000 schemdraw-0.9/test/test_intcircuits.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   339678 2021-01-30 19:41:03.000000 schemdraw-0.9/test/test_logic.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   130781 2021-01-30 19:41:15.000000 schemdraw-0.9/test/test_parselogic.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   652834 2021-01-30 19:41:53.000000 schemdraw-0.9/test/test_placement.ipynb
--rw-r--r--   0 collindelker  (1000) collindelker  (1000)   137708 2021-01-30 19:42:18.000000 schemdraw-0.9/test/test_styles.ipynb
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.770102 schemdraw-0.9.1/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7470 2021-01-30 20:15:18.000000 schemdraw-0.9.1/CHANGES.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1065 2021-01-23 23:03:29.000000 schemdraw-0.9.1/LICENSE.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      227 2020-12-18 16:01:07.000000 schemdraw-0.9.1/MANIFEST.in
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1933 2021-01-30 21:48:25.769101 schemdraw-0.9.1/PKG-INFO
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      859 2021-01-23 23:03:29.000000 schemdraw-0.9.1/README.txt
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.716102 schemdraw-0.9.1/docs/
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.716102 schemdraw-0.9.1/docs/.ipynb_checkpoints/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      634 2020-12-18 16:01:07.000000 schemdraw-0.9.1/docs/.ipynb_checkpoints/Makefile-checkpoint
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2245 2021-01-17 23:40:04.000000 schemdraw-0.9.1/docs/.ipynb_checkpoints/conf-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1323 2021-01-03 15:49:00.000000 schemdraw-0.9.1/docs/.ipynb_checkpoints/index-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      795 2020-12-18 16:01:07.000000 schemdraw-0.9.1/docs/.ipynb_checkpoints/make-checkpoint.bat
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       46 2021-01-30 21:17:34.000000 schemdraw-0.9.1/docs/.ipynb_checkpoints/requirements-checkpoint.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      634 2020-12-18 16:01:07.000000 schemdraw-0.9.1/docs/Makefile
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       50 2020-12-18 16:01:07.000000 schemdraw-0.9.1/docs/changes.rst
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.717102 schemdraw-0.9.1/docs/classes/
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.718102 schemdraw-0.9.1/docs/classes/.ipynb_checkpoints/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      711 2021-01-04 00:41:11.000000 schemdraw-0.9.1/docs/classes/.ipynb_checkpoints/drawing-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      103 2021-01-03 15:41:27.000000 schemdraw-0.9.1/docs/classes/.ipynb_checkpoints/dsp-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1154 2021-01-03 16:52:24.000000 schemdraw-0.9.1/docs/classes/.ipynb_checkpoints/electrical-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       79 2021-01-03 15:41:45.000000 schemdraw-0.9.1/docs/classes/.ipynb_checkpoints/flow-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      130 2021-01-03 16:28:37.000000 schemdraw-0.9.1/docs/classes/.ipynb_checkpoints/index-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      137 2021-01-03 15:54:26.000000 schemdraw-0.9.1/docs/classes/.ipynb_checkpoints/logic-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      139 2021-01-03 16:32:08.000000 schemdraw-0.9.1/docs/classes/.ipynb_checkpoints/segments-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      711 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/classes/drawing.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      103 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/classes/dsp.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1154 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/classes/electrical.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       79 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/classes/flow.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      130 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/classes/index.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      137 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/classes/logic.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      139 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/classes/segments.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2245 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/conf.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.719102 schemdraw-0.9.1/docs/elements/
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.720102 schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1896 2021-01-03 15:55:31.000000 schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/compound-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6481 2021-01-16 16:53:47.000000 schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/connectors-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2022 2021-01-03 16:41:09.000000 schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/dsp-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    16806 2021-01-18 01:42:55.000000 schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/electrical-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1965 2021-01-03 16:37:53.000000 schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/flow-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3781 2021-01-18 01:53:40.000000 schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/intcircuits-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2561 2021-01-18 00:35:20.000000 schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/logic-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1896 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/elements/compound.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6481 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/elements/connectors.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2022 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/elements/dsp.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    16806 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/elements/electrical.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1965 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/elements/flow.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3781 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/elements/intcircuits.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2561 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/elements/logic.rst
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.723101 schemdraw-0.9.1/docs/gallery/
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.725102 schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7948 2021-01-18 00:40:49.000000 schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/analog-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3389 2021-01-03 17:47:44.000000 schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/flowcharting-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    12307 2021-01-11 03:47:59.000000 schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/ic-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      291 2021-01-03 18:05:51.000000 schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/index-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5395 2021-01-11 00:28:42.000000 schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/logicgate-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6198 2021-01-03 17:50:13.000000 schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/opamp-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7011 2021-01-03 18:01:04.000000 schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/signalproc-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8505 2021-01-03 17:43:39.000000 schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/solidstate-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1525 2021-01-03 17:51:32.000000 schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/styles-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7948 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/gallery/analog.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3389 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/gallery/flowcharting.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    12307 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/gallery/ic.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      291 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/gallery/index.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5395 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/gallery/logicgate.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6198 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/gallery/opamp.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7011 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/gallery/signalproc.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8505 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/gallery/solidstate.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1525 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/gallery/styles.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1323 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/index.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      795 2020-12-18 16:01:07.000000 schemdraw-0.9.1/docs/make.bat
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       46 2021-01-30 21:17:34.000000 schemdraw-0.9.1/docs/requirements.txt
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.727102 schemdraw-0.9.1/docs/usage/
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.728102 schemdraw-0.9.1/docs/usage/.ipynb_checkpoints/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     9234 2021-01-30 18:41:01.000000 schemdraw-0.9.1/docs/usage/.ipynb_checkpoints/customizing-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    18483 2021-01-18 00:01:53.000000 schemdraw-0.9.1/docs/usage/.ipynb_checkpoints/placement-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6053 2021-01-03 18:56:20.000000 schemdraw-0.9.1/docs/usage/.ipynb_checkpoints/start-checkpoint.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8988 2021-01-30 19:45:23.000000 schemdraw-0.9.1/docs/usage/customizing.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    18483 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/usage/placement.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6053 2021-01-23 23:03:29.000000 schemdraw-0.9.1/docs/usage/start.rst
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      205 2020-12-18 16:01:07.000000 schemdraw-0.9.1/readthedocs.yml
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.729102 schemdraw-0.9.1/schemdraw/
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.730102 schemdraw-0.9.1/schemdraw/.ipynb_checkpoints/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      235 2021-01-30 21:48:07.000000 schemdraw-0.9.1/schemdraw/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      201 2020-12-19 23:20:49.000000 schemdraw-0.9.1/schemdraw/.ipynb_checkpoints/adddocs-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    17217 2021-01-30 20:31:00.000000 schemdraw-0.9.1/schemdraw/.ipynb_checkpoints/schemdraw-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    27824 2021-01-29 03:15:40.000000 schemdraw-0.9.1/schemdraw/.ipynb_checkpoints/segments-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1863 2021-01-29 02:53:20.000000 schemdraw-0.9.1/schemdraw/.ipynb_checkpoints/transform-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1302 2021-01-29 02:39:57.000000 schemdraw-0.9.1/schemdraw/.ipynb_checkpoints/types-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3148 2021-01-29 02:40:50.000000 schemdraw-0.9.1/schemdraw/.ipynb_checkpoints/util-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      235 2021-01-30 21:48:07.000000 schemdraw-0.9.1/schemdraw/__init__.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.731102 schemdraw-0.9.1/schemdraw/backends/
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.732102 schemdraw-0.9.1/schemdraw/backends/.ipynb_checkpoints/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     9078 2021-01-30 18:54:32.000000 schemdraw-0.9.1/schemdraw/backends/.ipynb_checkpoints/mpl-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    12837 2021-01-30 18:36:50.000000 schemdraw-0.9.1/schemdraw/backends/.ipynb_checkpoints/svg-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     2264 2021-01-26 16:37:30.000000 schemdraw-0.9.1/schemdraw/backends/.ipynb_checkpoints/svgdisplay-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    12697 2021-01-30 16:01:59.000000 schemdraw-0.9.1/schemdraw/backends/.ipynb_checkpoints/svgtext-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        0 2020-12-18 16:01:07.000000 schemdraw-0.9.1/schemdraw/backends/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     9078 2021-01-30 18:54:32.000000 schemdraw-0.9.1/schemdraw/backends/mpl.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    12837 2021-01-30 18:36:50.000000 schemdraw-0.9.1/schemdraw/backends/svg.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    12697 2021-01-30 16:01:59.000000 schemdraw-0.9.1/schemdraw/backends/svgtext.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.732102 schemdraw-0.9.1/schemdraw/dsp/
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.733101 schemdraw-0.9.1/schemdraw/dsp/.ipynb_checkpoints/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7985 2021-01-17 03:22:02.000000 schemdraw-0.9.1/schemdraw/dsp/.ipynb_checkpoints/dsp-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      737 2020-12-18 16:01:07.000000 schemdraw-0.9.1/schemdraw/dsp/.ipynb_checkpoints/legacy-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      584 2020-12-18 16:01:07.000000 schemdraw-0.9.1/schemdraw/dsp/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7985 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/dsp/dsp.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      737 2020-12-18 16:01:07.000000 schemdraw-0.9.1/schemdraw/dsp/legacy.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.738102 schemdraw-0.9.1/schemdraw/elements/
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.745102 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3071 2021-01-16 17:28:40.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6768 2021-01-16 17:40:44.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/cables-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8383 2021-01-29 03:17:37.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/compound-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    15861 2021-01-29 02:43:01.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/connectors-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    32010 2021-01-29 03:19:57.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/elements-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    29518 2021-01-29 03:23:47.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/intcircuits-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6595 2021-01-03 19:50:38.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/legacy-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    11628 2021-01-29 03:24:22.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/lines-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5973 2021-01-17 02:33:05.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/misc-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4750 2021-01-17 02:39:43.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/oneterm-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1718 2021-01-17 02:42:30.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/opamp-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    13606 2021-01-16 17:13:48.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/outlets-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7164 2021-01-17 02:47:44.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/sources-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10413 2021-01-17 02:53:32.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/switches-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8256 2021-01-18 00:20:54.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/transistors-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    19636 2021-01-29 03:25:25.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/twoterm-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3899 2021-01-17 02:59:00.000000 schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/xform-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3071 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/elements/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6768 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/elements/cables.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8383 2021-01-30 00:05:53.000000 schemdraw-0.9.1/schemdraw/elements/compound.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    15861 2021-01-30 00:05:53.000000 schemdraw-0.9.1/schemdraw/elements/connectors.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    32010 2021-01-30 00:05:53.000000 schemdraw-0.9.1/schemdraw/elements/elements.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    29518 2021-01-30 00:05:53.000000 schemdraw-0.9.1/schemdraw/elements/intcircuits.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6595 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/elements/legacy.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    11628 2021-01-30 00:05:53.000000 schemdraw-0.9.1/schemdraw/elements/lines.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5973 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/elements/misc.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4750 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/elements/oneterm.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1718 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/elements/opamp.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    13606 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/elements/outlets.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     7164 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/elements/sources.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    10413 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/elements/switches.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     8256 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/elements/transistors.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    19636 2021-01-30 00:05:53.000000 schemdraw-0.9.1/schemdraw/elements/twoterm.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3899 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/elements/xform.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.745102 schemdraw-0.9.1/schemdraw/flow/
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.745102 schemdraw-0.9.1/schemdraw/flow/.ipynb_checkpoints/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6172 2021-01-17 03:24:58.000000 schemdraw-0.9.1/schemdraw/flow/.ipynb_checkpoints/flow-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      467 2020-12-18 16:01:07.000000 schemdraw-0.9.1/schemdraw/flow/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6172 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/flow/flow.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      668 2020-12-18 16:01:07.000000 schemdraw-0.9.1/schemdraw/flow/legacy.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.746101 schemdraw-0.9.1/schemdraw/logic/
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.746101 schemdraw-0.9.1/schemdraw/logic/.ipynb_checkpoints/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1133 2020-12-18 16:01:07.000000 schemdraw-0.9.1/schemdraw/logic/.ipynb_checkpoints/legacy-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    11429 2021-01-17 03:32:50.000000 schemdraw-0.9.1/schemdraw/logic/.ipynb_checkpoints/logic-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      522 2020-12-18 16:01:07.000000 schemdraw-0.9.1/schemdraw/logic/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1133 2020-12-18 16:01:07.000000 schemdraw-0.9.1/schemdraw/logic/legacy.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    11429 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/logic/logic.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.746101 schemdraw-0.9.1/schemdraw/parsing/
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.747102 schemdraw-0.9.1/schemdraw/parsing/.ipynb_checkpoints/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       36 2020-12-18 16:01:07.000000 schemdraw-0.9.1/schemdraw/parsing/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4789 2020-12-18 16:01:07.000000 schemdraw-0.9.1/schemdraw/parsing/.ipynb_checkpoints/buchheim-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5488 2021-01-02 23:58:50.000000 schemdraw-0.9.1/schemdraw/parsing/.ipynb_checkpoints/logic_parser-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       36 2020-12-18 16:01:07.000000 schemdraw-0.9.1/schemdraw/parsing/__init__.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     4789 2020-12-18 16:01:07.000000 schemdraw-0.9.1/schemdraw/parsing/buchheim.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     5488 2021-01-23 23:03:29.000000 schemdraw-0.9.1/schemdraw/parsing/logic_parser.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    17217 2021-01-30 20:31:00.000000 schemdraw-0.9.1/schemdraw/schemdraw.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    27824 2021-01-30 00:05:53.000000 schemdraw-0.9.1/schemdraw/segments.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1863 2021-01-30 00:05:53.000000 schemdraw-0.9.1/schemdraw/transform.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1274 2021-01-29 02:49:18.000000 schemdraw-0.9.1/schemdraw/types.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     3148 2021-01-30 00:05:53.000000 schemdraw-0.9.1/schemdraw/util.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.729102 schemdraw-0.9.1/schemdraw.egg-info/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1933 2021-01-30 21:48:25.000000 schemdraw-0.9.1/schemdraw.egg-info/PKG-INFO
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     6940 2021-01-30 21:48:25.000000 schemdraw-0.9.1/schemdraw.egg-info/SOURCES.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)        1 2021-01-30 21:48:25.000000 schemdraw-0.9.1/schemdraw.egg-info/dependency_links.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       10 2021-01-30 21:48:25.000000 schemdraw-0.9.1/schemdraw.egg-info/top_level.txt
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)       38 2021-01-30 21:48:25.770102 schemdraw-0.9.1/setup.cfg
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1407 2021-01-30 21:47:55.000000 schemdraw-0.9.1/setup.py
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.756101 schemdraw-0.9.1/test/
+drwxr-xr-x   0 collindelker  (1000) collindelker  (1000)        0 2021-01-30 21:48:25.769101 schemdraw-0.9.1/test/.ipynb_checkpoints/
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1405449 2020-12-31 02:39:29.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/gallery_legacy-checkpoint.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      353 2021-01-26 20:08:36.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/schematic-checkpoint.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   131190 2021-01-30 19:37:27.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/test_backend-checkpoint.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1742566 2020-12-31 02:57:33.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/test_cases_legacy-checkpoint.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   195091 2021-01-30 19:37:36.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/test_dsp-checkpoint.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1876417 2021-01-30 19:37:56.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/test_elements-checkpoint.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   387409 2021-01-30 19:38:21.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/test_elements2-checkpoint.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    51822 2021-01-30 19:38:41.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/test_flow-checkpoint.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1857556 2021-01-30 19:40:15.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/test_gallery-checkpoint.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1597000 2021-01-30 19:39:24.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/test_gallery_kwargs-checkpoint.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   279222 2021-01-30 19:40:38.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/test_intcircuits-checkpoint.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   339678 2021-01-30 19:41:03.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/test_logic-checkpoint.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   130781 2021-01-30 19:41:15.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/test_parselogic-checkpoint.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   652834 2021-01-30 19:41:53.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/test_placement-checkpoint.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   137708 2021-01-30 19:42:18.000000 schemdraw-0.9.1/test/.ipynb_checkpoints/test_styles-checkpoint.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      297 2021-01-23 23:03:29.000000 schemdraw-0.9.1/test/headless.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      685 2021-01-30 20:07:01.000000 schemdraw-0.9.1/test/savetest.png
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)      353 2021-01-26 20:33:49.000000 schemdraw-0.9.1/test/schematic.py
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)     1122 2021-01-30 20:07:01.000000 schemdraw-0.9.1/test/testMPL.png
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   131190 2021-01-30 19:37:27.000000 schemdraw-0.9.1/test/test_backend.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   195091 2021-01-30 19:37:36.000000 schemdraw-0.9.1/test/test_dsp.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1876417 2021-01-30 19:37:56.000000 schemdraw-0.9.1/test/test_elements.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   387409 2021-01-30 19:38:21.000000 schemdraw-0.9.1/test/test_elements2.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)    51822 2021-01-30 19:38:41.000000 schemdraw-0.9.1/test/test_flow.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1857556 2021-01-30 19:40:15.000000 schemdraw-0.9.1/test/test_gallery.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)  1597000 2021-01-30 19:39:24.000000 schemdraw-0.9.1/test/test_gallery_kwargs.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   279222 2021-01-30 19:40:38.000000 schemdraw-0.9.1/test/test_intcircuits.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   339678 2021-01-30 19:41:03.000000 schemdraw-0.9.1/test/test_logic.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   130781 2021-01-30 19:41:15.000000 schemdraw-0.9.1/test/test_parselogic.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   652834 2021-01-30 19:41:53.000000 schemdraw-0.9.1/test/test_placement.ipynb
+-rw-r--r--   0 collindelker  (1000) collindelker  (1000)   137708 2021-01-30 19:42:18.000000 schemdraw-0.9.1/test/test_styles.ipynb
```

### Comparing `schemdraw-0.9/CHANGES.txt` & `schemdraw-0.9.1/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/LICENSE.txt` & `schemdraw-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/PKG-INFO` & `schemdraw-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemdraw
-Version: 0.9
+Version: 0.9.1
 Summary: Electrical circuit schematic drawing
 Home-page: https://schemdraw.readthedocs.io/
 Author: Collin J. Delker
 Author-email: schemdraw@collindelker.com
 License: UNKNOWN
 Project-URL: Source, https://bitbucket.org/cdelker/schemdraw
 Description: # schemdraw
```

### Comparing `schemdraw-0.9/README.txt` & `schemdraw-0.9.1/README.txt`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/.ipynb_checkpoints/conf-checkpoint.py` & `schemdraw-0.9.1/docs/.ipynb_checkpoints/conf-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/.ipynb_checkpoints/index-checkpoint.rst` & `schemdraw-0.9.1/docs/.ipynb_checkpoints/index-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/Makefile` & `schemdraw-0.9.1/docs/.ipynb_checkpoints/Makefile-checkpoint`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/classes/.ipynb_checkpoints/drawing-checkpoint.rst` & `schemdraw-0.9.1/docs/classes/.ipynb_checkpoints/drawing-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/classes/.ipynb_checkpoints/electrical-checkpoint.rst` & `schemdraw-0.9.1/docs/classes/.ipynb_checkpoints/electrical-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/classes/drawing.rst` & `schemdraw-0.9.1/docs/classes/drawing.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/classes/electrical.rst` & `schemdraw-0.9.1/docs/classes/electrical.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/conf.py` & `schemdraw-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/elements/.ipynb_checkpoints/compound-checkpoint.rst` & `schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/compound-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/elements/.ipynb_checkpoints/connectors-checkpoint.rst` & `schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/connectors-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/elements/.ipynb_checkpoints/dsp-checkpoint.rst` & `schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/dsp-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/elements/.ipynb_checkpoints/electrical-checkpoint.rst` & `schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/electrical-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/elements/.ipynb_checkpoints/flow-checkpoint.rst` & `schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/flow-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/elements/.ipynb_checkpoints/intcircuits-checkpoint.rst` & `schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/intcircuits-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/elements/.ipynb_checkpoints/logic-checkpoint.rst` & `schemdraw-0.9.1/docs/elements/.ipynb_checkpoints/logic-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/elements/compound.rst` & `schemdraw-0.9.1/docs/elements/compound.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/elements/connectors.rst` & `schemdraw-0.9.1/docs/elements/connectors.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/elements/dsp.rst` & `schemdraw-0.9.1/docs/elements/dsp.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/elements/electrical.rst` & `schemdraw-0.9.1/docs/elements/electrical.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/elements/flow.rst` & `schemdraw-0.9.1/docs/elements/flow.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/elements/intcircuits.rst` & `schemdraw-0.9.1/docs/elements/intcircuits.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/elements/logic.rst` & `schemdraw-0.9.1/docs/elements/logic.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/.ipynb_checkpoints/analog-checkpoint.rst` & `schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/analog-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/.ipynb_checkpoints/flowcharting-checkpoint.rst` & `schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/flowcharting-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/.ipynb_checkpoints/ic-checkpoint.rst` & `schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/ic-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/.ipynb_checkpoints/logicgate-checkpoint.rst` & `schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/logicgate-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/.ipynb_checkpoints/opamp-checkpoint.rst` & `schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/opamp-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/.ipynb_checkpoints/signalproc-checkpoint.rst` & `schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/signalproc-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/.ipynb_checkpoints/solidstate-checkpoint.rst` & `schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/solidstate-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/.ipynb_checkpoints/styles-checkpoint.rst` & `schemdraw-0.9.1/docs/gallery/.ipynb_checkpoints/styles-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/analog.rst` & `schemdraw-0.9.1/docs/gallery/analog.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/flowcharting.rst` & `schemdraw-0.9.1/docs/gallery/flowcharting.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/ic.rst` & `schemdraw-0.9.1/docs/gallery/ic.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/logicgate.rst` & `schemdraw-0.9.1/docs/gallery/logicgate.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/opamp.rst` & `schemdraw-0.9.1/docs/gallery/opamp.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/signalproc.rst` & `schemdraw-0.9.1/docs/gallery/signalproc.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/solidstate.rst` & `schemdraw-0.9.1/docs/gallery/solidstate.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/gallery/styles.rst` & `schemdraw-0.9.1/docs/gallery/styles.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/index.rst` & `schemdraw-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/make.bat` & `schemdraw-0.9.1/docs/.ipynb_checkpoints/make-checkpoint.bat`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/usage/.ipynb_checkpoints/customizing-checkpoint.rst` & `schemdraw-0.9.1/docs/usage/.ipynb_checkpoints/customizing-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/usage/.ipynb_checkpoints/placement-checkpoint.rst` & `schemdraw-0.9.1/docs/usage/.ipynb_checkpoints/placement-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/usage/.ipynb_checkpoints/start-checkpoint.rst` & `schemdraw-0.9.1/docs/usage/.ipynb_checkpoints/start-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/usage/customizing.rst` & `schemdraw-0.9.1/docs/usage/customizing.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/usage/placement.rst` & `schemdraw-0.9.1/docs/usage/placement.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/docs/usage/start.rst` & `schemdraw-0.9.1/docs/usage/start.rst`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/.ipynb_checkpoints/schemdraw-checkpoint.py` & `schemdraw-0.9.1/schemdraw/.ipynb_checkpoints/schemdraw-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/.ipynb_checkpoints/segments-checkpoint.py` & `schemdraw-0.9.1/schemdraw/.ipynb_checkpoints/segments-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/.ipynb_checkpoints/transform-checkpoint.py` & `schemdraw-0.9.1/schemdraw/.ipynb_checkpoints/transform-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/.ipynb_checkpoints/types-checkpoint.py` & `schemdraw-0.9.1/schemdraw/.ipynb_checkpoints/types-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/.ipynb_checkpoints/util-checkpoint.py` & `schemdraw-0.9.1/schemdraw/.ipynb_checkpoints/util-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/backends/.ipynb_checkpoints/mpl-checkpoint.py` & `schemdraw-0.9.1/schemdraw/backends/.ipynb_checkpoints/mpl-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/backends/.ipynb_checkpoints/svg-checkpoint.py` & `schemdraw-0.9.1/schemdraw/backends/.ipynb_checkpoints/svg-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/backends/.ipynb_checkpoints/svgdisplay-checkpoint.py` & `schemdraw-0.9.1/schemdraw/backends/.ipynb_checkpoints/svgdisplay-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/backends/.ipynb_checkpoints/svgtext-checkpoint.py` & `schemdraw-0.9.1/schemdraw/backends/.ipynb_checkpoints/svgtext-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/backends/mpl.py` & `schemdraw-0.9.1/schemdraw/backends/mpl.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/backends/svg.py` & `schemdraw-0.9.1/schemdraw/backends/svg.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/backends/svgtext.py` & `schemdraw-0.9.1/schemdraw/backends/svgtext.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/dsp/.ipynb_checkpoints/dsp-checkpoint.py` & `schemdraw-0.9.1/schemdraw/dsp/.ipynb_checkpoints/dsp-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/dsp/.ipynb_checkpoints/legacy-checkpoint.py` & `schemdraw-0.9.1/schemdraw/dsp/.ipynb_checkpoints/legacy-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/dsp/__init__.py` & `schemdraw-0.9.1/schemdraw/dsp/__init__.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/dsp/dsp.py` & `schemdraw-0.9.1/schemdraw/dsp/dsp.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/dsp/legacy.py` & `schemdraw-0.9.1/schemdraw/dsp/legacy.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/__init__-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/__init__-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/cables-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/cables-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/compound-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/compound-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/connectors-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/connectors-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/elements-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/elements-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/intcircuits-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/intcircuits-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/legacy-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/legacy-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/lines-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/lines-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/misc-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/misc-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/oneterm-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/oneterm-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/opamp-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/opamp-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/outlets-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/outlets-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/sources-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/sources-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/switches-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/switches-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/transistors-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/transistors-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/twoterm-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/twoterm-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/.ipynb_checkpoints/xform-checkpoint.py` & `schemdraw-0.9.1/schemdraw/elements/.ipynb_checkpoints/xform-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/__init__.py` & `schemdraw-0.9.1/schemdraw/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/cables.py` & `schemdraw-0.9.1/schemdraw/elements/cables.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/compound.py` & `schemdraw-0.9.1/schemdraw/elements/compound.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/connectors.py` & `schemdraw-0.9.1/schemdraw/elements/connectors.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/elements.py` & `schemdraw-0.9.1/schemdraw/elements/elements.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/intcircuits.py` & `schemdraw-0.9.1/schemdraw/elements/intcircuits.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/legacy.py` & `schemdraw-0.9.1/schemdraw/elements/legacy.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/lines.py` & `schemdraw-0.9.1/schemdraw/elements/lines.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/misc.py` & `schemdraw-0.9.1/schemdraw/elements/misc.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/oneterm.py` & `schemdraw-0.9.1/schemdraw/elements/oneterm.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/opamp.py` & `schemdraw-0.9.1/schemdraw/elements/opamp.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/outlets.py` & `schemdraw-0.9.1/schemdraw/elements/outlets.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/sources.py` & `schemdraw-0.9.1/schemdraw/elements/sources.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/switches.py` & `schemdraw-0.9.1/schemdraw/elements/switches.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/transistors.py` & `schemdraw-0.9.1/schemdraw/elements/transistors.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/twoterm.py` & `schemdraw-0.9.1/schemdraw/elements/twoterm.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/elements/xform.py` & `schemdraw-0.9.1/schemdraw/elements/xform.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/flow/.ipynb_checkpoints/flow-checkpoint.py` & `schemdraw-0.9.1/schemdraw/flow/.ipynb_checkpoints/flow-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/flow/flow.py` & `schemdraw-0.9.1/schemdraw/flow/flow.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/flow/legacy.py` & `schemdraw-0.9.1/schemdraw/flow/legacy.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/logic/.ipynb_checkpoints/legacy-checkpoint.py` & `schemdraw-0.9.1/schemdraw/logic/.ipynb_checkpoints/legacy-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/logic/.ipynb_checkpoints/logic-checkpoint.py` & `schemdraw-0.9.1/schemdraw/logic/.ipynb_checkpoints/logic-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/logic/__init__.py` & `schemdraw-0.9.1/schemdraw/logic/__init__.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/logic/legacy.py` & `schemdraw-0.9.1/schemdraw/logic/legacy.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/logic/logic.py` & `schemdraw-0.9.1/schemdraw/logic/logic.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/parsing/.ipynb_checkpoints/buchheim-checkpoint.py` & `schemdraw-0.9.1/schemdraw/parsing/.ipynb_checkpoints/buchheim-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/parsing/.ipynb_checkpoints/logic_parser-checkpoint.py` & `schemdraw-0.9.1/schemdraw/parsing/.ipynb_checkpoints/logic_parser-checkpoint.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/parsing/buchheim.py` & `schemdraw-0.9.1/schemdraw/parsing/buchheim.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/parsing/logic_parser.py` & `schemdraw-0.9.1/schemdraw/parsing/logic_parser.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/schemdraw.py` & `schemdraw-0.9.1/schemdraw/schemdraw.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/segments.py` & `schemdraw-0.9.1/schemdraw/segments.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/transform.py` & `schemdraw-0.9.1/schemdraw/transform.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/types.py` & `schemdraw-0.9.1/schemdraw/types.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw/util.py` & `schemdraw-0.9.1/schemdraw/util.py`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/schemdraw.egg-info/PKG-INFO` & `schemdraw-0.9.1/schemdraw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemdraw
-Version: 0.9
+Version: 0.9.1
 Summary: Electrical circuit schematic drawing
 Home-page: https://schemdraw.readthedocs.io/
 Author: Collin J. Delker
 Author-email: schemdraw@collindelker.com
 License: UNKNOWN
 Project-URL: Source, https://bitbucket.org/cdelker/schemdraw
 Description: # schemdraw
```

### Comparing `schemdraw-0.9/schemdraw.egg-info/SOURCES.txt` & `schemdraw-0.9.1/schemdraw.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 setup.py
 docs/Makefile
 docs/changes.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/requirements.txt
+docs/.ipynb_checkpoints/Makefile-checkpoint
 docs/.ipynb_checkpoints/conf-checkpoint.py
 docs/.ipynb_checkpoints/index-checkpoint.rst
+docs/.ipynb_checkpoints/make-checkpoint.bat
+docs/.ipynb_checkpoints/requirements-checkpoint.txt
 docs/classes/drawing.rst
 docs/classes/dsp.rst
 docs/classes/electrical.rst
 docs/classes/flow.rst
 docs/classes/index.rst
 docs/classes/logic.rst
 docs/classes/segments.rst
@@ -136,14 +139,15 @@
 schemdraw/logic/legacy.py
 schemdraw/logic/logic.py
 schemdraw/logic/.ipynb_checkpoints/legacy-checkpoint.py
 schemdraw/logic/.ipynb_checkpoints/logic-checkpoint.py
 schemdraw/parsing/__init__.py
 schemdraw/parsing/buchheim.py
 schemdraw/parsing/logic_parser.py
+schemdraw/parsing/.ipynb_checkpoints/__init__-checkpoint.py
 schemdraw/parsing/.ipynb_checkpoints/buchheim-checkpoint.py
 schemdraw/parsing/.ipynb_checkpoints/logic_parser-checkpoint.py
 test/headless.py
 test/savetest.png
 test/schematic.py
 test/testMPL.png
 test/test_backend.ipynb
```

### Comparing `schemdraw-0.9/setup.py` & `schemdraw-0.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.txt', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name = 'schemdraw',
-    version = '0.9',
+    version = '0.9.1',
     description = 'Electrical circuit schematic drawing',
     author = 'Collin J. Delker',
     author_email = 'schemdraw@collindelker.com',
     url = 'https://schemdraw.readthedocs.io/',
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
@@ -18,14 +18,15 @@
     python_requires='>=3.7',
     packages = ['schemdraw',
                 'schemdraw.elements',
                 'schemdraw.logic',
                 'schemdraw.dsp',
                 'schemdraw.flow',
                 'schemdraw.backends',
+                'schemdraw.parsing'
                ],
     package_dir={'schemdraw': 'schemdraw'},
     keywords = ['circuit', 'schematic', 'electrical', 'flowchart', 'logic'],
     install_requires=[],
     classifiers = [
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
```

### Comparing `schemdraw-0.9/test/.ipynb_checkpoints/gallery_legacy-checkpoint.ipynb` & `schemdraw-0.9.1/test/.ipynb_checkpoints/gallery_legacy-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/.ipynb_checkpoints/test_backend-checkpoint.ipynb` & `schemdraw-0.9.1/test/.ipynb_checkpoints/test_backend-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/.ipynb_checkpoints/test_cases_legacy-checkpoint.ipynb` & `schemdraw-0.9.1/test/.ipynb_checkpoints/test_cases_legacy-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/.ipynb_checkpoints/test_dsp-checkpoint.ipynb` & `schemdraw-0.9.1/test/.ipynb_checkpoints/test_dsp-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/.ipynb_checkpoints/test_elements-checkpoint.ipynb` & `schemdraw-0.9.1/test/.ipynb_checkpoints/test_elements-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/.ipynb_checkpoints/test_elements2-checkpoint.ipynb` & `schemdraw-0.9.1/test/.ipynb_checkpoints/test_elements2-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/.ipynb_checkpoints/test_flow-checkpoint.ipynb` & `schemdraw-0.9.1/test/.ipynb_checkpoints/test_flow-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/.ipynb_checkpoints/test_gallery-checkpoint.ipynb` & `schemdraw-0.9.1/test/.ipynb_checkpoints/test_gallery-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/.ipynb_checkpoints/test_gallery_kwargs-checkpoint.ipynb` & `schemdraw-0.9.1/test/.ipynb_checkpoints/test_gallery_kwargs-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/.ipynb_checkpoints/test_intcircuits-checkpoint.ipynb` & `schemdraw-0.9.1/test/.ipynb_checkpoints/test_intcircuits-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/.ipynb_checkpoints/test_logic-checkpoint.ipynb` & `schemdraw-0.9.1/test/.ipynb_checkpoints/test_logic-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/.ipynb_checkpoints/test_parselogic-checkpoint.ipynb` & `schemdraw-0.9.1/test/.ipynb_checkpoints/test_parselogic-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/.ipynb_checkpoints/test_placement-checkpoint.ipynb` & `schemdraw-0.9.1/test/.ipynb_checkpoints/test_placement-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/.ipynb_checkpoints/test_styles-checkpoint.ipynb` & `schemdraw-0.9.1/test/.ipynb_checkpoints/test_styles-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/savetest.png` & `schemdraw-0.9.1/test/savetest.png`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/testMPL.png` & `schemdraw-0.9.1/test/testMPL.png`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/test_backend.ipynb` & `schemdraw-0.9.1/test/test_backend.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/test_dsp.ipynb` & `schemdraw-0.9.1/test/test_dsp.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/test_elements.ipynb` & `schemdraw-0.9.1/test/test_elements.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/test_elements2.ipynb` & `schemdraw-0.9.1/test/test_elements2.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/test_flow.ipynb` & `schemdraw-0.9.1/test/test_flow.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/test_gallery.ipynb` & `schemdraw-0.9.1/test/test_gallery.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/test_gallery_kwargs.ipynb` & `schemdraw-0.9.1/test/test_gallery_kwargs.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/test_intcircuits.ipynb` & `schemdraw-0.9.1/test/test_intcircuits.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/test_logic.ipynb` & `schemdraw-0.9.1/test/test_logic.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/test_parselogic.ipynb` & `schemdraw-0.9.1/test/test_parselogic.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/test_placement.ipynb` & `schemdraw-0.9.1/test/test_placement.ipynb`

 * *Files identical despite different names*

### Comparing `schemdraw-0.9/test/test_styles.ipynb` & `schemdraw-0.9.1/test/test_styles.ipynb`

 * *Files identical despite different names*

