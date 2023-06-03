# Comparing `tmp/mmit-0.5.1.tar.gz` & `tmp/mmit-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmit-0.5.1.tar", last modified: Thu Jun  1 21:33:06 2023, max compression
+gzip compressed data, was "mmit-0.5.2.tar", last modified: Sat Jun  3 21:24:12 2023, max compression
```

## Comparing `mmit-0.5.1.tar` & `mmit-0.5.2.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.612474 mmit-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.576473 mmit-0.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-01 21:32:53.000000 mmit-0.5.1/.github/issue_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-01 21:32:53.000000 mmit-0.5.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.576473 mmit-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-01 21:32:53.000000 mmit-0.5.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-01 21:32:53.000000 mmit-0.5.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-01 21:32:53.000000 mmit-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-01 21:32:53.000000 mmit-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-01 21:32:53.000000 mmit-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-01 21:33:06.612474 mmit-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-01 21:32:53.000000 mmit-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.576473 mmit-0.5.1/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-01 21:32:53.000000 mmit-0.5.1/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)      116 2023-06-01 21:32:53.000000 mmit-0.5.1/docker/build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 21:32:53.000000 mmit-0.5.1/docker/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-06-01 21:32:53.000000 mmit-0.5.1/docker/start_container.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.580473 mmit-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.580473 mmit-0.5.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.568473 mmit-0.5.1/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.580473 mmit-0.5.1/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/_static/css/baseline.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.580473 mmit-0.5.1/docs/source/_static/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/_static/logo/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/_static/logo/logo_title.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.580473 mmit-0.5.1/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/api/create_decoder.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/api/create_encoder.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/api/create_model.md
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.580473 mmit-0.5.1/docs/source/guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/guide/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/guide/install.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/guide/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.568473 mmit-0.5.1/docs/source/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.584473 mmit-0.5.1/docs/source/modules/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/modules/decoders/deeplabv3+.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/modules/decoders/deeplabv3.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/modules/decoders/fpn.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/modules/decoders/linknet.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/modules/decoders/pan.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/modules/decoders/pspnet.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/modules/decoders/unet++.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/modules/decoders/unet.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.584473 mmit-0.5.1/docs/source/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-01 21:32:53.000000 mmit-0.5.1/docs/source/modules/encoders/timm.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.588473 mmit-0.5.1/mmit/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.592473 mmit-0.5.1/mmit/base/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/base/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/base/extra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/base/mismatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/base/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/base/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/base/upsamplers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.592473 mmit-0.5.1/mmit/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/basedecoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.592473 mmit-0.5.1/mmit/decoders/deeplabv3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/deeplabv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/deeplabv3/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/deeplabv3/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/deeplabv3/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.596474 mmit-0.5.1/mmit/decoders/deeplabv3plus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/deeplabv3plus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/deeplabv3plus/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/deeplabv3plus/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/deeplabv3plus/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.596474 mmit-0.5.1/mmit/decoders/fpn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/fpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/fpn/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/fpn/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.596474 mmit-0.5.1/mmit/decoders/linknet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/linknet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/linknet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/linknet/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.600473 mmit-0.5.1/mmit/decoders/pan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/pan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/pan/fpa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/pan/gau.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/pan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.600473 mmit-0.5.1/mmit/decoders/pspnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/pspnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/pspnet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/pspnet/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.604474 mmit-0.5.1/mmit/decoders/unet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/unet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/unet/parts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.604474 mmit-0.5.1/mmit/decoders/unetplusplus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/unetplusplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/unetplusplus/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.604474 mmit-0.5.1/mmit/decoders/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/utils/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/decoders/utils/resizing_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.604474 mmit-0.5.1/mmit/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/encoders/basencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.604474 mmit-0.5.1/mmit/encoders/timm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/encoders/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/encoders/timm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.608474 mmit-0.5.1/mmit/factory/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/factory/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/factory/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/factory/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.608474 mmit-0.5.1/mmit/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/heads/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/heads/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.608474 mmit-0.5.1/mmit/models/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-01 21:32:53.000000 mmit-0.5.1/mmit/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.588473 mmit-0.5.1/mmit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-01 21:33:06.000000 mmit-0.5.1/mmit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-01 21:33:06.000000 mmit-0.5.1/mmit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:33:06.000000 mmit-0.5.1/mmit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 21:33:06.000000 mmit-0.5.1/mmit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 21:33:06.000000 mmit-0.5.1/mmit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-01 21:32:53.000000 mmit-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:33:06.616474 mmit-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.612474 mmit-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-01 21:32:53.000000 mmit-0.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:33:06.612474 mmit-0.5.1/tests/demo_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-01 21:32:53.000000 mmit-0.5.1/tests/demo_blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-01 21:32:53.000000 mmit-0.5.1/tests/demo_blocks/classic_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-01 21:32:53.000000 mmit-0.5.1/tests/demo_blocks/classic_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-01 21:32:53.000000 mmit-0.5.1/tests/demo_blocks/cursed_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-01 21:32:53.000000 mmit-0.5.1/tests/test_base_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-01 21:32:53.000000 mmit-0.5.1/tests/test_decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:32:53.000000 mmit-0.5.1/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-01 21:32:53.000000 mmit-0.5.1/tests/test_end2end.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.821797 mmit-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.813797 mmit-0.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-03 21:24:02.000000 mmit-0.5.2/.github/issue_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-03 21:24:02.000000 mmit-0.5.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.813797 mmit-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-03 21:24:02.000000 mmit-0.5.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-03 21:24:02.000000 mmit-0.5.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-03 21:24:02.000000 mmit-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-03 21:24:02.000000 mmit-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-03 21:24:02.000000 mmit-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-03 21:24:12.821797 mmit-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-03 21:24:02.000000 mmit-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.813797 mmit-0.5.2/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-03 21:24:02.000000 mmit-0.5.2/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)      116 2023-06-03 21:24:02.000000 mmit-0.5.2/docker/build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-03 21:24:02.000000 mmit-0.5.2/docker/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-06-03 21:24:02.000000 mmit-0.5.2/docker/start_container.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.813797 mmit-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.813797 mmit-0.5.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.809797 mmit-0.5.2/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.813797 mmit-0.5.2/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/_static/css/baseline.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.813797 mmit-0.5.2/docs/source/_static/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/_static/logo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/_static/logo/logo_title.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.813797 mmit-0.5.2/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/api/create_decoder.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/api/create_encoder.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/api/create_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.813797 mmit-0.5.2/docs/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/guide/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/guide/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/guide/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.809797 mmit-0.5.2/docs/source/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.813797 mmit-0.5.2/docs/source/modules/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/modules/decoders/deeplabv3+.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/modules/decoders/deeplabv3.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/modules/decoders/fpn.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/modules/decoders/linknet.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/modules/decoders/pan.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/modules/decoders/pspnet.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/modules/decoders/unet++.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/modules/decoders/unet.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.813797 mmit-0.5.2/docs/source/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-03 21:24:02.000000 mmit-0.5.2/docs/source/modules/encoders/timm.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.813797 mmit-0.5.2/mmit/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.817798 mmit-0.5.2/mmit/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/base/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/base/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/base/mismatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/base/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/base/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/base/upsamplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.817798 mmit-0.5.2/mmit/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/basedecoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.817798 mmit-0.5.2/mmit/decoders/deeplabv3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/deeplabv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/deeplabv3/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/deeplabv3/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/deeplabv3/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.817798 mmit-0.5.2/mmit/decoders/deeplabv3plus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/deeplabv3plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/deeplabv3plus/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/deeplabv3plus/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/deeplabv3plus/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.817798 mmit-0.5.2/mmit/decoders/fpn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/fpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/fpn/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/fpn/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.817798 mmit-0.5.2/mmit/decoders/linknet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/linknet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/linknet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/linknet/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.817798 mmit-0.5.2/mmit/decoders/pan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/pan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/pan/fpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/pan/gau.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/pan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.817798 mmit-0.5.2/mmit/decoders/pspnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/pspnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/pspnet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/pspnet/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.821797 mmit-0.5.2/mmit/decoders/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/unet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/unet/parts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.821797 mmit-0.5.2/mmit/decoders/unetplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/unetplusplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/unetplusplus/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.821797 mmit-0.5.2/mmit/decoders/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/utils/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/decoders/utils/resizing_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.821797 mmit-0.5.2/mmit/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/encoders/basencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.821797 mmit-0.5.2/mmit/encoders/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/encoders/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/encoders/timm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.821797 mmit-0.5.2/mmit/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/factory/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/factory/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/factory/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.821797 mmit-0.5.2/mmit/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/heads/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/heads/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.821797 mmit-0.5.2/mmit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-03 21:24:02.000000 mmit-0.5.2/mmit/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.817798 mmit-0.5.2/mmit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-03 21:24:12.000000 mmit-0.5.2/mmit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-03 21:24:12.000000 mmit-0.5.2/mmit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 21:24:12.000000 mmit-0.5.2/mmit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-03 21:24:12.000000 mmit-0.5.2/mmit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-03 21:24:12.000000 mmit-0.5.2/mmit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-03 21:24:02.000000 mmit-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 21:24:12.821797 mmit-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.821797 mmit-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-03 21:24:02.000000 mmit-0.5.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:12.821797 mmit-0.5.2/tests/demo_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-03 21:24:02.000000 mmit-0.5.2/tests/demo_blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-03 21:24:02.000000 mmit-0.5.2/tests/demo_blocks/classic_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-03 21:24:02.000000 mmit-0.5.2/tests/demo_blocks/classic_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-03 21:24:02.000000 mmit-0.5.2/tests/demo_blocks/cursed_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-03 21:24:02.000000 mmit-0.5.2/tests/test_base_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-03 21:24:02.000000 mmit-0.5.2/tests/test_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:24:02.000000 mmit-0.5.2/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-03 21:24:02.000000 mmit-0.5.2/tests/test_end2end.py
```

### Comparing `mmit-0.5.1/.github/issue_template.md` & `mmit-0.5.2/.github/issue_template.md`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/.github/pull_request_template.md` & `mmit-0.5.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/.github/workflows/ci.yaml` & `mmit-0.5.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/.github/workflows/python-publish.yml` & `mmit-0.5.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/.gitignore` & `mmit-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/LICENSE` & `mmit-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/PKG-INFO` & `mmit-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmit
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Python package for computer vision experiments and research.
 Author-email: Andrea Boscolo Camiletto <abcamiletto@gmail.com>
 Project-URL: Homepage, https://github.com/abcamiletto/mmit
 Project-URL: Repository, https://github.com/abcamiletto/mmit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mmit-0.5.1/README.md` & `mmit-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/docker/start_container.sh` & `mmit-0.5.2/docker/start_container.sh`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/docs/.readthedocs.yaml` & `mmit-0.5.2/docs/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/docs/Makefile` & `mmit-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/docs/make.bat` & `mmit-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/docs/source/_static/css/baseline.css` & `mmit-0.5.2/docs/source/_static/css/baseline.css`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/docs/source/_static/logo/logo.png` & `mmit-0.5.2/docs/source/_static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/docs/source/_static/logo/logo_title.png` & `mmit-0.5.2/docs/source/_static/logo/logo_title.png`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/docs/source/conf.py` & `mmit-0.5.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/docs/source/guide/examples.md` & `mmit-0.5.2/docs/source/guide/examples.md`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/docs/source/index.md` & `mmit-0.5.2/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/base/activations.py` & `mmit-0.5.2/mmit/base/activations.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/base/extra.py` & `mmit-0.5.2/mmit/base/extra.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/base/mismatch.py` & `mmit-0.5.2/mmit/base/mismatch.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/base/modules.py` & `mmit-0.5.2/mmit/base/modules.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/base/norms.py` & `mmit-0.5.2/mmit/base/norms.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/base/upsamplers.py` & `mmit-0.5.2/mmit/base/upsamplers.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/basedecoder.py` & `mmit-0.5.2/mmit/decoders/basedecoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/deeplabv3/aspp.py` & `mmit-0.5.2/mmit/decoders/deeplabv3/aspp.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/deeplabv3/model.py` & `mmit-0.5.2/mmit/decoders/deeplabv3/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/deeplabv3/parts.py` & `mmit-0.5.2/mmit/decoders/deeplabv3/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/deeplabv3plus/model.py` & `mmit-0.5.2/mmit/decoders/deeplabv3plus/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/deeplabv3plus/parts.py` & `mmit-0.5.2/mmit/decoders/deeplabv3plus/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/fpn/model.py` & `mmit-0.5.2/mmit/decoders/fpn/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,26 +29,28 @@
         decoder_channel: The channel to use on the decoder.
         upsample_layer: Layer to use for the upsampling.
         norm_layer: Normalization layer to use.
         activation_layer: Activation function to use.
         extra_layer: Addional layer to use.
         mismatch_layer: Strategy to deal with odd resolutions.
 
+
     """
 
     def __init__(
         self,
         input_channels: List[int],
         input_reductions: List[int],
         decoder_channel: int = DEFAULT_CHANNEL,
         upsample_layer: Type[nn.Module] = up.ConvTranspose2d,
         norm_layer: Type[nn.Module] = nn.BatchNorm2d,
         activation_layer: Type[nn.Module] = nn.ReLU,
         extra_layer: Type[nn.Module] = nn.Identity,
         mismatch_layer: Type[nn.Module] = mm.Pad,
+        merge_mode: str = "sum",
     ):
         super().__init__(input_channels, input_reductions)
 
         up_lays = self._format_upsample_layers(input_reductions, upsample_layer)
 
         specs = norm_layer, activation_layer, extra_layer, mismatch_layer
         input_channels = input_channels[1:][::-1]
@@ -68,22 +70,30 @@
         out_blocks = []
         for red in input_reductions[1:][::-1]:
             up_lay = partial(upsample_layer, scale=red)
             block = md.ConvNormAct(decoder_channel, decoder_channel, 3, *specs, up_lay)
             out_blocks.append(block)
 
         self.out_blocks = nn.ModuleList(out_blocks)
-        self._out_classes = decoder_channel * len(out_blocks)
 
         # Input block for the first layer
         self.input_block = nn.Conv2d(input_channels[0], decoder_channel, 1)
 
         # Mismatch layer in case for weird sizes
         self.mismatch_layer = mismatch_layer()
 
+        # Merge mode
+        self.merge_mode = merge_mode
+        if merge_mode not in ["sum", "cat"]:
+            raise ValueError(f"Merge mode {merge_mode} not 'sum' or 'cat'.")
+
+        # Output classes
+        factor = len(out_blocks) if merge_mode == "cat" else 1
+        self._out_classes = decoder_channel * factor
+
     @size_control
     def forward(self, *features: torch.Tensor) -> torch.Tensor:
         # Dropping the first channel since we don't use the input image
         features = features[1:]
 
         # Reversing the input channels since we're going from the bottom up
         features = features[::-1]
@@ -98,23 +108,23 @@
         # We store build the pyramid of features
         out_maps = [x]
         for skip_block, skip_feature in zip(self.skip_blocks, skips):
             x = skip_block(x, skip_feature)
             out_maps.append(x)
 
         # We process the pyramid of features
-        outputs = []
+        pyram = []
         for out_block, out_map in zip(self.out_blocks, out_maps):
             x = out_block(out_map)
-            outputs.append(x.clone())
+            pyram.append(x.clone())
 
         # We fix the output sizes in case of weird shapes
-        outputs = self._fix_output_sizes(outputs)
+        pyram = self._fix_output_sizes(pyram)
 
-        result = torch.cat(outputs, dim=1)
+        result = self._merge_pyramid(pyram)
         return result
 
     @property
     def out_classes(self) -> int:
         return self._out_classes
 
     def _format_upsample_layers(self, input_reductions, upsample_layer):
@@ -137,7 +147,10 @@
         higher_res_output = outputs[-1]
         new_outputs = [higher_res_output]
         for output in outputs[:-1]:
             resized, _ = self.mismatch_layer(output, higher_res_output)
             new_outputs.append(resized)
 
         return new_outputs
+
+    def _merge_pyramid(self, pyram):
+        return torch.cat(pyram, dim=1) if self.merge_mode == "cat" else sum(pyram)
```

### Comparing `mmit-0.5.1/mmit/decoders/fpn/parts.py` & `mmit-0.5.2/mmit/decoders/fpn/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/linknet/model.py` & `mmit-0.5.2/mmit/decoders/linknet/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/linknet/parts.py` & `mmit-0.5.2/mmit/decoders/linknet/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/pan/fpa.py` & `mmit-0.5.2/mmit/decoders/pan/fpa.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/pan/gau.py` & `mmit-0.5.2/mmit/decoders/pan/gau.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/pan/model.py` & `mmit-0.5.2/mmit/decoders/pan/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/pspnet/model.py` & `mmit-0.5.2/mmit/decoders/pspnet/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/pspnet/parts.py` & `mmit-0.5.2/mmit/decoders/pspnet/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/unet/model.py` & `mmit-0.5.2/mmit/decoders/unet/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/unet/parts.py` & `mmit-0.5.2/mmit/decoders/unet/parts.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/unetplusplus/model.py` & `mmit-0.5.2/mmit/decoders/unetplusplus/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/decoders/utils/resize.py` & `mmit-0.5.2/mmit/decoders/utils/resize.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/encoders/basencoder.py` & `mmit-0.5.2/mmit/encoders/basencoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/encoders/timm/model.py` & `mmit-0.5.2/mmit/encoders/timm/model.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/factory/components.py` & `mmit-0.5.2/mmit/factory/components.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/factory/factory.py` & `mmit-0.5.2/mmit/factory/factory.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/factory/registry.py` & `mmit-0.5.2/mmit/factory/registry.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/heads/classification.py` & `mmit-0.5.2/mmit/heads/classification.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit/heads/segmentation.py` & `mmit-0.5.2/mmit/heads/segmentation.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/mmit.egg-info/PKG-INFO` & `mmit-0.5.2/mmit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmit
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Python package for computer vision experiments and research.
 Author-email: Andrea Boscolo Camiletto <abcamiletto@gmail.com>
 Project-URL: Homepage, https://github.com/abcamiletto/mmit
 Project-URL: Repository, https://github.com/abcamiletto/mmit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mmit-0.5.1/mmit.egg-info/SOURCES.txt` & `mmit-0.5.2/mmit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/pyproject.toml` & `mmit-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 readme = "README.md"
 authors = [{ name = "Andrea Boscolo Camiletto", email = "abcamiletto@gmail.com" }]
 dependencies = [
     "timm>=0.9.0",
     "torch>=1.10"
 ]
 requires-python = ">=3.8"
-version = "0.5.1"
+version = "0.5.2"
 
 [project.urls]
 Homepage = "https://github.com/abcamiletto/mmit"
 Repository = "https://github.com/abcamiletto/mmit"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pytest", "pytest-cov", "pytest-lazy-fixture", "pre-commit"]
```

### Comparing `mmit-0.5.1/tests/demo_blocks/classic_decoder.py` & `mmit-0.5.2/tests/demo_blocks/classic_decoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/tests/demo_blocks/classic_encoder.py` & `mmit-0.5.2/tests/demo_blocks/classic_encoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/tests/demo_blocks/cursed_encoder.py` & `mmit-0.5.2/tests/demo_blocks/cursed_encoder.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/tests/test_base_components.py` & `mmit-0.5.2/tests/test_base_components.py`

 * *Files identical despite different names*

### Comparing `mmit-0.5.1/tests/test_decoders.py` & `mmit-0.5.2/tests/test_decoders.py`

 * *Files identical despite different names*

