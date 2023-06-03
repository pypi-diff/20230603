# Comparing `tmp/loophost-1.2.8-py3-none-any.whl.zip` & `tmp/loophost-1.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 344765 bytes, number of entries: 33
+Zip file size: 344764 bytes, number of entries: 33
 -rw-r--r--  2.0 unx       68 b- defN 80-Jan-01 00:00 README.md
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 VERSION
 -rw-r--r--  2.0 unx     2201 b- defN 80-Jan-01 00:00 loophost/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 loophost/bins/.keep
 -rw-r--r--  2.0 unx     3934 b- defN 80-Jan-01 00:00 loophost/flingroute.py
 -rw-r--r--  2.0 unx     3326 b- defN 80-Jan-01 00:00 loophost/installer.py
 -rw-r--r--  2.0 unx      252 b- defN 80-Jan-01 00:00 loophost/keys.py
@@ -25,11 +25,11 @@
 -rw-r--r--  2.0 unx     1730 b- defN 80-Jan-01 00:00 loophost/templates/start/base.html
 -rw-r--r--  2.0 unx     3812 b- defN 80-Jan-01 00:00 loophost/tunnel.py
 -rw-r--r--  2.0 unx     1468 b- defN 80-Jan-01 00:00 loophost/uninstall.py
 -rw-r--r--  2.0 unx      564 b- defN 80-Jan-01 00:00 loophost/utils_mac.py
 -rw-r--r--  2.0 unx     2431 b- defN 80-Jan-01 00:00 loophost/win_hub.py
 -rw-r--r--  2.0 unx     2585 b- defN 80-Jan-01 00:00 loophost/win_lp.py
 -rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 setup.py
--rw-r--r--  2.0 unx     1163 b- defN 80-Jan-01 00:00 loophost-1.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 loophost-1.2.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2674 b- defN 16-Jan-01 00:00 loophost-1.2.8.dist-info/RECORD
-33 files, 443491 bytes uncompressed, 340507 bytes compressed:  23.2%
+-rw-r--r--  2.0 unx     1163 b- defN 80-Jan-01 00:00 loophost-1.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 loophost-1.2.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2674 b- defN 16-Jan-01 00:00 loophost-1.2.9.dist-info/RECORD
+33 files, 443491 bytes uncompressed, 340506 bytes compressed:  23.2%
```

## zipnote {}

```diff
@@ -84,17 +84,17 @@
 
 Filename: loophost/win_lp.py
 Comment: 
 
 Filename: setup.py
 Comment: 
 
-Filename: loophost-1.2.8.dist-info/METADATA
+Filename: loophost-1.2.9.dist-info/METADATA
 Comment: 
 
-Filename: loophost-1.2.8.dist-info/WHEEL
+Filename: loophost-1.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: loophost-1.2.8.dist-info/RECORD
+Filename: loophost-1.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## VERSION

```diff
@@ -1 +1 @@
-1.2.8
+1.2.9
```

## loophost/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.8"
+__version__ = "1.2.9"
 
 import getpass
 import os
 import pathlib
 import platform
 import sys
 from string import Template
```

## Comparing `loophost-1.2.8.dist-info/METADATA` & `loophost-1.2.9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loophost
-Version: 1.2.8
+Version: 1.2.9
 Summary: Loophost: for a better local dev
 License: Apache-2.0
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `loophost-1.2.8.dist-info/RECORD` & `loophost-1.2.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 README.md,sha256=_0gYbeCM0PS5aDAFtByWE7XzWzF8a9Ues39fzGa5yCQ,68
-VERSION,sha256=6JusvPsXJsFeJsXgV9QLCnIvPiWJ09rwZyg6esuAFnQ,5
-loophost/__init__.py,sha256=M1I82EbDsxQy3Gq9zvrK9BUqf5g8lNjEhhk9Ly5SGTg,2201
+VERSION,sha256=l2TdJ7h02m6gMYnTBUwLjNPXbDz8oEjbvL6SbYac2dI,5
+loophost/__init__.py,sha256=18tKneQapb6U4yF7ZPSv8JY-PZIzClz9wRIdvARfnLs,2201
 loophost/bins/.keep,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 loophost/flingroute.py,sha256=5Tj03zYNDGpTXxTFGpU9L3Ul41FmN25LnOl5txn-gEA,3934
 loophost/installer.py,sha256=gU5TQANnvFzLCWzBv5QH4v63Ij1Cq_Iiol0wXNSrec8,3326
 loophost/keys.py,sha256=Fm-OXFiJMS0EaR8ppzRzchKY07xZ1b8qVSxTgvRK3-U,252
 loophost/plist/hub.plist.template,sha256=S7xWW38mCKYNnucxBgW2QtXph1OMfx5XhxZtn2Judkk,788
 loophost/plist/loophost.plist.template,sha256=21nK1O8zsrjo_DDJUzGIDX3vjOeGiQa2_VV1P82b-5c,771
 loophost/plist/ssh.plist.template,sha256=aqlNCI-NFNDCHNPv3_f4emTZvogN2gwuyYvFHgnVYdU,1150
@@ -24,10 +24,10 @@
 loophost/templates/start/base.html,sha256=i4ua9YqaAP1reFW9oBHadyHmx40B2m3vzp_nMfx2_kw,1730
 loophost/tunnel.py,sha256=K3PWIUwfCB5Sdyc5XVOEMgO-iyJCPVxA7RvP-kPU--U,3812
 loophost/uninstall.py,sha256=W16eYSh91Jiuvx5Cuw9BDNxvGIOT36bWFcXSrgK9MmE,1468
 loophost/utils_mac.py,sha256=qVtMuamtCUPLgbWzo2Oa1Caa_BBHDdpMVD2UUa-L_YA,564
 loophost/win_hub.py,sha256=RRKlmBOHNY4B9EgoFWaW8bjcPKLyN8iy2SkFoj_sT4k,2431
 loophost/win_lp.py,sha256=dqY3_TfzWHdxfQJuy3mb6zD5-rGiMw_3tdVljxBOCM0,2585
 setup.py,sha256=JuQJ4tne5dED19WdRpw1_A1x9MvmvAxJpY0rCBuyCWM,39
-loophost-1.2.8.dist-info/METADATA,sha256=ai1FM_omqQWmmZEsz8mLH-weRw4K9OaBUCRFpO_fSzY,1163
-loophost-1.2.8.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-loophost-1.2.8.dist-info/RECORD,,
+loophost-1.2.9.dist-info/METADATA,sha256=dFEuM-V6J3fFeBmBmsYMRf8s49uvrWGb6xbsdgDHi9A,1163
+loophost-1.2.9.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+loophost-1.2.9.dist-info/RECORD,,
```

