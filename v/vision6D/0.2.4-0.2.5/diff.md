# Comparing `tmp/vision6D-0.2.4.tar.gz` & `tmp/vision6D-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.2.4.tar", last modified: Fri Jun  2 03:38:43 2023, max compression
+gzip compressed data, was "dist\vision6D-0.2.5.tar", last modified: Sat Jun  3 17:58:00 2023, max compression
```

## Comparing `vision6D-0.2.4.tar` & `vision6D-0.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 03:38:43.519089 vision6D-0.2.4/
--rw-rw-rw-   0        0        0     1086 2023-06-01 02:48:31.000000 vision6D-0.2.4/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1361 2023-06-02 03:38:43.520090 vision6D-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-06-01 02:48:31.000000 vision6D-0.2.4/README.md
--rw-rw-rw-   0        0        0      406 2023-06-01 02:48:31.000000 vision6D-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0     2042 2023-06-02 03:38:43.523137 vision6D-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      282 2023-06-01 02:48:31.000000 vision6D-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 03:38:43.265176 vision6D-0.2.4/test/
--rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.2.4/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.2.4/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-06-02 03:38:43.388173 vision6D-0.2.4/vision6D/
--rw-rw-rw-   0        0        0    51909 2023-06-02 01:15:28.000000 vision6D-0.2.4/vision6D/GUI.py
--rw-rw-rw-   0        0        0      913 2023-06-01 02:48:31.000000 vision6D-0.2.4/vision6D/__init__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.2.4/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-06-01 02:48:31.000000 vision6D-0.2.4/vision6D/config.py
-drwxrwxrwx   0        0        0        0 2023-06-02 03:38:43.517088 vision6D-0.2.4/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.2.4/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.2.4/vision6D/data/ossiclesCoordinateMappingv1.json
--rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.2.4/vision6D/data/style.qss
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.2.4/vision6D/interface.py
--rw-rw-rw-   0        0        0    26253 2023-06-01 02:48:31.000000 vision6D-0.2.4/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.2.4/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.2.4/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.2.4/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.2.4/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 03:38:43.455549 vision6D-0.2.4/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1361 2023-06-02 03:38:42.000000 vision6D-0.2.4/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2023-06-02 03:38:42.000000 vision6D-0.2.4/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 03:38:42.000000 vision6D-0.2.4/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-02 03:38:42.000000 vision6D-0.2.4/vision6D.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      276 2023-06-02 03:38:42.000000 vision6D-0.2.4/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-02 03:38:42.000000 vision6D-0.2.4/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 17:57:59.774731 vision6D-0.2.5/
+-rw-rw-rw-   0        0        0     1086 2023-06-02 21:40:49.000000 vision6D-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1361 2023-06-03 17:57:59.774731 vision6D-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-06-02 21:40:49.000000 vision6D-0.2.5/README.md
+-rw-rw-rw-   0        0        0      406 2023-06-02 21:40:49.000000 vision6D-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0     2050 2023-06-03 17:57:59.780997 vision6D-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      282 2023-06-02 21:40:49.000000 vision6D-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 17:57:59.629091 vision6D-0.2.5/test/
+-rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.2.5/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.2.5/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-06-03 17:57:59.657094 vision6D-0.2.5/vision6D/
+-rw-rw-rw-   0        0        0    52546 2023-06-03 17:56:36.000000 vision6D-0.2.5/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      913 2023-06-02 21:40:49.000000 vision6D-0.2.5/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.2.5/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-06-02 21:40:49.000000 vision6D-0.2.5/vision6D/config.py
+drwxrwxrwx   0        0        0        0 2023-06-03 17:57:59.771936 vision6D-0.2.5/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.2.5/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.2.5/vision6D/data/ossiclesCoordinateMappingv1.json
+-rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.2.5/vision6D/data/style.qss
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.2.5/vision6D/interface.py
+-rw-rw-rw-   0        0        0    27853 2023-06-03 17:53:50.000000 vision6D-0.2.5/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.2.5/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.2.5/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.2.5/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.2.5/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-03 17:57:59.727091 vision6D-0.2.5/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1361 2023-06-03 17:57:59.000000 vision6D-0.2.5/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2023-06-03 17:57:59.000000 vision6D-0.2.5/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 17:57:59.000000 vision6D-0.2.5/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-03 17:57:59.000000 vision6D-0.2.5/vision6D.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2023-06-03 17:57:59.000000 vision6D-0.2.5/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 17:57:59.000000 vision6D-0.2.5/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.2.4/LICENSE` & `vision6D-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.4/PKG-INFO` & `vision6D-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.2.4
+Version: 0.2.5
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.2.4/README.md` & `vision6D-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.4/setup.cfg` & `vision6D-0.2.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e32 2e34 0d0a 7572  sion = 0.2.4..ur
+00000020: 7369 6f6e 203d 2030 2e32 2e35 0d0a 7572  sion = 0.2.5..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
@@ -45,84 +45,85 @@
 000002c0: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
 000002d0: 7320 3d20 3e3d 2033 2e36 0d0a 7465 7374  s = >= 3.6..test
 000002e0: 5f73 7569 7465 203d 2074 6573 7473 0d0a  _suite = tests..
 000002f0: 7365 7475 705f 7265 7175 6972 6573 203d  setup_requires =
 00000300: 200d 0a09 7365 7475 7074 6f6f 6c73 0d0a   ...setuptools..
 00000310: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
 00000320: 203d 200d 0a09 7079 7669 7374 613e 3d30   = ...pyvista>=0
-00000330: 2e33 392e 310d 0a09 6e75 6d70 790d 0a09  .39.1...numpy...
-00000340: 6d61 7470 6c6f 746c 6962 3e3d 332e 352e  matplotlib>=3.5.
-00000350: 320d 0a09 7472 696d 6573 683e 3d33 2e31  2...trimesh>=3.1
-00000360: 342e 300d 0a09 6561 7379 6469 6374 3e3d  4.0...easydict>=
-00000370: 312e 390d 0a09 7069 6c6c 6f77 3e3d 392e  1.9...pillow>=9.
-00000380: 322e 300d 0a09 7363 6970 793e 3d31 2e38  2.0...scipy>=1.8
-00000390: 2e31 0d0a 0970 7974 6573 743e 3d37 2e32  .1...pytest>=7.2
-000003a0: 2e30 0d0a 0970 7974 6573 742d 6c61 7a79  .0...pytest-lazy
-000003b0: 2d66 6978 7475 7265 3e3d 302e 362e 330d  -fixture>=0.6.3.
-000003c0: 0a09 7072 652d 636f 6d6d 6974 3e3d 322e  ..pre-commit>=2.
-000003d0: 3231 2e30 0d0a 096f 7065 6e63 762d 7079  21.0...opencv-py
-000003e0: 7468 6f6e 2d68 6561 646c 6573 733e 3d34  thon-headless>=4
-000003f0: 2e37 2e30 2e36 380d 0a09 7363 696b 6974  .7.0.68...scikit
-00000400: 2d69 6d61 6765 3e3d 302e 3139 2e33 0d0a  -image>=0.19.3..
-00000410: 0963 6861 7264 6574 3e3d 352e 312e 300d  .chardet>=5.1.0.
-00000420: 0a09 7079 6765 6f64 6573 6963 3e3d 302e  ..pygeodesic>=0.
-00000430: 312e 380d 0a09 5079 5174 353e 3d35 2e31  1.8...PyQt5>=5.1
-00000440: 352e 390d 0a09 7079 7669 7374 6171 743e  5.9...pyvistaqt>
-00000450: 3d30 2e31 302e 300d 0a0d 0a5b 6f70 7469  =0.10.0....[opti
-00000460: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
-00000470: 5d0d 0a2a 203d 202a 2e70 6e67 2c20 2a2e  ]..* = *.png, *.
-00000480: 6a70 672c 202a 2e71 6d6c 0d0a 0d0a 5b62  jpg, *.qml....[b
-00000490: 6469 7374 5f77 6865 656c 5d0d 0a75 6e69  dist_wheel]..uni
-000004a0: 7665 7273 616c 203d 2074 7275 650d 0a0d  versal = true...
-000004b0: 0a5b 7364 6973 745d 0d0a 666f 726d 6174  .[sdist]..format
-000004c0: 7320 3d20 7a69 702c 2067 7a74 6172 0d0a  s = zip, gztar..
-000004d0: 0d0a 5b63 6f76 6572 6167 653a 7265 706f  ..[coverage:repo
-000004e0: 7274 5d0d 0a73 686f 775f 6d69 7373 696e  rt]..show_missin
-000004f0: 6720 3d20 7472 7565 0d0a 6578 636c 7564  g = true..exclud
-00000500: 655f 6c69 6e65 7320 3d20 0d0a 0970 7261  e_lines = ...pra
-00000510: 676d 613a 206e 6f20 636f 7665 720d 0a09  gma: no cover...
-00000520: 6966 2046 616c 7365 0d0a 0d0a 5b67 7265  if False....[gre
-00000530: 656e 5d0d 0a66 696c 652d 7061 7474 6572  en]..file-patter
-00000540: 6e20 3d20 7465 7374 5f2a 2e70 790d 0a76  n = test_*.py..v
-00000550: 6572 626f 7365 203d 2032 0d0a 6e6f 2d73  erbose = 2..no-s
-00000560: 6b69 702d 7265 706f 7274 203d 2074 7275  kip-report = tru
-00000570: 650d 0a71 7569 6574 2d73 7464 6f75 7420  e..quiet-stdout 
-00000580: 3d20 7472 7565 0d0a 7275 6e2d 636f 7665  = true..run-cove
-00000590: 7261 6765 203d 2074 7275 650d 0a0d 0a5b  rage = true....[
-000005a0: 7079 646f 6373 7479 6c65 5d0d 0a6d 6174  pydocstyle]..mat
-000005b0: 6368 2d64 6972 203d 2028 3f21 7465 7374  ch-dir = (?!test
-000005c0: 7329 283f 2172 6573 6f75 7263 6573 2928  s)(?!resources)(
-000005d0: 3f21 646f 6373 295b 5e5c 2e5d 2e2a 0d0a  ?!docs)[^\.].*..
-000005e0: 6d61 7463 6820 3d20 283f 2174 6573 7429  match = (?!test)
-000005f0: 283f 2173 6574 7570 295b 5e5c 2e5f 5d2e  (?!setup)[^\._].
-00000600: 2a5c 2e70 790d 0a69 6e68 6572 6974 203d  *\.py..inherit =
-00000610: 2066 616c 7365 0d0a 6967 6e6f 7265 203d   false..ignore =
-00000620: 2044 3230 302c 2044 3230 332c 2044 3231   D200, D203, D21
-00000630: 332c 2044 3430 362c 2044 3430 370d 0a0d  3, D406, D407...
-00000640: 0a5b 666c 616b 6538 5d0d 0a6d 6178 2d6c  .[flake8]..max-l
-00000650: 696e 652d 6c65 6e67 7468 203d 2039 390d  ine-length = 99.
-00000660: 0a64 6f63 7465 7374 7320 3d20 5472 7565  .doctests = True
-00000670: 0d0a 6578 636c 7564 6520 3d20 2e67 6974  ..exclude = .git
-00000680: 2c20 2e65 6767 732c 205f 5f70 7963 6163  , .eggs, __pycac
-00000690: 6865 5f5f 2c20 7465 7374 732f 2c20 646f  he__, tests/, do
-000006a0: 6373 2f2c 2062 7569 6c64 2f2c 2064 6973  cs/, build/, dis
-000006b0: 742f 0d0a 0d0a 5b6d 7970 795d 0d0a 6469  t/....[mypy]..di
-000006c0: 7361 6c6c 6f77 5f61 6e79 5f64 6563 6f72  sallow_any_decor
-000006d0: 6174 6564 203d 2074 7275 650d 0a64 6973  ated = true..dis
-000006e0: 616c 6c6f 775f 616e 795f 6765 6e65 7269  allow_any_generi
-000006f0: 6373 203d 2074 7275 650d 0a64 6973 616c  cs = true..disal
-00000700: 6c6f 775f 616e 795f 756e 696d 706f 7274  low_any_unimport
-00000710: 6564 203d 2066 616c 7365 0d0a 6469 7361  ed = false..disa
-00000720: 6c6c 6f77 5f73 7562 636c 6173 7369 6e67  llow_subclassing
-00000730: 5f61 6e79 203d 2066 616c 7365 0d0a 6469  _any = false..di
-00000740: 7361 6c6c 6f77 5f75 6e74 7970 6564 5f63  sallow_untyped_c
-00000750: 616c 6c73 203d 2074 7275 650d 0a64 6973  alls = true..dis
-00000760: 616c 6c6f 775f 756e 7479 7065 645f 6465  allow_untyped_de
-00000770: 6673 203d 2074 7275 650d 0a69 676e 6f72  fs = true..ignor
-00000780: 655f 6d69 7373 696e 675f 696d 706f 7274  e_missing_import
-00000790: 7320 3d20 7472 7565 0d0a 7761 726e 5f75  s = true..warn_u
-000007a0: 6e75 7365 645f 6967 6e6f 7265 7320 3d20  nused_ignores = 
-000007b0: 7472 7565 0d0a 7761 726e 5f72 6574 7572  true..warn_retur
-000007c0: 6e5f 616e 7920 3d20 7472 7565 0d0a 0d0a  n_any = true....
-000007d0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-000007e0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-000007f0: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000330: 2e33 392e 310d 0a09 6e75 6d70 793e 3d31  .39.1...numpy>=1
+00000340: 2e32 332e 350d 0a09 6d61 7470 6c6f 746c  .23.5...matplotl
+00000350: 6962 3e3d 332e 352e 320d 0a09 7472 696d  ib>=3.5.2...trim
+00000360: 6573 683e 3d33 2e31 342e 300d 0a09 6561  esh>=3.14.0...ea
+00000370: 7379 6469 6374 3e3d 312e 390d 0a09 7069  sydict>=1.9...pi
+00000380: 6c6c 6f77 3e3d 392e 322e 300d 0a09 7363  llow>=9.2.0...sc
+00000390: 6970 793e 3d31 2e38 2e31 0d0a 0970 7974  ipy>=1.8.1...pyt
+000003a0: 6573 743e 3d37 2e32 2e30 0d0a 0970 7974  est>=7.2.0...pyt
+000003b0: 6573 742d 6c61 7a79 2d66 6978 7475 7265  est-lazy-fixture
+000003c0: 3e3d 302e 362e 330d 0a09 7072 652d 636f  >=0.6.3...pre-co
+000003d0: 6d6d 6974 3e3d 322e 3231 2e30 0d0a 096f  mmit>=2.21.0...o
+000003e0: 7065 6e63 762d 7079 7468 6f6e 2d68 6561  pencv-python-hea
+000003f0: 646c 6573 733e 3d34 2e37 2e30 2e36 380d  dless>=4.7.0.68.
+00000400: 0a09 7363 696b 6974 2d69 6d61 6765 3e3d  ..scikit-image>=
+00000410: 302e 3139 2e33 0d0a 0963 6861 7264 6574  0.19.3...chardet
+00000420: 3e3d 352e 312e 300d 0a09 7079 6765 6f64  >=5.1.0...pygeod
+00000430: 6573 6963 3e3d 302e 312e 380d 0a09 5079  esic>=0.1.8...Py
+00000440: 5174 353e 3d35 2e31 352e 390d 0a09 7079  Qt5>=5.15.9...py
+00000450: 7669 7374 6171 743e 3d30 2e31 302e 300d  vistaqt>=0.10.0.
+00000460: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000470: 6167 655f 6461 7461 5d0d 0a2a 203d 202a  age_data]..* = *
+00000480: 2e70 6e67 2c20 2a2e 6a70 672c 202a 2e71  .png, *.jpg, *.q
+00000490: 6d6c 0d0a 0d0a 5b62 6469 7374 5f77 6865  ml....[bdist_whe
+000004a0: 656c 5d0d 0a75 6e69 7665 7273 616c 203d  el]..universal =
+000004b0: 2074 7275 650d 0a0d 0a5b 7364 6973 745d   true....[sdist]
+000004c0: 0d0a 666f 726d 6174 7320 3d20 7a69 702c  ..formats = zip,
+000004d0: 2067 7a74 6172 0d0a 0d0a 5b63 6f76 6572   gztar....[cover
+000004e0: 6167 653a 7265 706f 7274 5d0d 0a73 686f  age:report]..sho
+000004f0: 775f 6d69 7373 696e 6720 3d20 7472 7565  w_missing = true
+00000500: 0d0a 6578 636c 7564 655f 6c69 6e65 7320  ..exclude_lines 
+00000510: 3d20 0d0a 0970 7261 676d 613a 206e 6f20  = ...pragma: no 
+00000520: 636f 7665 720d 0a09 6966 2046 616c 7365  cover...if False
+00000530: 0d0a 0d0a 5b67 7265 656e 5d0d 0a66 696c  ....[green]..fil
+00000540: 652d 7061 7474 6572 6e20 3d20 7465 7374  e-pattern = test
+00000550: 5f2a 2e70 790d 0a76 6572 626f 7365 203d  _*.py..verbose =
+00000560: 2032 0d0a 6e6f 2d73 6b69 702d 7265 706f   2..no-skip-repo
+00000570: 7274 203d 2074 7275 650d 0a71 7569 6574  rt = true..quiet
+00000580: 2d73 7464 6f75 7420 3d20 7472 7565 0d0a  -stdout = true..
+00000590: 7275 6e2d 636f 7665 7261 6765 203d 2074  run-coverage = t
+000005a0: 7275 650d 0a0d 0a5b 7079 646f 6373 7479  rue....[pydocsty
+000005b0: 6c65 5d0d 0a6d 6174 6368 2d64 6972 203d  le]..match-dir =
+000005c0: 2028 3f21 7465 7374 7329 283f 2172 6573   (?!tests)(?!res
+000005d0: 6f75 7263 6573 2928 3f21 646f 6373 295b  ources)(?!docs)[
+000005e0: 5e5c 2e5d 2e2a 0d0a 6d61 7463 6820 3d20  ^\.].*..match = 
+000005f0: 283f 2174 6573 7429 283f 2173 6574 7570  (?!test)(?!setup
+00000600: 295b 5e5c 2e5f 5d2e 2a5c 2e70 790d 0a69  )[^\._].*\.py..i
+00000610: 6e68 6572 6974 203d 2066 616c 7365 0d0a  nherit = false..
+00000620: 6967 6e6f 7265 203d 2044 3230 302c 2044  ignore = D200, D
+00000630: 3230 332c 2044 3231 332c 2044 3430 362c  203, D213, D406,
+00000640: 2044 3430 370d 0a0d 0a5b 666c 616b 6538   D407....[flake8
+00000650: 5d0d 0a6d 6178 2d6c 696e 652d 6c65 6e67  ]..max-line-leng
+00000660: 7468 203d 2039 390d 0a64 6f63 7465 7374  th = 99..doctest
+00000670: 7320 3d20 5472 7565 0d0a 6578 636c 7564  s = True..exclud
+00000680: 6520 3d20 2e67 6974 2c20 2e65 6767 732c  e = .git, .eggs,
+00000690: 205f 5f70 7963 6163 6865 5f5f 2c20 7465   __pycache__, te
+000006a0: 7374 732f 2c20 646f 6373 2f2c 2062 7569  sts/, docs/, bui
+000006b0: 6c64 2f2c 2064 6973 742f 0d0a 0d0a 5b6d  ld/, dist/....[m
+000006c0: 7970 795d 0d0a 6469 7361 6c6c 6f77 5f61  ypy]..disallow_a
+000006d0: 6e79 5f64 6563 6f72 6174 6564 203d 2074  ny_decorated = t
+000006e0: 7275 650d 0a64 6973 616c 6c6f 775f 616e  rue..disallow_an
+000006f0: 795f 6765 6e65 7269 6373 203d 2074 7275  y_generics = tru
+00000700: 650d 0a64 6973 616c 6c6f 775f 616e 795f  e..disallow_any_
+00000710: 756e 696d 706f 7274 6564 203d 2066 616c  unimported = fal
+00000720: 7365 0d0a 6469 7361 6c6c 6f77 5f73 7562  se..disallow_sub
+00000730: 636c 6173 7369 6e67 5f61 6e79 203d 2066  classing_any = f
+00000740: 616c 7365 0d0a 6469 7361 6c6c 6f77 5f75  alse..disallow_u
+00000750: 6e74 7970 6564 5f63 616c 6c73 203d 2074  ntyped_calls = t
+00000760: 7275 650d 0a64 6973 616c 6c6f 775f 756e  rue..disallow_un
+00000770: 7479 7065 645f 6465 6673 203d 2074 7275  typed_defs = tru
+00000780: 650d 0a69 676e 6f72 655f 6d69 7373 696e  e..ignore_missin
+00000790: 675f 696d 706f 7274 7320 3d20 7472 7565  g_imports = true
+000007a0: 0d0a 7761 726e 5f75 6e75 7365 645f 6967  ..warn_unused_ig
+000007b0: 6e6f 7265 7320 3d20 7472 7565 0d0a 7761  nores = true..wa
+000007c0: 726e 5f72 6574 7572 6e5f 616e 7920 3d20  rn_return_any = 
+000007d0: 7472 7565 0d0a 0d0a 5b65 6767 5f69 6e66  true....[egg_inf
+000007e0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+000007f0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+00000800: 0d0a                                     ..
```

### Comparing `vision6D-0.2.4/test/test_create_dataset.py` & `vision6D-0.2.5/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.4/test/test_projection.py` & `vision6D-0.2.5/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.4/vision6D/GUI.py` & `vision6D-0.2.5/vision6D/GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -911,17 +911,17 @@
                 elif actor_name == 'mask': self.opacity_value_change(self.store_mask_opacity * 100)
                 else: self.opacity_value_change(self.store_mesh_opacity[actor_name] * 100)
 
             checked_button = self.button_group_actors_names.checkedButton()
             if checked_button is not None:
                 actor_name = checked_button.text()
                 self.ignore_slider_value_change = True
-                if actor_name == 'image': self.opacity_slider.setValue(self.image_opacity * 100)
-                elif actor_name == 'mask': self.opacity_slider.setValue(self.mask_opacity * 100)
-                else: self.opacity_slider.setValue(self.mesh_opacity[actor_name] * 100)
+                if actor_name == 'image': self.opacity_slider.setValue(int(self.image_opacity * 100))
+                elif actor_name == 'mask': self.opacity_slider.setValue(int(self.mask_opacity * 100))
+                else: self.opacity_slider.setValue(int(self.mesh_opacity[actor_name] * 100))
                 self.ignore_slider_value_change = False
             else: QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
     def panel_display(self):
         self.display = QtWidgets.QGroupBox("Console")
         display_layout = QtWidgets.QVBoxLayout()
         display_layout.setContentsMargins(10, 20, 10, 10)
@@ -1058,14 +1058,22 @@
 
         # registration related key bindings
         self.plotter.add_key_event('k', self.reset_gt_pose)
         self.plotter.add_key_event('l', self.update_gt_pose)
         self.plotter.add_key_event('t', self.current_pose)
         self.plotter.add_key_event('s', self.undo_pose)
 
+        # change opacity key bindings
+        self.plotter.add_key_event('b', functools.partial(self.toggle_image_opacity, up=True))
+        self.plotter.add_key_event('n', functools.partial(self.toggle_image_opacity, up=False))
+        self.plotter.add_key_event('g', functools.partial(self.toggle_mask_opacity, up=True))
+        self.plotter.add_key_event('h', functools.partial(self.toggle_mask_opacity, up=False))
+        self.plotter.add_key_event('y', functools.partial(self.toggle_surface_opacity, up=True))
+        self.plotter.add_key_event('u', functools.partial(self.toggle_surface_opacity, up=False))
+
         self.plotter.add_axes()
         self.plotter.add_camera_orientation_widget()
 
         self.plotter.show()
         self.show()
 
     def showMaximized(self):
```

### Comparing `vision6D-0.2.4/vision6D/__init__.py` & `vision6D-0.2.5/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.4/vision6D/app.py` & `vision6D-0.2.5/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.4/vision6D/config.py` & `vision6D-0.2.5/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.4/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.2.5/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.4/vision6D/data/ossiclesCoordinateMappingv1.json` & `vision6D-0.2.5/vision6D/data/ossiclesCoordinateMappingv1.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.4/vision6D/data/style.qss` & `vision6D-0.2.5/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.4/vision6D/interface.py` & `vision6D-0.2.5/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.4/vision6D/interface_gui.py` & `vision6D-0.2.5/vision6D/interface_gui.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,20 +57,20 @@
     def button_actor_name_clicked(self, text):
         if text in self.mesh_actors:
             # set the current mesh color
             self.color_button.setText(self.mesh_colors[text])
             # set mesh reference
             self.reference = text
             curr_opacity = self.mesh_actors[self.reference].GetProperty().opacity
-            self.opacity_slider.setValue(curr_opacity * 100)
+            self.opacity_slider.setValue(int(curr_opacity * 100))
         else:
             self.color_button.setText("Color")
             if text == 'image': curr_opacity = self.image_opacity
             elif text == 'mask': curr_opacity = self.mask_opacity
-            self.opacity_slider.setValue(curr_opacity * 100)
+            self.opacity_slider.setValue(int(curr_opacity * 100))
             self.reference = None
         
         output = f"-> Actor {text}, and its opacity is {curr_opacity}"
         if output not in self.output_text.toPlainText(): self.output_text.append(output)
                                             
     def set_image_opacity(self, image_opacity: float):
         assert image_opacity>=0 and image_opacity<=1, "image opacity should range from 0 to 1!"
@@ -258,14 +258,50 @@
             if actor_name in self.mesh_actors:        
                 if actor_name not in self.undo_poses: self.undo_poses[actor_name] = []
                 self.undo_poses[actor_name].append(self.mesh_actors[actor_name].user_matrix)
                 if len(self.undo_poses[actor_name]) > 20: self.undo_poses[actor_name].pop(0)
                 # check the picked button
                 self.check_button(actor_name)
 
+    def toggle_image_opacity(self, *args, up):
+        if up:
+            self.image_opacity += 0.05
+            if self.image_opacity > 1: self.image_opacity = 1
+        else:
+            self.image_opacity -= 0.05
+            if self.image_opacity < 0: self.image_opacity = 0
+        self.image_actor.GetProperty().opacity = self.image_opacity
+        self.plotter.add_actor(self.image_actor, pickable=False, name="image")
+        self.ignore_slider_value_change = True
+        self.opacity_slider.setValue(int(self.image_opacity * 100))
+        self.ignore_slider_value_change = False
+
+    def toggle_mask_opacity(self, *args, up):
+        if up:
+            self.mask_opacity += 0.05
+            if self.mask_opacity > 1: self.mask_opacity = 1
+        else:
+            self.mask_opacity -= 0.05
+            if self.mask_opacity < 0: self.mask_opacity = 0
+        self.mask_actor.GetProperty().opacity = self.mask_opacity
+        self.plotter.add_actor(self.mask_actor, pickable=False, name="mask")
+        self.ignore_slider_value_change = True
+        self.opacity_slider.setValue(int(self.mask_opacity * 100))
+        self.ignore_slider_value_change = False
+
+    def toggle_surface_opacity(self, *args, up):
+        current_opacity = self.opacity_slider.value() / 100
+        if up:
+            current_opacity += 0.05
+            if current_opacity > 1: current_opacity = 1
+        else:
+            current_opacity -= 0.05
+            if current_opacity < 0: current_opacity = 0
+        self.opacity_slider.setValue(int(current_opacity * 100))
+
     def reset_gt_pose(self, *args):
         self.output_text.append(f"-> Reset the GT pose to: \n{self.initial_pose}")
         for actor_name, actor in self.mesh_actors.items():
             actor.user_matrix = self.initial_pose
             self.plotter.add_actor(actor, pickable=True, name=actor_name)
 
     def update_gt_pose(self, *args):
```

### Comparing `vision6D-0.2.4/vision6D/mainwindow.py` & `vision6D-0.2.5/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.4/vision6D/run_gui.py` & `vision6D-0.2.5/vision6D/run_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.4/vision6D/utils.py` & `vision6D-0.2.5/vision6D/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.4/vision6D.egg-info/PKG-INFO` & `vision6D-0.2.5/vision6D.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.2.4
+Version: 0.2.5
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.2.4/vision6D.egg-info/SOURCES.txt` & `vision6D-0.2.5/vision6D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

