# Comparing `tmp/jingan-0.0.2-py3-none-any.whl.zip` & `tmp/jingan-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 84271 bytes, number of entries: 38
+Zip file size: 84272 bytes, number of entries: 38
 -rw-rw-r--  2.0 unx      478 b- defN 23-Jun-02 18:59 dnnlib/__init__.py
 -rw-rw-r--  2.0 unx    16627 b- defN 23-Jun-02 18:59 dnnlib/util.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-03 01:37 jingan/__init__.py
 -rw-rw-r--  2.0 unx       54 b- defN 23-Jun-03 00:29 jingan/jin_test.py
 -rw-rw-r--  2.0 unx     3354 b- defN 23-Jun-03 01:14 jingan/jin_util.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-03 01:39 jingan/res.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-03 01:40 jingan/session.py
@@ -28,13 +28,13 @@
 -rw-rw-r--  2.0 unx    16287 b- defN 23-Jun-02 18:59 torch_utils/ops/upfirdn2d.py
 -rw-rw-r--  2.0 unx      435 b- defN 23-Jun-02 18:59 training/__init__.py
 -rw-rw-r--  2.0 unx    26375 b- defN 23-Jun-02 18:59 training/augment.py
 -rw-rw-r--  2.0 unx     8553 b- defN 23-Jun-02 18:59 training/dataset.py
 -rw-rw-r--  2.0 unx     7299 b- defN 23-Jun-02 18:59 training/loss.py
 -rw-rw-r--  2.0 unx    37394 b- defN 23-Jun-02 18:59 training/networks.py
 -rw-rw-r--  2.0 unx    21598 b- defN 23-Jun-02 18:59 training/training_loop.py
--rwxrwxr-x  2.0 unx     4421 b- defN 23-Jun-03 01:40 jingan-0.0.2.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx    26170 b- defN 23-Jun-03 01:40 jingan-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-03 01:40 jingan-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       43 b- defN 23-Jun-03 01:40 jingan-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3049 b- defN 23-Jun-03 01:40 jingan-0.0.2.dist-info/RECORD
-38 files, 274149 bytes uncompressed, 79467 bytes compressed:  71.0%
+-rwxrwxr-x  2.0 unx     4421 b- defN 23-Jun-03 01:42 jingan-0.0.3.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx    26170 b- defN 23-Jun-03 01:42 jingan-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-03 01:42 jingan-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       43 b- defN 23-Jun-03 01:42 jingan-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3049 b- defN 23-Jun-03 01:42 jingan-0.0.3.dist-info/RECORD
+38 files, 274149 bytes uncompressed, 79468 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -93,23 +93,23 @@
 
 Filename: training/networks.py
 Comment: 
 
 Filename: training/training_loop.py
 Comment: 
 
-Filename: jingan-0.0.2.dist-info/LICENSE.txt
+Filename: jingan-0.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: jingan-0.0.2.dist-info/METADATA
+Filename: jingan-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: jingan-0.0.2.dist-info/WHEEL
+Filename: jingan-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: jingan-0.0.2.dist-info/top_level.txt
+Filename: jingan-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: jingan-0.0.2.dist-info/RECORD
+Filename: jingan-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `jingan-0.0.2.dist-info/LICENSE.txt` & `jingan-0.0.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `jingan-0.0.2.dist-info/METADATA` & `jingan-0.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jingan
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Home-page: https://github.com/Seokhee-Jin/stylegan2-ada-pytorch
 Author: not my work
 Author-email: seokhee749@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `jingan-0.0.2.dist-info/RECORD` & `jingan-0.0.3.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -27,12 +27,12 @@
 torch_utils/ops/upfirdn2d.py,sha256=e1hl5wrEFW7a77Kjcv7ifcVetWYVaLM3y0Fo6JNjhKg,16287
 training/__init__.py,sha256=XvoCq52tzXwBbH3mAWGwgoiuZNM3Xtbyh8FQGyY189k,435
 training/augment.py,sha256=_YHIcam_u3_qrROLHoddsFxkAGC9vwNCJH0gnrSLqPk,26375
 training/dataset.py,sha256=EOQz_95uPmOWNxE5Dujuqm8OWgDan4gxFzMaSLNuUUU,8553
 training/loss.py,sha256=G9aNfcHJLBt4uR8ZOkWkM7H_N0YU-RkJ6oy4jqx7wtc,7299
 training/networks.py,sha256=30n8eKA2QBWgm1krtDVGr4OmzarXU9iaKhppvW4XHCQ,37394
 training/training_loop.py,sha256=C1iacxcSxReR6yLv4Nwe5oVr8-kzWSDbAqPjje6QnrM,21598
-jingan-0.0.2.dist-info/LICENSE.txt,sha256=14Kh52X0hIYJNS_Z10zDaxA-9vUZALrtBvscmVGIuV8,4421
-jingan-0.0.2.dist-info/METADATA,sha256=BXyxmAVG7f6LLzOzfYfZSeXCJVavB84LtAbNM4F2rEk,26170
-jingan-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-jingan-0.0.2.dist-info/top_level.txt,sha256=81EPsD9yUyhSej2DcErVCwTuBIfHp7lI7lrVR0DNa3U,43
-jingan-0.0.2.dist-info/RECORD,,
+jingan-0.0.3.dist-info/LICENSE.txt,sha256=14Kh52X0hIYJNS_Z10zDaxA-9vUZALrtBvscmVGIuV8,4421
+jingan-0.0.3.dist-info/METADATA,sha256=6u26IhQVeqpQdVpvmVGp0oAyrAa62TqHPdfmI04aJR8,26170
+jingan-0.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+jingan-0.0.3.dist-info/top_level.txt,sha256=81EPsD9yUyhSej2DcErVCwTuBIfHp7lI7lrVR0DNa3U,43
+jingan-0.0.3.dist-info/RECORD,,
```

