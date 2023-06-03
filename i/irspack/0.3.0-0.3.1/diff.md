# Comparing `tmp/irspack-0.3.0.tar.gz` & `tmp/irspack-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/irspack-0.3.0.tar", last modified: Thu Jun 30 08:47:54 2022, max compression
+gzip compressed data, was "irspack-0.3.1.tar", last modified: Sat Jun  3 05:41:49 2023, max compression
```

## Comparing `irspack-0.3.0.tar` & `irspack-0.3.1.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-06-30 08:47:51.000000 irspack-0.3.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-06-30 08:47:51.000000 irspack-0.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-06-30 08:47:51.000000 irspack-0.3.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-06-30 08:47:51.000000 irspack-0.3.0/.github/workflows/run-test.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4771 2022-06-30 08:47:51.000000 irspack-0.3.0/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-06-30 08:47:51.000000 irspack-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-06-30 08:47:51.000000 irspack-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-06-30 08:47:51.000000 irspack-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-06-30 08:47:51.000000 irspack-0.3.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-06-30 08:47:51.000000 irspack-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-06-30 08:47:51.000000 irspack-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6670 2022-06-30 08:47:54.000000 irspack-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5200 2022-06-30 08:47:51.000000 irspack-0.3.0/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/cpp_source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/cpp_source/als/
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-06-30 08:47:51.000000 irspack-0.3.0/cpp_source/als/IALSLearningConfig.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    26349 2022-06-30 08:47:51.000000 irspack-0.3.0/cpp_source/als/IALSTrainer.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-06-30 08:47:51.000000 irspack-0.3.0/cpp_source/als/definitions.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     5313 2022-06-30 08:47:51.000000 irspack-0.3.0/cpp_source/als/wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-06-30 08:47:51.000000 irspack-0.3.0/cpp_source/argcheck.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    16352 2022-06-30 08:47:51.000000 irspack-0.3.0/cpp_source/evaluator.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/cpp_source/knn/
--rw-r--r--   0 runner    (1001) docker     (121)     5567 2022-06-30 08:47:51.000000 irspack-0.3.0/cpp_source/knn/knn.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    12290 2022-06-30 08:47:51.000000 irspack-0.3.0/cpp_source/knn/similarities.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2908 2022-06-30 08:47:51.000000 irspack-0.3.0/cpp_source/knn/wrapper.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-06-30 08:47:51.000000 irspack-0.3.0/cpp_source/util.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    18127 2022-06-30 08:47:51.000000 irspack-0.3.0/cpp_source/util.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)      605 2022-06-30 08:47:51.000000 irspack-0.3.0/create_pb_stubs.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-06-30 08:47:51.000000 irspack-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-06-30 08:47:51.000000 irspack-0.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2022-06-30 08:47:51.000000 irspack-0.3.0/docs/source/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3069 2022-06-30 08:47:51.000000 irspack-0.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2022-06-30 08:47:51.000000 irspack-0.3.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)    13557 2022-06-30 08:47:51.000000 irspack-0.3.0/examples/1-vs-100-negative.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     8626 2022-06-30 08:47:51.000000 irspack-0.3.0/examples/evaluate-recommender.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    44927 2022-06-30 08:47:51.000000 irspack-0.3.0/examples/hyperparameter-optimization.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/examples/movielens/
--rw-r--r--   0 runner    (1001) docker     (121)     2831 2022-06-30 08:47:51.000000 irspack-0.3.0/examples/movielens/movielens_1m.py
--rw-r--r--   0 runner    (1001) docker     (121)     2801 2022-06-30 08:47:51.000000 irspack-0.3.0/examples/movielens/movielens_1m_cold.py
--rw-r--r--   0 runner    (1001) docker     (121)     4545 2022-06-30 08:47:51.000000 irspack-0.3.0/examples/movielens/movielens_20m_cold.py
--rw-r--r--   0 runner    (1001) docker     (121)    19226 2022-06-30 08:47:51.000000 irspack-0.3.0/examples/split1.png
--rw-r--r--   0 runner    (1001) docker     (121)    23010 2022-06-30 08:47:51.000000 irspack-0.3.0/examples/split2.png
--rw-r--r--   0 runner    (1001) docker     (121)    26372 2022-06-30 08:47:51.000000 irspack-0.3.0/examples/train-first-recommender.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-06-30 08:47:51.000000 irspack-0.3.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-06-30 08:47:51.000000 irspack-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-06-30 08:47:51.000000 irspack-0.3.0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      169 2022-06-30 08:47:51.000000 irspack-0.3.0/run_autobuild.sh
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-30 08:47:54.000000 irspack-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-06-30 08:47:51.000000 irspack-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/src/irspack/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/_threading.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/src/irspack/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2104 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/dataset/amazon_music.py
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/dataset/citeulike.py
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/dataset/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/src/irspack/dataset/movielens/
--rw-r--r--   0 runner    (1001) docker     (121)     2680 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/dataset/movielens/ML100K.py
--rw-r--r--   0 runner    (1001) docker     (121)     2486 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/dataset/movielens/ML1M.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/dataset/movielens/ML20M.py
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/dataset/movielens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/dataset/movielens/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3720 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/dataset/neu_mf.py
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/default_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/src/irspack/evaluation/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/evaluation/_core.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/evaluation/evaluate_df_to_df.py
--rw-r--r--   0 runner    (1001) docker     (121)    14764 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/src/irspack/optimization/
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7317 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/optimization/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3226 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/optimization/parameter_range.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/src/irspack/recommenders/
--rw-r--r--   0 runner    (1001) docker     (121)     2501 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5782 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/_ials.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/_knn.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    18433 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/base_earlystop.py
--rw-r--r--   0 runner    (1001) docker     (121)     5450 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/bpr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1616 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/dense_slim.py
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/edlae.py
--rw-r--r--   0 runner    (1001) docker     (121)    24724 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/ials.py
--rw-r--r--   0 runner    (1001) docker     (121)    11796 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/knn.py
--rw-r--r--   0 runner    (1001) docker     (121)    11969 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/multvae.py
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/nmf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2929 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/p3.py
--rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/rp3.py
--rw-r--r--   0 runner    (1001) docker     (121)     3725 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/slim.py
--rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/toppop.py
--rw-r--r--   0 runner    (1001) docker     (121)     3371 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/truncsvd.py
--rw-r--r--   0 runner    (1001) docker     (121)     8025 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/recommenders/user_knn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/src/irspack/split/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5355 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/split/specified.py
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/split/time.py
--rw-r--r--   0 runner    (1001) docker     (121)    13279 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/split/userwise.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/src/irspack/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     4866 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2593 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/utils/_util_cpp.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    18027 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/utils/id_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-06-30 08:47:51.000000 irspack-0.3.0/src/irspack/utils/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/src/irspack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6670 2022-06-30 08:47:54.000000 irspack-0.3.0/src/irspack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3802 2022-06-30 08:47:54.000000 irspack-0.3.0/src/irspack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-30 08:47:54.000000 irspack-0.3.0/src/irspack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-30 08:47:54.000000 irspack-0.3.0/src/irspack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-30 08:47:54.000000 irspack-0.3.0/src/irspack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/tests/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5517 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/dataset/test_ml1m.py
--rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/dataset/test_neumf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/tests/evaluation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3061 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/evaluation/test_df_vs_df.py
--rw-r--r--   0 runner    (1001) docker     (121)     8741 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/evaluation/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4960 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/evaluation/test_restricted_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/mock_recommender.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/tests/optimization/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3825 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/optimization/test_earlystop_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/optimization/test_ials_doubling_dimension.py
--rw-r--r--   0 runner    (1001) docker     (121)     4009 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/optimization/test_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/tests/recommenders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/recommenders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/recommenders/test_bpr.py
--rw-r--r--   0 runner    (1001) docker     (121)     9415 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/recommenders/test_ials.py
--rw-r--r--   0 runner    (1001) docker     (121)     6963 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/recommenders/test_knn.py
--rw-r--r--   0 runner    (1001) docker     (121)     1723 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/recommenders/test_learn_all.py
--rw-r--r--   0 runner    (1001) docker     (121)     2757 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/recommenders/test_slim.py
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/recommenders/test_topop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/recommenders/test_truncsvd.py
--rw-r--r--   0 runner    (1001) docker     (121)     2211 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/recommenders/test_user_knn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/tests/split/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6534 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/split/test_specific_holdout.py
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/split/test_time_holdout.py
--rw-r--r--   0 runner    (1001) docker     (121)     6622 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/split/test_userwise_split.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:54.000000 irspack-0.3.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11534 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/utils/test_id_mapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2536 2022-06-30 08:47:51.000000 irspack-0.3.0/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.435490 irspack-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-03 05:41:45.000000 irspack-0.3.1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-03 05:41:45.000000 irspack-0.3.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.423490 irspack-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.423490 irspack-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-03 05:41:45.000000 irspack-0.3.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-03 05:41:45.000000 irspack-0.3.1/.github/workflows/run-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-03 05:41:45.000000 irspack-0.3.1/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-03 05:41:45.000000 irspack-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-03 05:41:45.000000 irspack-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-03 05:41:45.000000 irspack-0.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-03 05:41:45.000000 irspack-0.3.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-03 05:41:45.000000 irspack-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-03 05:41:45.000000 irspack-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-06-03 05:41:49.435490 irspack-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-03 05:41:45.000000 irspack-0.3.1/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.427490 irspack-0.3.1/cpp_source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.427490 irspack-0.3.1/cpp_source/als/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-03 05:41:45.000000 irspack-0.3.1/cpp_source/als/IALSLearningConfig.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26349 2023-06-03 05:41:45.000000 irspack-0.3.1/cpp_source/als/IALSTrainer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-03 05:41:45.000000 irspack-0.3.1/cpp_source/als/definitions.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-06-03 05:41:45.000000 irspack-0.3.1/cpp_source/als/wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-03 05:41:45.000000 irspack-0.3.1/cpp_source/argcheck.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16352 2023-06-03 05:41:45.000000 irspack-0.3.1/cpp_source/evaluator.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.427490 irspack-0.3.1/cpp_source/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-06-03 05:41:45.000000 irspack-0.3.1/cpp_source/knn/knn.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12290 2023-06-03 05:41:45.000000 irspack-0.3.1/cpp_source/knn/similarities.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-03 05:41:45.000000 irspack-0.3.1/cpp_source/knn/wrapper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-03 05:41:45.000000 irspack-0.3.1/cpp_source/util.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18127 2023-06-03 05:41:45.000000 irspack-0.3.1/cpp_source/util.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      605 2023-06-03 05:41:45.000000 irspack-0.3.1/create_pb_stubs.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.427490 irspack-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-03 05:41:45.000000 irspack-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-03 05:41:45.000000 irspack-0.3.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.427490 irspack-0.3.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-03 05:41:45.000000 irspack-0.3.1/docs/source/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-03 05:41:45.000000 irspack-0.3.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-03 05:41:45.000000 irspack-0.3.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.427490 irspack-0.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    13557 2023-06-03 05:41:45.000000 irspack-0.3.1/examples/1-vs-100-negative.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-06-03 05:41:45.000000 irspack-0.3.1/examples/evaluate-recommender.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    44927 2023-06-03 05:41:45.000000 irspack-0.3.1/examples/hyperparameter-optimization.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.427490 irspack-0.3.1/examples/movielens/
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-03 05:41:45.000000 irspack-0.3.1/examples/movielens/movielens_1m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-03 05:41:45.000000 irspack-0.3.1/examples/movielens/movielens_1m_cold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-03 05:41:45.000000 irspack-0.3.1/examples/movielens/movielens_20m_cold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19226 2023-06-03 05:41:45.000000 irspack-0.3.1/examples/split1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23010 2023-06-03 05:41:45.000000 irspack-0.3.1/examples/split2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26372 2023-06-03 05:41:45.000000 irspack-0.3.1/examples/train-first-recommender.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-03 05:41:45.000000 irspack-0.3.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-03 05:41:45.000000 irspack-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-03 05:41:45.000000 irspack-0.3.1/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      169 2023-06-03 05:41:45.000000 irspack-0.3.1/run_autobuild.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 05:41:49.435490 irspack-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-03 05:41:45.000000 irspack-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.423490 irspack-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.427490 irspack-0.3.1/src/irspack/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/_threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.427490 irspack-0.3.1/src/irspack/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/dataset/amazon_music.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/dataset/citeulike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/dataset/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.427490 irspack-0.3.1/src/irspack/dataset/movielens/
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/dataset/movielens/ML100K.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/dataset/movielens/ML1M.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/dataset/movielens/ML20M.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/dataset/movielens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/dataset/movielens/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/dataset/neu_mf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/default_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.427490 irspack-0.3.1/src/irspack/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/evaluation/_core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/evaluation/evaluate_df_to_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.427490 irspack-0.3.1/src/irspack/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/optimization/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/optimization/parameter_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.431490 irspack-0.3.1/src/irspack/recommenders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/_ials.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/_knn.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18489 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/base_earlystop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/bpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/dense_slim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/edlae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24829 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/ials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/multvae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/rp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/slim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/toppop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/truncsvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/recommenders/user_knn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.431490 irspack-0.3.1/src/irspack/split/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/split/specified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/split/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/split/userwise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.431490 irspack-0.3.1/src/irspack/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/utils/_util_cpp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18027 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/utils/id_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-03 05:41:45.000000 irspack-0.3.1/src/irspack/utils/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.427490 irspack-0.3.1/src/irspack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-06-03 05:41:49.000000 irspack-0.3.1/src/irspack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-03 05:41:49.000000 irspack-0.3.1/src/irspack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 05:41:49.000000 irspack-0.3.1/src/irspack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-03 05:41:49.000000 irspack-0.3.1/src/irspack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-03 05:41:49.000000 irspack-0.3.1/src/irspack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.431490 irspack-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.431490 irspack-0.3.1/tests/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/dataset/test_ml1m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/dataset/test_neumf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.431490 irspack-0.3.1/tests/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/evaluation/test_df_vs_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/evaluation/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/evaluation/test_restricted_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/mock_recommender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.431490 irspack-0.3.1/tests/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/optimization/test_earlystop_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/optimization/test_ials_doubling_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/optimization/test_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.431490 irspack-0.3.1/tests/recommenders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/recommenders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/recommenders/test_bpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/recommenders/test_ials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/recommenders/test_knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/recommenders/test_learn_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/recommenders/test_slim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/recommenders/test_topop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/recommenders/test_truncsvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/recommenders/test_user_knn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.435490 irspack-0.3.1/tests/split/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/split/test_specific_holdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/split/test_time_holdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/split/test_userwise_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:49.435490 irspack-0.3.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/utils/test_id_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-03 05:41:45.000000 irspack-0.3.1/tests/utils/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `irspack-0.3.0/.github/workflows/run-test.yml` & `irspack-0.3.1/.github/workflows/run-test.yml`

 * *Files 21% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 on: [push, pull_request]
 jobs:
   run_pytest_upload_coverage:
     runs-on: ubuntu-latest
     env:
       OS: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Setup Python
-        uses: actions/setup-python@master
+        uses: actions/setup-python@v3
         with:
-          python-version: 3.8
+          python-version: 3.11
       - name: Build irspack (ubuntu)
         run: |
           pip install --upgrade pip
           sudo apt-get install lcov
           FLAGS="-fprofile-arcs -ftest-coverage"
           CFLAGS="$FLAGS" CXXFLAGS="$FLAGS" pip install -e .
       - name: Run pytest
         run: |
-          pip install pytest pytest-mock pytest-cov
-          pip install lightfm jaxlib jax dm-haiku optax
+          pip install setuptools wheel pytest pytest-mock pytest-cov
+          pip install jaxlib jax dm-haiku optax
+          pip install --no-use-pep517 lightfm
           pytest --cov=./src/irspack tests/
       - name: Generate coverage (ubuntu)
         run: |
           coverage xml
           lcov -d `pwd` -c -o coverage.info
       - name: Upload coverage to Codecov
         uses: codecov/codecov-action@v3
```

### Comparing `irspack-0.3.0/.github/workflows/wheels.yml` & `irspack-0.3.1/.github/workflows/wheels.yml`

 * *Files 12% similar despite different names*

```diff
@@ -3,138 +3,146 @@
   push:
     branches:
       - main
   release:
     types:
       - created
 env:
-  cibuildwheel_version: "2.7.0"
+  cibuildwheel_version: '2.13.0'
 jobs:
   build_sdist:
     name: Build source distribution
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v3
         name: Install Python
         with:
-          python-version: "3.7"
+          python-version: '3.11'
       - name: Build sdist
         run: pip install pybind11 setuptools_scm && python setup.py sdist
       - uses: actions/upload-artifact@v2
         with:
           path: dist/*.tar.gz
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     env:
-      MACOSX_DEPLOYMENT_TARGET: "10.9"
-      CIBW_BUILD_VERBOSITY: "1"
+      MACOSX_DEPLOYMENT_TARGET: '10.14'
+      CIBW_BUILD_VERBOSITY: '1'
       CIBW_BUILD: "${{ matrix.cibw.build || '*' }}"
       CIBW_SKIP: "${{ matrix.cibw.skip || '' }}"
       CIBW_ENVIRONMENT: "${{ matrix.cibw.env || '' }}"
       CIBW_TEST_COMMAND: pytest {project}/tests
       CIBW_TEST_REQUIRES: pytest pytest-mock
-      CIBW_MANYLINUX_X86_64_IMAGE: "${{ matrix.cibw.manylinux_image }}"
-      CIBW_MANYLINUX_I686_IMAGE: "${{ matrix.cibw.manylinux_image }}"
-      CIBW_MANYLINUX_AARCH64_IMAGE: "${{ matrix.cibw.manylinux_image }}"
+      CIBW_MANYLINUX_X86_64_IMAGE: '${{ matrix.cibw.manylinux_image }}'
+      CIBW_MANYLINUX_I686_IMAGE: '${{ matrix.cibw.manylinux_image }}'
+      CIBW_MANYLINUX_AARCH64_IMAGE: '${{ matrix.cibw.manylinux_image }}'
       CIBW_ARCHS_LINUX: "${{ matrix.cibw.arch || 'auto' }}"
       CIBW_ARCHS_MACOS: "${{ matrix.cibw.arch || 'auto' }}"
     strategy:
       matrix:
         include:
-          - os: macos-10.15
+          - os: macos-12
             name: mac
             cibw:
               arch: x86_64
               env: CFLAGS='-march=core-avx-i'
-              build: "cp37* cp38*"
+              build: 'cp37* cp38*'
 
-          - os: macos-10.15
+          - os: macos-12
             name: mac-arm
             cibw:
               arch: universal2
-              build: "cp39* cp310*"
-              env: ""
+              build: 'cp39* cp310* cp311*'
+              env: ''
 
           - os: ubuntu-20.04
             name: manylinux1
             cibw:
-              build: "cp37*"
-              skip: "*musllinux*"
+              build: 'cp37*'
+              skip: '*musllinux*'
               manylinux_image: manylinux2010
               env: CFLAGS='-march=core-avx-i'
               arch: auto64
 
           - os: ubuntu-20.04
             name: manylinux2014
             cibw:
-              build: "cp38* cp39* cp310*"
-              skip: "*musllinux*"
+              build: 'cp38* cp39* cp310* cp311*'
+              skip: '*musllinux*'
               manylinux_image: manylinux2014
               env: CFLAGS='-march=core-avx-i'
               arch: auto64
 
           - os: ubuntu-20.04
             name: manylinux_aarch64_cp37
             cibw:
-              build: "cp37*"
-              skip: "*musllinux*"
+              build: 'cp37*'
+              skip: '*musllinux*'
               manylinux_image: manylinux2014
               arch: aarch64
 
           - os: ubuntu-20.04
             name: manylinux_aarch64_cp38
             cibw:
-              build: "cp38*"
-              skip: "*musllinux*"
+              build: 'cp38*'
+              skip: '*musllinux*'
               manylinux_image: manylinux2014
               arch: aarch64
 
           - os: ubuntu-20.04
             name: manylinux_aarch64_cp39
             cibw:
-              build: "cp39*"
-              skip: "*musllinux*"
+              build: 'cp39*'
+              skip: '*musllinux*'
               manylinux_image: manylinux2014
               arch: aarch64
 
           - os: ubuntu-20.04
             name: manylinux_aarch64_cp310
             cibw:
-              build: "cp310*"
-              skip: "*musllinux*"
+              build: 'cp310*'
+              skip: '*musllinux*'
+              manylinux_image: manylinux2014
+              arch: aarch64
+
+          - os: ubuntu-20.04
+            name: manylinux_aarch64_cp311
+            cibw:
+              build: 'cp311*'
+              skip: '*musllinux*'
               manylinux_image: manylinux2014
               arch: aarch64
 
           - os: windows-2019
             name: win_amd64
             architecture: x64
             cibw:
-              build: "cp*win_amd64"
+              build: 'cp*win_amd64'
               env: "CL='/arch:AVX'"
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v3
         name: Install Python
       - name: register qemu
         if: contains(matrix.cibw.arch, 'aarch64')
         run: |
           docker run --rm --privileged hypriot/qemu-register:v4.2.0
       - name: Install cibuildwheel
         run: python -m pip install cibuildwheel=="${{env.cibuildwheel_version}}"
       - name: Build wheels
         run: python -m cibuildwheel --output-dir wheelhouse
 
-      - uses: actions/upload-artifact@v2
+      - uses: actions/upload-artifact@v3
         with:
           path: ./wheelhouse/*.whl
 
   upload_pypi:
     needs: [build_wheels, build_sdist]
     runs-on: ubuntu-latest
     steps:
```

### Comparing `irspack-0.3.0/CMakeLists.txt` & `irspack-0.3.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/LICENSE` & `irspack-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/Readme.md` & `irspack-0.3.1/Readme.md`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/cpp_source/als/IALSLearningConfig.hpp` & `irspack-0.3.1/cpp_source/als/IALSLearningConfig.hpp`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/cpp_source/als/IALSTrainer.hpp` & `irspack-0.3.1/cpp_source/als/IALSTrainer.hpp`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/cpp_source/als/wrapper.cpp` & `irspack-0.3.1/cpp_source/als/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/cpp_source/argcheck.hpp` & `irspack-0.3.1/cpp_source/argcheck.hpp`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/cpp_source/evaluator.cpp` & `irspack-0.3.1/cpp_source/evaluator.cpp`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/cpp_source/knn/knn.hpp` & `irspack-0.3.1/cpp_source/knn/knn.hpp`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/cpp_source/knn/similarities.hpp` & `irspack-0.3.1/cpp_source/knn/similarities.hpp`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/cpp_source/knn/wrapper.cpp` & `irspack-0.3.1/cpp_source/knn/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/cpp_source/util.cpp` & `irspack-0.3.1/cpp_source/util.cpp`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/cpp_source/util.hpp` & `irspack-0.3.1/cpp_source/util.hpp`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/create_pb_stubs.sh` & `irspack-0.3.1/create_pb_stubs.sh`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/docs/Makefile` & `irspack-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/docs/source/api_reference.rst` & `irspack-0.3.1/docs/source/api_reference.rst`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/docs/source/conf.py` & `irspack-0.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/docs/source/index.rst` & `irspack-0.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/examples/1-vs-100-negative.ipynb` & `irspack-0.3.1/examples/1-vs-100-negative.ipynb`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/examples/evaluate-recommender.ipynb` & `irspack-0.3.1/examples/evaluate-recommender.ipynb`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/examples/hyperparameter-optimization.ipynb` & `irspack-0.3.1/examples/hyperparameter-optimization.ipynb`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/examples/movielens/movielens_1m.py` & `irspack-0.3.1/examples/movielens/movielens_1m.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/examples/movielens/movielens_1m_cold.py` & `irspack-0.3.1/examples/movielens/movielens_1m_cold.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/examples/movielens/movielens_20m_cold.py` & `irspack-0.3.1/examples/movielens/movielens_20m_cold.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/examples/split1.png` & `irspack-0.3.1/examples/split1.png`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/examples/split2.png` & `irspack-0.3.1/examples/split2.png`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/examples/train-first-recommender.ipynb` & `irspack-0.3.1/examples/train-first-recommender.ipynb`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/mypy.ini` & `irspack-0.3.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/pyproject.toml` & `irspack-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/setup.py` & `irspack-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/dataset/amazon_music.py` & `irspack-0.3.1/src/irspack/dataset/amazon_music.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/dataset/citeulike.py` & `irspack-0.3.1/src/irspack/dataset/citeulike.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/dataset/downloader.py` & `irspack-0.3.1/src/irspack/dataset/downloader.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/dataset/movielens/ML100K.py` & `irspack-0.3.1/src/irspack/dataset/movielens/ML100K.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/dataset/movielens/ML1M.py` & `irspack-0.3.1/src/irspack/dataset/movielens/ML1M.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/dataset/movielens/ML20M.py` & `irspack-0.3.1/src/irspack/dataset/movielens/ML20M.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/dataset/movielens/base.py` & `irspack-0.3.1/src/irspack/dataset/movielens/base.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/dataset/neu_mf.py` & `irspack-0.3.1/src/irspack/dataset/neu_mf.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/default_logger.py` & `irspack-0.3.1/src/irspack/default_logger.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/evaluation/_core.pyi` & `irspack-0.3.1/src/irspack/evaluation/_core.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 m: int
 n: int
-from numpy import float32
-
-import irspack.evaluation._core
 import typing
+
 import numpy
 import scipy.sparse
+from numpy import float32
+
+import irspack.evaluation._core
 
 _Shape = typing.Tuple[int, ...]
 
 __all__ = ["EvaluatorCore", "Metrics", "evaluate_list_vs_list"]
 
 class EvaluatorCore:
     def __getstate__(self) -> tuple: ...
@@ -19,23 +20,23 @@
         recommendable: typing.List[typing.List[int]],
     ) -> None: ...
     def __setstate__(self, arg0: tuple) -> None: ...
     def cache_X_as_set(self, arg0: int) -> None: ...
     def get_ground_truth(self) -> scipy.sparse.csr_matrix[numpy.float64]: ...
     def get_metrics_f32(
         self,
-        score_array: numpy.ndarray[numpy.float32, _Shape[m, n]],
+        score_array: numpy.ndarray[typing.Tuple[int, int], numpy.dtype[numpy.float32]],
         cutoff: int,
         offset: int,
         n_threads: int,
         recall_with_cutoff: bool = False,
     ) -> Metrics: ...
     def get_metrics_f64(
         self,
-        score_array: numpy.ndarray[numpy.float64, _Shape[m, n]],
+        score_array: numpy.ndarray[typing.Tuple[int, int], numpy.dtype[numpy.float64]],
         cutoff: int,
         offset: int,
         n_threads: int,
         recall_with_cutoff: bool = False,
     ) -> Metrics: ...
     pass
```

### Comparing `irspack-0.3.0/src/irspack/evaluation/evaluate_df_to_df.py` & `irspack-0.3.1/src/irspack/evaluation/evaluate_df_to_df.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/evaluation/evaluator.py` & `irspack-0.3.1/src/irspack/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/optimization/optimizer.py` & `irspack-0.3.1/src/irspack/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/optimization/parameter_range.py` & `irspack-0.3.1/src/irspack/optimization/parameter_range.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/recommenders/__init__.py` & `irspack-0.3.1/src/irspack/recommenders/__init__.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/recommenders/_ials.pyi` & `irspack-0.3.1/src/irspack/recommenders/_ials.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 m: int
 n: int
-from numpy import float32
 
 """irspack's core module for "IALSRecommender".
 Built to use
 	SSE, SSE2"""
 from __future__ import annotations
-import irspack.recommenders._ials
+
 import typing
+
 import numpy
 import scipy.sparse
 
-_Shape = typing.Tuple[int, ...]
+import irspack.recommenders._ials
 
 __all__ = [
     "CG",
     "CHOLESKY",
     "IALSModelConfig",
     "IALSModelConfigBuilder",
     "IALSPP",
@@ -78,36 +78,40 @@
         self, arg0: IALSModelConfig, arg1: scipy.sparse.csr_matrix[numpy.float32]
     ) -> None: ...
     def __setstate__(self, arg0: tuple) -> None: ...
     def compute_loss(self, arg0: IALSSolverConfig) -> float: ...
     def step(self, arg0: IALSSolverConfig) -> None: ...
     def transform_item(
         self, arg0: scipy.sparse.csr_matrix[numpy.float32], arg1: IALSSolverConfig
-    ) -> numpy.ndarray[numpy.float32, _Shape[m, n]]: ...
+    ) -> numpy.ndarray[typing.Tuple[int, int], numpy.dtype[numpy.float32]]: ...
     def transform_user(
         self, arg0: scipy.sparse.csr_matrix[numpy.float32], arg1: IALSSolverConfig
-    ) -> numpy.ndarray[numpy.float32, _Shape[m, n]]: ...
+    ) -> numpy.ndarray[typing.Tuple[int, int], numpy.dtype[numpy.float32]]: ...
     def user_scores(
         self, arg0: int, arg1: int, arg2: IALSSolverConfig
-    ) -> numpy.ndarray[numpy.float32, _Shape[m, n]]: ...
+    ) -> numpy.ndarray[typing.Tuple[int, int], numpy.dtype[numpy.float32]]: ...
     @property
-    def item(self) -> numpy.ndarray[numpy.float32, _Shape[m, n]]:
+    def item(self) -> numpy.ndarray[typing.Tuple[int, int], numpy.dtype[numpy.float32]]:
         """
-        :type: numpy.ndarray[numpy.float32, _Shape[m, n]]
+        :type: numpy.ndarray[typing.Tuple[int, int], numpy.dtype[numpy.float32]]
         """
     @item.setter
-    def item(self, arg0: numpy.ndarray[numpy.float32, _Shape[m, n]]) -> None:
+    def item(
+        self, arg0: numpy.ndarray[typing.Tuple[int, int], numpy.dtype[numpy.float32]]
+    ) -> None:
         pass
     @property
-    def user(self) -> numpy.ndarray[numpy.float32, _Shape[m, n]]:
+    def user(self) -> numpy.ndarray[typing.Tuple[int, int], numpy.dtype[numpy.float32]]:
         """
-        :type: numpy.ndarray[numpy.float32, _Shape[m, n]]
+        :type: numpy.ndarray[typing.Tuple[int, int], numpy.dtype[numpy.float32]]
         """
     @user.setter
-    def user(self, arg0: numpy.ndarray[numpy.float32, _Shape[m, n]]) -> None:
+    def user(
+        self, arg0: numpy.ndarray[typing.Tuple[int, int], numpy.dtype[numpy.float32]]
+    ) -> None:
         pass
     pass
 
 class LossType:
     """
     Members:
```

### Comparing `irspack-0.3.0/src/irspack/recommenders/_knn.pyi` & `irspack-0.3.1/src/irspack/recommenders/_knn.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 m: int
 n: int
-from numpy import float32
-
-import irspack.recommenders._knn
 import typing
+
 import numpy
 import scipy.sparse
+from numpy import float32
+
+import irspack.recommenders._knn
 
 _Shape = typing.Tuple[int, ...]
 
 __all__ = [
     "AsymmetricSimilarityComputer",
     "CosineSimilarityComputer",
     "JaccardSimilarityComputer",
```

### Comparing `irspack-0.3.0/src/irspack/recommenders/base.py` & `irspack-0.3.1/src/irspack/recommenders/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,18 +35,21 @@
 )
 from ..optimization.parameter_range import ParameterRange
 
 R = TypeVar("R", bound="BaseRecommender")
 
 
 def _sparse_to_array(U: Any) -> np.ndarray:
+    res: np.ndarray
     if sps.issparse(U):
-        return U.toarray()
+        res = U.toarray()
+        return res
     else:
-        return U
+        res = U
+        return res
 
 
 class CallBeforeFitError(Exception):
     pass
 
 
 class RecommenderConfig(BaseModel):
```

### Comparing `irspack-0.3.0/src/irspack/recommenders/base_earlystop.py` & `irspack-0.3.1/src/irspack/recommenders/base_earlystop.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/recommenders/bpr.py` & `irspack-0.3.1/src/irspack/recommenders/bpr.py`

 * *Files 5% similar despite different names*

```diff
@@ -140,37 +140,45 @@
     @property
     def fm(self) -> LightFM:
         if self.trainer is None:
             raise RuntimeError("tried to fetch fm instance before the fit.")
         return self.trainer.fm
 
     def get_score(self, index: UserIndexArray) -> np.ndarray:
-        return (
+        res: np.ndarray = (
             self.fm.user_embeddings[index].dot(self.fm.item_embeddings.T)
             + self.fm.item_biases[np.newaxis, :]
         )
+        return res
 
     def get_score_block(self, begin: int, end: int) -> np.ndarray:
-        return (
+        res: np.ndarray = (
             self.fm.user_embeddings[begin:end].dot(self.fm.item_embeddings.T)
             + self.fm.item_biases[np.newaxis, :]
         )
+        return res
 
     def get_user_embedding(self) -> DenseMatrix:
-        return self.fm.user_embeddings
+        res: DenseMatrix = self.fm.user_embeddings
+        return res
 
     def get_score_from_user_embedding(
         self, user_embedding: DenseMatrix
     ) -> DenseScoreArray:
-        return (
+        res: DenseScoreArray = (
             user_embedding.dot(self.fm.item_embeddings.T)
             + self.fm.item_biases[np.newaxis, :]
         )
+        return res
 
     def get_item_embedding(self) -> DenseMatrix:
-        return self.fm.item_embeddings
+        res: DenseMatrix = self.fm.item_embeddings
+        return res
 
     def get_score_from_item_embedding(
         self, user_indices: UserIndexArray, item_embedding: DenseMatrix
     ) -> DenseScoreArray:
         # ignore bias
-        return self.fm.user_embeddings[user_indices].dot(item_embedding.T)
+        res: DenseScoreArray = self.fm.user_embeddings[user_indices].dot(
+            item_embedding.T
+        )
+        return res
```

### Comparing `irspack-0.3.0/src/irspack/recommenders/dense_slim.py` & `irspack-0.3.1/src/irspack/recommenders/dense_slim.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/recommenders/edlae.py` & `irspack-0.3.1/src/irspack/recommenders/edlae.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/recommenders/ials.py` & `irspack-0.3.1/src/irspack/recommenders/ials.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,32 +375,34 @@
     @property
     def trainer_as_ials(self) -> IALSTrainer:
         if self.trainer is None:
             raise RuntimeError("tried to fetch trainer before the training.")
         return self.trainer
 
     def get_score(self, user_indices: UserIndexArray) -> DenseScoreArray:
-        return self.trainer_as_ials.core_trainer.user[user_indices].dot(
+        res: DenseScoreArray = self.trainer_as_ials.core_trainer.user[user_indices].dot(
             self.get_item_embedding().T
         )
+        return res
 
     def get_score_block(self, begin: int, end: int) -> DenseScoreArray:
         return self.trainer_as_ials.user_scores(begin, end)
 
     def get_score_cold_user(self, X: InteractionMatrix) -> DenseScoreArray:
         user_vector = self.compute_user_embedding(X)
         return self.get_score_from_user_embedding(user_vector)
 
     def get_user_embedding(self) -> DenseMatrix:
         return self.trainer_as_ials.core_trainer.user
 
     def get_score_from_user_embedding(
         self, user_embedding: DenseMatrix
     ) -> DenseScoreArray:
-        return user_embedding.dot(self.get_item_embedding().T)
+        res: DenseScoreArray = user_embedding.dot(self.get_item_embedding().T)
+        return res
 
     def get_item_embedding(self) -> DenseMatrix:
         return self.trainer_as_ials.core_trainer.item
 
     def compute_user_embedding(self, X: InteractionMatrix) -> DenseMatrix:
         r"""Given an unknown users' interaction with known items,
         computes the latent factors of the users by least square (fixing item embeddings).
@@ -435,17 +437,18 @@
                 self.epsilon,
             )
         )
 
     def get_score_from_item_embedding(
         self, user_indices: UserIndexArray, item_embedding: DenseMatrix
     ) -> DenseScoreArray:
-        return self.trainer_as_ials.core_trainer.user[user_indices].dot(
+        res: DenseScoreArray = self.trainer_as_ials.core_trainer.user[user_indices].dot(
             item_embedding.T
         )
+        return res
 
     @classmethod
     def tune_doubling_dimension(
         cls,
         data: InteractionMatrix,
         evaluator: Evaluator,
         initial_dimension: int,
```

### Comparing `irspack-0.3.0/src/irspack/recommenders/knn.py` & `irspack-0.3.1/src/irspack/recommenders/knn.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/recommenders/multvae.py` & `irspack-0.3.1/src/irspack/recommenders/multvae.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
             X_mb = X_csr[mb_start:mb_end].astype(np.float32).toarray()
             X_jax = jnp.asarray(X_mb)
             mvresult: MultVAEOutput = self.vae_f.apply(
                 self.params, next(self.rng_seq), X_jax, self.dropout_p, False
             )
 
             mb_arrays.append(np.asarray(mvresult.log_softmax, dtype=np.float64))
-        score_concat = np.concatenate(mb_arrays, axis=0)
+        score_concat: DenseScoreArray = np.concatenate(mb_arrays, axis=0)
         return score_concat
 
     def run_epoch(self) -> None:
         user_indices = np.arange(self.n_users)
         np.random.shuffle(user_indices)
         for mb_start in range(0, self.n_users, self.minibatch_size):
             current_kl_coeff = jnp.asarray(
```

### Comparing `irspack-0.3.0/src/irspack/recommenders/p3.py` & `irspack-0.3.1/src/irspack/recommenders/p3.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/recommenders/rp3.py` & `irspack-0.3.1/src/irspack/recommenders/rp3.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/recommenders/slim.py` & `irspack-0.3.1/src/irspack/recommenders/slim.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/recommenders/toppop.py` & `irspack-0.3.1/src/irspack/recommenders/toppop.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,22 +27,24 @@
 
     def __init__(self, X_train: InteractionMatrix):
 
         super().__init__(X_train)
         self.score_ = None
 
     def _learn(self) -> None:
-        self.score_ = self.X_train_all.sum(axis=0).astype(np.float64)
+        self.score_ = self.X_train_all.sum(axis=0).astype(np.float64).A
 
     @property
     def score(self) -> np.ndarray:
         if self.score_ is None:
             raise RuntimeError("The method called before ``learn``.")
         return self.score_
 
     def get_score(self, user_indices: UserIndexArray) -> DenseScoreArray:
         n_users: int = user_indices.shape[0]
-        return np.repeat(self.score, n_users, axis=0).A
+        res: DenseScoreArray = np.repeat(self.score, n_users, axis=0)
+        return res
 
     def get_score_cold_user(self, X: InteractionMatrix) -> DenseScoreArray:
         n_users: int = X.shape[0]
-        return np.repeat(self.score, n_users, axis=0).A
+        res: DenseScoreArray = np.repeat(self.score, n_users, axis=0)
+        return res
```

### Comparing `irspack-0.3.0/src/irspack/recommenders/truncsvd.py` & `irspack-0.3.1/src/irspack/recommenders/truncsvd.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,30 +79,38 @@
     def _learn(self) -> None:
         self.decomposer_ = TruncatedSVD(
             n_components=self.n_components, random_state=self.random_seed
         )
         self.z_ = self.decomposer_.fit_transform(self.X_train_all)
 
     def get_score(self, user_indices: UserIndexArray) -> DenseScoreArray:
-        return self.z[user_indices].dot(self.decomposer.components_)
+        res: DenseScoreArray = self.z[user_indices].dot(self.decomposer.components_)
+        return res
 
     def get_score_block(self, begin: int, end: int) -> DenseScoreArray:
-        return self.z[begin:end].dot(self.decomposer.components_)
+        res: DenseScoreArray = self.z[begin:end].dot(self.decomposer.components_)
+        return res
 
     def get_score_cold_user(self, X: InteractionMatrix) -> DenseScoreArray:
-        return self.decomposer.transform(X).dot(self.decomposer.components_)
+        res: DenseScoreArray = self.decomposer.transform(X).dot(
+            self.decomposer.components_
+        )
+        return res
 
     def get_user_embedding(self) -> DenseMatrix:
         return self.z
 
     def get_score_from_user_embedding(
         self, user_embedding: DenseMatrix
     ) -> DenseScoreArray:
-        return user_embedding.dot(self.decomposer.components_)
+        res: DenseScoreArray = user_embedding.dot(self.decomposer.components_)
+        return res
 
     def get_item_embedding(self) -> DenseMatrix:
-        return self.decomposer.components_.T
+        res: DenseMatrix = self.decomposer.components_.T
+        return res
 
     def get_score_from_item_embedding(
         self, user_indices: UserIndexArray, item_embedding: DenseMatrix
     ) -> DenseScoreArray:
-        return self.z[user_indices].dot(item_embedding.T)
+        res: DenseScoreArray = self.z[user_indices].dot(item_embedding.T)
+        return res
```

### Comparing `irspack-0.3.0/src/irspack/recommenders/user_knn.py` & `irspack-0.3.1/src/irspack/recommenders/user_knn.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/split/specified.py` & `irspack-0.3.1/src/irspack/split/specified.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import uuid
 from typing import Any, Dict, List, Tuple
 
 import numpy as np
+import numpy.typing as npt
 import pandas as pd
 from scipy import sparse as sps
 
 from ..definitions import OptionalRandomState
 from ..utils.random import convert_randomstate
 from .userwise import UserTrainTestInteractionPair, _split_list
 
@@ -73,14 +74,18 @@
     df[item_index_colname] = item_index
 
     flg_colname = str(uuid.uuid1())
     flg_column = np.zeros(df.shape[0])
     flg_column[interaction_indicator] = 1
     df[flg_colname] = flg_column
 
+    v_train_users: npt.ArrayLike
+    v_val_users: npt.ArrayLike
+    v_test_users: npt.ArrayLike
+
     validatable_users = np.unique(df[flg_column > 0][user_column])
     n_validatable_users: int = validatable_users.shape[0]
     val_test_ratio = 1 - v_user_ratio_train
 
     rns = convert_randomstate(random_state)
     if val_test_ratio >= 1.0:
         v_train_users = np.ndarray((0,), dtype=validatable_users.dtype)
```

### Comparing `irspack-0.3.0/src/irspack/split/time.py` & `irspack-0.3.1/src/irspack/split/time.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/split/userwise.py` & `irspack-0.3.1/src/irspack/split/userwise.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/utils/__init__.py` & `irspack-0.3.1/src/irspack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/utils/_util_cpp.pyi` & `irspack-0.3.1/src/irspack/utils/_util_cpp.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 m: int
 n: int
-from numpy import float32
-
-import irspack.utils._util_cpp
 import typing
+
 import numpy
 import scipy.sparse
+from numpy import float32
+
+import irspack.utils._util_cpp
 
 _Shape = typing.Tuple[int, ...]
 
 __all__ = [
     "okapi_BM_25_weight",
     "remove_diagonal",
     "retrieve_recommend_from_score_f32",
@@ -29,23 +30,23 @@
 
 def remove_diagonal(
     arg0: scipy.sparse.csr_matrix[numpy.float64],
 ) -> scipy.sparse.csr_matrix[numpy.float64]:
     pass
 
 def retrieve_recommend_from_score_f32(
-    score: numpy.ndarray[numpy.float32, _Shape[m, n]],
+    score: numpy.ndarray[typing.Tuple[int, int], numpy.dtype[numpy.float32]],
     allowed_indices: typing.List[typing.List[int]],
     cutoff: int,
     n_threads: int = 1,
 ) -> typing.List[typing.List[typing.Tuple[int, float]]]:
     pass
 
 def retrieve_recommend_from_score_f64(
-    score: numpy.ndarray[numpy.float64, _Shape[m, n]],
+    score: numpy.ndarray[typing.Tuple[int, int], numpy.dtype[numpy.float64]],
     allowed_indices: typing.List[typing.List[int]],
     cutoff: int,
     n_threads: int = 1,
 ) -> typing.List[typing.List[typing.Tuple[int, float]]]:
     pass
 
 def rowwise_train_test_split_by_fixed_n(
@@ -84,14 +85,14 @@
 ) -> scipy.sparse.csc_matrix[numpy.float32]:
     pass
 
 def sparse_mm_threaded(
     arg0: scipy.sparse.csr_matrix[numpy.float64],
     arg1: scipy.sparse.csc_matrix[numpy.float64],
     arg2: int,
-) -> numpy.ndarray[numpy.float64, _Shape[m, n]]:
+) -> numpy.ndarray[typing.Tuple[int, int], numpy.dtype[numpy.float64]]:
     pass
 
 def tf_idf_weight(
     X: scipy.sparse.csr_matrix[numpy.float64], smooth: bool = True
 ) -> scipy.sparse.csr_matrix[numpy.float64]:
     pass
```

### Comparing `irspack-0.3.0/src/irspack/utils/id_mapping.py` & `irspack-0.3.1/src/irspack/utils/id_mapping.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack/utils/sample_data.py` & `irspack-0.3.1/src/irspack/utils/sample_data.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/src/irspack.egg-info/SOURCES.txt` & `irspack-0.3.1/src/irspack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/tests/dataset/test_ml1m.py` & `irspack-0.3.1/tests/dataset/test_ml1m.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/tests/dataset/test_neumf.py` & `irspack-0.3.1/tests/dataset/test_neumf.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/tests/evaluation/test_df_vs_df.py` & `irspack-0.3.1/tests/evaluation/test_df_vs_df.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/tests/evaluation/test_evaluator.py` & `irspack-0.3.1/tests/evaluation/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/tests/evaluation/test_restricted_evaluator.py` & `irspack-0.3.1/tests/evaluation/test_restricted_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,28 +11,29 @@
 
 class MockRecommender(BaseRecommender, register_class=False):
     def __init__(self, X_all: sps.csr_matrix, scores: np.ndarray) -> None:
         super().__init__(X_all)
         self.scores = scores
 
     def get_score(self, user_indices: np.ndarray) -> np.ndarray:
-        return self.scores[user_indices]
+        scores: np.ndarray = self.scores[user_indices]
+        return scores
 
     def _learn(self) -> None:
         pass
 
 
 @pytest.mark.parametrize("U, I, R", [(10, 30, 10), (100, 30, 5), (30, 100, 2)])
 def test_restriction_global(U: int, I: int, R: int) -> None:
     try:
         from sklearn.metrics import ndcg_score
     except:
         pytest.skip()
     rns = np.random.RandomState(42)
-    recommendable = rns.choice(np.arange(I), replace=False, size=R)
+    recommendable = rns.choice(np.arange(I), replace=False, size=R).tolist()
     scores = rns.randn(U, I)
     X_gt = (rns.rand(U, I) >= 0.3).astype(np.float64)
     evaluator_ = Evaluator(
         sps.csr_matrix(X_gt),
         offset=0,
         cutoff=I,
         n_threads=1,
```

### Comparing `irspack-0.3.0/tests/optimization/test_earlystop_optimizer.py` & `irspack-0.3.1/tests/optimization/test_earlystop_optimizer.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/tests/optimization/test_ials_doubling_dimension.py` & `irspack-0.3.1/tests/optimization/test_ials_doubling_dimension.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/tests/optimization/test_optimizer.py` & `irspack-0.3.1/tests/optimization/test_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         self.flag = flag
         self.rns = np.random.RandomState(0)
 
     def _learn(self) -> None:
         pass
 
     def get_score(self, user_indices: UserIndexArray) -> DenseScoreArray:
+        score: DenseScoreArray
         score = self.answer[user_indices] * self.p1
         score = score + 10 * self.rns.rand(*score.shape) * (1 - self.p1)
         return score
 
 
 @pytest.mark.parametrize("X", [X_small, X_large])
 def test_optimizer_by_mock(X: sps.csr_matrix) -> None:
```

### Comparing `irspack-0.3.0/tests/recommenders/test_ials.py` & `irspack-0.3.1/tests/recommenders/test_ials.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/tests/recommenders/test_knn.py` & `irspack-0.3.1/tests/recommenders/test_knn.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,32 +12,33 @@
 )
 from irspack.recommenders.p3 import P3alphaRecommender
 from irspack.recommenders.rp3 import RP3betaRecommender
 
 X_small = sps.csr_matrix(
     np.asfarray([[1, 1, 2, 3, 4], [0, 1, 0, 1, 0], [0, 0, 1, 0, 0], [0, 0, 0, 0, 0]])
 )
-X_many = np.random.rand(888, 512)
-X_many[X_many <= 0.9] = 0
-X_many[X_many > 0.9] = 1
-X_many = sps.csr_matrix(X_many)
+X_many_dense = np.random.rand(888, 512)
+X_many_dense[X_many_dense <= 0.9] = 0
+X_many_dense[X_many_dense > 0.9] = 1
+X_many = sps.csr_matrix(X_many_dense)
 X_many.sort_indices()
 
 X_many_dense = sps.csr_matrix(np.random.rand(133, 245))
 
 
 @pytest.mark.parametrize(
     "X, normalize", [(X_many, True), (X_small, False), (X_many_dense, True)]
 )
 def test_cosine(X: sps.csr_matrix, normalize: bool) -> None:
     rec = CosineKNNRecommender(
         X, shrinkage=0, n_threads=5, top_k=X.shape[1], normalize=normalize
     )
     rec.learn()
-    sim = rec.W.toarray()
+    W: sps.csr_matrix = rec.W
+    sim = W.toarray()
     manual = X.T.toarray()  # I x U
     norm = (manual**2).sum(axis=1) ** 0.5
     manual = manual.dot(manual.T)
     if normalize:
         denom = norm[:, None] * norm[None, :] + 1e-6
         manual /= denom
     np.fill_diagonal(manual, 0)
@@ -47,15 +48,16 @@
     )
 
 
 @pytest.mark.parametrize("X", [X_many, X_small, X_many_dense])
 def test_jaccard(X: sps.csr_matrix) -> None:
     rec = JaccardKNNRecommender(X, shrinkage=0, top_k=X.shape[1], n_threads=1)
     rec.learn()
-    sim = rec.W.toarray()
+    W: sps.csr_matrix = rec.W
+    sim = W.toarray()
     X_bin = X.copy()
     X_bin.sort_indices()
     X_bin.data[:] = 1
     manual = X_bin.T.toarray()  # I x U
     norm = manual.sum(axis=1)
     manual = manual.dot(manual.T)
     denom = norm[:, None] + norm[None, :] - manual + 1e-6
@@ -70,15 +72,16 @@
     [(X_many, 0.5, 0.0), (X_small, 0.7, 1.0), (X_many_dense, 0.01, 3)],
 )
 def test_asymmetric_cosine(X: sps.csr_matrix, alpha: float, shrinkage: float) -> None:
     rec = AsymmetricCosineKNNRecommender(
         X, shrinkage=shrinkage, alpha=alpha, n_threads=1, top_k=X.shape[1]
     )
     rec.learn()
-    sim = rec.W.toarray()
+    W: sps.csr_matrix = rec.W
+    sim = W.toarray()
 
     manual = X.T.toarray()  # I x U
     norm = (manual**2).sum(axis=1)
     norm_alpha = np.power(norm, alpha)
     norm_1malpha = np.power(norm, 1 - alpha)
     manual_sim = manual.dot(manual.T)
     denom = norm_alpha[:, None] * norm_1malpha[None, :] + 1e-6 + shrinkage
@@ -98,15 +101,16 @@
     X: sps.csr_matrix, alpha: float, beta: float, shrinkage: float
 ) -> None:
     RNS = np.random.RandomState(0)
     rec = TverskyIndexKNNRecommender(
         X, shrinkage=shrinkage, alpha=alpha, beta=beta, n_threads=1, top_k=X.shape[1]
     )
     rec.learn()
-    sim = rec.W.toarray()
+    W: sps.csr_matrix = rec.W
+    sim = W.toarray()
     tested_index_row = RNS.randint(0, sim.shape[0], size=100)
     tested_index_col = RNS.randint(0, sim.shape[0], size=100)
     X_csc = X.tocsc()
     X_csc.sorted_indices()
     for i, j in zip(tested_index_row, tested_index_col):
         if i == j:
             continue
@@ -126,23 +130,25 @@
         assert computed == pytest.approx(target)
 
 
 @pytest.mark.parametrize("X", [X_many, X_small])
 def test_topk(X: sps.csr_matrix) -> None:
     rec = CosineKNNRecommender(X, shrinkage=0, top_k=30, n_threads=5)
     rec.learn()
-    sim = rec.W.toarray()
+    W: sps.csr_matrix = rec.W
+    sim = W.toarray()
     assert np.all((sim > 0).sum(axis=1) <= 30)
 
 
 @pytest.mark.parametrize("X, alpha", [(X_small, 0.001), (X_many_dense, 2), (X_many, 1)])
 def test_p3(X: sps.csr_matrix, alpha: float) -> None:
     rec = P3alphaRecommender(X, alpha=alpha, n_threads=4)
     rec.learn()
-    W = rec.W.toarray()
+    W_csr: sps.csr_matrix = rec.W
+    W = W_csr.toarray()
 
     P_ui = np.power(X.toarray(), alpha)
     P_iu = np.power(X.T.toarray(), alpha)
 
     def zero_or_1(X: np.ndarray) -> np.ndarray:
         X = X.copy()
         X[X == 0] = 1
@@ -165,15 +171,16 @@
 
 @pytest.mark.parametrize(
     "X, alpha, beta", [(X_small, 0.001, 3), (X_many_dense, 2, 5), (X_many, 1, 0.2)]
 )
 def test_rp3(X: sps.csr_matrix, alpha: float, beta: float) -> None:
     rec = RP3betaRecommender(X, alpha=alpha, beta=beta, n_threads=4)
     rec.learn()
-    W = rec.W.toarray()
+    W_csr: sps.csr_matrix = rec.W
+    W = W_csr.toarray()
     W_sum = W.sum(axis=1)
     W_sum = W_sum[W_sum >= 0]
 
     popularity = X.sum(axis=0).A1.ravel() ** beta
 
     def zero_or_1(X: np.ndarray) -> np.ndarray:
         X = X.copy()
```

### Comparing `irspack-0.3.0/tests/recommenders/test_learn_all.py` & `irspack-0.3.1/tests/recommenders/test_learn_all.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/tests/recommenders/test_slim.py` & `irspack-0.3.1/tests/recommenders/test_slim.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,15 +31,16 @@
         l1_ratio=l1_ratio,
         fit_intercept=False,
         positive=True,
         max_iter=100,
         tol=1e-8,
     )
     for iind in range(rec.W.shape[1]):
-        m = rec.W[:, iind].toarray().ravel()
+        W: sps.csr_matrix = rec.W
+        m = W[:, iind].toarray().ravel()
         Xcp = X.toarray()
         y = X[:, iind].toarray().ravel()
         Xcp[:, iind] = 0.0
         enet.fit(Xcp, y)
         np.testing.assert_allclose(enet.coef_, m, rtol=1e-2)
 
 
@@ -64,15 +65,16 @@
     )
     rec.learn()
 
     enet = ElasticNet(
         alpha=alpha, l1_ratio=l1_ratio, fit_intercept=False, max_iter=ITER, tol=1e-8
     )
     for iind in range(rec.W.shape[1]):
-        m = rec.W[:, iind].toarray().ravel()
+        W: sps.csr_matrix = rec.W
+        m = W[:, iind].toarray().ravel()
         Xcp = X.toarray()
         y = X[:, iind].toarray().ravel()
         Xcp[:, iind] = 0.0
         enet.fit(Xcp, y)
         np.testing.assert_allclose(enet.coef_, m, rtol=1e-2)
 
 
@@ -86,26 +88,28 @@
         l1_ratio=l1_ratio,
         positive_only=True,
         n_iter=100,
         n_threads=1,
         tol=0,
     )
     rec.learn()
-    W_non_restricted = rec.W.toarray()
+    W_non_restricted_csr: sps.csr_matrix = rec.W
+    W_non_restricted = W_non_restricted_csr.toarray()
 
     rec_restricted = SLIMRecommender(
         X,
         alpha=alpha,
         l1_ratio=l1_ratio,
         positive_only=True,
         n_iter=100,
         n_threads=1,
         tol=0,
         top_k=1,
     )
     rec_restricted.learn()
-    W_restricted = rec_restricted.W.toarray()
+    W_restricted_csr: sps.csr_matrix = rec_restricted.W
+    W_restricted = W_restricted_csr.toarray()
     for i in range(rec.n_items):
         gt = W_non_restricted[:, i]
         target = W_restricted[:, i]
         assert np.sum(target > 0) <= 1
         assert target.max() == pytest.approx(gt.max())
```

### Comparing `irspack-0.3.0/tests/recommenders/test_topop.py` & `irspack-0.3.1/tests/recommenders/test_topop.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/tests/recommenders/test_user_knn.py` & `irspack-0.3.1/tests/recommenders/test_user_knn.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     AsymmetricCosineUserKNNRecommender,
     CosineUserKNNRecommender,
 )
 
 X_small = sps.csr_matrix(
     np.asfarray([[1, 1, 2, 3, 4], [0, 1, 0, 1, 0], [0, 0, 1, 0, 0], [0, 0, 0, 0, 0]])
 )
-X_many = np.random.rand(888, 512)
-X_many[X_many <= 0.9] = 0
-X_many[X_many > 0.9] = 1
-X_many = sps.csr_matrix(X_many)
+X_many_dense = np.random.rand(888, 512)
+X_many_dense[X_many_dense <= 0.9] = 0
+X_many_dense[X_many_dense > 0.9] = 1
+X_many = sps.csr_matrix(X_many_dense)
 X_many.sort_indices()
 
 X_many_dense = sps.csr_matrix(np.random.rand(133, 245))
 
 
 @pytest.mark.parametrize(
     "X, normalize", [(X_many, True), (X_small, False), (X_many_dense, True)]
@@ -25,15 +25,16 @@
 def test_cosine(X: sps.csr_matrix, normalize: bool) -> None:
     rec = CosineUserKNNRecommender(
         X, shrinkage=0, n_threads=5, top_k=X.shape[0], normalize=normalize
     )
     with pytest.raises(RuntimeError):
         rec.U
     rec.learn()
-    sim = rec.U.toarray()
+    U: sps.csr_matrix = rec.U
+    sim = U.toarray()
     manual = X.toarray()  # U x I
     norm = (manual**2).sum(axis=1) ** 0.5
     manual = manual.dot(manual.T)
     if normalize:
         denom = norm[:, None] * norm[None, :] + 1e-6
         manual /= denom
     np.fill_diagonal(manual, 0)
@@ -48,15 +49,16 @@
     [(X_many, 0.5, 0.0), (X_small, 0.7, 1.0), (X_many_dense, 0.01, 3)],
 )
 def test_asymmetric_cosine(X: sps.csr_matrix, alpha: float, shrinkage: float) -> None:
     rec = AsymmetricCosineUserKNNRecommender(
         X, shrinkage=shrinkage, alpha=alpha, n_threads=1, top_k=X.shape[0]
     )
     rec.learn()
-    sim = rec.U.toarray()
+    U: sps.csr_matrix = rec.U
+    sim = U.toarray()
 
     manual = X.toarray()
     norm = (manual**2).sum(axis=1)
     norm_alpha = np.power(norm, alpha)
     norm_1malpha = np.power(norm, 1 - alpha)
     manual_sim = manual.dot(manual.T)
     denom = norm_alpha[:, None] * norm_1malpha[None, :] + 1e-6 + shrinkage
@@ -68,9 +70,10 @@
     )
 
 
 @pytest.mark.parametrize("X", [X_many, X_small])
 def test_topk(X: sps.csr_matrix) -> None:
     rec = AsymmetricCosineUserKNNRecommender(X, shrinkage=0, top_k=30, n_threads=5)
     rec.learn()
-    sim = rec.U.toarray()
+    U: sps.csr_matrix = rec.U
+    sim = U.toarray()
     assert np.all((sim > 0).sum(axis=1) <= 30)
```

### Comparing `irspack-0.3.0/tests/split/test_specific_holdout.py` & `irspack-0.3.1/tests/split/test_specific_holdout.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     test_validatable_user_ratio = 0.3
     train_validatable_user_ratio = (
         1 - val_validatable_user_ratio - test_validatable_user_ratio
     )
     validatable_item_ids = np.random.choice(
         item_ids, size=len(item_ids) // 5, replace=False
     )
-    indicator = np.where(df.item_id.isin(validatable_item_ids).values)
+    indicator: np.ndarray = df.item_id.isin(validatable_item_ids).values.nonzero()
     item_id_reprod, dataset = holdout_specific_interactions(
         df,
         "user_id",
         "item_id",
         interaction_indicator=indicator,
         validatable_user_ratio_val=val_validatable_user_ratio,
         validatable_user_ratio_test=test_validatable_user_ratio,
@@ -167,22 +167,22 @@
         rows, cols = X.nonzero()
         return pd.DataFrame(
             dict(user_id=[uids[row] for row in rows], item_id=unique_item_ids[cols])
         )
 
     for userset in [val_users, test_users]:
         # check all of the train_interactions are in the future
-        train_interactions = X_to_df(userset.X_train, userset.user_ids)
+        train_interactions = X_to_df(userset.X_train, np.asarray(userset.user_ids))
         train_interactions_with_ts = train_interactions.merge(
             df_master, on=["user_id", "item_id"], how="inner"
         )
         assert train_interactions.shape[0] == train_interactions_with_ts.shape[0]
         assert np.all(train_interactions_with_ts.timestamp.values < 0)
 
         # check all of the test_interactions are in the future
-        test_interactions = X_to_df(userset.X_test, userset.user_ids)
+        test_interactions = X_to_df(userset.X_test, np.asarray(userset.user_ids))
         test_interactions_with_ts = test_interactions.merge(
             df_master, on=["user_id", "item_id"], how="inner"
         )
 
         assert test_interactions.shape[0] == test_interactions_with_ts.shape[0]
         assert np.all(test_interactions_with_ts.timestamp.values >= 0)
```

### Comparing `irspack-0.3.0/tests/split/test_time_holdout.py` & `irspack-0.3.1/tests/split/test_time_holdout.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/tests/split/test_userwise_split.py` & `irspack-0.3.1/tests/split/test_userwise_split.py`

 * *Files identical despite different names*

### Comparing `irspack-0.3.0/tests/utils/test_id_mapper.py` & `irspack-0.3.1/tests/utils/test_id_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 
 class MockRecommender(BaseRecommender):
     def __init__(self, X_all: sps.csr_matrix, scores: np.ndarray) -> None:
         super().__init__(X_all)
         self.scores = scores
 
     def get_score(self, user_indices: np.ndarray) -> np.ndarray:
-        return self.scores[user_indices]
+        score: np.ndarray = self.scores[user_indices]
+        return score
 
     def _learn(self) -> None:
         pass
 
     def get_score_cold_user(self, X: InteractionMatrix) -> DenseScoreArray:
-        score = np.exp(X.toarray())
+        score: np.ndarray = np.exp(X.toarray())
         score /= score.sum(axis=1)[:, None]
         return score
 
 
 def check_descending(id_score: List[Tuple[Any, float]]) -> None:
     for i, (_, score) in enumerate(id_score):
         if i > 0:
@@ -92,15 +93,15 @@
             )
         )
 
         recommended_with_restriction = id_mapper.recommend_for_known_user_id(
             rec, uid, cutoff=n_items, forbidden_item_ids=forbbiden_item
         )
         check_descending(recommended_with_restriction)
-        for iid, score in recommended_with_restriction:
+        for iid, _ in recommended_with_restriction:
             assert iid not in forbbiden_item
 
         random_allowed_items = list(
             RNS.choice(
                 list(item_id_set.difference(nonzero_items)),
                 size=min(n_items - len(nonzero_items), n_items // 3),
             )
@@ -203,21 +204,20 @@
         nonzero_batch_dict.append(profile)
     batch_result_dict = id_mapper.recommend_for_new_user_batch(
         rec, nonzero_batch_dict, cutoff=n_items, n_threads=1
     )
     for i, result in enumerate(batch_result_dict):
         nnz = len(X[i].nonzero()[1])
         softmax_denom = X.shape[1] - nnz + np.exp(2) * nnz
-        for _, score in result:
-            assert score == pytest.approx(1 / softmax_denom)
+        for _, val in result:
+            assert val == pytest.approx(1 / softmax_denom)
 
 
 def test_item_id_mapper_per_user_allowed_item() -> None:
-    ids = [(i, f"{i}") for i in range(1, 11)]
-    np.random.shuffle(ids)
+    ids = [(i, f"{i}") for i in np.random.choice(10, size=10, replace=False) + 1]
     id_mapepr = ItemIDMapper(ids)
     N_users = 10
     score = np.random.random((N_users, len(ids)))
     per_user_allowed_item_ids = [
         list(set([random.choice(ids) for _ in range(random.randint(2, 5))]))
         for __ in range(N_users)
     ]
@@ -235,16 +235,15 @@
             assert score[i, item_index] == pytest.approx(score_value)
             if previous_score is not None:
                 assert score_value <= previous_score
             previous_score = score_value
 
 
 def test_item_id_mapper_uniform_allowed_item() -> None:
-    ids = [(i, f"{i}") for i in range(1, 11)]
-    np.random.shuffle(ids)
+    ids = [(i, f"{i}") for i in np.random.choice(10, size=10, replace=False) + 1]
     id_mapepr = ItemIDMapper(ids)
     N_users = 10
     score = np.random.random((N_users, len(ids)))
 
     allowed_items_uniform = list(set([random.choice(ids) for _ in range(5)]))
     assert allowed_items_uniform
     recommendation = id_mapepr.score_to_recommended_items_batch(
```

### Comparing `irspack-0.3.0/tests/utils/test_utils.py` & `irspack-0.3.1/tests/utils/test_utils.py`

 * *Files identical despite different names*

