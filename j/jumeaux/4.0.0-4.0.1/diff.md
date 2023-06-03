# Comparing `tmp/jumeaux-4.0.0-py3-none-any.whl.zip` & `tmp/jumeaux-4.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 99776 bytes, number of entries: 178
+Zip file size: 99779 bytes, number of entries: 178
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 jumeaux/__init__.py
 -rw-r--r--  2.0 unx     4120 b- defN 80-Jan-01 00:00 jumeaux/addons/__init__.py
 -rw-r--r--  2.0 unx      292 b- defN 80-Jan-01 00:00 jumeaux/addons/did_challenge/__init__.py
 -rw-r--r--  2.0 unx      781 b- defN 80-Jan-01 00:00 jumeaux/addons/did_challenge/sleep.py
 -rw-r--r--  2.0 unx     2485 b- defN 80-Jan-01 00:00 jumeaux/addons/did_challenge/tag.py
 -rw-r--r--  2.0 unx      192 b- defN 80-Jan-01 00:00 jumeaux/addons/dump/__init__.py
 -rw-r--r--  2.0 unx      708 b- defN 80-Jan-01 00:00 jumeaux/addons/dump/encoding.py
@@ -168,13 +168,13 @@
 -rwxr-xr-x  2.0 unx       36 b- defN 80-Jan-01 00:00 jumeaux/sample/template/simple/requests
 -rwxr-xr-x  2.0 unx      723 b- defN 80-Jan-01 00:00 jumeaux/sample/template/xml/api/one/diff-1.xml
 -rwxr-xr-x  2.0 unx      723 b- defN 80-Jan-01 00:00 jumeaux/sample/template/xml/api/other/diff-1.xml
 -rwxr-xr-x  2.0 unx      894 b- defN 80-Jan-01 00:00 jumeaux/sample/template/xml/config.yml
 -rwxr-xr-x  2.0 unx       12 b- defN 80-Jan-01 00:00 jumeaux/sample/template/xml/requests
 -rw-r--r--  2.0 unx    17106 b- defN 80-Jan-01 00:00 jumeaux/sample/viewer/index.html
 -rw-r--r--  2.0 unx     2613 b- defN 80-Jan-01 00:00 jumeaux/utils.py
-?rw-r--r--  2.0 unx       45 b- defN 16-Jan-01 00:00 jumeaux-4.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 jumeaux-4.0.0.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 jumeaux-4.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     3904 b- defN 16-Jan-01 00:00 jumeaux-4.0.0.dist-info/METADATA
-?rw-r--r--  2.0 unx    17361 b- defN 16-Jan-01 00:00 jumeaux-4.0.0.dist-info/RECORD
-178 files, 206927 bytes uncompressed, 71332 bytes compressed:  65.5%
+-rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 jumeaux-4.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3864 b- defN 80-Jan-01 00:00 jumeaux-4.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 jumeaux-4.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 jumeaux-4.0.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    17361 b- defN 16-Jan-01 00:00 jumeaux-4.0.1.dist-info/RECORD
+178 files, 206887 bytes uncompressed, 71335 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -513,23 +513,23 @@
 
 Filename: jumeaux/sample/viewer/index.html
 Comment: 
 
 Filename: jumeaux/utils.py
 Comment: 
 
-Filename: jumeaux-4.0.0.dist-info/entry_points.txt
+Filename: jumeaux-4.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: jumeaux-4.0.0.dist-info/LICENSE
+Filename: jumeaux-4.0.1.dist-info/METADATA
 Comment: 
 
-Filename: jumeaux-4.0.0.dist-info/WHEEL
+Filename: jumeaux-4.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: jumeaux-4.0.0.dist-info/METADATA
+Filename: jumeaux-4.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: jumeaux-4.0.0.dist-info/RECORD
+Filename: jumeaux-4.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jumeaux/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '4.0.0'
+__version__ = '4.0.1'
```

## Comparing `jumeaux-4.0.0.dist-info/LICENSE` & `jumeaux-4.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jumeaux-4.0.0.dist-info/METADATA` & `jumeaux-4.0.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jumeaux
-Version: 4.0.0
+Version: 4.0.1
 Summary: Check difference between two responses of API.
 Home-page: https://tadashi-aikawa.github.io/jumeaux
 License: MIT
 Keywords: diff rest api response regression test
 Author: tadashi-aikawa
 Author-email: syou.maman@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -30,48 +30,45 @@
 Requires-Dist: owcli (>=0.7.0,<0.8.0)
 Requires-Dist: owlmixin (>=5.5.0,<6.0.0)
 Requires-Dist: pydash (>=4.7.6,<5.0.0)
 Requires-Dist: requests (>=2.22.0,<3.0.0)
 Requires-Dist: requests-toolbelt (>=0.9.1,<0.10.0)
 Requires-Dist: schema (>=0.7.1,<0.8.0)
 Requires-Dist: tzlocal (>=2.0.0,<3.0.0)
+Requires-Dist: urllib3 (<2)
 Requires-Dist: xmltodict (>=0.12.0,<0.13.0)
 Project-URL: Documentation, https://tadashi-aikawa.github.io/jumeaux
 Project-URL: Repository, https://github.com/tadashi-aikawa/jumeaux/blob/master/README.md
 Description-Content-Type: text/markdown
 
-Jumeaux
-=======
+# Jumeaux
 
 [![pypi](https://img.shields.io/pypi/v/jumeaux.svg)](https://pypi.org/project/jumeaux/)
 [![Versions](https://img.shields.io/pypi/pyversions/jumeaux.svg)](https://pypi.org/project/jumeaux/)
 [![Actions Status](https://github.com/tadashi-aikawa/jumeaux/workflows/Tests/badge.svg)](https://github.com/tadashi-aikawa/jumeaux/actions)
 [![codecov](https://codecov.io/gh/tadashi-aikawa/jumeaux/branch/master/graph/badge.svg)](https://codecov.io/gh/tadashi-aikawa/jumeaux)
 [![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/tadashi-aikawa/jumeaux/blob/master/LICENSE)
 
 <img src="https://github.com/tadashi-aikawa/jumeaux/blob/master/logo.png?raw=true" width=400 height=400 />
 
 Check difference between two responses of API.
 
-📚 Documentation
-------------------
+## 📚 Documentation
 
 https://tadashi-aikawa.github.io/jumeaux/
 
 There is a 🎥demo, too.
 
 
-🦉 Install
-------------
+## 🦉 Install
 
 See [quick start in documentation](https://tadashi-aikawa.github.io/jumeaux/ja/getstarted/quickstart/).
 
 
-💻 For developer
-------------------
+## 💻 For developer
 
 ### Requirements
 
 * poetry
 * make
 
 ### Flow
@@ -110,16 +107,15 @@
 
 ```
 $ make test-e2e
 ```
 
 
 
-📦 Release
-------------
+## 📦 Release
 
 ### 1. Update release note (mkdocs/ja/releases/*)
 
 ```
 $ git commit -m "📝 Update release note"
 $ git push
 ```
@@ -143,15 +139,14 @@
 #### (a2) Commands
 
 ```bash
 make release version=x.y.z
 ```
 
 
-🎫 Licence
-------------
+## 🎫 Licence
 
 ### MIT
 
 This software is released under the MIT License, see LICENSE.txt.
```

## Comparing `jumeaux-4.0.0.dist-info/RECORD` & `jumeaux-4.0.1.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-jumeaux/__init__.py,sha256=61rJjfThnbRdElpSP2tm31hPmFnHJmcwoPhtqA0Bi_Q,22
+jumeaux/__init__.py,sha256=t3_GiRZvVdqtOM0gRAa8vnfrcrUkhvgVNLEwrIaUIcw,22
 jumeaux/addons/__init__.py,sha256=7ABV74dDROhf3EazIxP-x-4V5TehAgAZOoRmgRnAn-I,4120
 jumeaux/addons/did_challenge/__init__.py,sha256=z5huqocLirmhlBATVJ2p1LwKRcUqpx55A7SyLt_zjkY,292
 jumeaux/addons/did_challenge/sleep.py,sha256=_c-RXEGu478kWqvH4msgDCLHGRmLaYeZ4Ki_lo4mt3M,781
 jumeaux/addons/did_challenge/tag.py,sha256=e7XI-v6j1DmrBmO0IL7b7EsCUSNafinHO3_xuHqjo_M,2485
 jumeaux/addons/dump/__init__.py,sha256=4EWZ5rhl_x_rhyLLwVMCgvT79_wNT0ll8_4WoJ8I79k,192
 jumeaux/addons/dump/encoding.py,sha256=qnBGdhVJf78dWqBg605cB3bAo0WkbjsTGdvrbFGPjKo,708
 jumeaux/addons/dump/html.py,sha256=1uXoLCdCLf6KSdrp_WdWcpcgFqZpwjYgvHy5i4yHFY4,1227
@@ -167,12 +167,12 @@
 jumeaux/sample/template/simple/requests,sha256=CKesNRdVTWgdWnCY_K8ExCSqNToFtqgStiSidgK_YsI,36
 jumeaux/sample/template/xml/api/one/diff-1.xml,sha256=5taqNoq8pN-s79ly8py-ZGSRnZVLkTbm1rOdtMQvNSs,723
 jumeaux/sample/template/xml/api/other/diff-1.xml,sha256=8I9ugp9u551mKdV9OHYi8KWUy_RXPM4l2hYTgDMrkXA,723
 jumeaux/sample/template/xml/config.yml,sha256=vqt2P-nyw9i2zqlrmLwZMjE2WMZOXisyBNkLq7LtUG0,894
 jumeaux/sample/template/xml/requests,sha256=mHMfrprQFLPOo0ugwFKwu7t2Fp8634eNEUkDG_PeFVI,12
 jumeaux/sample/viewer/index.html,sha256=RZytfGSvOn5FRFi1c6PzuLdaUBxYRKR-8p7s5_nL-BA,17106
 jumeaux/utils.py,sha256=gpA-Xr-UpHM03i4lGzBOYhEbRpxDKuQlDKA7T5kxERc,2613
-jumeaux-4.0.0.dist-info/entry_points.txt,sha256=CyOBZ_wPw8RqgutUO-RZsifwAQrqa95A2q9Rv98CB5A,45
-jumeaux-4.0.0.dist-info/LICENSE,sha256=IKkX_iHGJtElV0t6vav-LLicUlhxOLt0Jl65lql1Wuw,1081
-jumeaux-4.0.0.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
-jumeaux-4.0.0.dist-info/METADATA,sha256=oOmYzdNOT-YczKAOQcaoDPEh8omPy75GsgDO1QyPYA4,3904
-jumeaux-4.0.0.dist-info/RECORD,,
+jumeaux-4.0.1.dist-info/LICENSE,sha256=IKkX_iHGJtElV0t6vav-LLicUlhxOLt0Jl65lql1Wuw,1081
+jumeaux-4.0.1.dist-info/METADATA,sha256=OcNBSnfANa5HWtnGLhbPD687etj2ZLg539K6-u5NJ_U,3864
+jumeaux-4.0.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+jumeaux-4.0.1.dist-info/entry_points.txt,sha256=CyOBZ_wPw8RqgutUO-RZsifwAQrqa95A2q9Rv98CB5A,45
+jumeaux-4.0.1.dist-info/RECORD,,
```

