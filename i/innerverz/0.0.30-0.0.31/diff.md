# Comparing `tmp/innerverz-0.0.30.tar.gz` & `tmp/innerverz-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innerverz-0.0.30.tar", last modified: Sat Jun  3 01:27:56 2023, max compression
+gzip compressed data, was "innerverz-0.0.31.tar", last modified: Sat Jun  3 07:04:52 2023, max compression
```

## Comparing `innerverz-0.0.30.tar` & `innerverz-0.0.31.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.737748 innerverz-0.0.30/
--rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.0.30/LICENSE.txt
--rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-03 01:27:56.737833 innerverz-0.0.30/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.0.30/README.md
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.719008 innerverz-0.0.30/innerverz/
--rw-r--r--   0 jjy        (501) staff       (20)     1501 2023-06-01 06:15:38.000000 innerverz-0.0.30/innerverz/__init__.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.720423 innerverz-0.0.30/innerverz/data_process/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:31.000000 innerverz-0.0.30/innerverz/data_process/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3493 2023-06-01 06:13:31.000000 innerverz-0.0.30/innerverz/data_process/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.721110 innerverz-0.0.30/innerverz/deblurrer/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:31.000000 innerverz-0.0.30/innerverz/deblurrer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2171 2023-06-01 06:13:31.000000 innerverz-0.0.30/innerverz/deblurrer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-06-01 06:13:31.000000 innerverz-0.0.30/innerverz/deblurrer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      867 2023-06-01 06:13:31.000000 innerverz-0.0.30/innerverz/deblurrer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.721585 innerverz-0.0.30/innerverz/deca/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:13:31.000000 innerverz-0.0.30/innerverz/deca/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)    17533 2023-06-03 01:27:07.000000 innerverz-0.0.30/innerverz/deca/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.722929 innerverz-0.0.30/innerverz/deca/models/
--rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-06-01 06:13:31.000000 innerverz-0.0.30/innerverz/deca/models/FLAME.py
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:31.000000 innerverz-0.0.30/innerverz/deca/models/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/models/decoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/models/detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/models/encoders.py
--rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/models/face_detectors.py
--rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/models/lbs.py
--rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/models/resnet.py
--rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.724015 innerverz-0.0.30/innerverz/deca/utils/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/utils/cfg.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.724342 innerverz-0.0.30/innerverz/deca/utils/rasterizer/
--rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/utils/rasterizer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)      706 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/utils/rasterizer/setup.py
--rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/utils/renderer.py
--rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/utils/rotation_converter.py
--rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/utils/tensor_cropper.py
--rw-r--r--   0 jjy        (501) staff       (20)    26962 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deca/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.725013 innerverz-0.0.30/innerverz/deep3dmm/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deep3dmm/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3414 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deep3dmm/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deep3dmm/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      651 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/deep3dmm/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.725952 innerverz-0.0.30/innerverz/face_alignment/
--rw-r--r--   0 jjy        (501) staff       (20)      125 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_alignment/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_alignment/graphic_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_alignment/landmark.py
--rw-r--r--   0 jjy        (501) staff       (20)     9719 2023-06-01 06:14:15.000000 innerverz-0.0.30/innerverz/face_alignment/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_alignment/retina_face.py
--rw-r--r--   0 jjy        (501) staff       (20)      656 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_alignment/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.726733 innerverz-0.0.30/innerverz/face_alignment/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_alignment/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_alignment/utils/face_align.py
--rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_alignment/utils/transform.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.727670 innerverz-0.0.30/innerverz/face_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5238 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.728524 innerverz-0.0.30/innerverz/face_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.729142 innerverz-0.0.30/innerverz/face_enhancer/
--rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_enhancer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3760 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_enhancer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_enhancer/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      792 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_enhancer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.729792 innerverz-0.0.30/innerverz/face_parser/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_parser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2682 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_parser/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_parser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      713 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/face_parser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.730479 innerverz-0.0.30/innerverz/head_color_transfer/
--rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/head_color_transfer/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     5409 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/head_color_transfer/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/head_color_transfer/nets.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.731310 innerverz-0.0.30/innerverz/head_color_transfer/sub_nets/
--rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/head_color_transfer/sub_nets/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/head_color_transfer/sub_nets/blend_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/head_color_transfer/sub_nets/discriminator.py
--rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/head_color_transfer/sub_nets/vgg19_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/head_color_transfer/sub_nets/warp_net.py
--rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/head_color_transfer/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.732294 innerverz-0.0.30/innerverz/id_extractor/
--rw-r--r--   0 jjy        (501) staff       (20)       29 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/id_extractor/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2253 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/id_extractor/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/id_extractor/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      717 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/id_extractor/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.733683 innerverz-0.0.30/innerverz/reage/
--rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:15:17.000000 innerverz-0.0.30/innerverz/reage/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1944 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/reage/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-06-01 07:03:50.000000 innerverz-0.0.30/innerverz/reage/net.py
--rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/reage/net_utils.py
--rw-r--r--   0 jjy        (501) staff       (20)      763 2023-06-01 06:19:21.000000 innerverz-0.0.30/innerverz/reage/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.734512 innerverz-0.0.30/innerverz/relighter/
--rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/relighter/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2912 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/relighter/main.py
--rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/relighter/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/relighter/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.735257 innerverz-0.0.30/innerverz/upsampler/
--rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/upsampler/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     2250 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/upsampler/main.py
--rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/upsampler/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      854 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/upsampler/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.735967 innerverz-0.0.30/innerverz/utils/
--rw-r--r--   0 jjy        (501) staff       (20)      109 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/utils/download.py
--rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/utils/input.py
--rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/utils/utils.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.736619 innerverz-0.0.30/innerverz/video_faceparser/
--rw-r--r--   0 jjy        (501) staff       (20)       34 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/video_faceparser/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/video_faceparser/main.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.736792 innerverz-0.0.30/innerverz/video_faceparser/model/
--rw-r--r--   0 jjy        (501) staff       (20)       79 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/video_faceparser/model/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/video_faceparser/nets.py
--rw-r--r--   0 jjy        (501) staff       (20)      217 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/video_faceparser/test.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.737603 innerverz-0.0.30/innerverz/video_faceparser/utils/
--rw-r--r--   0 jjy        (501) staff       (20)       94 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/video_faceparser/utils/__init__.py
--rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/video_faceparser/utils/corr.py
--rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/video_faceparser/utils/extractor.py
--rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/video_faceparser/utils/update.py
--rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-06-01 06:13:32.000000 innerverz-0.0.30/innerverz/video_faceparser/utils/util.py
-drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 01:27:56.719761 innerverz-0.0.30/innerverz.egg-info/
--rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-03 01:27:56.000000 innerverz-0.0.30/innerverz.egg-info/PKG-INFO
--rw-r--r--   0 jjy        (501) staff       (20)     3612 2023-06-03 01:27:56.000000 innerverz-0.0.30/innerverz.egg-info/SOURCES.txt
--rw-r--r--   0 jjy        (501) staff       (20)        1 2023-06-03 01:27:56.000000 innerverz-0.0.30/innerverz.egg-info/dependency_links.txt
--rw-r--r--   0 jjy        (501) staff       (20)       74 2023-06-03 01:27:56.000000 innerverz-0.0.30/innerverz.egg-info/requires.txt
--rw-r--r--   0 jjy        (501) staff       (20)       10 2023-06-03 01:27:56.000000 innerverz-0.0.30/innerverz.egg-info/top_level.txt
--rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.0.30/pyproject.toml
--rw-r--r--   0 jjy        (501) staff       (20)       38 2023-06-03 01:27:56.738741 innerverz-0.0.30/setup.cfg
--rw-r--r--   0 jjy        (501) staff       (20)      809 2023-06-03 01:21:57.000000 innerverz-0.0.30/setup.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.283971 innerverz-0.0.31/
+-rw-r--r--   0 jjy        (501) staff       (20)     1073 2023-05-23 07:04:26.000000 innerverz-0.0.31/LICENSE.txt
+-rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-03 07:04:52.284073 innerverz-0.0.31/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-05-23 07:04:26.000000 innerverz-0.0.31/README.md
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.264226 innerverz-0.0.31/innerverz/
+-rw-r--r--   0 jjy        (501) staff       (20)     1501 2023-06-01 06:15:38.000000 innerverz-0.0.31/innerverz/__init__.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.265439 innerverz-0.0.31/innerverz/data_process/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:31.000000 innerverz-0.0.31/innerverz/data_process/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3493 2023-06-01 06:13:31.000000 innerverz-0.0.31/innerverz/data_process/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.266549 innerverz-0.0.31/innerverz/deblurrer/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:31.000000 innerverz-0.0.31/innerverz/deblurrer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2171 2023-06-01 06:13:31.000000 innerverz-0.0.31/innerverz/deblurrer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3609 2023-06-01 06:13:31.000000 innerverz-0.0.31/innerverz/deblurrer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      867 2023-06-01 06:13:31.000000 innerverz-0.0.31/innerverz/deblurrer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.267359 innerverz-0.0.31/innerverz/deca/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:13:31.000000 innerverz-0.0.31/innerverz/deca/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)    17533 2023-06-03 07:04:21.000000 innerverz-0.0.31/innerverz/deca/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.269182 innerverz-0.0.31/innerverz/deca/models/
+-rw-r--r--   0 jjy        (501) staff       (20)    12616 2023-06-01 06:13:31.000000 innerverz-0.0.31/innerverz/deca/models/FLAME.py
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:31.000000 innerverz-0.0.31/innerverz/deca/models/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2464 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deca/models/decoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deca/models/detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1427 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deca/models/encoders.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1983 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deca/models/face_detectors.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13786 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deca/models/lbs.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8386 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deca/models/resnet.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1126 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deca/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.270157 innerverz-0.0.31/innerverz/deca/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deca/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5036 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deca/utils/cfg.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.270502 innerverz-0.0.31/innerverz/deca/utils/rasterizer/
+-rw-r--r--   0 jjy        (501) staff       (20)        0 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deca/utils/rasterizer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)      706 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deca/utils/rasterizer/setup.py
+-rw-r--r--   0 jjy        (501) staff       (20)    22281 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deca/utils/renderer.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12710 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deca/utils/rotation_converter.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5574 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deca/utils/tensor_cropper.py
+-rw-r--r--   0 jjy        (501) staff       (20)    26982 2023-06-03 07:04:12.000000 innerverz-0.0.31/innerverz/deca/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.271234 innerverz-0.0.31/innerverz/deep3dmm/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deep3dmm/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3414 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deep3dmm/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    25860 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deep3dmm/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      651 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/deep3dmm/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.272228 innerverz-0.0.31/innerverz/face_alignment/
+-rw-r--r--   0 jjy        (501) staff       (20)      125 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_alignment/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6646 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_alignment/graphic_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5089 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_alignment/landmark.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9737 2023-06-03 07:00:23.000000 innerverz-0.0.31/innerverz/face_alignment/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    12774 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_alignment/retina_face.py
+-rw-r--r--   0 jjy        (501) staff       (20)      656 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_alignment/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.272765 innerverz-0.0.31/innerverz/face_alignment/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       24 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_alignment/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3354 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_alignment/utils/face_align.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4933 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_alignment/utils/transform.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.273493 innerverz-0.0.31/innerverz/face_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5238 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8503 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.274385 innerverz-0.0.31/innerverz/face_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2047 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.275038 innerverz-0.0.31/innerverz/face_enhancer/
+-rw-r--r--   0 jjy        (501) staff       (20)       30 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_enhancer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3760 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_enhancer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4079 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_enhancer/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      792 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_enhancer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.275666 innerverz-0.0.31/innerverz/face_parser/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_parser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2682 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_parser/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    11822 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_parser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      713 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/face_parser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.276320 innerverz-0.0.31/innerverz/head_color_transfer/
+-rw-r--r--   0 jjy        (501) staff       (20)       22 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/head_color_transfer/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5409 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/head_color_transfer/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8742 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/head_color_transfer/nets.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.277207 innerverz-0.0.31/innerverz/head_color_transfer/sub_nets/
+-rw-r--r--   0 jjy        (501) staff       (20)      100 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/head_color_transfer/sub_nets/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     7018 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/head_color_transfer/sub_nets/blend_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3642 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/head_color_transfer/sub_nets/discriminator.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3788 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/head_color_transfer/sub_nets/vgg19_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     9366 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/head_color_transfer/sub_nets/warp_net.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1997 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/head_color_transfer/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.278309 innerverz-0.0.31/innerverz/id_extractor/
+-rw-r--r--   0 jjy        (501) staff       (20)       29 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/id_extractor/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2253 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/id_extractor/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     5192 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/id_extractor/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      717 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/id_extractor/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.279207 innerverz-0.0.31/innerverz/reage/
+-rw-r--r--   0 jjy        (501) staff       (20)       23 2023-06-01 06:15:17.000000 innerverz-0.0.31/innerverz/reage/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1944 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/reage/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3843 2023-06-01 07:03:50.000000 innerverz-0.0.31/innerverz/reage/net.py
+-rw-r--r--   0 jjy        (501) staff       (20)    13178 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/reage/net_utils.py
+-rw-r--r--   0 jjy        (501) staff       (20)      763 2023-06-01 06:19:21.000000 innerverz-0.0.31/innerverz/reage/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.280127 innerverz-0.0.31/innerverz/relighter/
+-rw-r--r--   0 jjy        (501) staff       (20)       27 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/relighter/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2912 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/relighter/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4546 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/relighter/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3078 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/relighter/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.280863 innerverz-0.0.31/innerverz/upsampler/
+-rw-r--r--   0 jjy        (501) staff       (20)       28 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/upsampler/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     2250 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/upsampler/main.py
+-rw-r--r--   0 jjy        (501) staff       (20)    36818 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/upsampler/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      854 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/upsampler/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.281505 innerverz-0.0.31/innerverz/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)      109 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1438 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/utils/download.py
+-rw-r--r--   0 jjy        (501) staff       (20)     1135 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/utils/input.py
+-rw-r--r--   0 jjy        (501) staff       (20)    15896 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/utils/utils.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.282383 innerverz-0.0.31/innerverz/video_faceparser/
+-rw-r--r--   0 jjy        (501) staff       (20)       34 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/video_faceparser/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6039 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/video_faceparser/main.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.282651 innerverz-0.0.31/innerverz/video_faceparser/model/
+-rw-r--r--   0 jjy        (501) staff       (20)       79 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/video_faceparser/model/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     4009 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/video_faceparser/nets.py
+-rw-r--r--   0 jjy        (501) staff       (20)      217 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/video_faceparser/test.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.283798 innerverz-0.0.31/innerverz/video_faceparser/utils/
+-rw-r--r--   0 jjy        (501) staff       (20)       94 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/video_faceparser/utils/__init__.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3079 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/video_faceparser/utils/corr.py
+-rw-r--r--   0 jjy        (501) staff       (20)     8847 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/video_faceparser/utils/extractor.py
+-rw-r--r--   0 jjy        (501) staff       (20)     3984 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/video_faceparser/utils/update.py
+-rw-r--r--   0 jjy        (501) staff       (20)     6502 2023-06-01 06:13:32.000000 innerverz-0.0.31/innerverz/video_faceparser/utils/util.py
+drwxr-xr-x   0 jjy        (501) staff       (20)        0 2023-06-03 07:04:52.265070 innerverz-0.0.31/innerverz.egg-info/
+-rw-r--r--   0 jjy        (501) staff       (20)      194 2023-06-03 07:04:52.000000 innerverz-0.0.31/innerverz.egg-info/PKG-INFO
+-rw-r--r--   0 jjy        (501) staff       (20)     3612 2023-06-03 07:04:52.000000 innerverz-0.0.31/innerverz.egg-info/SOURCES.txt
+-rw-r--r--   0 jjy        (501) staff       (20)        1 2023-06-03 07:04:52.000000 innerverz-0.0.31/innerverz.egg-info/dependency_links.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       74 2023-06-03 07:04:52.000000 innerverz-0.0.31/innerverz.egg-info/requires.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       10 2023-06-03 07:04:52.000000 innerverz-0.0.31/innerverz.egg-info/top_level.txt
+-rw-r--r--   0 jjy        (501) staff       (20)       89 2023-05-23 07:04:26.000000 innerverz-0.0.31/pyproject.toml
+-rw-r--r--   0 jjy        (501) staff       (20)       38 2023-06-03 07:04:52.285305 innerverz-0.0.31/setup.cfg
+-rw-r--r--   0 jjy        (501) staff       (20)      809 2023-06-03 07:04:50.000000 innerverz-0.0.31/setup.py
```

### Comparing `innerverz-0.0.30/LICENSE.txt` & `innerverz-0.0.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/__init__.py` & `innerverz-0.0.31/innerverz/__init__.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/data_process/main.py` & `innerverz-0.0.31/innerverz/data_process/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deblurrer/main.py` & `innerverz-0.0.31/innerverz/deblurrer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deblurrer/nets.py` & `innerverz-0.0.31/innerverz/deblurrer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deblurrer/test.py` & `innerverz-0.0.31/innerverz/deblurrer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/main.py` & `innerverz-0.0.31/innerverz/deca/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/models/FLAME.py` & `innerverz-0.0.31/innerverz/deca/models/FLAME.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/models/decoders.py` & `innerverz-0.0.31/innerverz/deca/models/decoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/models/detectors.py` & `innerverz-0.0.31/innerverz/deca/models/detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/models/encoders.py` & `innerverz-0.0.31/innerverz/deca/models/encoders.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/models/face_detectors.py` & `innerverz-0.0.31/innerverz/deca/models/face_detectors.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/models/lbs.py` & `innerverz-0.0.31/innerverz/deca/models/lbs.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/models/resnet.py` & `innerverz-0.0.31/innerverz/deca/models/resnet.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/test.py` & `innerverz-0.0.31/innerverz/deca/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/utils/cfg.py` & `innerverz-0.0.31/innerverz/deca/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/utils/rasterizer/setup.py` & `innerverz-0.0.31/innerverz/deca/utils/rasterizer/setup.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/utils/renderer.py` & `innerverz-0.0.31/innerverz/deca/utils/renderer.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/utils/rotation_converter.py` & `innerverz-0.0.31/innerverz/deca/utils/rotation_converter.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/utils/tensor_cropper.py` & `innerverz-0.0.31/innerverz/deca/utils/tensor_cropper.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deca/utils/util.py` & `innerverz-0.0.31/innerverz/deca/utils/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,15 +653,15 @@
         else:
             image_landmarks = plot_verts(image, predicted_landmark, color)
             if gt_landmarks is not None:
                 image_landmarks = plot_verts(image_landmarks, gt_landmarks_np[i]*image.shape[0]/2 + image.shape[0]/2, 'r')
         vis_landmarks.append(image_landmarks)
     vis_landmarks = np.stack(vis_landmarks)
     vis_landmarks = torch.from_numpy(vis_landmarks[:,:,:,[2,1,0]].transpose(0,3,1,2))/255.#, dtype=torch.float32)
-    return vis_landmarks
+    return vis_landmarks, predicted_landmark
 
 
 ############### for training
 def load_local_mask(image_size=256, mode='bbx'):
     if mode == 'bbx':
         # UV space face attributes bbx in size 2048 (l r t b)
         # face = np.array([512, 1536, 512, 1536]) #
```

### Comparing `innerverz-0.0.30/innerverz/deep3dmm/main.py` & `innerverz-0.0.31/innerverz/deep3dmm/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deep3dmm/nets.py` & `innerverz-0.0.31/innerverz/deep3dmm/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/deep3dmm/test.py` & `innerverz-0.0.31/innerverz/deep3dmm/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_alignment/graphic_utils.py` & `innerverz-0.0.31/innerverz/face_alignment/graphic_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_alignment/landmark.py` & `innerverz-0.0.31/innerverz/face_alignment/landmark.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_alignment/main.py` & `innerverz-0.0.31/innerverz/face_alignment/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
             quad = np.stack([c - x - y, c - x + y, c + x + y, c + x - y])
 
             src_pts = quad 
             ref_pts = np.array(((0, 0), (0, size), (size, size), (size, 0)))
             tfm, tfm_inv = get_similarity_transform_for_cv2(src_pts, ref_pts)
             face_img = cv2.warpAffine(np.array(img), tfm, (size, size), borderMode=None)
 
-            return face_img, tfm, tfm_inv
+            return face_img, tfm, tfm_inv, quad
             
             
     def align_face_from_106(self, img, full_lms, size = None):
         """
         Input
         ---------
             - img
@@ -222,15 +222,15 @@
             quad = np.stack([c - x - y, c - x + y, c + x + y, c + x - y])
 
             src_pts = quad + 0.01*np.random.rand(4,2)
             ref_pts = np.array(((0, 0), (0, size), (size, size), (size, 0)))
             tfm, tfm_inv = get_similarity_transform_for_cv2(src_pts, ref_pts)
             face_img = cv2.warpAffine(np.array(img), tfm, (size, size), borderMode=None)
 
-            return face_img, tfm, tfm_inv
+            return face_img, tfm, tfm_inv, quad
     
             
         elif self.align_style == 'invz':   
             eye_left     = (full_lms[39] + full_lms[35])*0.5
             eye_right    = (full_lms[89] + full_lms[93])*0.5
             eye_avg      = (eye_left + eye_right) * 0.5
             eye_to_eye   = eye_right - eye_left
@@ -248,15 +248,15 @@
             quad = np.stack([c - x - y, c - x + y, c + x + y, c + x - y])
             src_pts = quad + 0.01*np.random.rand(4,2)
             ref_pts = np.array(((0, 0), (0, size), (size, size), (size, 0)))
             tfm, tfm_inv = get_similarity_transform_for_cv2(src_pts, ref_pts)
             face_img = cv2.warpAffine(np.array(img), tfm, (size, size), borderMode=None)
             # face_img = cv2.warpAffine(np.array(img), tfm, (size, size), borderMode=cv2.BORDER_REFLECT)
         
-            return face_img, tfm, tfm_inv
+            return face_img, tfm, tfm_inv, quad
     
     
     def affine_transform(self, full_lms, tfm):
         """
         Input
         ---------
             - full_lms
```

### Comparing `innerverz-0.0.30/innerverz/face_alignment/retina_face.py` & `innerverz-0.0.31/innerverz/face_alignment/retina_face.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_alignment/test.py` & `innerverz-0.0.31/innerverz/face_alignment/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_alignment/utils/face_align.py` & `innerverz-0.0.31/innerverz/face_alignment/utils/face_align.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_alignment/utils/transform.py` & `innerverz-0.0.31/innerverz/face_alignment/utils/transform.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_color_transfer/main.py` & `innerverz-0.0.31/innerverz/face_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_color_transfer/nets.py` & `innerverz-0.0.31/innerverz/face_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.31/innerverz/face_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.31/innerverz/face_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.31/innerverz/face_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.31/innerverz/face_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_color_transfer/test.py` & `innerverz-0.0.31/innerverz/face_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_enhancer/main.py` & `innerverz-0.0.31/innerverz/face_enhancer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_enhancer/nets.py` & `innerverz-0.0.31/innerverz/face_enhancer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_enhancer/test.py` & `innerverz-0.0.31/innerverz/face_enhancer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_parser/main.py` & `innerverz-0.0.31/innerverz/face_parser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_parser/nets.py` & `innerverz-0.0.31/innerverz/face_parser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/face_parser/test.py` & `innerverz-0.0.31/innerverz/face_parser/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/head_color_transfer/main.py` & `innerverz-0.0.31/innerverz/head_color_transfer/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/head_color_transfer/nets.py` & `innerverz-0.0.31/innerverz/head_color_transfer/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/head_color_transfer/sub_nets/blend_net.py` & `innerverz-0.0.31/innerverz/head_color_transfer/sub_nets/blend_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/head_color_transfer/sub_nets/discriminator.py` & `innerverz-0.0.31/innerverz/head_color_transfer/sub_nets/discriminator.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/head_color_transfer/sub_nets/vgg19_net.py` & `innerverz-0.0.31/innerverz/head_color_transfer/sub_nets/vgg19_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/head_color_transfer/sub_nets/warp_net.py` & `innerverz-0.0.31/innerverz/head_color_transfer/sub_nets/warp_net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/head_color_transfer/test.py` & `innerverz-0.0.31/innerverz/head_color_transfer/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/id_extractor/main.py` & `innerverz-0.0.31/innerverz/id_extractor/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/id_extractor/nets.py` & `innerverz-0.0.31/innerverz/id_extractor/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/id_extractor/test.py` & `innerverz-0.0.31/innerverz/id_extractor/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/reage/main.py` & `innerverz-0.0.31/innerverz/reage/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/reage/net.py` & `innerverz-0.0.31/innerverz/reage/net.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/reage/net_utils.py` & `innerverz-0.0.31/innerverz/reage/net_utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/reage/test.py` & `innerverz-0.0.31/innerverz/reage/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/relighter/main.py` & `innerverz-0.0.31/innerverz/relighter/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/relighter/nets.py` & `innerverz-0.0.31/innerverz/relighter/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/relighter/test.py` & `innerverz-0.0.31/innerverz/relighter/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/upsampler/main.py` & `innerverz-0.0.31/innerverz/upsampler/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/upsampler/nets.py` & `innerverz-0.0.31/innerverz/upsampler/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/upsampler/test.py` & `innerverz-0.0.31/innerverz/upsampler/test.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/utils/download.py` & `innerverz-0.0.31/innerverz/utils/download.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/utils/input.py` & `innerverz-0.0.31/innerverz/utils/input.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/utils/utils.py` & `innerverz-0.0.31/innerverz/utils/utils.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/video_faceparser/main.py` & `innerverz-0.0.31/innerverz/video_faceparser/main.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/video_faceparser/nets.py` & `innerverz-0.0.31/innerverz/video_faceparser/nets.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/video_faceparser/utils/corr.py` & `innerverz-0.0.31/innerverz/video_faceparser/utils/corr.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/video_faceparser/utils/extractor.py` & `innerverz-0.0.31/innerverz/video_faceparser/utils/extractor.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/video_faceparser/utils/update.py` & `innerverz-0.0.31/innerverz/video_faceparser/utils/update.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz/video_faceparser/utils/util.py` & `innerverz-0.0.31/innerverz/video_faceparser/utils/util.py`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/innerverz.egg-info/SOURCES.txt` & `innerverz-0.0.31/innerverz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `innerverz-0.0.30/setup.py` & `innerverz-0.0.31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 except (IOError, ImportError, ModuleNotFoundError):
     print('WARNING: pandoc not enabled')
     long_description = open('README.md').read()
     pypandoc_enabled = False
 
 setup(
     name="innerverz",
-    version="0.0.30",
+    version="0.0.31",
     author="Innerverz",
     author_email="study@innerverz.com",
     description="innerverz package",
     long_description=long_description,
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages()
```

