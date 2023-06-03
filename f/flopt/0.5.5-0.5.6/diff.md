# Comparing `tmp/flopt-0.5.5.tar.gz` & `tmp/flopt-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flopt-0.5.5.tar", last modified: Sat Oct 15 04:37:15 2022, max compression
+gzip compressed data, was "flopt-0.5.6.tar", last modified: Sat Jun  3 02:01:55 2023, max compression
```

## Comparing `flopt-0.5.5.tar` & `flopt-0.5.6.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2022-10-15 04:37:15.443529 flopt-0.5.5/
--rw-r--r--   0 tateiwa    (501) staff       (20)     1067 2022-09-19 02:14:43.000000 flopt-0.5.5/LICENSE
--rw-r--r--   0 tateiwa    (501) staff       (20)     4721 2022-10-15 04:37:15.443134 flopt-0.5.5/PKG-INFO
--rw-r--r--   0 tateiwa    (501) staff       (20)     4124 2022-10-15 04:34:35.000000 flopt-0.5.5/README.md
-drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2022-10-15 04:37:15.376895 flopt-0.5.5/datasets/
--rw-r--r--   0 tateiwa    (501) staff       (20)        0 2022-09-19 02:14:43.000000 flopt-0.5.5/datasets/__init__.py
-drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2022-10-15 04:37:15.389109 flopt-0.5.5/datasets/funcLib/
--rw-r--r--   0 tateiwa    (501) staff       (20)      481 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Ackley.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      479 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Beale.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      377 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Booth.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      497 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Bukin.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      386 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Camel.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      356 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/DeJongF3.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      462 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Easom.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      471 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Eggholder.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      421 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Ellipsoid.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      757 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/FiveWell.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      585 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Goldstain.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      430 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Griewank.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      411 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Ktable.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      562 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Levi.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      373 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Matyas.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      504 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/McCormick.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      437 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Michalewicz.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      361 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Rastrigin.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      416 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Rosenbrock.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      484 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Schaffer2.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      499 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Schaffer4.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      411 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Schwefel.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      579 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Shuberts.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      547 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/SixHump.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      258 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Sphere.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      319 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/SumDiffPower.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      318 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/WeitedSphere.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      402 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/XinShe.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      351 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/Zahkarov.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     7008 2022-09-27 05:54:11.000000 flopt-0.5.5/datasets/funcLib/__init__.py
-drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2022-10-15 04:37:15.400088 flopt-0.5.5/flopt/
--rw-r--r--   0 tateiwa    (501) staff       (20)      887 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/__init__.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     2916 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/constants.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     4072 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/constraint.py
-drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2022-10-15 04:37:15.405582 flopt-0.5.5/flopt/convert/
--rw-r--r--   0 tateiwa    (501) staff       (20)      309 2022-09-19 02:14:43.000000 flopt-0.5.5/flopt/convert/__init__.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     3518 2022-09-19 02:14:43.000000 flopt-0.5.5/flopt/convert/_pulp.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     5032 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/convert/binarize.py
--rw-r--r--   0 tateiwa    (501) staff       (20)    11146 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/convert/linearize.py
--rw-r--r--   0 tateiwa    (501) staff       (20)    23207 2022-10-08 12:14:03.000000 flopt-0.5.5/flopt/convert/structure.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     2821 2022-10-11 00:01:28.000000 flopt-0.5.5/flopt/env.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      266 2022-09-19 02:14:43.000000 flopt-0.5.5/flopt/error.py
--rw-r--r--   0 tateiwa    (501) staff       (20)    40434 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/expression.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      606 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/flopt.config
-drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2022-10-15 04:37:15.415662 flopt-0.5.5/flopt/performance/
--rw-r--r--   0 tateiwa    (501) staff       (20)      685 2022-09-27 05:54:11.000000 flopt-0.5.5/flopt/performance/__init__.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     1528 2022-09-27 05:54:11.000000 flopt-0.5.5/flopt/performance/base_dataset.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     3495 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/performance/custom_dataset.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     3300 2022-09-27 05:54:11.000000 flopt-0.5.5/flopt/performance/func_dataset.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     8695 2022-09-27 05:54:11.000000 flopt-0.5.5/flopt/performance/log_visualizer.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     3172 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/performance/mip_dataset.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     5495 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/performance/performance.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     6579 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/performance/tsp_dataset.py
--rw-r--r--   0 tateiwa    (501) staff       (20)    12870 2022-09-19 02:14:43.000000 flopt-0.5.5/flopt/polynomial.py
--rw-r--r--   0 tateiwa    (501) staff       (20)    11031 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/problem.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     8559 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solution.py
-drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2022-10-15 04:37:15.422394 flopt-0.5.5/flopt/solvers/
--rw-r--r--   0 tateiwa    (501) staff       (20)     4870 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solvers/__init__.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     4073 2022-10-09 14:59:05.000000 flopt-0.5.5/flopt/solvers/amplify_search.py
-drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2022-10-15 04:37:15.424249 flopt-0.5.5/flopt/solvers/auto_search/
--rw-r--r--   0 tateiwa    (501) staff       (20)       36 2022-09-27 05:54:11.000000 flopt-0.5.5/flopt/solvers/auto_search/__init__.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     5676 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solvers/auto_search/auto_search.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     5015 2022-09-27 05:54:11.000000 flopt-0.5.5/flopt/solvers/auto_search/selector.py
--rw-r--r--   0 tateiwa    (501) staff       (20)    13203 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solvers/base.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     3899 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solvers/cvxopt_qp_search.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     3243 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solvers/hyperopt_search.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     6284 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solvers/optuna_searches.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     5005 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solvers/pulp_search.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     1485 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solvers/random_search.py
-drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2022-10-15 04:37:15.426073 flopt-0.5.5/flopt/solvers/scipy_searches/
--rw-r--r--   0 tateiwa    (501) staff       (20)       85 2022-09-27 05:54:11.000000 flopt-0.5.5/flopt/solvers/scipy_searches/__init__.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     3386 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solvers/scipy_searches/scipy_milp_search.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     4327 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solvers/scipy_searches/scipy_search.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     7015 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solvers/shuffled_frog_leaping_search.py
-drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2022-10-15 04:37:15.427889 flopt-0.5.5/flopt/solvers/solver_utils/
--rw-r--r--   0 tateiwa    (501) staff       (20)      163 2022-09-19 02:14:43.000000 flopt-0.5.5/flopt/solvers/solver_utils/__init__.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     3413 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solvers/solver_utils/common.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     2585 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solvers/solver_utils/solver_log.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     1731 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/solvers/two_opt.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     4411 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/utils.py
--rw-r--r--   0 tateiwa    (501) staff       (20)    33489 2022-10-15 04:34:35.000000 flopt-0.5.5/flopt/variable.py
-drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2022-10-15 04:37:15.402549 flopt-0.5.5/flopt.egg-info/
--rw-r--r--   0 tateiwa    (501) staff       (20)     4721 2022-10-15 04:37:15.000000 flopt-0.5.5/flopt.egg-info/PKG-INFO
--rw-r--r--   0 tateiwa    (501) staff       (20)     2897 2022-10-15 04:37:15.000000 flopt-0.5.5/flopt.egg-info/SOURCES.txt
--rw-r--r--   0 tateiwa    (501) staff       (20)        1 2022-10-15 04:37:15.000000 flopt-0.5.5/flopt.egg-info/dependency_links.txt
--rw-r--r--   0 tateiwa    (501) staff       (20)      129 2022-10-15 04:37:15.000000 flopt-0.5.5/flopt.egg-info/requires.txt
--rw-r--r--   0 tateiwa    (501) staff       (20)       21 2022-10-15 04:37:15.000000 flopt-0.5.5/flopt.egg-info/top_level.txt
--rw-r--r--   0 tateiwa    (501) staff       (20)       38 2022-10-15 04:37:15.443679 flopt-0.5.5/setup.cfg
--rw-r--r--   0 tateiwa    (501) staff       (20)     1320 2022-10-15 04:34:35.000000 flopt-0.5.5/setup.py
-drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2022-10-15 04:37:15.442434 flopt-0.5.5/tests/
--rw-r--r--   0 tateiwa    (501) staff       (20)        0 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/__init__.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      109 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/conftest.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     2770 2022-10-15 04:34:35.000000 flopt-0.5.5/tests/test_Constraint.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     9592 2022-10-15 04:34:35.000000 flopt-0.5.5/tests/test_Convert.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     4320 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/test_CustomExpression.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     7171 2022-10-15 04:34:35.000000 flopt-0.5.5/tests/test_Expression.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     2126 2022-10-15 04:34:35.000000 flopt-0.5.5/tests/test_Performance.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     4142 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/test_Polynomial.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     2152 2022-09-27 05:54:11.000000 flopt-0.5.5/tests/test_Problem.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     3472 2022-09-27 05:54:11.000000 flopt-0.5.5/tests/test_ProblemType.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     3160 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/test_Solution.py
--rw-r--r--   0 tateiwa    (501) staff       (20)    14575 2022-10-15 04:34:35.000000 flopt-0.5.5/tests/test_Solver.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     3237 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/test_VarBinary.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     2792 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/test_VarContinuous.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     2758 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/test_VarInteger.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      700 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/test_VarPermutation.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     3358 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/test_VarSpin.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      999 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/test_VariableArray.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     1454 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/test_VariableFactory.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      238 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/test_example.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     4843 2022-10-15 04:34:35.000000 flopt-0.5.5/tests/test_linearize.py
--rw-r--r--   0 tateiwa    (501) staff       (20)      708 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/test_logger.py
--rw-r--r--   0 tateiwa    (501) staff       (20)     2135 2022-09-19 02:14:43.000000 flopt-0.5.5/tests/test_utils.py
+drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2023-06-03 02:01:55.738383 flopt-0.5.6/
+-rw-r--r--   0 tateiwa    (501) staff       (20)     1067 2023-05-11 09:13:54.000000 flopt-0.5.6/LICENSE
+-rw-r--r--   0 tateiwa    (501) staff       (20)     4719 2023-06-03 02:01:55.738065 flopt-0.5.6/PKG-INFO
+-rw-r--r--   0 tateiwa    (501) staff       (20)     4172 2023-06-03 01:03:16.000000 flopt-0.5.6/README.md
+drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2023-06-03 02:01:55.692518 flopt-0.5.6/datasets/
+-rw-r--r--   0 tateiwa    (501) staff       (20)        0 2023-05-11 09:13:54.000000 flopt-0.5.6/datasets/__init__.py
+drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2023-06-03 02:01:55.705035 flopt-0.5.6/datasets/funcLib/
+-rw-r--r--   0 tateiwa    (501) staff       (20)      527 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Ackley.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      575 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Beale.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      435 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Booth.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      642 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Bukin.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      515 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Camel.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      403 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/DeJongF3.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      483 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Easom.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      580 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Eggholder.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      408 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Ellipsoid.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      873 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/FiveWell.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     1056 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/G1.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      694 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Goldstain.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      485 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Griewank.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      454 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Ktable.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      690 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Levi.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      428 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Matyas.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      689 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/McCormick.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      527 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Michalewicz.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      418 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Rastrigin.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      447 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Rosenbrock.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      526 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Schaffer2.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      544 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Schaffer4.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      406 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Schwefel.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      755 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Shuberts.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      724 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/SixHump.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      328 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Sphere.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      407 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/SumDiffPower.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      402 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/WeightedSphere.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      513 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/XinShe.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      459 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/Zahkarov.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     1708 2023-06-03 01:03:16.000000 flopt-0.5.6/datasets/funcLib/__init__.py
+drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2023-06-03 02:01:55.711828 flopt-0.5.6/flopt/
+-rw-r--r--   0 tateiwa    (501) staff       (20)     1641 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/__init__.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      188 2023-05-20 12:29:08.000000 flopt-0.5.6/flopt/apis.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     3418 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/constants.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     4223 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/constraint.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     1290 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/container.py
+drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2023-06-03 02:01:55.715684 flopt-0.5.6/flopt/convert/
+-rw-r--r--   0 tateiwa    (501) staff       (20)      309 2023-05-11 09:13:54.000000 flopt-0.5.6/flopt/convert/__init__.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     3499 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/convert/_pulp.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     5072 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/convert/binarize.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)    11152 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/convert/linearize.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)    24355 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/convert/structure.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     3102 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/env.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      266 2023-05-11 09:13:54.000000 flopt-0.5.6/flopt/error.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)    50815 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/expression.py
+drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2023-06-03 02:01:55.719100 flopt-0.5.6/flopt/performance/
+-rw-r--r--   0 tateiwa    (501) staff       (20)      866 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/performance/__init__.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     1528 2023-05-11 09:13:54.000000 flopt-0.5.6/flopt/performance/base_dataset.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     3432 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/performance/custom_dataset.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     2974 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/performance/func_dataset.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     8757 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/performance/log_visualizer.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     3168 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/performance/mip_dataset.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     5485 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/performance/performance.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     6576 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/performance/tsp_dataset.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)    12700 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/polynomial.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)    18434 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/problem.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)    10071 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solution.py
+drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2023-06-03 02:01:55.725169 flopt-0.5.6/flopt/solvers/
+-rw-r--r--   0 tateiwa    (501) staff       (20)     7393 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/__init__.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     4013 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/amplify_search.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     5802 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/auto_search.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)    13431 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/base.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     4584 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/cvxopt_search.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     3177 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/hyperopt_search.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     6401 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/optuna_searches.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     4984 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/pulp_search.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     1442 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/random_search.py
+drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2023-06-03 02:01:55.726449 flopt-0.5.6/flopt/solvers/scipy_searches/
+-rw-r--r--   0 tateiwa    (501) staff       (20)       85 2023-05-11 09:13:54.000000 flopt-0.5.6/flopt/solvers/scipy_searches/__init__.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     3366 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/scipy_searches/scipy_milp_search.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     4474 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/scipy_searches/scipy_search.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     5085 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/selector.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     7069 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/shuffled_frog_leaping_search.py
+drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2023-06-03 02:01:55.727828 flopt-0.5.6/flopt/solvers/solver_utils/
+-rw-r--r--   0 tateiwa    (501) staff       (20)      163 2023-05-11 09:13:54.000000 flopt-0.5.6/flopt/solvers/solver_utils/__init__.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     3506 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/solver_utils/common.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     2577 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/solver_utils/solver_log.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     2326 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/solvers/steepest_descent.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     1731 2023-05-11 09:13:54.000000 flopt-0.5.6/flopt/solvers/two_opt.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     5598 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/utils.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)    32226 2023-06-03 01:03:17.000000 flopt-0.5.6/flopt/variable.py
+drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2023-06-03 02:01:55.713605 flopt-0.5.6/flopt.egg-info/
+-rw-r--r--   0 tateiwa    (501) staff       (20)     4719 2023-06-03 02:01:55.000000 flopt-0.5.6/flopt.egg-info/PKG-INFO
+-rw-r--r--   0 tateiwa    (501) staff       (20)     2877 2023-06-03 02:01:55.000000 flopt-0.5.6/flopt.egg-info/SOURCES.txt
+-rw-r--r--   0 tateiwa    (501) staff       (20)        1 2023-06-03 02:01:55.000000 flopt-0.5.6/flopt.egg-info/dependency_links.txt
+-rw-r--r--   0 tateiwa    (501) staff       (20)      123 2023-06-03 02:01:55.000000 flopt-0.5.6/flopt.egg-info/requires.txt
+-rw-r--r--   0 tateiwa    (501) staff       (20)       21 2023-06-03 02:01:55.000000 flopt-0.5.6/flopt.egg-info/top_level.txt
+-rw-r--r--   0 tateiwa    (501) staff       (20)       38 2023-06-03 02:01:55.738505 flopt-0.5.6/setup.cfg
+-rw-r--r--   0 tateiwa    (501) staff       (20)     1276 2023-06-03 01:04:09.000000 flopt-0.5.6/setup.py
+drwxr-xr-x   0 tateiwa    (501) staff       (20)        0 2023-06-03 02:01:55.737461 flopt-0.5.6/tests/
+-rw-r--r--   0 tateiwa    (501) staff       (20)        0 2023-05-11 09:13:54.000000 flopt-0.5.6/tests/__init__.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      109 2023-05-11 09:13:54.000000 flopt-0.5.6/tests/conftest.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     2770 2023-05-11 09:13:54.000000 flopt-0.5.6/tests/test_Constraint.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)    10034 2023-06-03 01:03:17.000000 flopt-0.5.6/tests/test_Convert.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     4320 2023-05-11 09:13:54.000000 flopt-0.5.6/tests/test_CustomExpression.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)    10640 2023-06-03 01:03:17.000000 flopt-0.5.6/tests/test_Expression.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     2117 2023-06-03 01:03:17.000000 flopt-0.5.6/tests/test_Performance.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     4411 2023-06-03 01:03:17.000000 flopt-0.5.6/tests/test_Polynomial.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     3391 2023-06-03 01:03:17.000000 flopt-0.5.6/tests/test_Problem.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     3494 2023-06-03 01:03:17.000000 flopt-0.5.6/tests/test_ProblemType.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     3582 2023-06-03 01:03:17.000000 flopt-0.5.6/tests/test_Solution.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)    19395 2023-06-03 01:03:17.000000 flopt-0.5.6/tests/test_Solver.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     3237 2023-05-11 09:13:54.000000 flopt-0.5.6/tests/test_VarBinary.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     2792 2023-05-11 09:13:54.000000 flopt-0.5.6/tests/test_VarContinuous.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     2758 2023-05-11 09:13:54.000000 flopt-0.5.6/tests/test_VarInteger.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      700 2023-05-11 09:13:54.000000 flopt-0.5.6/tests/test_VarPermutation.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     3308 2023-06-03 01:03:17.000000 flopt-0.5.6/tests/test_VarSpin.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     1454 2023-05-11 09:13:54.000000 flopt-0.5.6/tests/test_VariableFactory.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      238 2023-05-11 09:13:54.000000 flopt-0.5.6/tests/test_example.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     4636 2023-06-03 01:03:17.000000 flopt-0.5.6/tests/test_linearize.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)      708 2023-05-11 09:13:54.000000 flopt-0.5.6/tests/test_logger.py
+-rw-r--r--   0 tateiwa    (501) staff       (20)     2136 2023-06-03 01:03:17.000000 flopt-0.5.6/tests/test_utils.py
```

### Comparing `flopt-0.5.5/LICENSE` & `flopt-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flopt-0.5.5/PKG-INFO` & `flopt-0.5.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: flopt
-Version: 0.5.5
+Version: 0.5.6
 Summary: A python Non-Linear Programming API with Heuristic approach
 Home-page: https://flopt.readthedocs.io/en/latest/index.html
 Author: nariaki tateiwa
 Author-email: nariaki3551@gmail.com
 License: MIT
 Keywords: optimization nonliear search heuristics algorithm
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flopt
 
 A Python Flexible Modeler for Optimization Problems.<br><br>
-flopt allows modeling of various problems such as LP, QP, Ising, QUBO, etc.<br>
-Users can also solve the modeled problem using some solvers and obtain the optimal or good solutions.
+
+flopt is a modeling tool for optimization problems such as LP, QP, Ising, QUBO, etc.
+flopt provides various functions for flexible and easy modeling.
+Users can also solve modeled problems with several solvers to obtain optimal or good solutions.
 
 [![Documentation Status](https://readthedocs.org/projects/flopt/badge/?version=latest)](https://flopt.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/flopt.svg)](https://badge.fury.io/py/flopt) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flopt) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 [documentation](https://flopt.readthedocs.io/en/latest/) | [tutorial](https://flopt.readthedocs.io/en/latest/tutorial/index.html) | [case studies](https://flopt.readthedocs.io/en/latest/case_studies/index.html)
 
 <br>
 
@@ -78,27 +79,27 @@
 <br>
 
 ## Simple Example
 
 You  can write codes like PuLP application.
 
 ```python
-from flopt import Variable, Problem, Solver
+from flopt import Variable, Problem
 
 # Variables
 a = Variable('a', lowBound=0, upBound=1, cat='Continuous')
 b = Variable('b', lowBound=1, upBound=2, cat='Continuous')
 c = Variable('c', upBound=3, cat='Continuous')
 
 # Problem
 prob = Problem()
 prob += 2 * (3*a+b) * c**2 + 3 # set the objective function
 prob += a + b * c <= 3         # set the constraint
 
-# Solver
+# Solve
 prob.solve(timelimit=0.5, msg=True) # run solver to solve the problem
 
 # display the result, incumbent solution
 print('obj value', prob.getObjectiveValue())
 print('a', a.value())
 print('b', b.value())
 print('c', c.value())
@@ -115,32 +116,32 @@
 a = Variable('a', lowBound=0, upBound=1, cat='Integer')
 b = Variable('b', lowBound=1, upBound=2, cat='Continuous')
 
 def user_func(a, b):
     from math import sin, cos
     return (0.7*a + 0.3*cos(b)**2 + 0.1*sin(b))*abs(a)
 
-custom_obj = CustomExpression(func=user_func, arg=[a, b])
+custom_obj = CustomExpression(func=user_func, args=[a, b])
 
 prob = Problem(name='CustomExpression')
 prob += custom_obj
 
-# Solver
+# Solve
 prob.solve(timelimit=1, msg=True)  # run solver to solve the problem
 
 # display the result, incumbent solution
 print('obj value', prob.getObjectiveValue())
 ```
 
 <br>
 
 In the case you solve TSP, *Permutation Variable* is useful.
 
 ```python
-from flopt import Variable, Problem, Solver, CustomExpression
+from flopt import Variable, Problem, CustomExpression
 
 N = 4  # Number of city
 D = [[0,1,2,3],  # Distance matrix
      [3,0,2,1],
      [1,2,0,3],
      [2,3,1,0]]
 
@@ -149,21 +150,21 @@
 
 # Object
 def tsp_dist(x):
     distance = 0
     for head, tail in zip(x, x[1:]+[x[0]]):
         distance += D[head][tail]  # D is the distance matrix
     return distance
-tsp_obj = CustomExpression(func=tsp_dist, arg=[x])
+tsp_obj = CustomExpression(func=tsp_dist, args=[x])
 
 # Problem
 prob = Problem(name='TSP')
 prob += tsp_obj
 
-# Solver
+# Solve
 prob.solve(timelimit=10, msg=True)    # run solver to solve the problem
 
 # display the result, incumbent solution
 print('obj value', prob.getObjectiveValue())
 print('x', x.value())
 ```
```

### Comparing `flopt-0.5.5/README.md` & `flopt-0.5.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # flopt
 
 A Python Flexible Modeler for Optimization Problems.<br><br>
-flopt allows modeling of various problems such as LP, QP, Ising, QUBO, etc.<br>
-Users can also solve the modeled problem using some solvers and obtain the optimal or good solutions.
+
+flopt is a modeling tool for optimization problems such as LP, QP, Ising, QUBO, etc.
+flopt provides various functions for flexible and easy modeling.
+Users can also solve modeled problems with several solvers to obtain optimal or good solutions.
 
 [![Documentation Status](https://readthedocs.org/projects/flopt/badge/?version=latest)](https://flopt.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/flopt.svg)](https://badge.fury.io/py/flopt) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flopt) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 [documentation](https://flopt.readthedocs.io/en/latest/) | [tutorial](https://flopt.readthedocs.io/en/latest/tutorial/index.html) | [case studies](https://flopt.readthedocs.io/en/latest/case_studies/index.html)
 
 <br>
 
@@ -61,27 +63,27 @@
 <br>
 
 ## Simple Example
 
 You  can write codes like PuLP application.
 
 ```python
-from flopt import Variable, Problem, Solver
+from flopt import Variable, Problem
 
 # Variables
 a = Variable('a', lowBound=0, upBound=1, cat='Continuous')
 b = Variable('b', lowBound=1, upBound=2, cat='Continuous')
 c = Variable('c', upBound=3, cat='Continuous')
 
 # Problem
 prob = Problem()
 prob += 2 * (3*a+b) * c**2 + 3 # set the objective function
 prob += a + b * c <= 3         # set the constraint
 
-# Solver
+# Solve
 prob.solve(timelimit=0.5, msg=True) # run solver to solve the problem
 
 # display the result, incumbent solution
 print('obj value', prob.getObjectiveValue())
 print('a', a.value())
 print('b', b.value())
 print('c', c.value())
@@ -98,32 +100,32 @@
 a = Variable('a', lowBound=0, upBound=1, cat='Integer')
 b = Variable('b', lowBound=1, upBound=2, cat='Continuous')
 
 def user_func(a, b):
     from math import sin, cos
     return (0.7*a + 0.3*cos(b)**2 + 0.1*sin(b))*abs(a)
 
-custom_obj = CustomExpression(func=user_func, arg=[a, b])
+custom_obj = CustomExpression(func=user_func, args=[a, b])
 
 prob = Problem(name='CustomExpression')
 prob += custom_obj
 
-# Solver
+# Solve
 prob.solve(timelimit=1, msg=True)  # run solver to solve the problem
 
 # display the result, incumbent solution
 print('obj value', prob.getObjectiveValue())
 ```
 
 <br>
 
 In the case you solve TSP, *Permutation Variable* is useful.
 
 ```python
-from flopt import Variable, Problem, Solver, CustomExpression
+from flopt import Variable, Problem, CustomExpression
 
 N = 4  # Number of city
 D = [[0,1,2,3],  # Distance matrix
      [3,0,2,1],
      [1,2,0,3],
      [2,3,1,0]]
 
@@ -132,21 +134,21 @@
 
 # Object
 def tsp_dist(x):
     distance = 0
     for head, tail in zip(x, x[1:]+[x[0]]):
         distance += D[head][tail]  # D is the distance matrix
     return distance
-tsp_obj = CustomExpression(func=tsp_dist, arg=[x])
+tsp_obj = CustomExpression(func=tsp_dist, args=[x])
 
 # Problem
 prob = Problem(name='TSP')
 prob += tsp_obj
 
-# Solver
+# Solve
 prob.solve(timelimit=10, msg=True)    # run solver to solve the problem
 
 # display the result, incumbent solution
 print('obj value', prob.getObjectiveValue())
 print('x', x.value())
 ```
```

### Comparing `flopt-0.5.5/datasets/funcLib/FiveWell.py` & `flopt-0.5.6/datasets/funcLib/FiveWell.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import flopt
 
 
-def create_objective(*args, **kwargs):
-    def obj(x):
-        x1, x2 = x
-        c1 = 1 + 0.05 * (x1 * x1 + (x2 - 10) * (x2 - 10))
-        c2 = 1 + 0.05 * ((x1 - 10) * (x1 - 10) + x2 * x2)
-        c3 = 1 * 0.03 * ((x1 + 10) * (x1 + 10) + x2 * x2)
-        c4 = 1 + 0.05 * ((x1 - 5) * (x1 - 5) + (x2 + 10) * (x2 + 10))
-        c5 = 1 + 0.1 * ((x1 + 5) * (x1 + 5) + (x2 + 10) * (x2 + 10))
-        c6 = 1 + 0.0001 * (x1 * x1 + x2 * x2) ** (1.2)
-        return (1 - 1 / c1 - 1 / c2 - 1 / c3 - 1 / c4 - 1 / c5) * c6
-
-    return obj
-
-
-def create_variables(cat="Continuous", *args, **kwargs):
-    variables = flopt.Variable.array("x", 2, lowBound=-20, upBound=20, cat=cat)
-    return variables
-
-
-def minimum_obj(*args, **kwargs):
-    return -1.4616
+class FiveWell:
+    @staticmethod
+    def create_objective(*args, **kwargs):
+        def obj(x):
+            x1, x2 = x
+            c1 = 1 + 0.05 * (x1 * x1 + (x2 - 10) * (x2 - 10))
+            c2 = 1 + 0.05 * ((x1 - 10) * (x1 - 10) + x2 * x2)
+            c3 = 1 * 0.03 * ((x1 + 10) * (x1 + 10) + x2 * x2)
+            c4 = 1 + 0.05 * ((x1 - 5) * (x1 - 5) + (x2 + 10) * (x2 + 10))
+            c5 = 1 + 0.1 * ((x1 + 5) * (x1 + 5) + (x2 + 10) * (x2 + 10))
+            c6 = 1 + 0.0001 * (x1 * x1 + x2 * x2) ** (1.2)
+            return (1 - 1 / c1 - 1 / c2 - 1 / c3 - 1 / c4 - 1 / c5) * c6
+
+        return obj
+
+    @staticmethod
+    def create_variables(cat="Continuous", *args, **kwargs):
+        x = flopt.Variable.array("x", 2, lowBound=-20, upBound=20, cat=cat)
+        return x
+
+    @staticmethod
+    def minimum_obj(*args, **kwargs):
+        return -1.4616
```

### Comparing `flopt-0.5.5/datasets/funcLib/Goldstain.py` & `flopt-0.5.6/datasets/funcLib/Goldstain.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import flopt
 
 
-def create_objective(*args, **kwargs):
-    def obj(x):
-        x1, x2 = x
-        c1 = (x1 + x2 + 1) ** 2
-        c2 = 19 - 14 * x1 + 3 * x1 * x1 - 14 * x2 + 6 * x1 * x2 + 3 * x2 * x2
-        c3 = (2 * x1 - 3 * x2) ** 2
-        c4 = 18 - 32 * x1 + 12 * x1 * x1 + 48 * x2 - 36 * x1 * x2 + 27 * x2 * x2
-        return (1 + c1 * c2) * (30 + c3 * c4)
-
-    return obj
-
-
-def create_variables(cat="Continuous", *args, **kwargs):
-    variables = flopt.Variable.array("x", 2, lowBound=-2, upBound=2, cat=cat)
-    return variables
-
-
-def minimum_obj(*args, **kwargs):
-    return 3
+class Goldstain:
+    @staticmethod
+    def create_objective(*args, **kwargs):
+        def obj(x):
+            x1, x2 = x
+            c1 = (x1 + x2 + 1) ** 2
+            c2 = 19 - 14 * x1 + 3 * x1 * x1 - 14 * x2 + 6 * x1 * x2 + 3 * x2 * x2
+            c3 = (2 * x1 - 3 * x2) ** 2
+            c4 = 18 - 32 * x1 + 12 * x1 * x1 + 48 * x2 - 36 * x1 * x2 + 27 * x2 * x2
+            return (1 + c1 * c2) * (30 + c3 * c4)
+
+        return obj
+
+    @staticmethod
+    def create_variables(cat="Continuous", *args, **kwargs):
+        x = flopt.Variable.array("x", 2, lowBound=-2, upBound=2, cat=cat)
+        return x
+
+    @staticmethod
+    def minimum_obj(*args, **kwargs):
+        return 3
```

### Comparing `flopt-0.5.5/flopt/constants.py` & `flopt-0.5.6/flopt/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,50 +62,64 @@
             return {vt.Binary, vt.Spin}
         elif self == vt.Spin:
             return {vt.Binary, vt.Spin}
         elif self == vt.Number:
             return {vt.Continuous, vt.Integer, vt.Binary, vt.Spin}
         elif self == vt.Any:
             return vt.Number.expand() | {vt.Permutation}
-        else:
-            return {self}
+        return {self}
 
 
 # expression type
 class ExpressionType(enum.IntEnum):
     Unknown = 200
-    Custom = 201
-    Const = 202
-    Any = 203
-    Linear = 204
-    Quadratic = 205
-    BlackBox = 206
-    Non = 207
+    Any = 201
+    Linear = 202
+    Quadratic = 203
+    Polynomial = 204
+    Nonlinear = 205
+    Permutation = 206
+    BlackBox = 207
+    Non = 208
 
     def __str__(self):
         return self.name
 
     def expand(self):
         et = self.__class__
         if self == et.Any:
             return {
                 et.Unknown,
-                et.Custom,
-                et.Const,
                 et.Linear,
                 et.Quadratic,
+                et.Polynomial,
+                et.Nonlinear,
+                et.Permutation,
                 et.BlackBox,
                 et.Non,
             }
-        elif self == et.Quadratic:
-            return {et.Const, et.Linear, et.Quadratic, et.Non}
         elif self == et.Linear:
-            return {et.Const, et.Linear, et.Non}
-        else:
-            return {self, et.Non}
+            return {et.Linear, et.Non}
+        elif self == et.Quadratic:
+            return {et.Linear, et.Quadratic, et.Non}
+        elif self == et.Polynomial:
+            return {et.Linear, et.Quadratic, et.Polynomial, et.Non}
+        elif self == et.Permutation:
+            return {et.Permutation, et.Non}
+        elif self == et.BlackBox:
+            return {et.Permutation, et.BlackBox, et.Non}
+        elif self == et.Nonlinear:
+            return {
+                et.Linear,
+                et.Quadratic,
+                et.Polynomial,
+                et.Nonlinear,
+                et.Non,
+            }
+        return {self, et.Non}
 
 
 # expression type
 class ConstraintType(enum.IntEnum):
     Le = 300
     Eq = 301
```

### Comparing `flopt-0.5.5/flopt/constraint.py` & `flopt-0.5.6/flopt/constraint.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,26 +38,34 @@
     def __init__(self, expression, _type, name=None):
         assert isinstance(_type, ConstraintType)
         self.expression = expression
         self._type = _type
         self.name = name
         self.hash = None
 
+    def clone(self):
+        """
+        Returns
+        -------
+        Reduction
+        """
+        return Constraint(self.expression.clone(), self._type, self.name)
+
     def type(self):
         return self._type
 
     def value(self, solution=None):
         return self.expression.value(solution)
 
     def feasible(self, solution=None):
         exp_value = self.value(solution)
         if self._type == ConstraintType.Eq:
             return exp_value == 0
-        else:  # self._type == ConstraintType.Le
-            return exp_value <= 0
+        # self._type == ConstraintType.Le
+        return exp_value <= 0
 
     def getVariables(self):
         return self.expression.getVariables()
 
     def isLinear(self):
         return self.expression.isLinear()
 
@@ -92,15 +100,15 @@
 
         def sazm(v):
             """Slide value for Avoiding Zero in minus direction"""
             if v != 0:
                 return v
             return vv if (vv := v - slide_epsilon) != 0 else vv - slide_epsilon
 
-        constraints = list()
+        constraints = []
         x = self.expression
         y = other.expression
 
         with create_variable_mode():
             delta = flopt.Variable(f"delta", cat="Binary")
         constraints += [sazm(x.min()) * delta <= x - epsilon]
 
@@ -132,8 +140,8 @@
         if self._type == ConstraintType.Eq:
             type_str = "=="
         else:  # self._type == ConstraintType.Le
             type_str = "<="
         return f"{self.expression.getName()} {type_str} 0"
 
     def __repr__(self):
-        return f"Constraint({repr(self.expression)}, {self._type}, {self.name})"
+        return f"Constraint({self.expression!r}, {self._type}, {self.name})"
```

### Comparing `flopt-0.5.5/flopt/convert/_pulp.py` & `flopt-0.5.6/flopt/convert/_pulp.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,22 @@
         prob = Problem()
         prob += c + b       # set the objective function
         prob += a + c == 0  # set the constraint
         prob += a + b <= 1  # set the constraint
         prob += a + d >= -1 # set the constraint
 
         # check wheter prob can be converted into pulp modeling
-        flopt.Solver(algo='PulpSearch').available(prob)
+        flopt.Solver(algo="Pulp").available(prob)
 
         # convert flopt to pulp
         from flopt.solvers.convert import flopt_to_pulp
         lp_prob, lp_solution = flopt_to_pulp(prob)
     """
     assert PulpSearch().available(prob, verbose=True)
-    solution = Solution("s", prob.getVariables())
+    solution = Solution(prob.getVariables())
     lp_prob, lp_solution = PulpSearch().createLpProblem(solution, prob)
     return lp_prob, lp_solution
 
 
 def pulp_to_flopt(prob):
     """
     Parameters
@@ -76,27 +76,27 @@
 
         # convert pulp to flopt
         from flopt.solvers.convert import pulp_to_flopt
         flopt_prob = pulp_to_flopt(prob)
 
     """
     # conver LpVariable -> VarElement
-    flopt_variables = dict()
+    flopt_variables = {}
     for var in prob.variables():
         flopt_var = flopt.Variable(
             var.getName(), lowBound=var.getLb(), upBound=var.getUb(), cat=var.cat
         )
         flopt_variables[var.getName()] = flopt_var
 
     # convert Problem -> pulp.LpProblem
     name = "" if prob.name is None else prob.name
     flopt_prob = flopt.Problem(name=name)
 
     def flopt_exp(const, var_dicts):
-        elms = list()
+        elms = []
         for var_dict in var_dicts:
             name, value = var_dict["name"], var_dict["value"]
             elms.append(value * flopt_variables[name])
         return flopt.Sum(elms) + const
 
     # convert objective function
     obj = flopt_exp(prob.objective.constant, prob.objective.to_dict())
```

### Comparing `flopt-0.5.5/flopt/convert/binarize.py` & `flopt-0.5.6/flopt/convert/binarize.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,84 +11,82 @@
     ----------
     prob : Problem
 
     Examples
     --------
     .. code-block:: python
 
-        from flopt import Variable, Problem
-        x = Variable.array('x', 2, cat='Binary')
-        y = Variable.array('y', 1, lowBound=1, upBound=3, cat='Integer')
-        x = np.hstack([x, y])
+        import flopt
+
+        x = flopt.Variable.array('x', 2, cat='Binary')
+        y = flopt.Variable('y', lowBound=1, upBound=3, cat='Integer')
+
+        prob = flopt.Problem()
+        prob += y * x[0] + x[1]
 
-        prob = Problem()
-        prob += x[2] * x[0] + x[1]
         print('[ original ]')
-        print(prob.show())
+        prob.show()
+        >>> [ original ]
+        >>>  Name: None
+        >>>   Type         : Problem
+        >>>   sense        : minimize
+        >>>   objective    : y_0*x_0+x_1
+        >>>   #constraints : 0
+        >>>   #variables   : 3 (Binary 2, Integer 1)
 
         from flopt.convert import linearize, binarize
+
         binarize(prob)
+
         print('[ binarized ]')
-        print(prob.show())
+        prob.show()
+        >>> [ binarized ]
+        >>>  Name: None
+        >>>   Type         : Problem
+        >>>   sense        : minimize
+        >>>   objective    : x_0*(1*bin_y_0_0+2*bin_y_0_1+3*bin_y_0_2)+x_1
+        >>>   #constraints : 2
+        >>>   #variables   : 6 (Binary 5, Integer 1)
 
-        linearize(prob)
-        print('[ linearized ]')
-        print(prob.show())
+        >>>   C 0, name for_bin_y_0_sum, bin_y_0_0+bin_y_0_2+bin_y_0_1-1 == 0
+        >>>   C 1, name for_bin_y_0_eq, y_0-(1*bin_y_0_0+2*bin_y_0_1+3*bin_y_0_2) == 0
 
-    ::
+        linearize(prob)
 
-        [ original ]
-         Name: None
-          Type         : Problem
-          sense        : minimize
-          objective    : y_0*x_0+x_1
-          #constraints : 0
-          #variables   : 3 (Binary 2, Integer 1)
-
-        [ binarized ]
-         Name: None
-          Type         : Problem
-          sense        : minimize
-          objective    : x_0*(1*bin_y_0_0+2*bin_y_0_1+3*bin_y_0_2)+x_1
-          #constraints : 2
-          #variables   : 6 (Binary 5, Integer 1)
-
-          C 0, name for_bin_y_0_sum, bin_y_0_0+bin_y_0_2+bin_y_0_1-1 == 0
-          C 1, name for_bin_y_0_eq, y_0-(1*bin_y_0_0+2*bin_y_0_1+3*bin_y_0_2) == 0
-
-        [ linearized ]
-         Name: None
-          Type         : Problem
-          sense        : minimize
-          objective    : mul_0+2*mul_1+3*mul_2+x_1
-          #constraints : 11
-          #variables   : 9 (Binary 8, Integer 1)
-
-          C 0, name for_bin_y_0_sum, bin_y_0_0+bin_y_0_1+bin_y_0_2-1 == 0
-          C 1, name for_bin_y_0_eq, -bin_y_0_0-(2*bin_y_0_1)-(3*bin_y_0_2)+y_0 == 0
-          C 2, name for_mul_0_1, mul_0-bin_y_0_0 <= 0
-          C 3, name for_mul_0_2, mul_0-x_0 <= 0
-          C 4, name for_mul_0_3, mul_0-(bin_y_0_0+x_0-1) >= 0
-          C 5, name for_mul_1_1, mul_1-bin_y_0_1 <= 0
-          C 6, name for_mul_1_2, mul_1-x_0 <= 0
-          C 7, name for_mul_1_3, mul_1-(bin_y_0_1+x_0-1) >= 0
-          C 8, name for_mul_2_1, mul_2-bin_y_0_2 <= 0
-          C 9, name for_mul_2_2, mul_2-x_0 <= 0
-          C 10, name for_mul_2_3, mul_2-(bin_y_0_2+x_0-1) >= 0
+        print('[ linearized ]')
+        prob.show()
+        >>> [ linearized ]
+        >>>  Name: None
+        >>>   Type         : Problem
+        >>>   sense        : minimize
+        >>>   objective    : mul_0+2*mul_1+3*mul_2+x_1
+        >>>   #constraints : 11
+        >>>   #variables   : 9 (Binary 8, Integer 1)
+
+        >>>   C 0, name for_bin_y_0_sum, bin_y_0_0+bin_y_0_1+bin_y_0_2-1 == 0
+        >>>   C 1, name for_bin_y_0_eq, -bin_y_0_0-(2*bin_y_0_1)-(3*bin_y_0_2)+y_0 == 0
+        >>>   C 2, name for_mul_0_1, mul_0-bin_y_0_0 <= 0
+        >>>   C 3, name for_mul_0_2, mul_0-x_0 <= 0
+        >>>   C 4, name for_mul_0_3, mul_0-(bin_y_0_0+x_0-1) >= 0
+        >>>   C 5, name for_mul_1_1, mul_1-bin_y_0_1 <= 0
+        >>>   C 6, name for_mul_1_2, mul_1-x_0 <= 0
+        >>>   C 7, name for_mul_1_3, mul_1-(bin_y_0_1+x_0-1) >= 0
+        >>>   C 8, name for_mul_2_1, mul_2-bin_y_0_2 <= 0
+        >>>   C 9, name for_mul_2_2, mul_2-x_0 <= 0
+        >>>   C 10, name for_mul_2_3, mul_2-(bin_y_0_2+x_0-1) >= 0
     """
-    binarizes = dict()
+    binarizes = {}
     prob.obj = binarize_expression(prob.obj, binarizes)
     for const in prob.getConstraints():
         const.expression = binarize_expression(const.expression, binarizes)
 
     for source, binaries in binarizes.items():
         prob += flopt.Sum(binaries) == 1, f"for_bin_{source.name}_sum"
         prob += source == source.toBinary(), f"for_bin_{source.name}_eq"
 
-    prob.resetVariables()
     return prob
 
 
 def binarize_expression(e, binarizes):
     """binarize a expression
 
     Parameters
@@ -144,14 +142,14 @@
                 node.elmB.parents.append(node)
                 update = True
             elif node.elmB.type() == VariableType.Spin:
                 node.elmB = node.elmB.toBinary()
                 node.elmB.parents.append(node)
                 update = True
             if update:
-                node.setName()
-                node.setPolynomial()
+                node.resetName()
+                node.polynomial = None
                 for parent in node.traverseAncestors():
-                    parent.setName()
-                    parent.setPolynomial()
+                    parent.resetName()
+                    parent.polynomial = None
                 return True
     return False
```

### Comparing `flopt-0.5.5/flopt/convert/linearize.py` & `flopt-0.5.6/flopt/convert/linearize.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,57 +23,56 @@
     prob : Problem
 
     Examples
     --------
 
     .. code-block:: python
 
-        from flopt import Variable, Problem
+        import flopt
 
-        x = Variable.array('x', 3, cat='Binary')
+        x = flopt.Variable.array('x', 3, cat='Binary')
 
-        prob = Problem()
+        prob = flopt.Problem()
         prob += x[0] - 2*x[1] - x[0]*x[1]*x[2]
+
         print('[ original ]')
-        print(prob.show())
+        prob.show()
+        >>> [ original ]
+        >>>  Name: None
+        >>>   Type         : Problem
+        >>>   sense        : minimize
+        >>>   objective    : x_0-(2*x_1)-((x_0*x_1)*x_2)
+        >>>   #constraints : 0
+        >>>   #variables   : 3 (Binary 3)
+
 
         from flopt.convert import linearize
-        linearize(prob)
-        print('[ linearized ])
-        print(prob.show())
 
-    ::
+        linearize(prob)
 
-        [ original ]
-         Name: None
-          Type         : Problem
-          sense        : minimize
-          objective    : x_0-(2*x_1)-((x_0*x_1)*x_2)
-          #constraints : 0
-          #variables   : 3 (Binary 3)
-
-
-        [ linearized ]
-         Name: None
-          Type         : Problem
-          sense        : minimize
-          objective    : 0-mul_1+x_0-(2*x_1)
-          #constraints : 6
-          #variables   : 5 (Binary 5)
-
-          C 0, name for_mul_0_1, mul_0-x_0 <= 0
-          C 1, name for_mul_0_2, mul_0-x_1 <= 0
-          C 2, name for_mul_0_3, mul_0-(x_0+x_1-1) >= 0
-          C 3, name for_mul_1_1, mul_1-mul_0 <= 0
-          C 4, name for_mul_1_2, mul_1-x_2 <= 0
-          C 5, name for_mul_1_3, mul_1-(mul_0+x_2-1) >= 0
+        print('[ linearized ])
+        prob.show()
+        >>> [ linearized ]
+        >>>  Name: None
+        >>>   Type         : Problem
+        >>>   sense        : minimize
+        >>>   objective    : 0-mul_1+x_0-(2*x_1)
+        >>>   #constraints : 6
+        >>>   #variables   : 5 (Binary 5)
+
+        >>>   C 0, name for_mul_0_1, mul_0-x_0 <= 0
+        >>>   C 1, name for_mul_0_2, mul_0-x_1 <= 0
+        >>>   C 2, name for_mul_0_3, mul_0-(x_0+x_1-1) >= 0
+        >>>   C 3, name for_mul_1_1, mul_1-mul_0 <= 0
+        >>>   C 4, name for_mul_1_2, mul_1-x_2 <= 0
+        >>>   C 5, name for_mul_1_3, mul_1-(mul_0+x_2-1) >= 0
 
     """
     try:
-        var_muls = dict()
+        var_muls = {}
         prob.setObjective(linearize_expression(prob.obj, var_muls))
         for const in prob.getConstraints():
             const.expression = linearize_expression(const.expression, var_muls)
     except NeedToBinarize:
         logger.info(
             f"problem will be binarized because it includes dislinearable multipry"
         )
@@ -95,37 +94,36 @@
             VariableType.Binary,
             VariableType.Integer,
         }:
             if var_a.type() == VariableType.Binary:
                 var_bin, var_int = var_a, var_b
             else:
                 var_bin, var_int = var_b, var_a
-            l = var_int.getLb(must_number=True)
-            u = var_int.getUb(must_number=True)
+            l = var_int.getLb(number=True)
+            u = var_int.getUb(number=True)
             prob += var_mul >= l * var_bin, f"for_{var_mul.name}_1"
             prob += var_mul <= u * var_bin, f"for_{var_mul.name}_2"
             prob += var_mul >= var_int - u * (1 - var_bin), f"for_{var_mul.name}_3"
             prob += var_mul <= var_int - l * (1 - var_bin), f"for_{var_mul.name}_4"
         #  (Binary, Continuous)
         elif {var_a.type(), var_b.type()} == {
             VariableType.Binary,
             VariableType.Continuous,
         }:
             if var_a.type() == VariableType.Binary:
                 var_bin, var_con = var_a, var_b
             else:
                 var_bin, var_con = var_b, var_a
-            l = var_con.getLb(must_number=True)
-            u = var_con.getUb(must_number=True)
+            l = var_con.getLb(number=True)
+            u = var_con.getUb(number=True)
             prob += var_mul >= l * var_bin, f"for_{var_mul.name}_1"
             prob += var_mul <= u * var_bin, f"for_{var_mul.name}_2"
             prob += var_mul >= var_con - l * (1 - var_bin), f"for_{var_mul.name}_3"
             prob += var_mul <= var_con - u * (1 - var_bin), f"for_{var_mul.name}_4"
 
-    prob.resetVariables()
     return prob
 
 
 def linearize_expression(e, var_muls):
     """linearize a expression
 
     Parameters
@@ -186,19 +184,19 @@
                 if not is_linearable(node.elmB):
                     raise LinearizeError()
                 elif need_binarize(node.elmB):
                     raise NeedToBinarize()
                 node.elmB = create_var_mul(node.elmB, var_muls)
                 update = True
             if update:
-                node.setName()
-                node.setPolynomial()
+                node.resetName()
+                node.polynomial = None
                 for parent in node.traverseAncestors():
-                    parent.setName()
-                    parent.setPolynomial()
+                    parent.resetName()
+                    parent.polynomial = None
                 return False, e
     return True, e
 
 
 def create_var_mul(node, var_muls):
     """create new variable and replace variable-multiply to it
     Parameters
```

### Comparing `flopt-0.5.5/flopt/convert/structure.py` & `flopt-0.5.6/flopt/convert/structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 from flopt import Variable, Problem
-from flopt.variable import VariableArray
+from flopt.container import FloptNdarray
 from flopt.convert.linearize import linearize
 from flopt.constants import VariableType, ConstraintType, array_classes, np_float
 from flopt.error import ConversionError
 from flopt.env import setup_logger, create_variable_mode
 
 logger = setup_logger(__name__)
 
@@ -39,23 +39,21 @@
         non_nones = [coeff * array for array, coeff in arrays if array is not None]
         return func(non_nones)
 
 
 def zero_percentage(array):
     if array is None:
         return None
-    else:
-        return f"{(1 - np.count_nonzero(array)/array.size)*100:.3f}"
+    return f"{(1 - np.count_nonzero(array)/array.size)*100:.3f}"
 
 
 def shape(array):
     if array is None:
         return None
-    else:
-        return array.shape
+    return array.shape
 
 
 # -------------------------------------------------------
 #   Expression Structures
 # -------------------------------------------------------
 
 
@@ -161,25 +159,31 @@
     def fromFlopt(cls, prob, x=None, option=None, progress=False):
         """
         Parameters
         ----------
         prob : Problem
         x : None or list of VarElement family
         progress: bool
-        option : {"all_neq", "all_eq"}
+        option : {"ineq", "eq"}
 
         Returns
         -------
         QpStructure
         """
+        assert option is None or option in {
+            "ineq",
+            "eq",
+        }, f"option must be None, ineq or eq, but got {option}"
         assert prob.obj.isQuadratic()
         assert all(const.isLinear() for const in prob.getConstraints())
-
         if x is None:
-            x = VariableArray(list(prob.getVariables()), dtype=object)
+            variables = list(prob.getVariables())
+            x = FloptNdarray(sorted(variables, key=lambda v: ("__" in v.name, v.name)))
+        elif not isinstance(x, np.ndarray):
+            x = FloptNdarray(x)
 
         quadratic = prob.obj.toQuadratic(x)
         Q, c, C = quadratic.Q, quadratic.c, quadratic.C
         if Q is not None:
             num_x = Q.shape[0]
         elif c is not None:
             num_x = len(c)
@@ -194,34 +198,34 @@
 
         else:
 
             def iter_wrapper(x, *args, **kwargs):
                 return x
 
         # create G, h
-        num_neq_consts = sum(
+        num_ineq_consts = sum(
             const.type() == ConstraintType.Le for const in prob.getConstraints()
         )
-        if num_neq_consts == 0:
+        if num_ineq_consts == 0:
             G = None
             h = None
         else:
-            G = np.zeros((num_neq_consts, num_x), dtype=np_float)
-            h = np.zeros((num_neq_consts,), dtype=np_float)
+            G = np.zeros((num_ineq_consts, num_x), dtype=np_float)
+            h = np.zeros((num_ineq_consts,), dtype=np_float)
             i = 0
             for const in iter_wrapper(
-                prob.getConstraints(), desc="convert neq constraints"
+                prob.getConstraints(), desc="convert ineq constraints"
             ):
                 if const.type() == ConstraintType.Le:
                     # c.T.dot(x) + C <= 0
                     linear = const.expression.toLinear(x)
                     G[i, :] = linear.c.T
                     h[i] = -linear.C
                     i += 1
-            assert i == num_neq_consts
+            assert i == num_ineq_consts
 
         # create A, b
         num_eq_consts = sum(
             const.type() == ConstraintType.Eq for const in prob.getConstraints()
         )
         if num_eq_consts == 0:
             A = None
@@ -251,22 +255,21 @@
             VariableType.Binary: "Binary",
             VariableType.Spin: "Spin",
         }
         types = [type2str[var.type()] for var in x]
 
         qp = cls(Q, c, C, G, h, A, b, lb, ub, types, x)
 
-        if option == "all_neq":
-            return qp.toAllNeq()
-        elif option == "all_eq":
-            return qp.toAllEq()
-        else:
-            return qp
+        if option == "ineq":
+            return qp.toIneq()
+        elif option == "eq":
+            return qp.toEq()
+        return qp
 
-    def toAllNeq(self):
+    def toIneq(self):
         """convert all non eqaual constraint type
 
         ::
 
           obj  1/2 x.T.dot(Q).dot(x) + c.T.dot(x) + C
           s.t. [G; A; -A] x <= [h; b; -b]
                lb <= x <= ub
@@ -279,15 +282,15 @@
         h = merge(np.hstack, [(self.h, 1), (self.b, 1), (self.b, -1)])
         A = None
         b = None
         return QpStructure(
             self.Q, self.c, self.C, G, h, A, b, self.lb, self.ub, self.types, self.x
         )
 
-    def toAllEq(self):
+    def toEq(self):
         """convert all eqaual constraint type
 
         ::
 
           obj  1/2 x.T.dot([Q, O; O, O]).dot([x; s]) + [c; O].T.dot([x; s]) + C
           s.t. [A, O; G, I] [x; s] == [b; h]
                lb <= x <= ub
@@ -298,41 +301,50 @@
         if self.G is None:
             return self
         num_stack = len(self.G)
         num_var = self.numVariables()
         Q = np.zeros((num_var + num_stack, num_var + num_stack), dtype=np_float)
         Q[: self.Q.shape[0], : self.Q.shape[1]] = self.Q
         c = np.hstack([self.c, np.zeros((num_stack,), dtype=np_float)])
-        A = np.zeros((self.A.shape[0] + num_stack, num_var + num_stack), dtype=np_float)
-        A[: self.A.shape[0], : self.A.shape[1]] = self.A
-        A[self.A.shape[0] :, : self.G.shape[1]] = self.G
-        A[self.A.shape[0] :, self.G.shape[1] :] = np.identity(num_stack, dtype=np_float)
-        b = np.hstack([self.b, self.h])
+        if self.A is None:
+            A_row, A_col = 0, 0
+        else:
+            A_row, A_col = self.A.shape
+        A = np.zeros((A_row + num_stack, num_var + num_stack), dtype=np_float)
+        A[:A_row, :A_col] = self.A
+        A[A_row:, : self.G.shape[1]] = self.G
+        A[A_row:, self.G.shape[1] :] = np.identity(num_stack, dtype=np_float)
+        if self.b is None:
+            b = self.h
+        else:
+            b = np.hstack([self.b, self.h])
         if self.lb is not None:
             lb = np.hstack([self.lb, np.zeros((num_stack,), dtype=np_float)])
         else:
             lb = None
         if self.ub is not None:
             ub = np.hstack([self.ub, np.full((num_stack,), None, dtype=np_float)])
         else:
             ub = None
         if self.types is not None:
             types = self.types + ["Continuous"] * num_stack
         else:
             types = self.types
         if self.x is not None:
             with create_variable_mode():
-                s = Variable.array("slack", num_stack, lowBound=0, cat="Continuous")
+                s = Variable.array(
+                    "slack", num_stack, lowBound=0, cat="Continuous", ini_value=0
+                )
             x = np.hstack([self.x, s])
         else:
             x = self.x
         return QpStructure(Q, c, self.C, None, None, A, b, lb, ub, types, x)
 
-    def boundsToNeq(self):
-        """convert bounds constraints into neq constraints
+    def boundsToIneq(self):
+        """convert bounds constraints into inequality constraints
 
         ::
 
           obj  1/2 x.T.dot(Q).dot(x) + c.T.dot(x) + C
           s.t. [G; -I; I] x <= [h; -lb; ub]
                A x == b
 
@@ -340,41 +352,43 @@
         -------
         QpStructure
         """
         G = np.array(self.G) if self.G is not None else None
         h = np.array(self.h) if self.h is not None else None
         if self.lb is not None:
             I = np.identity(self.numVariables(), dtype=np_float)
-            G = merge(np.vstack, [(G, 1), (I, -1)])
-            h = merge(np.hstack, [(h, 1), (self.lb, -1)])
+            non_none_ix = np.logical_not(np.isnan(self.lb))
+            G = merge(np.vstack, [(G, 1), (I[non_none_ix], -1)])
+            h = merge(np.hstack, [(h, 1), (self.lb[non_none_ix], -1)])
         if self.ub is not None:
             I = np.identity(self.numVariables(), dtype=np_float)
-            G = merge(np.vstack, [(G, 1), (I, 1)])
-            h = merge(np.hstack, [(h, 1), (self.ub, 1)])
+            non_none_ix = np.logical_not(np.isnan(self.ub))
+            G = merge(np.vstack, [(G, 1), (I[non_none_ix], 1)])
+            h = merge(np.hstack, [(h, 1), (self.ub[non_none_ix], 1)])
         lb, ub = None, None
         return QpStructure(
             self.Q, self.c, self.C, G, h, self.A, self.b, lb, ub, self.types, self.x
         )
 
-    def toFlopt(self, name=None):
+    def toFlopt(self, var_name="x"):
         """
         Parameters
         ----------
-        name : str
-            name of problem
+        var_name : str
+            variable prefix
 
         Returns
         -------
         Problem
         """
         if self.x is not None:
             x = self.x
         else:
-            x = Variable.array("x", len(self.Q), self.lb, self.ub, self.types)
-        prob = Problem(name)
+            x = Variable.array(var_name, len(self.Q), self.lb, self.ub, self.types)
+        prob = Problem()
         prob += (0.5 * (x.T.dot(self.Q).dot(x)) + self.c.T.dot(x) + self.C).expand()
         if self.G is not None:
             for g, h_ in zip(self.G, self.h):
                 prob += g.dot(x) <= h_
         if self.A is not None:
             for a, b_ in zip(self.A, self.b):
                 prob += a.dot(x) == b_
@@ -439,15 +453,15 @@
         Returns
         -------
         QuboStructure
         """
         assert self.G is None and self.A is None
         return self.toIsing().toQubo()
 
-    def show(self):
+    def show(self, to_str=False):
         s = f"QpStructure\n"
         s += f"obj  1/2 x.T.dot(Q).dot(x) + c.T.dot(x) + C\n"
         s += f"s.t. Gx <= h\n"
         s += f"     Ax == b\n"
         s += f"     lb <= x <= ub\n\n"
         s += f"#x\n{self.numVariables()}\n\n"
         s += f"Q\n{self.Q}\n\n"
@@ -456,15 +470,17 @@
         s += f"G\n{self.G}\n\n"
         s += f"h\n{self.h}\n\n"
         s += f"A\n{self.A}\n\n"
         s += f"b\n{self.b}\n\n"
         s += f"lb\n{self.lb}\n\n"
         s += f"ub\n{self.ub}\n\n"
         s += f"x\n{self.x}"
-        return s
+        if to_str:
+            return s
+        print(s)
 
     def __repr__(self):
         return f"QpStructure{self.Q, self.c, self.C, self.G, self.h, self.A, self.b, self.lb, self.ub, self.types, self.x}"
 
     def __str__(self):
         s = f"QpStructure\n"
         s += f"  #x  {self.numVariables()}\n"
@@ -519,71 +535,75 @@
         if self.x is not None:
             return len(self.x)
         elif self.G is not None:
             return self.G.shape[1]
         elif self.A is not None:
             return self.A.shape[1]
 
-    def toAllNeq(self):
+    def toIneq(self):
         """
         Returns
         -------
         LpStructure
         """
-        return self.toQp().toAllNeq().toLp()
+        return self.toQp().toIneq().toLp()
 
-    def toAllEq(self):
+    def toEq(self):
         """
         Returns
         -------
         LpStructure
         """
-        return self.toQp().toAllEq().toLp()
+        return self.toQp().toEq().toLp()
 
     @classmethod
     def fromFlopt(cls, prob, x=None, option=None, progress=False):
         """
         ::
 
             Problem (flopt) --> QpStructure --> LpStructure
 
         Parameters
         ----------
         prob : Problem
         x : None or list of Variable family
-        option : {"all_neq", "all_eq"}
+        option : {"ineq", "eq"}
         progress : bool
 
         Returns
         -------
         LpStructure
         """
         assert option is None or option in {
-            "all_neq",
-            "all_eq",
-        }, f"option must be None, all_neq or all_eq, but got {option}"
+            "ineq",
+            "eq",
+        }, f"option must be None, ineq or eq, but got {option}"
         qp = QpStructure.fromFlopt(prob, x, progress=progress)
-        if option == "all_neq":
-            return qp.toAllNeq().toLp()
-        elif option == "all_eq":
-            return qp.toAllEq().toLp()
-        else:
-            return qp.toLp()
+        if option == "ineq":
+            return qp.toIneq().toLp()
+        elif option == "eq":
+            return qp.toEq().toLp()
+        return qp.toLp()
 
-    def toFlopt(self):
+    def toFlopt(self, var_name="x"):
         """
         ::
 
             LpStructure --> QpStructure --> Problem (flopt)
 
+        Parameters
+        ----------
+        var_name : str
+            variable prefix
+
         Returns
         -------
         Problem
         """
-        return self.toQp().toFlopt()
+        return self.toQp().toFlopt(var_name)
 
     def toQp(self):
         """
         Returns
         -------
         QpStructure
         """
@@ -624,15 +644,15 @@
         Returns
         -------
         QuboStructure
         """
         assert self.G is None and self.A is None
         return self.toIsing().toQubo()
 
-    def show(self):
+    def show(self, to_str=False):
         s = f"LpStructure\n"
         s += f"obj  c.T.dot(x) + C\n"
         s += f"s.t. Gx <= h\n"
         s += f"     Ax == b\n"
         s += f"     lb <= x <= ub\n\n"
         s += f"#x\n{self.numVariables()}\n\n"
         s += f"c\n{self.c}\n\n"
@@ -640,15 +660,17 @@
         s += f"G\n{self.G}\n\n"
         s += f"h\n{self.h}\n\n"
         s += f"A\n{self.A}\n\n"
         s += f"b\n{self.b}\n\n"
         s += f"lb\n{self.lb}\n\n"
         s += f"ub\n{self.ub}\n\n"
         s += f"x\n{self.x}"
-        return s
+        if to_str:
+            return s
+        print(s)
 
     def __repr__(self):
         return f"LpStructure{self.c, self.C, self.G, self.h, self.A, self.b, self.lb, self.ub, self.types, self.x}"
 
     def __str__(self):
         s = f"LpStructure\n"
         s += f"  #x  {self.numVariables()}\n"
@@ -684,19 +706,29 @@
         elif self.J is not None:
             return self.J.shape[0]
 
     @classmethod
     def fromFlopt(cls, prob, x=None):
         return prob.obj.toIsing()
 
-    def toFlopt(self):
+    def toFlopt(self, var_name="x"):
+        """
+        Parameters
+        ----------
+        var_name : str
+            variable prefix
+
+        Returns
+        -------
+        Problem
+        """
         if self.x is not None:
             x = self.x
         else:
-            x = Variable.array("x", len(self.J), cat="Spin")
+            x = Variable.array(var_name, len(self.J), cat="Spin")
         prob = Problem()
         prob += -x.T.dot(self.J).dot(x) - self.h.T.dot(x) + self.C
         return prob
 
     def toQp(self):
         """
         ::
@@ -745,23 +777,25 @@
             x = None
         else:
             for var in self.x:
                 var.toBinary()
             x = np.array([var.binary for var in self.x], dtype=object)
         return QuboStructure(Q, C, x)
 
-    def show(self):
+    def show(self, to_str=False):
         s = f"IsingStructure\n"
         s += f"- x.T.dot(J).dot(x) - h.T.dot(x) + C\n\n"
         s += f"#x\n{self.numVariables()}\n\n"
         s += f"J\n{self.J}\n\n"
         s += f"h\n{self.h}\n\n"
         s += f"C\n{self.C}\n\n"
         s += f"x\n{self.x}"
-        return s
+        if to_str:
+            return s
+        print(s)
 
     def __repr__(self):
         return f"IsingStructure{self.J, self.h, self.C, self.x}"
 
     def __str__(self):
         s = f"IsingStructure\n"
         s += f"  #x  {self.numVariables()}\n"
@@ -794,24 +828,29 @@
         """
         ::
 
             Problem (flopt) --> IsingStructure --> QuboStructure
         """
         return IsingStructure.fromFlopt(prob, x).toQubo()
 
-    def toFlopt(self):
+    def toFlopt(self, var_name="x"):
         """
+        Parameters
+        ----------
+        var_name : str
+            variable prefix
+
         Returns
         -------
         Problem
         """
         if self.x is not None:
             x = self.x
         else:
-            x = Variable.array("x", len(self.Q), cat="Binary")
+            x = Variable.array(var_name, len(self.Q), cat="Binary")
         prob = Problem()
         prob += (x.T.dot(self.Q).dot(x) + self.C).expand()
         return prob
 
     def toQp(self):
         """
         ::
@@ -844,22 +883,24 @@
 
         Returns
         -------
         IsingStructure
         """
         return self.toFlopt().obj.toIsing()
 
-    def show(self):
+    def show(self, to_str=False):
         s = f"QuboStructure\n"
         s += f"x.T.dot(Q).dot(x) + C\n\n"
         s += f"#x\n{self.numVariables()}\n\n"
         s += f"Q\n{self.Q}\n\n"
         s += f"C\n{self.C}\n\n"
         s += f"x\n{self.x}"
-        return s
+        if to_str:
+            return s
+        print(s)
 
     def __repr__(self):
         return f"QuboStructure{self.Q, self.C, self.x}"
 
     def __str__(self):
         s = f"QuboStructure\n"
         s += f"  #x  {self.numVariables()}\n"
```

### Comparing `flopt-0.5.5/flopt/env.py` & `flopt-0.5.6/flopt/env.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,32 +30,31 @@
     Environment.variable_id += 1
     return var_id
 
 
 def get_variable_lower_bound(to_int=False):
     if to_int:
         return int(Environment.VARIABLE_LOWER_BOUND)
-    else:
-        return Environment.VARIABLE_LOWER_BOUND
+    return Environment.VARIABLE_LOWER_BOUND
 
 
 def get_variable_upper_bound(to_int=False):
     if to_int:
         return int(Environment.VARIABLE_UPPER_BOUND)
-    else:
-        return Environment.VARIABLE_UPPER_BOUND
+    return Environment.VARIABLE_UPPER_BOUND
 
 
 class Environment:
 
     variable_id = 0
     CREATE_VARIABLE_MODE = False
     VARIABLE_LOWER_BOUND = None
     VARIABLE_UPPER_BOUND = None
     TRAINED_MODELS_CONFIG = None
+    FLOPT_SEED = None
 
     SOURCE_DIR = os.path.dirname(__file__)
     DATASETS_DIR = os.path.join(SOURCE_DIR, "..", "datasets")
     PERFORMANCE_DIR = os.path.join(SOURCE_DIR, "..", "performance")
     MODELS_DIR = os.path.join(SOURCE_DIR, "tuning")
 
     root_logger = getLogger()
@@ -74,23 +73,35 @@
         Environment.VARIABLE_UPPER_BOUND = float(
             config["DEFAULT"]["VARIABLE_UPPER_BOUND"]
         )
 
         # download trained model
         Environment.TRAINED_MODELS_CONFIG = config["TRAINED_MODELS"]
 
+        # set seed
+        if "FLOPT_SEED" in os.environ:
+            self.FLOPT_SEED = int(os.environ["FLOPT_SEED"])
+            self.seed(self.FLOPT_SEED)
+
     def setLogLevel(self, log_level):
         if isinstance(log_level, str):
             assert log_level in log_name, f"log level {log_level} is invalid."
             log_level = log_name[log_level]
         self.root_logger.setLevel(log_level)
 
     def getConfig(self, name, section="DEFAULT"):
         return self.config[section][name]
 
+    def seed(self, seed):
+        import random
+        import numpy
+
+        random.seed(seed)
+        numpy.random.seed(seed)
+
 
 def setup_logger(name):
     """Return a logger with a ColoredFormatter."""
     formatter = colorlog.ColoredFormatter(
         "%(log_color)s%(levelname)s:%(filename)s:%(funcName)s:%(message)s",
         datefmt=None,
         reset=True,
```

### Comparing `flopt-0.5.5/flopt/expression.py` & `flopt-0.5.6/flopt/variable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1412 +1,1067 @@
-import weakref
-import functools
-import operator
+import math
+import types
+import random
 import itertools
 
 import numpy as np
 
+import flopt
 from flopt.polynomial import Monomial, Polynomial
+from flopt.container import FloptNdarray
+from flopt.expression import ExpressionElement, Expression, Const
 from flopt.constraint import Constraint
 from flopt.constants import (
     VariableType,
-    ExpressionType,
     ConstraintType,
     number_classes,
     array_classes,
     np_float,
 )
-from flopt.env import setup_logger, get_variable_lower_bound, get_variable_upper_bound
-
-logger = setup_logger(__name__)
-
-
-class SelfReturn:
-    def __init__(self, var):
-        self.var = var
-
-    def value(self):
-        return self.var
-
-
-# ------------------------------------------------
-#   Expression Base Class
-# ------------------------------------------------
-
-
-class ExpressionElement:
-    """Expression Base Class
-
-    Attributes
-    ----------
-    name : str
-    var_dict : None or dict
-    polynomial : None or Polynomial
-    parents : list of ExpressionElement
-    """
-
-    def __init__(self, name=None):
-        self.name = name
-        self.var_dict = None
-        self.polynomial = None
-        self.parents = list()
-
-    def setName(self):
-        raise NotImplementedError
+from flopt.env import (
+    setup_logger,
+    create_variable_mode,
+    is_create_variable_mode,
+    get_variable_id,
+    get_variable_lower_bound,
+    get_variable_upper_bound,
+)
 
-    def getName(self):
-        if self.name is None:
-            self.setName()
-        return self.name
 
-    def linkChildren(self):
-        raise NotImplementedError
+logger = setup_logger(__name__)
 
-    def resetlinkChildren(self):
-        for elm in self.traverse():
-            if isinstance(elm, ExpressionElement):
-                elm.parents = list()
-        self.linkChildren()
-        return self
 
-    def isPolynomial(self):
-        raise NotImplementedError
+# -------------------------------------------------------
+#   Variable and Variable Container Factory
+# -------------------------------------------------------
+
+
+class VariableFactory:
+    """API of variable generation"""
+
+    def checkName(self, name):
+        assert "+" not in name, f"The + character cannot be used in the name."
+        assert "-" not in name, f"The - character cannot be used in the name."
+        assert "*" not in name, f"The * character cannot be used in the name."
+        assert "/" not in name, f"The / character cannot be used in the name."
+        assert "%" not in name, f"The % character cannot be used in the name."
+        assert "^" not in name, f"The ^ character cannot be used in the name."
+        assert "(" not in name, f"The ( character cannot be used in the name."
+        assert ")" not in name, f"The ) character cannot be used in the name."
+        if is_create_variable_mode():
+            assert name.startswith("__"), f"The name must be started with __ characters"
+        else:
+            assert not name.startswith(
+                "__"
+            ), f"The name must not be started with __ characters"
+
+    def __call__(
+        self, name, lowBound=None, upBound=None, cat="Continuous", ini_value=None
+    ):
+        """Create Variable object
 
-    def setPolynomial(self):
-        raise NotImplementedError
+        Parameters
+        ----------
+        name : str
+          name of variable
+        lowBound : float, optional
+          lowBound
+        upBound : float, optional
+          upBound
+        cat : str, optional
+          category of variable
+        ini_value : float, optional
+          set value to variable
 
-    def _value(self):
-        """
         Returns
         -------
-        float or int
-            return value of expression
-        """
-        raise NotImplementedError
+        Variable Family
+          return Variable Family
 
-    def getVariables(self):
-        """
-        Returns
-        -------
-        set
-          return the variable object used in this expressiono
-        """
-        raise NotImplementedError
+        Examples
+        --------
+        Create Integer, Continuous and Binary Variable
 
-    def isNeg(self):
-        """
-        Returns
-        -------
-        bool
-            return if it is - value form else false
+        >>> from flopt import Variable
+        >>> a = Variable(name='a', lowBound=0, upBound=1, cat='Integer')
+        >>> c = Variable(name='c', lowBound=1, upBound=2, cat='Continuous')
+        >>> b = Variable(name='b', cat='Binary')
+        >>> s = Variable(name='s', cat='Spin')
+
+        Create [lowBound, ..., upBound] range permutation variable
+
+        >>> p = Variable(name='p', lowBound=0, upBound=10, cat='Permutation')
+
+        We can see the data of variable, print().
+
+        >>> print(p)
+        >>> Name: p
+        >>> Type    : VarPermutation
+        >>> Value   : [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
+        >>> lowBound: 0
+        >>> upBound : 10
+        """
+        if is_create_variable_mode():
+            assert name is not None
+            name = f"__{get_variable_id()}_" + name
+        self.checkName(name)
+        cat = str(cat)
+        if cat == "Continuous":
+            return VarContinuous(name, lowBound, upBound, ini_value)
+        elif cat == "Integer":
+            return VarInteger(name, lowBound, upBound, ini_value)
+        elif cat == "Binary":
+            if lowBound is not None and lowBound != 0:
+                logger.warning(
+                    f"lowBound of {name} is ignored because its category is Binary"
+                )
+            if upBound is not None and upBound != 1:
+                logger.warning(
+                    f"upBound of {name} is ignored because its category is Binary"
+                )
+            return VarBinary(name, ini_value)
+        elif cat == "Spin":
+            return VarSpin(name, ini_value)
+        elif cat == "Permutation":
+            assert lowBound is not None and upBound is not None
+            return VarPermutation(name, lowBound, upBound, ini_value)
+        else:
+            raise ValueError(f"cat {cat} cannot be used")
+
+    @classmethod
+    def dicts(
+        cls,
+        name,
+        indices=None,
+        lowBound=None,
+        upBound=None,
+        cat=VariableType.Continuous,
+        ini_value=None,
+        index_start=[],
+    ):
         """
-        raise NotImplementedError
-
-    def setVarDict(self, var_dict):
-        self.var_dict = var_dict
-
-    def unsetVarDict(self):
-        self.var_dict = None
-
-    def value(self, solution=None):
-        if solution is None:
-            return self._value()
-        else:
-            self.setVarDict(solution.toDict())
-            return self._value()
-
-    def type(self):
-        if self.isLinear():
-            return ExpressionType.Linear
-        elif self.isQuadratic():
-            return ExpressionType.Quadratic
-        return self._type
-
-    def constant(self):
-        if self.polynomial is not None:
-            return self.polynomial.constant()
-        elif self.isPolynomial():
-            self.setPolynomial()
-            return self.polynomial.constant()
-        else:
-            import sympy
-
-            return float(
-                sympy.sympify(self.getName()).expand().as_coefficients_dict()[1]
-            )
-
-    def isMonomial(self):
-        if self.polynomial is not None:
-            return self.polynomial.isMonomial()
-        elif self.isPolynomial():
-            self.setPolynomial()
-            return self.polynomial.isMonomial()
-        else:
-            return False
-
-    def toMonomial(self):
-        if self.polynomial is None:
-            self.setPolynomial()
-        return self.polynomial.toMonomial()
-
-    def toPolynomial(self):
-        if self.polynomial is None:
-            self.setPolynomial()
-        return self.polynomial
+        Parameters
+        ----------
+        name : str
+          name of variable
+        indices : tuple or generator
+            keys of variable dictionary
+        lowBound : float, optional
+          lowBound
+        upBound : float, optional
+          upBound
+        cat : str, optional
+          category of variable
+        ini_value : float, optional
+          set value to variable
 
-    def isQuadratic(self):
-        """
         Returns
         -------
-        bool
-            return true if this expression is quadratic else false
+        dict
+
         """
-        if self.polynomial is not None:
-            return (
-                self.polynomial.isQuadratic()
-                or self.polynomial.simplify().isQuadratic()
-            )
-        elif self.isPolynomial():
-            self.setPolynomial()
-            return (
-                self.polynomial.isQuadratic()
-                or self.polynomial.simplify().isQuadratic()
+
+        if indices is None:
+            raise TypeError(
+                "LpVariable.dicts missing both 'indices' and deprecated 'indexs' arguments."
             )
-        else:
-            return False
 
-    def toQuadratic(self, x=None):
+        if isinstance(indices, types.GeneratorType):
+            indices = tuple(indices)
+        elif not isinstance(indices, tuple):
+            indices = (indices,)
+
+        index = indices[0]
+        indices = indices[1:]
+        variables = {}
+        if len(indices) == 0:
+            for i in index:
+                if isinstance(i, array_classes):
+                    var_name = f"{name}_" + "_".join(map(str, i))
+                else:
+                    var_name = f"{name}_{i}"
+                variables[i] = Variable(
+                    var_name,
+                    lowBound,
+                    upBound,
+                    cat,
+                    ini_value,
+                )
+        else:
+            for i in index:
+                variables[i] = Variable.dicts(
+                    name, indices, lowBound, upBound, cat, ini_value, index_start + [i]
+                )
+        return variables
+
+    @classmethod
+    def dict(
+        cls, name, keys, lowBound=None, upBound=None, cat="Continuous", ini_value=None
+    ):
         """
         Parameters
         ----------
-        x : list or numpy.array or VarElement family
+        name : str
+          name of variable
+        keys : tuple or generator
+            keys of variable dictionary
+        lowBound : float, optional
+          lowBound
+        upBound : float, optional
+          upBound
+        cat : str, optional
+          category of variable
+        ini_value : float, optional
+          set value to variable
 
         Returns
         -------
-        collections.namedtuple
-            QuadraticStructure('QuadraticStructure', 'Q c C x'),
-            such that 1/2 x^T Q x + c^T x + C, Q^T = Q
-        """
-        assert self.isQuadratic()
-        from flopt.variable import VariableArray
-
-        assert x is None or isinstance(
-            x, VariableArray
-        ), f"x must be None or VariableArray"
-        from flopt.convert import QuadraticStructure
-
-        if self.polynomial is None:
-            self.setPolynomial()
-        polynomial = self.polynomial.simplify()
-        if x is None:
-            x = VariableArray(sorted(self.getVariables(), key=lambda var: var.name))
-
-        num_variables = len(x)
-
-        Q = np.zeros((num_variables, num_variables), dtype=np_float)
-        c = np.zeros((num_variables,), dtype=np_float)
-
-        # set matrix Q and vector c
-        # psude-code
-        # |   if not polynomial.isLinear():
-        # |       for i in range(num_variables):
-        # |           Q[i, i] = 2 * polynomial.coeff(x[i], x[i])
-        # |           for j in range(i+1, num_variables):
-        # |               Q[i, j] = Q[j, i] = polynomial.coeff(x[i], x[j])
-        for mono, coeff in polynomial:
-            if mono.isLinear():
-                c[x.index(mono)] = coeff
-            elif mono.isQuadratic():
-                if len(mono.terms) == 1:
-                    var_a = list(mono.terms)[0]
-                    a_ix = x.index(var_a.toMonomial())
-                    Q[a_ix, a_ix] = 2 * coeff
-                else:
-                    var_a, var_b = list(mono.terms.keys())
-                    a_ix = x.index(var_a.toMonomial())
-                    b_ix = x.index(var_b.toMonomial())
-                    Q[a_ix, b_ix] = Q[b_ix, a_ix] = coeff
+        dict
 
-        C = polynomial.constant()
-        return QuadraticStructure(Q, c, C, x=x)
+        Examples
+        --------
 
-    def isLinear(self):
+        >>> Variable.dict('x', [0, 1])
+        >>> {0: Variable(x_0, cat="Continuous", ini_value=0.0),
+        >>>  1: Variable(x_1, cat="Continuous", ini_value=0.0)}
+        >>>
+        >>> Variable.dict('x', range(2), cat='Binary')
+        >>> {0: Variable(x_0, cat="Binary", ini_value=0),
+        >>>  1: Variable(x_1, cat="Binary", ini_value=0)}
+        >>>
+        >>> Variable.dict('x', (range(2), range(2)), cat='Binary')
+        >>> {(0, 0): Variable(x_0_0, cat="Binary", ini_value=0),
+             (0, 1): Variable(x_0_1, cat="Binary", ini_value=0),
+             (1, 0): Variable(x_1_0, cat="Binary", ini_value=0),
+             (1, 1): Variable(x_1_1, cat="Binary", ini_value=0)}
+        >>>
+        >>> # not work
+        >>> # Variable.dict('x', [range(2), range(2)], cat='Binary')
+
+        """
+        if not isinstance(keys, tuple):
+            iterator = keys
+        else:
+            iterator = itertools.product(*keys)
+        variables = {}
+        for key in iterator:
+            if isinstance(key, (range, types.GeneratorType)):
+                raise ValueError(f"key must not be generator")
+            if isinstance(key, array_classes):
+                var_name = f"{name}_" + "_".join(map(str, key))
+            else:
+                var_name = f"{name}_{key}"
+            variables[key] = Variable(var_name, lowBound, upBound, cat, ini_value)
+        return variables
+
+    def array(
+        self, name, shape, lowBound=None, upBound=None, cat="Continuous", ini_value=None
+    ):
         """
+        Parameters
+        ----------
+        name : str
+          name of variable
+        shape : int of tuple of int
+            shape of array
+        lowBound : number class or array of number class
+          lowBound
+        upBound : number class or array of number class
+          upBound
+        cat : str or array of cat
+          category of variable
+        ini_value : number class or array of number class
+          set value to variable
+
         Returns
         -------
-        bool
-            return true if this expression is linear else false
+        numpy.array
 
         Examples
         --------
-        >>> from flopt import Variable
-        >>> a = Variable('a', ini_value=3)
-        >>> b = Variable('b', ini_value=3)
-        >>> (a+b).isLinear()
-        >>> True
-        >>> (a*b).isLinear()
-        >>> False
-        """
-        if self.polynomial is not None:
-            return self.polynomial.isLinear() or self.polynomial.simplify().isLinear()
-        elif self.isPolynomial():
-            self.setPolynomial()
-            return self.polynomial.isLinear() or self.polynomial.simplify().isLinear()
-        else:
-            return False
 
-    def toLinear(self, x=None):
-        """
+        >>> Variable.array('x', 2, cat='Binary')
+        >>> array([Variable(x_0, cat="Binary", ini_value=0),
+        >>>        Variable(x_1, cat="Binary", ini_value=0)], dtype=object)
+        >>>
+        >>> Variable.array('x', (2, 2), cat='Binary')
+        >>> array([[Variable(x_0_0, cat="Binary", ini_value=0),
+        >>>         Variable(x_0_1, cat="Binary", ini_value=0)],
+        >>>        [Variable(x_1_0, cat="Binary", ini_value=0),
+        >>>         Variable(x_1_1, cat="Binary", ini_value=0)]], dtype=object)
+        """
+        if isinstance(shape, int):
+            shape = (shape,)
+        if isinstance(lowBound, array_classes):
+            lowBound = np.array(lowBound, dtype=np_float)
+        if isinstance(upBound, array_classes):
+            upBound = np.array(upBound, dtype=np_float)
+        if isinstance(cat, array_classes):
+            cat = np.array(cat, dtype=str)
+        if isinstance(ini_value, array_classes):
+            ini_value = np.array(ini_value, dtype=np_float)
+        iterator = itertools.product(*map(range, shape))
+        variables = np.ndarray(shape, dtype=object)
+        digits = [len(str(s)) for s in shape]
+        for i in iterator:
+            var_name = f"{name}_" + "_".join(
+                str(s).zfill(digit) for s, digit in zip(i, digits)
+            )
+            _lowBound = lowBound[i] if isinstance(lowBound, array_classes) else lowBound
+            _upBound = upBound[i] if isinstance(upBound, array_classes) else upBound
+            _cat = cat[i] if isinstance(cat, array_classes) else cat
+            _ini_value = (
+                ini_value[i] if isinstance(ini_value, array_classes) else ini_value
+            )
+            variables[i] = Variable(var_name, _lowBound, _upBound, _cat, _ini_value)
+        return FloptNdarray(variables)
+
+    @classmethod
+    def matrix(
+        cls,
+        name,
+        n_row,
+        n_col,
+        lowBound=None,
+        upBound=None,
+        cat="Continuous",
+        ini_value=None,
+    ):
+        """Overwrap of VariableFactory.array
+
         Parameters
         ----------
-        x: list or numpy.array of VarElement family
+        name : str
+          name of variable
+        n_row : int
+            number of rows
+        n_col : int
+            number of columns
+        lowBound : number class or array of number class
+          lowBound
+        upBound : number class or array of number class
+          upBound
+        cat : str or array of cat
+          category of variable
+        ini_value : number class or array of number class
+          set value to variable
 
         Returns
         -------
-        collections.namedtuple
-            LinearStructure = collections.namedtuple('LinearStructure', 'c C x'),
-            where c.T.dot(x) + C
-        """
-        assert self.isLinear()
-        from flopt.variable import VariableArray
+        numpy.array
 
-        assert x is None or isinstance(
-            x, VariableArray
-        ), f"x must be None or VariableArray"
-        from flopt.convert import LinearStructure
+        Examples
+        --------
 
-        if x is None:
-            x = VariableArray(sorted(self.getVariables(), key=lambda var: var.name))
+        >>> Variable.matrix('x', 2, 2, cat='Binary')
+        >>> array([[Variable(x_0_0, cat="Binary", ini_value=0),
+        >>>         Variable(x_0_1, cat="Binary", ini_value=0)],
+        >>>        [Variable(x_1_0, cat="Binary", ini_value=0),
+        >>>         Variable(x_1_1, cat="Binary", ini_value=0)]], dtype=object)
 
-        num_variables = len(x)
-        if self.polynomial is None:
-            self.setPolynomial()
+        """
+        return Variable.array(name, (n_row, n_col), lowBound, upBound, cat, ini_value)
 
-        c = np.zeros((num_variables,), dtype=np_float)
-        for mono, coeff in self.polynomial:
-            c[x.index(mono)] = coeff
 
-        C = self.polynomial.constant()
-        return LinearStructure(c, C, x=x)
 
-    def isIsing(self):
-        """
-        Returns
-        -------
-        bool
-            return true if this expression is ising else false
-        """
-        if any(
-            var.type() not in {VariableType.Spin, VariableType.Binary}
-            for var in self.getVariables()
-        ):
-            return False
-        return self.isQuadratic()
+# -------------------------------------------------------
+#   Variable Classes
+# -------------------------------------------------------
 
-    def toIsing(self, x=None):
-        """
-        Parameters
-        ----------
-        x : list or numpy.array or VarElement family
 
-        Returns
-        -------
-        collections.namedtuple
-            IsingStructure('IsingStructure', 'J h x'),
-            converted from sum(a_ij x_i x_j; i >= j) + sum(b_i x_i) + c
-            = sum(a_ij x_i x_j; i >= j) + sum(b_i x_i) + sum(c/n x_i x_i),
-            as J_ij = a_ij (i != j), a_ii + c/n (i == j), h_i = b_i
-        """
-        assert self.isIsing()
-        from flopt.convert import IsingStructure
-
-        if any(var.type() == VariableType.Binary for var in self.getVariables()):
-            return self.toSpin().toIsing()
-        quadratic = self.toQuadratic(x)
-        J = -np.triu(quadratic.Q)
-        np.fill_diagonal(J, 0.5 * np.diag(J))
-        return IsingStructure(J, -quadratic.c, quadratic.C, quadratic.x)
+class VarElement:
+    """Base Variable class"""
 
-    def simplify(self):
+    def __init__(self, name, lowBound=None, upBound=None, ini_value=None):
+        self._name = name
+        self.lowBound = lowBound
+        self.upBound = upBound
+        self._value = None
+        if ini_value is not None:
+            self._value = ini_value
+        elif self._type == VariableType.Permutation:
+            self.setRandom()
+        elif self.lowBound is not None and self.upBound is None:
+            self._value = self.lowBound
+        elif self.lowBound is None and self.upBound is not None:
+            self._value = self.upBound
+        else:
+            self.setRandom()
+        self.monomial = Monomial({self: 1})
+
+    def type(self):
         """
         Returns
         -------
-        Expression
+        str
+          return variable type
         """
-        import sympy
-
-        expr = eval(
-            str(sympy.sympify(self.getName()).simplify()),
-            {var.name: var for var in self.getVariables()},
-        )
-        if isinstance(expr, number_classes):
-            expr = Const(expr)
-        return expr
+        return self._type
 
-    def expand(self):
+    def value(self, *args, **kwargs):
         """
         Returns
         -------
-        Expression
+        float or int
+          return value of variable
         """
-        import sympy
+        return self._value
 
-        expr = eval(
-            str(sympy.simplify(self.getName()).expand()),
-            {var.name: var for var in self.getVariables()},
-        )
-        if isinstance(expr, number_classes):
-            expr = Const(expr)
-            return expr
-        elif isinstance(expr, Expression):
-            expr = eval(
-                str(sympy.sympify(expr.getName()).expand()),
-                {var.name: var for var in self.getVariables()},
-            )
-            return expr
-        else:
-            # VarElement family
-            return Expression(expr, Const(0), "+")
+    def setValue(self, value):
+        if isinstance(value, np.ndarray):
+            value = value.item()
+        self._value = value
 
-    def toBinary(self):
-        """create expression replased binary to spin
+    @property
+    def name(self):
+        return self._name
 
-        Returns
-        -------
-        Expression
-        """
-        assert all(
-            var.type() in {VariableType.Binary, VariableType.Spin, VariableType.Integer}
-            for var in self.getVariables()
-        )
-        if all(var.type() == VariableType.Binary for var in self.getVariables()):
-            return self
-        var_dict = {
-            var.name: SelfReturn(
-                var.toBinary()
-                if var.type() in {VariableType.Spin, VariableType.Integer}
-                else var
+    def getName(self):
+        return self._name
+
+    def getLb(self, number=False):
+        if number:
+            return (
+                self.lowBound
+                if self.lowBound is not None
+                else get_variable_lower_bound(to_int=True)
             )
-            for var in self.getVariables()
-        }
-        self.setVarDict(var_dict)
-        return self.value().expand()
+        return self.lowBound
 
-    def toSpin(self):
-        """create expression replased binary to spin
+    def getUb(self, number=False):
+        if number:
+            return (
+                self.upBound
+                if self.upBound is not None
+                else get_variable_upper_bound(to_int=True)
+            )
+        return self.upBound
 
+    def feasible(self):
+        """
         Returns
         -------
-        Expression
+        bool
+          return true if value of self is in between lowBound and upBound else false
         """
-        assert all(
-            var.type() in {VariableType.Binary, VariableType.Spin, VariableType.Integer}
-            for var in self.getVariables()
+        return (
+            self.getLb(number=True) <= self._value <= self.getUb(number=True)
         )
-        if all(var.type() == VariableType.Spin for var in self.getVariables()):
-            return self
-        var_dict = {
-            var.name: SelfReturn(
-                var.toSpin()
-                if var.type() in {VariableType.Binary, VariableType.Integer}
-                else var
-            )
-            for var in self.getVariables()
-        }
-        self.setVarDict(var_dict)
-        return self.value().expand()
 
-    def __calculate(self, sense, default_value):
-        """Calculate min/max value of expression
+    def clip(self):
+        """
+        map in an feasible area by clipping.
+        ex. value < lowBound -> value = lowBound,
+        value > upBound  -> value = upBound
+        """
+        if self.getLb() is not None:
+            lb = self.getLb(number=True)
+            self._value = max(self._value, lb)
+        if self.getUb() is not None:
+            ub = self.getUb(number=True)
+            self._value = min(self._value, ub)
 
-        Parameters
-        ----------
-        sense : str
-        default_value : default value of excepsion case
+    def getVariables(self):
+        return {self}
 
-        Returns
-        -------
-        float
-            value of this expression can take
-        """
-        import flopt
+    def isPolynomial(self):
+        return True
 
-        if self.isLinear():
-            solver = flopt.Solver("ScipyMilpSearch")
-        elif self.isQuadratic():
-            solver = flopt.Solver("CvxoptQpSearch")
-        else:
-            logger.warning(
-                f"{sense} value of {self.getName()} cannot be calculated because it is not linear or quaratic"
-            )
-            return default_value
-        prob = flopt.Problem(sense=sense)
-        prob += self
-        status, logs = prob.solve(solver, msg=False)
-        if status == flopt.SolverTerminateState.Normal:
-            return prob.getObjectiveValue()
-        elif status == flopt.SolverTerminateState.Unbounded:
-            logger.warning(
-                f"{sense} value of {self.getName()} cannot be calculated because it is unbounded"
-            )
-            return default_value
-        else:
-            logger.warning(
-                f"{sense} value of {self.getName()} cannot be calculated by any reasons"
-            )
-            return default_value
+    def toMonomial(self):
+        return self.monomial
 
-    def max(self):
-        """Calculate max value of expression when expression is linear or quadratic
+    @property
+    def polynomial(self):
+        return self.toPolynomial()
 
-        Returns
-        -------
-        float
-            maximum value of this expression can take
-        """
-        return self.__calculate("Maximize", get_variable_upper_bound())
+    def toPolynomial(self):
+        return Polynomial({self.monomial: 1})
 
-    def min(self):
-        """Calculate min value of expression when expression is linear or quadratic
+    def isLinear(self):
+        return True
 
-        Returns
-        -------
-        float
-            minimum value of this expression can take
-        """
-        return self.__calculate("Minimize", get_variable_lower_bound())
+    def isQuadratic(self):
+        return True
 
-    def traverse(self):
-        """traverse Expression tree as root is self
+    def setRandom(self):
+        """set random value to variable"""
+        raise NotImplementedError()
 
-        Yield
-        -----
-        Expression or VarElement
-        """
+    def clone(self, *args, **kwargs):
+        raise NotImplementedError()
+
+    def max(self):
+        if self.upBound is not None:
+            return self.upBound
+        return get_variable_upper_bound()
+
+    def min(self):
+        if self.lowBound is not None:
+            return self.lowBound
+        return get_variable_lower_bound()
+
+    def traverse(self):
         yield self
 
     def traverseAncestors(self):
-        """traverse ancestors of self
-
-        Yield
-        -----
-        Expression or VarElement
-        """
-        for parent in self.parents:
-            yield parent
-            yield from parent.traverseAncestors()
+        raise NotImplementedError
 
     def __add__(self, other):
         if isinstance(other, number_classes):
             if other == 0:
                 return self
             return Expression(self, Const(other), "+")
+        elif isinstance(other, VarElement):
+            return Expression(self, other, "+")
         elif isinstance(other, ExpressionElement):
             if other.isNeg():
                 # self + (-other) --> self - other
                 return Expression(self, other.elmB, "-")
             else:
                 return Expression(self, other, "+")
-        else:
-            return NotImplemented
+        return NotImplemented
 
     def __radd__(self, other):
         if isinstance(other, number_classes):
             if other == 0:
                 return self
             return Expression(Const(other), self, "+")
-        else:
-            return NotImplemented
+        elif isinstance(other, (VarElement, ExpressionElement)):
+            return Expression(other, self, "+")
+        return NotImplemented
 
     def __sub__(self, other):
         if isinstance(other, number_classes):
             if other == 0:
                 return self
             elif other < 0:
                 return Expression(self, Const(-other), "+")
             else:
                 return Expression(self, Const(other), "-")
+        elif isinstance(other, VarElement):
+            return Expression(self, other, "-")
         elif isinstance(other, ExpressionElement):
             if other.isNeg() and isinstance(other, Expression):
-                # self - (-1*other) -> self + other
+                # self - (-1*other) --> self + other
                 return Expression(self, other.elmB, "+")
             return Expression(self, other, "-")
-        else:
-            return NotImplemented
+        return NotImplemented
 
     def __rsub__(self, other):
         if isinstance(other, number_classes):
             if other == 0:
                 # 0 - self --> -1 * self
                 return -self
             else:
                 return Expression(Const(other), self, "-")
-        else:
-            return NotImplemented
+        elif isinstance(other, (VarElement, ExpressionElement)):
+            return Expression(other, self, "-")
+        return NotImplemented
 
     def __mul__(self, other):
         if isinstance(other, number_classes):
             if other == 0:
-                return Const(0)
+                return 0
             elif other == 1:
                 return self
             elif other == -1:
                 return -self
             return Expression(Const(other), self, "*")
-        elif isinstance(other, ExpressionElement):
+        elif isinstance(other, VarElement):
             return Expression(self, other, "*")
-        else:
-            return NotImplemented
+        elif isinstance(other, ExpressionElement):
+            if isinstance(other, Expression):
+                if other.operator == "*" and isinstance(other.elmA, Const):
+                    # self * (a*other) -> a * (self * other)
+                    return other.elmA * Expression(self, other.elmB, "*")
+                else:
+                    return Expression(other, self, "*")
+            return Expression(other, self, "*")
+        return NotImplemented
 
     def __rmul__(self, other):
         if isinstance(other, number_classes):
             if other == 0:
-                return Const(0)
+                return 0
             elif other == 1:
                 return self
+            elif other == -1:
+                return -self
             return Expression(Const(other), self, "*")
         elif isinstance(other, ExpressionElement):
+            if isinstance(other, Expression):
+                if other.operator == "*" and isinstance(other.elmA, Const):
+                    # (a*other) * self -> a * (self * other)
+                    return other.elmA * Expression(other.elmB, self, "*")
+                else:
+                    return Expression(other, self, "*")
             return Expression(other, self, "*")
-        else:
-            return NotImplemented
+        return NotImplemented
 
     def __truediv__(self, other):
         if isinstance(other, number_classes):
             if other == 1:
                 return self
+            elif other == -1:
+                return -self
             return Expression(self, Const(other), "/")
-        elif isinstance(other, ExpressionElement):
+        elif isinstance(other, (VarElement, ExpressionElement)):
             return Expression(self, other, "/")
-        else:
-            return NotImplemented
+        return NotImplemented
 
     def __rtruediv__(self, other):
         if isinstance(other, number_classes):
             if other == 0:
-                return Const(0)
+                return 0
             return Expression(Const(other), self, "/")
-        else:
-            return NotImplemented
+        elif isinstance(other, (VarElement, ExpressionElement)):
+            return Expression(other, self, "/")
+        return NotImplemented
+
+    def __mod__(self, other):
+        if isinstance(other, int):
+            return Expression(self, Const(other), "%")
+        elif isinstance(other, (VarInteger, ExpressionElement)):
+            return Expression(self, other, "%")
+        raise NotImplementedError()
 
     def __pow__(self, other):
         if isinstance(other, number_classes):
-            if other == 1:
+            if other == 0:
+                return 1
+            elif other == 1:
                 return self
             return Expression(self, Const(other), "^")
-        elif isinstance(other, ExpressionElement):
+        elif isinstance(other, (VarElement, ExpressionElement)):
             return Expression(self, other, "^")
-        else:
-            return NotImplemented
+        return NotImplemented
 
     def __rpow__(self, other):
         if isinstance(other, number_classes):
             if other == 1:
-                return Const(1)
+                return 1
             return Expression(Const(other), self, "^")
-        else:
-            return NotImplemented
-
-    def __and__(self, other):
-        if isinstance(other, number_classes):
-            return Expression(self, Const(other), "&")
-        elif isinstance(other, ExpressionElement):
-            return Expression(self, other, "&")
-        else:
-            return NotImplemented
-
-    def __rand__(self, other):
-        return self & other
-
-    def __or__(self, other):
-        if isinstance(other, number_classes):
-            return Expression(self, Const(other), "|")
-        elif isinstance(other, ExpressionElement):
-            return Expression(self, other, "|")
-        else:
-            return NotImplemented
-
-    def __ror__(self, other):
-        return self | other
-
-    def __neg__(self):
-        # -1 * self
-        return Expression(Const(-1), self, "*", name=f"-({self.getName()})")
+        elif isinstance(other, (VarElement, ExpressionElement)):
+            return Expression(other, self, "^")
+        return NotImplemented
 
     def __abs__(self):
-        return abs(self.value())
+        return abs(self._value)
 
     def __int__(self):
-        return int(self.value())
+        return int(self._value)
 
     def __float__(self):
-        return float(self.value())
+        return float(self._value)
+
+    def __neg__(self):
+        # -1 * self
+        return Expression(Const(-1), self, "*", name=f"-{self.name}")
 
     def __pos__(self):
         return self
 
     def __hash__(self):
-        if (
-            self.operator == "+"
-            and isinstance(self.elmB, number_classes)
-            and self.elmB == 0
-        ):
-            # a + 0
-            return hash(self.elmA)
-        elif (
-            self.operator == "-"
-            and isinstance(self.elmB, number_classes)
-            and self.elmB == 0
-        ):
-            # a - 0
-            return hash(self.elmA)
-        elif (
-            self.operator == "*"
-            and isinstance(self.elmA, number_classes)
-            and self.elmA == 1
-        ):
-            # 1 * b
-            return hash(self.elmB)
-        else:
-            return hash((hash(self.elmA), hash(self.elmB), hash(self.operator)))
+        return hash(self.name)
 
     def __eq__(self, other):
         # self == other --> self - other == 0
+        if isinstance(other, (number_classes)) and other == 0:
+            return Constraint(
+                Expression(self, Const(0), "+", name=self.name) - other,
+                ConstraintType.Eq,
+            )
         return Constraint(self - other, ConstraintType.Eq)
 
     def __le__(self, other):
         # self <= other --> self - other <= 0
+        if isinstance(other, (number_classes)) and other == 0:
+            return Constraint(
+                Expression(self, Const(0), "+", name=self.name), ConstraintType.Le
+            )
         return Constraint(self - other, ConstraintType.Le)
 
     def __ge__(self, other):
         # self >= other --> other - self <= 0
         return Constraint(other - self, ConstraintType.Le)
 
-    def __repr__(self):
-        raise NotImplementedError
-
-
-# ------------------------------------------------
-#   Expression Class
-# ------------------------------------------------
-
-
-class Expression(ExpressionElement):
-    """Expression Base Class
-
-    This represents the operation of two items
-    elmA (operator) elmB
-
-    Parameters
-    ----------
-    elmA : Variable family or Expression family
-      first element
-    elmB : Variable family or Expression family
-      later element
-    operator : str
-      operator between elmA and elmB
-
-    Attributes
-    ----------
-    elmA : Variable family or Expression family
-      first element
-    elmB : Variable family or Expression family
-      later element
-    operator : str
-      operator between elmA and elmB
-
-    Examples
-    --------
-
-    .. code-block:: python
+    def __str__(self):
+        return self.name
 
-        a = Variable(name="a", ini_value=1, cat="Integer")
-        b = Variable(name="b", ini_value=2, cat="Continuous")
-        c = Expression(a, b, "+")
-        >>> print(c)
-        >>> Name: a+b
-             Type    : Expression
-             Value   : 3
-        c.value()
-        >>> 3
-        c.getVariables()
-        >>> {VarElement("b", 1, 2, 2), VarElement("a", 0, 1, 1)}
-
-    operator "+", "-", "*", "/", "^" and "%" are supported for Integer, Binary and
-    Continuous Variables.
-
-    .. code-block:: python
-
-        a = Variable(name="a", ini_value=1, cat="Integer")  # a.value() is 1
-        b = Variable(name="b", ini_value=2, cat="Continuous")  # b.value() is 2
-        Expression(a, b, "+").value()  # a+b addition
-        >>> 3
-        Expression(a, b, "-").value()  # a-b substraction
-        >>> -1
-        Expression(a, b, "*").value()  # a*b multiplication
-        >>> 2
-        Expression(a, b, "/").value()  # a/b division
-        >>> 0.5
-        Expression(a, b, "^").value()  # a/b division
-        >>> 1
-        Expression(a, b, "%").value()  # a%b modulo
-        >>> 1
-
-    operator "&", "|" are supported for Binary Variable.
-
-    .. code-block:: python
-
-        a = Variable(name="a", ini_value=1, cat="Binary")
-        b = Variable(name="b", ini_value=0, cat="Binary")
-        Expression(a, b, "&").value().value()  # a&b bitwise and
-        >>> 0
-        Expression(a, b, "|").value().value()  # a&b bitwise or
-        >>> 1
-    """
+    def __repr__(self):
+        return f'VarElement("{self.name}", {self.lowBound}, {self.upBound}, {self.value()})'
 
-    _type = ExpressionType.Unknown
 
-    def __init__(self, elmA, elmB, operator, name=None):
-        self.elmA = elmA
-        self.elmB = elmB
-        self.operator = operator
-        super().__init__(name=name)
-
-    def setName(self):
-        elmA_name = self.elmA.getName()
-        elmB_name = self.elmB.getName()
-        if isinstance(self.elmA, (Expression, Reduction)):
-            if self.operator in {"*", "/", "^", "%"}:
-                elmA_name = f"({elmA_name})"
-        if isinstance(self.elmB, Expression):
-            if self.operator != "+" or self.elmB.getName().startswith("-"):
-                elmB_name = f"({elmB_name})"
-        elif isinstance(self.elmB, Reduction):
-            elmB_name = f"({elmB_name})"
-        self.name = f"{elmA_name}{self.operator}{elmB_name}"
-
-    def linkChildren(self):
-        if isinstance(self.elmA, ExpressionElement):
-            self.elmA.parents.append(self)
-            self.elmA.linkChildren()
-        if isinstance(self.elmB, ExpressionElement):
-            self.elmB.parents.append(self)
-            self.elmB.linkChildren()
+class VarInteger(VarElement):
+    """Integer Variable"""
 
-    def isPolynomial(self):
-        return (
-            self.elmA.isPolynomial()
-            and self.elmB.isPolynomial()
-            and (
-                self.operator == "+"
-                or self.operator == "-"
-                or self.operator == "*"
-                or self.operator == "^"
-            )
-        )
+    _type = VariableType.Integer
 
-    def setPolynomial(self):
-        if self.operator == "+":
-            self.polynomial = self.elmA.toPolynomial() + self.elmB.toPolynomial()
-        elif self.operator == "-":
-            self.polynomial = self.elmA.toPolynomial() - self.elmB.toPolynomial()
-        elif self.operator == "*":
-            self.polynomial = self.elmA.toPolynomial() * self.elmB.toPolynomial()
-        elif (
-            self.operator == "^"
-            and isinstance(self.elmB, Const)
-            and isinstance(self.elmB.value(), int)
-        ):
-            self.polynomial = self.elmA.toPolynomial() ** self.elmB.value()
-        else:
-            assert "check whethere this expresson is polynomial or not by .isPolynomial() before execution of setPolynomial()"
+    def __init__(self, name, lowBound, upBound, ini_value):
+        lowBound = lowBound if lowBound is None else math.ceil(lowBound)
+        upBound = upBound if upBound is None else math.floor(upBound)
+        super().__init__(name, lowBound, upBound, ini_value)
+        self.binarized = None
+        self.binaries = set()
 
-    def _value(self):
+    def value(self, *args, **kwargs):
         """
         Returns
         -------
         float or int
-            return value of expression
+          return value of variable
         """
-        elmA = self.elmA
-        elmB = self.elmB
-        if self.var_dict is not None:
-            if isinstance(self.elmA, ExpressionElement):
-                self.elmA.setVarDict(self.var_dict)
-            elif self.elmA.name in self.var_dict:
-                elmA = self.var_dict[self.elmA.name]
-            if isinstance(self.elmB, ExpressionElement):
-                self.elmB.setVarDict(self.var_dict)
-            elif self.elmB.name in self.var_dict:
-                elmB = self.var_dict[self.elmB.name]
-            self.unsetVarDict()
-
-        if self.operator == "+":
-            return elmA.value() + elmB.value()
-        elif self.operator == "-":
-            return elmA.value() - elmB.value()
-        elif self.operator == "*":
-            return elmA.value() * elmB.value()
-        elif self.operator == "/":
-            return elmA.value() / elmB.value()
-        elif self.operator == "^":
-            return elmA.value() ** elmB.value()
-        elif self.operator == "%":
-            return elmA.value() % elmB.value()
-        elif self.operator == "&":
-            return elmA.value() & elmB.value()
-        elif self.operator == "|":
-            return elmA.value() | elmB.value()
+        return round(self._value)
 
-    def getVariables(self):
-        return self.elmA.getVariables() | self.elmB.getVariables()
+    def getLb(self, number=False):
+        if number:
+            return (
+                self.lowBound
+                if self.lowBound is not None
+                else get_variable_lower_bound(to_int=True)
+            )
+        return self.lowBound
 
-    def traverse(self):
-        yield self
-        yield from self.elmA.traverse()
-        yield from self.elmB.traverse()
+    def getUb(self, number=False):
+        if number:
+            return (
+                self.upBound
+                if self.upBound is not None
+                else get_variable_upper_bound(to_int=True)
+            )
+        return self.upBound
 
-    def isNeg(self):
-        return (
-            self.operator == "*"
-            and isinstance(self.elmA, Const)
-            and self.elmA.value() == -1
-        )
+    def setRandom(self):
+        lb = self.getLb(number=True)
+        ub = self.getUb(number=True)
+        self._value = random.randint(lb, ub)
 
-    def __mul__(self, other):
-        if isinstance(other, number_classes):
-            if other == 0:
-                return Const(0)
-            elif other == 1:
-                return self
-            elif other == -1:
-                return -self
-            return Expression(Const(other), self, "*")
-        elif isinstance(other, Expression):
-            if self.operator == "*" and isinstance(self.elmA, Const):
-                if other.operator == "*" and isinstance(other.elmA, Const):
-                    # (a*self) * (b*other) --> a * b * (self*other)
-                    return (
-                        self.elmA * other.elmA * Expression(self.elmB, other.elmB, "*")
-                    )
-                else:
-                    # (a*self) * other --> a * (self*other)
-                    return self.elmA * Expression(self.elmB, other, "*")
-            else:
-                if other.operator == "*" and isinstance(other.elmA, Const):
-                    # self * (b*other) --> b * (self*other)
-                    return other.elmA * Expression(self, other.elmB, "*")
-                else:
-                    return Expression(self, other, "*")
-        elif isinstance(other, CustomExpression):
-            return Expression(self, other, "*")
-        else:
-            return NotImplemented
+    def toBinary(self):
+        if self.binarized is None:
+            l, u = int(self.getLb()), int(self.getUb())
+            with create_variable_mode():
+                self.binaries = Variable.array(
+                    f"__bin_{self.name}", u - l + 1, cat="Binary"
+                )
+            self.binarized = flopt.Sum(
+                Const(i) * var_bin for i, var_bin in zip(range(l, u + 1), self.binaries)
+            )
+            if isinstance(self.binarized, VarElement):
+                self.binarized = Expression(self.binarized, Const(0), "+")
+        return self.binarized
+
+    def getBinaries(self):
+        if self.binarized is None:
+            self.toBinary()
+        return self.binaries
 
-    def __rmul__(self, other):
-        if isinstance(other, number_classes):
-            if other == 0:
-                return Const(0)
-            elif other == 1:
-                return self
-            return Expression(Const(other), self, "*")
-        else:
-            return NotImplemented
+    def toSpin(self):
+        return self.toBinary().toSpin()
 
-    def __str__(self):
-        return self.getName()
+    def clone(self):
+        """
+        Parameters
+        ----------
+        variable_clone : bool
+            if it is true, return a cloned variable
+        """
+        return VarInteger(self.name, self.lowBound, self.upBound, self._value)
 
-    def __repr__(self):
-        s = f"Expression({self.elmA.getName()}, {self.elmB.getName()}, {self.operator})"
-        return s
+    def __and__(self, other):
+        if isinstance(other, number_classes):
+            other = Const(other)
+        return Expression(self, other, "&")
 
-    def __del__(self):
-        if isinstance(self.elmA, Const):
-            del self.elmA
-        if isinstance(self.elmB, Const):
-            del self.elmB
-
-
-# ------------------------------------------------
-#   CustomExpression Class
-# ------------------------------------------------
-
-
-def unpack_variables(var_or_array):
-    variables = set()
-    if isinstance(var_or_array, array_classes):
-        array = var_or_array
-        for var in array:
-            variables |= unpack_variables(var)
-    else:
-        var = var_or_array
-        variables.add(var)
-    return variables
-
-
-def pack_variables(var_or_array, var_dict):
-    if isinstance(var_or_array, array_classes):
-        cls = var_or_array.__class__
-        array = var_or_array
-        import flopt.variable
+    def __rand__(self, other):
+        if isinstance(other, number_classes):
+            other = Const(other)
+        return Expression(other, self, "&")
 
-        if isinstance(array, flopt.variable.VariableArray):
-            return array.to_value(var_dict)
-        else:
-            return cls(
-                itertools.starmap(pack_variables, [(var, var_dict) for var in array])
-            )
-    else:
-        var = var_or_array
-        return var_dict[var.name].value()
+    def __or__(self, other):
+        if isinstance(other, number_classes):
+            other = Const(other)
+        return Expression(self, other, "|")
 
+    def __ror__(self, other):
+        if isinstance(other, number_classes):
+            other = Const(other)
+        return Expression(other, self, "|")
 
-class CustomExpression(ExpressionElement):
-    """Objective function from using user defined function.
-
-    Parameters
-    ----------
-    func : function
-      objective function
-    arg: list of variables
+    def __repr__(self):
+        return f'Variable("{self.name}", {self.lowBound}, {self.upBound}, "Integer", {self.value()})'
 
-    Examples
-    --------
 
-    We have the objective funcion :math:`simulater(a, b)` where simulater is
-    a black box function, a and b are continuous variable.
-    In this case, we can input objective function into Problem
-    by using CustomExpression as follows.
-
-    .. code-block:: python
-
-      a = Variable("a", cat="Continuous")
-      b = Variable("b", cat="Continuous")
-      def user_simulater(a, b):
-          return simulater(a, b)
-      obj = CustomExpression(func=user_simulater, arg=[a, b])
-      prob = Problem("simulater")
-      prob += obj
+class VarBinary(VarInteger):
+    """Binary Variable
 
     .. note::
+      Binary Variable behaves differently in "-" and "~" operation.
 
-      The order of variables in arg parameter must be the same as
-      the func argument. (However even the name does not have to be the same.)
+      "-" is the subtraction as interger variable, and
+      "~" is the inversion as binary (bool) variable.
 
-    In addition, we can use some operations ("+", "-", "*", "/") between CustomExpression and
-    Variable, Expression and CustomExpression.
-
-    >>> def user_func(x):
-    >>>     return x
-    >>> a = Variable('a', ini_value=3)
-    >>> obj = CustomExpression(user_func, [a])
-    >>> obj.value()
-    >>> 3
-
-    For example,
-
-    >>> b = Variable('b', ini_value=1)
-    >>> obj_b = obj + b  # 3+1
-    >>> obj_b.value()
-    >>> 4
-    >>> obj_b.getVariables()
-    >>> [VarElement("a", -10000000000.0, 10000000000.0, 3),
-         VarElement("b", -10000000000.0, 10000000000.0, 1)]
-
-    See Also
-    --------
-    flopt.expression.Expression
+      >>> a = Variable('a', intValue=1, cat='Binary')
+      >>> a.value()
+      >>> 1
+      >>> (-a).value()
+      >>> -1
+      >>> (~a).value()
+      >>> 0
     """
 
-    _type = ExpressionType.Custom
+    _type = VariableType.Binary
 
-    def __init__(self, func, arg, name=None):
-        self.func = func
-        self.arg = arg
-        self.variables = unpack_variables(arg)
-        super().__init__(name=name)
+    def __init__(self, name, ini_value=None, spin=None):
+        super().__init__(name, 0, 1, ini_value)
+        self.spin = spin
 
-    def setName(self):
-        self.name = f"{self.func.__name__}(*)"
-
-    def linkChildren(self):
-        return
-
-    def isPolynomial(self):
-        return False
+    def setValue(self, value):
+        self._value = value
+        if self.spin is not None:
+            self.spin._value = 2 * value - 1
 
-    def setPolynomial(self):
-        self.polynomial = None
+    def setRandom(self):
+        self._value = random.randint(0, 1)
 
-    def _value(self):
-        if self.var_dict is None:
-            arg = self.arg
-        else:
-            arg = pack_variables(self.arg, self.var_dict)
+    def toBinary(self):
+        return self
 
-        value = self.func(*arg)
-        if not isinstance(value, number_classes):
-            value = value.value()
+    def toSpin(self):
+        """
+        Returns
+        -------
+        Expression
 
-        self.unsetVarDict()
-        return value
+        Notes
+        -----
+        to convert Spin expression
+        {0, 1} to {-1, 1}
+        """
+        if self.spin is None:
+            with create_variable_mode():
+                self.spin = VarSpin(
+                    f"{self.name}_s",
+                    ini_value=int(2 * self._value - 1),
+                    binary=self,
+                )
+        return (self.spin + 1) * 0.5
 
-    def getVariables(self):
-        return self.variables
+    def clone(self):
+        return VarBinary(self.name, self._value, self.spin)
 
-    def isNeg(self):
-        return False
+    def __mul__(self, other):
+        if id(other) == id(self):
+            # a * a = a
+            return self
+        elif isinstance(other, ExpressionElement) and other.operator == "*":
+            if id(other.elmA) == id(self) or id(other.elmB) == id(self):
+                # a * (a * b) = a * b
+                # a * (b * a) = b * a
+                return other
+        return super().__mul__(other)
 
-    def __hash__(self):
-        tmp = [hash(self.func)]
-        for var in self.variables:
-            tmp.append(hash(var))
-        return hash(tuple(tmp))
+    def __pow__(self, other):
+        if isinstance(other, int):
+            return self
+        return super().__pow__(other)
 
-    def __str__(self):
-        return f"{self.func.__name__}(*)"
+    def __invert__(self):
+        # 1 -> 0
+        # 0 -> 1
+        return Expression(Const(1), self, "-")
 
     def __repr__(self):
-        return f"CustomExpression({self.func.__name__, self.arg, self.getName()})"
+        return f'Variable("{self.name}", cat="Binary", ini_value={self.value()})'
 
 
-class Const(ExpressionElement):
-    """
-    It is the expression of constant value.
+class VarSpin(VarElement):
+    """Spin Variable, which takes only 1 or -1"""
 
-    Parameters
-    ----------
-    value : int or float
-      value
-    name : str or None
-        name of constant
-    """
+    _type = VariableType.Spin
 
-    _type = ExpressionType.Const
+    def __init__(self, name, ini_value, binary=None):
+        super().__init__(name, -1, 1, ini_value)
+        self.binary = binary
 
-    def __init__(self, value, name=None):
-        if name is None:
-            name = f"{value}"
-        if isinstance(value, Const):
-            value = value._value
+    def setValue(self, value):
         self._value = value
-        super().__init__(name=name)
-
-    def setName(self):
-        return NotImplemented
-
-    def linkChildren(self):
-        return
-
-    def setPolynomial(self):
-        self.polynomial = Polynomial(constant=self._value)
-
-    def _value(self):
-        return NotImplemented
-
-    def getVariables(self):
-        return set()
-
-    def isNeg(self):
-        return self._value < 0
-
-    def value(self, *args, **kwargs):
-        return self._value
-
-    def constant(self):
-        return self._value
-
-    def isMonomial(self):
-        return True
-
-    def toMonomial(self):
-        return Monomial(coeff=self._value)
-
-    def isPolynomial(self):
-        return True
-
-    def toPolynomial(self):
-        return Polynomial(constant=self._value)
+        if self.binary is not None:
+            self.binary._value = int((value + 1) / 2)
 
-    def isQuadratic(self):
-        return True
-
-    def toQuadratic(self, x=None):
-        return Expression(Const(0), Const(0), "+").toQuadratic(x)
+    def feasible(self):
+        """
+        Returns
+        -------
+        bool
+          return true if value of self is 1 or -1 else false
+        """
+        return self._value in {-1, 1}
 
-    def isLinear(self):
-        return True
+    def setRandom(self):
+        """set random value to variable"""
+        self._value = random.choice([-1, 1])
 
-    def toLinear(self, x=None):
-        return Expression(Const(0), Const(0), "+").toLinear(x)
+    def toBinary(self):
+        """
+        Returns
+        -------
+        Expression
 
-    def isIsing(self):
-        return True
+        Notes
+        -----
+        to convert Binary expression
+        {-1, 1} to {0, 1}
+        """
+        if self.binary is None:
+            with create_variable_mode():
+                self.binary = VarBinary(
+                    f"{self.name}_b",
+                    ini_value=int((self._value + 1) / 2),
+                    spin=self,
+                )
+        return 2 * self.binary - 1
 
-    def simplify(self):
+    def toSpin(self):
         return self
 
-    def expand(self, *args, **kwargs):
-        return self
-
-    def __add__(self, other):
-        if isinstance(other, number_classes):
-            return Const(self._value + other)
-        return self._value + other
-
-    def __radd__(self, other):
-        return self + other
-
-    def __sub__(self, other):
-        if isinstance(other, number_classes):
-            return Const(self._value - other)
-        return self._value - other
-
-    def __rsub__(self, other):
-        if isinstance(other, number_classes):
-            return Const(other - self._value)
-        if self._value < 0:
-            return other + (-self)
-        else:
-            return other - self._value
+    def clone(self):
+        return VarSpin(self.name, self._value, self.binary)
 
     def __mul__(self, other):
-        if isinstance(other, number_classes):
-            return Const(self._value * other)
-        return self._value * other
+        if id(other) == id(self):
+            return 1
+        elif isinstance(other, ExpressionElement) and other.operator == "*":
+            if id(other.elmA) == id(self):
+                # a * (a * b) = b
+                if isinstance(other.elmB, number_classes):
+                    return other.elmB
+                else:
+                    return other.elmB
+            elif id(other.elmB) == id(self):
+                # a * (b * a) = b
+                if isinstance(other.elmA, number_classes):
+                    return other.elmA
+                else:
+                    return other.elmA
+        return super().__mul__(other)
 
     def __rmul__(self, other):
-        return self * other
-
-    def __truediv__(self, other):
-        if isinstance(other, number_classes):
-            return Const(self._value / other)
-        return self._value / other
-
-    def __rtruediv__(self, other):
-        return self / other
+        if id(other) == id(self):
+            return 1
+        elif isinstance(other, ExpressionElement) and other.operator == "*":
+            if id(other.elmA) == id(self):
+                # (a * b) * a = b
+                if isinstance(other.elmB, number_classes):
+                    return other.elmB
+                else:
+                    return other.elmB
+            elif id(other.elmB) == id(self):
+                # (b * a) * a = b
+                if isinstance(other.elmA, number_classes):
+                    return other.elmA
+                else:
+                    return other.elmA
+        return super().__rmul__(other)
 
     def __pow__(self, other):
-        if isinstance(other, number_classes):
-            return Const(self._value**other)
-        return self._value**other
-
-    def __rpow__(self, other):
-        return self**other
-
-    def __neg__(self):
-        return Const(-self._value)
-
-    def __hash__(self):
-        return hash((self._value, self._type))
+        if isinstance(other, int):
+            if other % 2 == 0:
+                return 1
+            else:
+                return self
+        return super().__pow__(other)
 
-    def __str__(self):
-        return str(self._value)
+    def __invert__(self):
+        # -self
+        return self.__neg__()
 
     def __repr__(self):
-        s = f"Const({self._value})"
-        return s
-
-
-# ------------------------------------------------
-#   Utilities
-# ------------------------------------------------
-to_value_ufunc = np.frompyfunc(lambda x: x.value(), 1, 1)
-
+        return f'Variable("{self.name}", cat="Spin", ini_value={self._value})'
 
-def to_const(x):
-    if isinstance(x, number_classes):
-        return Const(x)
-    return x
 
+class VarContinuous(VarElement):
+    """Continuous Variable"""
 
-to_const_ufunc = np.frompyfunc(to_const, 1, 1)
+    _type = VariableType.Continuous
 
+    def setRandom(self):
+        lb = self.getLb(number=True)
+        ub = self.getUb(number=True)
+        self._value = random.uniform(lb, ub)
 
-# ------------------------------------------------
-#   Reduction Class
-# ------------------------------------------------
-class Reduction(ExpressionElement):
+    def clone(self):
+        return VarContinuous(self.name, self.lowBound, self.upBound, self._value)
 
-    _type = ExpressionType.Unknown
-
-    def __init__(self, var_or_exps, name=None):
-        assert len(var_or_exps) > 0
-        self.elms = to_const_ufunc(np.array(var_or_exps, dtype=object))
-        super().__init__(name=name)
-
-    def linkChildren(self):
-        for elm in self.elms:
-            if isinstance(elm, ExpressionElement):
-                elm.parents.append(self)
-                elm.linkChildren()
-
-    def getVariables(self):
-        return functools.reduce(operator.or_, (elm.getVariables() for elm in self.elms))
-
-    def traverse(self):
-        """traverse Expression tree as root is self
-
-        Yield
-        -----
-        Expression or VarElement
-        """
-        yield self
-        for elm in self.elms:
-            yield from elm.traverse()
+    def __repr__(self):
+        return f'Variable("{self.name}", {self.lowBound}, {self.upBound}, "Continuous", {self._value})'
 
-    def isNeg(self):
-        return False
 
-    def __hash__(self):
-        return hash(tuple(elm for elm in self.elms)) + hash(self._type)
+class VarPermutation(VarElement):
+    """Permutation Variable
 
-    def __del__(self):
-        for elm in self.elms:
-            if isinstance(elm, Const):
-                del elm
+    This has [lowBound, ... upBound] range permutation.
 
+    Examples
+    --------
 
-class Sum(Reduction):
-    """
-    Parameters
-    ----------
-    var_of_exps : list of VarELement or ExpressionElement
+    >>> a = Variable('a', lowBound=0, upBound=3, cat='Permutation')
+    >>> a.value()
+    >>> [2, 1, 3, 0]   # randomized
+    >>> b = Variable('b', lowBound=0, upBound=3, ini_value=[0,1,2,3], cat='Permutation')
+    >>> b.value()
+    >>> [0, 1, 2, 3]
+
+    We can use list operation to Permutation Variable
+
+    >>> b[1]
+    >>> 1
+    >>> len(b)
+    >>> 4
+    >>> b[1:3]
+    >>> [1, 2]
     """
 
-    def setName(self):
-        self.name = ""
-        const = 0
-
-        elm = self.elms[0]
-        if isinstance(elm, number_classes):
-            const += elm
-        elif isinstance(elm, ExpressionElement) and elm.getName().startswith("-"):
-            self.name += f"({elm.getName()})"
-        else:
-            self.name += f"{elm.getName()}"
+    _type = VariableType.Permutation
 
-        for elm in self.elms[1:]:
-            if isinstance(elm, number_classes):
-                const += elm
-            elif isinstance(elm, ExpressionElement) and elm.getName().startswith("-"):
-                self.name += f"+({elm.getName()})"
-            else:
-                self.name += f"+{elm.getName()}"
+    def __init__(self, name, lowBound=None, upBound=None, ini_value=None):
+        if ini_value is None:
+            ini_value = list(range(lowBound, upBound + 1))
+            random.shuffle(ini_value)
+        super().__init__(name, lowBound, upBound, ini_value)
 
-        if const > 0:
-            self.name += f"+{const}"
-        elif const < 0:
-            self.name += f"-{-const}"
-
-    def isPolynomial(self):
-        return all(elm.isPolynomial() for elm in self.elms)
-
-    def setPolynomial(self):
-        self.polynomial = sum(elm.toPolynomial() for elm in self.elms)
-
-    def _value(self):
+    def value(self, *args, **kwargs):
         """
         Returns
         -------
-        float or int
-            return value of expression
+        list
         """
+        _value = self._value[:]  # copy
+        return _value
 
-        if self.var_dict is not None:
-            ret = 0
-            for elm in self.elms:
-                if isinstance(elm, ExpressionElement):
-                    elm.setVarDict(self.var_dict)
-                    ret += elm.value()
-                elif elm.name in self.var_dict:
-                    ret += self.var_dict[elm.name].value()
-                else:
-                    ret += elm.value()
-            self.unsetVarDict()
-            return ret
-        else:
-            return to_value_ufunc(self.elms).sum()
+    def setRandom(self):
+        """shuffle the list"""
+        return random.shuffle(self._value)
+
+    def isPolynomial(self):
+        return False
 
     def isLinear(self):
-        return all(elm.isLinear() for elm in self.elms)
+        return False
 
     def isQuadratic(self):
-        return all(elm.isQuadratic() for elm in self.elms)
-
-    def __repr__(self):
-        s = f"Sum({self.elms})"
-        return s
-
-
-class Prod(Reduction):
-    """
-    Parameters
-    ----------
-    var_of_exps : list of VarELement or ExpressionElement
-    """
-
-    def setName(self):
-        self.name = ""
-        const = 0
-
-        elm = self.elms[0]
-        if isinstance(elm, number_classes):
-            const += elm
-        elif isinstance(elm, ExpressionElement) and elm.getName().startswith("-"):
-            self.name += f"({elm.getName()})"
-        else:
-            self.name += f"{elm.getName()}"
-
-        for elm in self.elms[1:]:
-            if isinstance(elm, number_classes):
-                const += elm
-            elif isinstance(elm, ExpressionElement) and elm.getName().startswith("-"):
-                self.name += f"*({elm.getName()})"
-            else:
-                self.name += f"*{elm.getName()}"
-
-        if const != 0:
-            self.name = f"{const}*" + self.name
+        return False
 
-    def isPolynomial(self):
-        return all(elm.isPolynomial() for elm in self.elms)
+    def clone(self):
+        return VarPermutation(self.name, self.lowBound, self.upBound, self._value)
 
-    def setPolynomial(self):
-        self.polynomial = functools.reduce(
-            operator.mul, (elm.toPolynomial() for elm in self.elms)
-        )
+    def __iter__(self):
+        return iter(self._value)
 
-    def _value(self):
-        """
-        Returns
-        -------
-        float or int
-            return value of expression
-        """
-        if self.var_dict is not None:
-            ret = 1
-            for elm in self.elms:
-                if isinstance(elm, ExpressionElement):
-                    elm.setVarDict(self.var_dict)
-                    ret *= elm.value()
-                elif elm.name in self.var_dict:
-                    ret *= self.var_dict[elm.name].value()
-                else:
-                    ret *= elm.value()
-            self.unsetVarDict()
-            return ret
-        else:
-            return to_value_ufunc(self.elms).prod()
+    def __getitem__(self, k):
+        return self._value[k]
 
-    def isLinear(self):
-        if self.polynomial is None:
-            self.setPolynomial()
-        return self.polynomial.isLinear()
+    def __len__(self):
+        return len(self._value)
 
-    def isQuadratic(self):
-        if self.polynomial is None:
-            self.setPolynomial()
-        return self.polynomial.isQuadratic()
 
-    def __repr__(self):
-        s = f"Prod({self.elms})"
-        return s
+# Variable
+Variable = VariableFactory()
```

### Comparing `flopt-0.5.5/flopt/performance/base_dataset.py` & `flopt-0.5.6/flopt/performance/base_dataset.py`

 * *Files identical despite different names*

### Comparing `flopt-0.5.5/flopt/performance/custom_dataset.py` & `flopt-0.5.6/flopt/performance/custom_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,18 +51,18 @@
       flopt.performance.performance(cd)
 
 
     We can select the solvers to calculate the performance.
 
     .. code-block:: python
 
-      rs_solver = Solver('RandomSearch')
-      tpe_solver = Solver('OptunaTPESearch')
-      cma_solver = Solver('OptunaCmaEsSearch')
-      htpe_solver = Solver('HyperoptTPESearch')
+      rs_solver = Solver('Random')
+      tpe_solver = Solver('OptunaTPE')
+      cma_solver = Solver('OptunaCmaEs')
+      htpe_solver = Solver('Hyperopt')
 
       logs = flopt.performance.compute(
           cd,  # dataset or dataset list
           [rs_solver, tpe_solver, cma_solver, htpe_solver],  # solver list
           timelimit=2,
           msg=True
       )
@@ -80,16 +80,15 @@
         self.instance_names = [prob.name for prob in probs]
         self.instance_dict = {prob.name: prob for prob in probs}
 
     def createInstance(self, instance_name):
         prob = self.instance_dict[instance_name]
         if isinstance(prob, CustomInstance):
             return prob
-        else:
-            return CustomInstance(prob)
+        return CustomInstance(prob)
 
     def addProblem(self, prob):
         self.instance_names.append(prob.name)
         self.instance_dict[prob.name] = prob
 
     def __iadd__(self, prob):
         assert prob.name is not None, "problem must be named"
@@ -119,16 +118,15 @@
         self.best_bound = None
 
     def createProblem(self, solver):
         if solver.available(self.prob):
             for variable in self.prob.getVariables():
                 variable.setValue(self.var_values[variable.name])
             return True, self.prob
-        else:
-            return False, None
+        return False, None
 
     def getBestBound(self):
         """return the optimal value of objective function"""
         return self.prob.best_bound
 
     def setBestBound(self, best_bound):
         self.prob.setBestBound(best_bound)
```

### Comparing `flopt-0.5.5/flopt/performance/func_dataset.py` & `flopt-0.5.6/flopt/performance/func_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,48 +21,44 @@
     name = "func"
     instance_names = list(benchmark_func)
 
     def createInstance(self, instance_name):
         """create FuncInstance"""
         logger.debug(f"{instance_name}")
         func_data = benchmark_func[instance_name]
-        create_objective = func_data["co"]
-        create_variables = func_data["cv"]
-        minimum_value = func_data["mo"]
-        func_instance = FuncInstance(
-            instance_name, create_objective, create_variables, minimum_value
-        )
+        func_instance = FuncInstance(instance_name, func_data)
         return func_instance
 
 
 class FuncInstance(BaseInstance):
     """Function Benchmark Instance
 
     Parameters
     ----------
     name : str
         instance name
-    create_objective : function
-        function which generates the objective function using dimension n
-    create_variables : function
-        function which generates the variables using dimension n
+    func_data : class
+        create_objective : function
+            function which generates the objective function using dimension n
+        create_variables : function
+            function which generates the variables using dimension n
+        minimum_obj : function
+            minimum value
     n : int
         dimension (for some instance)
     """
 
-    def __init__(self, name, create_objective, create_variables, minimum_value, n=10):
+    def __init__(self, name, func_data, n=10):
         self.name = name
-        self.create_objective = create_objective
-        self.create_variables = create_variables
-        self.minimum_value = minimum_value
+        self.func_data = func_data
         self.n = n
 
     def getBestBound(self):
         """return the optimal value of objective function"""
-        return self.minimum_value(self.n)
+        return self.func_data.minimum_obj(self.n)
 
     def createProblem(self, solver):
         """Create problem according to solver
 
         Parameters
         ----------
         solver : Solver
@@ -96,19 +92,17 @@
             type of variables
 
         Returns
         -------
         Problem
             problem
         """
-        variables = self.create_variables(n=n, cat=cat)
-        for var in variables:
-            var.setRandom()
-        func = self.create_objective(n)
-        obj = CustomExpression(lambda *x: func(x), variables)
+        x = self.func_data.create_variables(n=n, cat=cat)
+        x.setRandom()
+        obj = self.func_data.create_objective(n)
         prob = Problem(name=f"Function:{self.name}_n{n}")
-        prob.setObjective(obj)
+        prob += obj(x)
         self.n = n
         return prob
 
     def __str__(self):
         return f"Instance: {self.name}"
```

### Comparing `flopt-0.5.5/flopt/performance/log_visualizer.py` & `flopt-0.5.6/flopt/performance/log_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,22 +29,25 @@
     Examples
     --------
 
     .. code-block:: python
 
       log_visualizer = LogVisualiser()
       log_visualizer.load(
-          solver_names=['RandomSearch', '2-Opt'],
+          solver_names=['Random', '2-Opt'],
           datasets=['tsp']
       )
       log_visualizer.plot()
     """
 
-    def __init__(self, logs=dict()):
-        self.logs = logs
+    def __init__(self, logs=None):
+        if logs is None:
+            self.logs = {}
+        else:
+            self.logs = logs
 
     def load(self, solver_names, datasets, load_prefix=PERFORMANCE_DIR):
         if isinstance(solver_names, str):
             solver_names = [solver_names]
         if isinstance(datasets, str):
             datasets = [datasets]
         for solver_name, dataset in product(solver_names, datasets):
```

### Comparing `flopt-0.5.5/flopt/performance/mip_dataset.py` & `flopt-0.5.6/flopt/performance/mip_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         "gen-ip054",
         "neos-3046615-murg",
         "gen-ip002",
         "neos-3754480-nidda",
     ]
 
     def __init__(self):
-        self.sol_data = dict()
+        self.sol_data = {}
         sol_file = "miplib2017-v23.solu"
         pattern = re.compile("=(?P<status>.*)=\s+(?P<name>.*)\s+(?P<best_value>.*)")
         for line in open(f"{mip_storage}/{sol_file}", "r"):
             line = line.strip()
             m = pattern.match(line)
             if m is not None:
                 d = m.groupdict()
```

### Comparing `flopt-0.5.5/flopt/performance/performance.py` & `flopt-0.5.6/flopt/performance/performance.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         log_visualizer.plot()
 
 
     We can select the solver to calculate the performance.
 
     .. code-block:: python
 
-        rs_solver = flopt.Solver("RandomSearch")
+        rs_solver = flopt.Solver("Random")
 
         # compute the performance
         logs = flopt.performance.compute(
             [func_dataset, tsp_dataset],  # dataset list
             [rs_solver],  # solver list
             timelimit=2,
             msg=True
@@ -102,15 +102,15 @@
     for solver in solvers:
         solver.setParams(timelimit=timelimit, **kwargs)
 
     # save_prefix setting
     if save_prefix is None:
         save_prefix = PERFORMANCE_DIR
 
-    logs = dict()
+    logs = {}
 
     for dataset in datasets:
         for instance in dataset:
             logger.info(instance)
             for solver in solvers:
                 solver.reset()
                 formulatable, prob = instance.createProblem(solver)
```

### Comparing `flopt-0.5.5/flopt/performance/tsp_dataset.py` & `flopt-0.5.6/flopt/performance/tsp_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                 D[i, j] = D[j, i] = elm
                 j = j + 1
             i, j = i + 1, 0
         return D
 
 
 def read_node_coord(f, edge_weight_type, dim, D):
-    N = dict()
+    N = {}
     for _ in range(dim):
         line = f.readline()
         node_ix, x, y = line.split()
         node_ix, x, y = int(node_ix), float(x), float(y)
         N[node_ix] = (x, y)
     if edge_weight_type == "EUC_2D":
         D = np.zeros((dim, dim))
@@ -182,15 +182,15 @@
         # Object
         def tsp_dist(perm):
             distance = 0
             for head, tail in zip(perm, perm[1:] + [perm[0]]):
                 distance += self.D[head][tail]
             return distance
 
-        tsp_obj = CustomExpression(func=tsp_dist, arg=[perm])
+        tsp_obj = CustomExpression(func=tsp_dist, args=[perm])
 
         # Problem
         prob = Problem(name=f"TSP:{self.name}")
         prob += tsp_obj
         return prob
 
     def createLpProblem(self):
```

### Comparing `flopt-0.5.5/flopt/polynomial.py` & `flopt-0.5.6/flopt/polynomial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import operator
+import functools
+
 from flopt.constants import VariableType
 
 
 class Monomial:
     """
     Parameters
     ----------
@@ -13,29 +16,35 @@
         coefficient of monomial
 
     Notes
     -----
     If terms is empty dictionary, then this monomial is constant whose value is self.coeff
     """
 
-    def __init__(self, terms=dict(), coeff=1):
+    def __init__(self, terms={}, coeff=1):
         self.terms = terms
         self.coeff = coeff
         self.max_degree = None
         self.is_linear = None
         self._hash = None
 
-    def copy(self):
+    def clone(self):
         """
         Returns
         -------
         Monomial
         """
         return Monomial(dict(self.terms), self.coeff)
 
+    def value(self):
+        return self.coeff * functools.reduce(
+            operator.mul,
+            (var.value() ** exponent for var, exponent in self.terms.items()),
+        )
+
     def maxDegree(self):
         """
         Returns
         -------
         int
             maximum degree of variables
         """
@@ -97,50 +106,51 @@
         """
         Returns
         -------
         Polynomial
         """
         if self.terms:
             return Polynomial({Monomial(self.terms): self.coeff})
-        else:
-            return Polynomial(constant=self.coeff)
+        return Polynomial(constant=self.coeff)
+
+    def toExpression(self):
+        """
+        Returns
+        -------
+        Expression
+        """
+        expression = self.coeff
+        for var, exponent in self.terms.items():
+            expression *= var**exponent
+        return expression
 
     def simplify(self):
         """Simplify this monomial
 
         Returns
         -------
         Monomial
         """
-        terms = dict()
+        terms = {}
         for x in self.terms:
             if x.type() == VariableType.Binary:
                 terms[x] = 1  # x * x = x
             elif x.type() == VariableType.Spin:
                 if self.terms[x] % 2 == 1:
                     terms[x] = 1  # x * x = 1 --> x^{2n+1} = x
                 else:
                     pass  # x * x = 1 --> x^{2n} = 1 (become constant 1)
             else:
                 terms[x] = self.terms[x]
         return Monomial(terms, self.coeff)
 
     def __mul__(self, other):
-        if isinstance(other, (int, float)):
-            return Monomial(self.terms, self.coeff * other)
-        elif isinstance(other, Monomial):
-            terms = dict(self.terms)
-            for x in other.terms:
-                if x in self.terms:
-                    terms[x] += other[x]
-                else:
-                    terms[x] = other[x]
-            return Monomial(terms, self.coeff * other.coeff)
-        else:
-            return NotImplemented
+        mono = self.clone()
+        mono *= other
+        return mono
 
     def __rmul__(self, other):
         return self * other
 
     def __imul__(self, other):
         if isinstance(other, (int, float)):
             self.coeff *= other
@@ -159,14 +169,17 @@
         return self
 
     def __pow__(self, other):
         assert isinstance(other, int)
         terms = {x: exp * other for x, exp in self.terms.items()}
         return Monomial(terms, self.coeff**other)
 
+    def __iter__(self):
+        return iter(self.terms.items())
+
     def __getitem__(self, item):
         return self.terms[item]
 
     def __hash__(self):
         if self._hash is None:
             self._hash = hash(
                 tuple(
@@ -205,25 +218,22 @@
     ----------
     terms : dict(Monomial=coeff)
         sum( coeff_i * mono_i for mono_i, coeff_i in terms.items() ) + constant
     constant : int of float
         constant of polynomial
     """
 
-    def __init__(self, terms=dict(), constant=0):
+    def __init__(self, terms={}, constant=0):
         self.terms = terms
         self._constant = constant
 
-    def monos(self):
-        """
-        Returns
-        -------
-        set of Monomial
-        """
-        return set(self.terms.keys())
+    def value(self):
+        return (
+            sum(coeff * mono.value() for mono, coeff in terms.items()) + self.constant()
+        )
 
     def coeff(self, *args):
         """
         Returns
         -------
         int or float
             coefficient of monomial
@@ -257,30 +267,22 @@
         get coefficient of `y^3` term, it is 0
 
         .. code-block:: python
 
             e.polynomial.coeff(y**3)
             >>> 3
         """
-        if isinstance(args[0], Monomial):
-            mono = args[0]
-        else:
-            mono = args[0].toMonomial()
+        mono = args[0].toMonomial()
         if len(args) > 1:
-            mono = mono.copy()
-        for elm in args[1:]:
-            if isinstance(elm, Monomial):
-                assert elm.coeff == 1
-                mono *= elm
-            else:
+            mono = mono.clone()
+            for elm in args[1:]:
                 mono *= elm.toMonomial()
         if mono in self.terms:
             return self.terms[mono]
-        else:
-            return 0
+        return 0
 
     def constant(self):
         """
         Returns
         -------
         int or float
         """
@@ -322,15 +324,15 @@
         Returns
         -------
         Polynomial
             return polynomial differentiated by x
         """
         poly = Polynomial(constant=0)
         for mono, coeff in self:
-            poly += mono.diff(x)
+            poly += coeff * mono.diff(x)
         return poly
 
     def maxDegree(self):
         """
         Returns
         -------
         int
@@ -358,15 +360,15 @@
     def simplify(self):
         """
         Returns
         -------
         Polynomial
             return simplified self polynomial
         """
-        terms = dict()
+        terms = {}
         constant = 0
         for mono in self.terms.keys():
             _mono = mono.simplify()
             if _mono.isConstant():
                 constant += _mono.coeff
             else:
                 terms[_mono] = self.terms[mono]
@@ -385,16 +387,15 @@
                 else:
                     terms[mono] = coeff
                 # clean up
                 if terms[mono] == 0:
                     del terms[mono]
             constant = self._constant + other._constant
             return Polynomial(terms, constant)
-        else:
-            return NotImplemented
+        return NotImplemented
 
     def __radd__(self, other):
         return self + other
 
     def __sub__(self, other):
         return self + (-other)
 
@@ -404,15 +405,15 @@
     def __mul__(self, other):
         if isinstance(other, (int, float)):
             terms = {mono: coeff * other for mono, coeff in self}
             return Polynomial(terms, self._constant * other)
         elif isinstance(other, Monomial):
             return self * other.toPolynomial()
         elif isinstance(other, Polynomial):
-            terms = dict()
+            terms = {}
             for mono, coeff in other:
                 for mono_, coeff_ in self:
                     mono__ = mono * mono_
                     if mono__ in terms:
                         terms[mono__] += coeff * coeff_
                     else:
                         terms[mono__] = coeff * coeff_
@@ -433,16 +434,15 @@
                 else:
                     terms[mono] = self._constant * coeff
                 # clean up
                 if terms[mono] == 0:
                     del terms[mono]
             constant = self._constant * other._constant
             return Polynomial(terms, constant)
-        else:
-            return NotImplemented
+        return NotImplemented
 
     def __rmul__(self, other):
         return self * other
 
     def __pow__(self, other):
         assert isinstance(other, int)
         poly = Polynomial(constant=1)
@@ -469,16 +469,16 @@
         if isinstance(other, Polynomial):
             return hash(self) == hash(other)
 
     def __str__(self):
         s = ""
         for mono, coeff in self.terms.items():
             if coeff == 1:
-                s += f"{str(mono)}+"
+                s += f"{mono}+"
             elif coeff > 0:
-                s += f"{coeff}*{str(mono)}+"
+                s += f"{coeff}*{mono}+"
             else:
-                s += f"({coeff}*{str(mono)})+"
+                s += f"({coeff}*{mono})+"
         return s + f"{self._constant}"
 
     def __repr__(self):
         return str(self)
```

### Comparing `flopt-0.5.5/flopt/problem.py` & `flopt-0.5.6/flopt/problem.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import flopt
 from flopt.variable import VarElement
-from flopt.expression import Expression, CustomExpression, Const
+from flopt.expression import Expression, CustomExpression, Const, SelfReturn
 from flopt.constraint import Constraint
 from flopt.solvers import Solver
 from flopt.solution import Solution
 from flopt.constants import (
     VariableType,
     ExpressionType,
+    ConstraintType,
     OptimizationType,
     array_classes,
 )
-from flopt.env import setup_logger
+from flopt.env import setup_logger, create_variable_mode
 
 
 logger = setup_logger(__name__)
 
 
 class Problem:
     """
@@ -44,64 +46,80 @@
 
     >>> prob = Problem(name='test')
 
     When we want to solve the maximize problem, then
 
     >>> prob = Problem(name='test', sense='maximize')
 
-    Input solver, when we solve
+    We solve
 
-    >>> solve = Solver(algo=...)
-    >>> prob.solve(solver=solver, timelimit=10)
+    >>> prob.solve(solver=solver_name or solver object, timelimit=10)
 
     After solving, we can obtain the objective value.
 
     >>> prob.getObjectiveValue()
     """
 
     def __init__(self, name=None, sense=OptimizationType.Minimize):
-        if sense == "minimize" or sense == "maximize":
-            logger.warning(
-                f"'minimize' and 'maximize' is deprecated. You have to use 'Minimize', 'Maximize', flopt.Minimize or flopt.Maximize"
-            )
         self.type = "Problem"
         self.name = name
         self.sense = str(sense)
         self.obj = Const(0)
         self.obj_name = None
         self.constraints = []
         self.__variables = set()
         self.solver = None
         self.time = None
         self.best_bound = None
 
+    def clone(self, variable_clone=False):
+        """create clone object
+        Parameters
+        ----------
+        variable_clone : bool
+            if it is true, variables are cloned in expression
+
+        Returns
+        -------
+        prob : Problem
+        """
+        prob = Problem(
+            name=f"{self.name}" if self.name is not None else None,
+            sense=self.sense,
+        )
+        if not variable_clone:
+            prob.setObjective(self.obj.clone(), self.obj_name)
+            for const in self.constraints:
+                prob.addConstraint(const.clone(), const.name)
+            return prob
+
+        var_dict = {var.name: SelfReturn(var.clone()) for var in self.getVariables()}
+        prob.setObjective(self.obj.value(var_dict=var_dict), self.obj_name)
+        for const in self.constraints:
+            const_exp = const.expression.value(var_dict=var_dict)
+            if const.type == ConstraintType.Eq:
+                prob.addConstraint(const_exp == 0, const.name)
+            else:
+                prob.addConstraint(const_exp <= 0, const.name)
+        return prob
+
     def setObjective(self, obj, name=None):
         """set objective function. __iadd__(), "+=" operations call this function.
 
         Parameters
         ----------
         obj : int, float, Variable family or Expression family
             objective function
         """
         if isinstance(obj, (int, float)):
             obj = Const(obj)
         elif isinstance(obj, VarElement):
             obj = Expression(obj, Const(0), "+")
         self.obj = obj
         self.obj_name = name
-        try:
-            self.__variables |= obj.getVariables()
-        except RecursionError:
-            import sys
-
-            logger.warning(f"recursion reaches {sys.getrecursionlimit}")
-            sys.setrecursionlimit(sys.getrecursionlimit() * 100)
-            self.__variables |= obj.getVariables()
-        except Exception as e:
-            raise e
 
     def setBestBound(self, best_bound):
         """
         Parameters
         ----------
         best_bound : float
             best objective value of this problem
@@ -131,15 +149,14 @@
 
         """
         assert isinstance(
             const, Constraint
         ), f"assume Constraint class, but got {type(const)}"
         const.name = name
         self.constraints.append(const)
-        self.__variables |= const.getVariables()
 
     def addConstraints(self, consts, name=None):
         for i, const in enumerate(consts):
             _name = const.name if name is None else name + f"_{i}"
             self.addConstraint(const, _name)
 
     def removeDuplicatedConstraints(self):
@@ -186,39 +203,48 @@
     def getVariables(self):
         """
         Returns
         -------
         set
             set of VarElement used in this problem
         """
+        self.__variables = self.obj.getVariables()
+        for const in self.constraints:
+            self.__variables |= const.getVariables()
+
         return self.__variables
 
     def getConstraints(self):
         """
         Returns
         -------
         list of Constraint
             list of constraints in this problem
         """
         return self.constraints
 
-    def resetVariables(self):
-        self.__variables = self.obj.getVariables()
-        for const in self.constraints:
-            self.__variables |= const.getVariables()
-
-    def solve(self, solver=None, timelimit=None, lowerbound=None, msg=False, **kwargs):
+    def solve(
+        self,
+        solver=None,
+        timelimit=None,
+        lowerbound=None,
+        optimized_variables=None,
+        msg=False,
+        **kwargs,
+    ):
         """solve this problem
 
         Parameters
         ----------
         solver : Solver or None
         timelimit : float or None
         lowerbound : float or None
             solver terminates when it obtains the solution whose objective value is lower than this value
+        optimized_variables : None or list, tuple, np.ndarray or any container of Variable
+            if it is specified, solver will optimize only the variables in optimized_variables
         msg : bool
             if true, display the message from solver
 
         Returns
         -------
         Status
             return the status of solving
@@ -238,38 +264,54 @@
             prob = flopt.Problem(name="Test")
             prob += a + b
             prob += a + b >= 0
 
             solver = flopt.Solver("auto")
             status, logs = prob.solve(solver=solver)
 
+        When user want to optimize a part of variables under otherwise variables are fixed,
+        user specify optmized_variables in problem.solve().
+
+        .. code-block:: python
+
+            # optimize only a
+            status, log = prob.solve(optimized_variables=[a], timelimit=1)
+
         """
         if solver is None:
             solver = Solver("auto")
+        elif isinstance(solver, str):
+            solver = Solver(solver)
         if timelimit is not None:
             solver.setParams(timelimit=timelimit)
         if lowerbound is not None:
             solver.setParams(lowerbound=lowerbound)
         solver.setParams(**kwargs)
         self.solver = solver
 
-        if self.sense == "maximize" or self.sense == "Maximize":
+        if self.sense.lower() == "maximize":
             self.obj = -self.obj
 
-        solution = Solution("s", self.getVariables())
+        if optimized_variables is None:
+            solution = Solution(self.getVariables())
+        else:
+            assert (
+                set(optimized_variables) <= self.getVariables()
+            ), "optimized_variables containes variables that are not in the problem"
+            solution = Solution(optimized_variables)
 
         status, log, self.time = self.solver.solve(
             solution,
             self.obj,
             self.constraints,
             self,
             msg=msg,
         )
 
-        if self.sense == "maximize" or self.sense == "Maximize":
+        if self.sense.lower() == "maximize":
             self.obj = -self.obj
 
         return status, log
 
     def getSolution(self, k=1):
         """get the k-top solution
 
@@ -300,48 +342,47 @@
     def toProblemType(self):
         """
         Returns
         -------
         problem_type : dict
             key is "Variable", "Objective", "Constraint"
         """
-        problem_type = dict()
+        problem_type = {}
 
         variable_types = [
             VariableType.Binary,
             VariableType.Integer,
             VariableType.Continuous,
             VariableType.Permutation,
             VariableType.Number,
             VariableType.Any,
         ]
 
         expression_types = [
             ExpressionType.Linear,
             ExpressionType.Quadratic,
+            ExpressionType.Polynomial,
+            ExpressionType.Nonlinear,
+            ExpressionType.Permutation,
+            ExpressionType.BlackBox,
             ExpressionType.Any,
         ]
 
         # variables
         prob_variables_types = set(var.type() for var in self.getVariables())
         for variable_type in variable_types:
             if prob_variables_types <= variable_type.expand():
                 problem_type["Variable"] = variable_type
                 break
 
         # objective
         for expression_type in expression_types:
-            for elm in self.obj.traverse():
-                if isinstance(elm, CustomExpression):
-                    problem_type["Objective"] = ExpressionType.BlackBox
-                    break
-            else:
-                if self.obj.type() in expression_type.expand():
-                    problem_type["Objective"] = expression_type
-                    break
+            if self.obj.type() in expression_type.expand():
+                problem_type["Objective"] = expression_type
+                break
 
         # constraint
         if not self.constraints:
             problem_type["Constraint"] = ExpressionType.Non
         else:
             prob_expression_types = set(
                 const.expression.type() for const in self.getConstraints()
@@ -349,44 +390,217 @@
             for expression_type in expression_types:
                 if prob_expression_types <= expression_type.expand():
                     problem_type["Constraint"] = expression_type
                     break
 
         return problem_type
 
+    def toEq(self):
+        """Create a problem object with only equal constraints
+
+        Returns
+        -------
+        prob : Problem
+        """
+        prob = self.clone()
+        constraints = []
+        for const in prob.constraints:
+            if const.type() == ConstraintType.Eq:
+                constraints.append(const)
+            else:  # ConstraintType.Le
+                with create_variable_mode():
+                    s = flopt.Variable(
+                        "slack", lowBound=0, cat="Continuous", ini_value=0
+                    )
+                constraints.append(const.expression + s == 0)
+        prob.constraints = constraints
+        return prob
+
+    def toIneq(self):
+        """Create a problem object with only inequal constraints
+
+        Returns
+        -------
+        prob : Problem
+        """
+        prob = self.clone()
+        constraints = []
+        for const in prob.constraints:
+            if const.type() == ConstraintType.Le:
+                constraints.append(const)
+            else:  # ConstraintType.Eq
+                constraints.append(const.expression <= 0)
+                constraints.append(const.expression >= 0)
+        prob.constraints = constraints
+        return prob
+
+    def boundsToIneq(self):
+        """Create a problem object has bounds constraints of variables as inequal constraints
+
+        Returns
+        -------
+        prob : Problem
+        """
+        prob = self.clone()
+        for var in prob.getVariables():
+            if var.getLb() is not None:
+                prob += var >= var.getLb()
+            if var.getUb() is not None:
+                prob += var <= var.getUb()
+            var.lowBound = None
+            var.upBound = None
+        return prob
+
+    def toRelax(self):
+        """Create relaxed problem
+
+        Returns
+        -------
+        prob : Problem
+        """
+        prob = self.clone()
+        correspondence_dict = dict()
+        for var in prob.getVariables():
+            if var.type() == VariableType.Continuous:
+                pass
+            elif var.type() == VariableType.Integer:
+                with create_variable_mode():
+                    relaxed_var = flopt.Variable(
+                        var.getName(),
+                        lowBound=var.getLb(),
+                        upBound=var.getUb(),
+                        ini_value=var.value(),
+                    )
+                correspondence_dict[var] = relaxed_var
+            elif var.type() == VariableType.Binary:
+                with create_variable_mode():
+                    relaxed_var = flopt.Variable(
+                        var.getName(), lowBound=0, upBound=1, ini_value=var.value()
+                    )
+                correspondence_dict[var] = relaxed_var
+            elif var.type() == VariableType.Spin:
+                with create_variable_mode():
+                    relaxed_var = flopt.Variable(
+                        var.getName(), lowBound=0, upBound=1, ini_value=(var.value() + 1)//2
+                    )
+                correspondence_dict[var] = 2 * relaxed_var - 1
+            else:
+                assert True
+        return prob.replace(correspondence_dict)
+
+    def replace(self, correspondence_dict):
+        """Replace variable to another variables or expression
+
+        Parameters
+        ----------
+        correspondence_dict : dict
+            key is Variable and value is Variable or ExpressionElement
+
+        Examples
+        --------
+
+        .. code-block:: python
+
+            import flopt
+
+            # create problem
+            x = flopt.Variable("x", lowBound=4, upBound=5)
+            prob = flopt.Problem()
+            prob += x
+            prob.show()
+            >>> Name: None
+            >>> Type         : Problem
+            >>> sense        : Minimize
+            >>> objective    : x+0
+            >>> #constraints : 0
+            >>> #variables   : 1 (Continuous 1)
+            >>>
+            >>>
+            >>> V 0, name x, Continuous 4 <= x <= 5
+
+            # convert bounds of variables to constraints
+            prob = prob.clone().boundsToIneq()
+            prob.show()
+            >>> Name: None
+            >>>   Type         : Problem
+            >>>   sense        : Minimize
+            >>>   objective    : x+0
+            >>>   #constraints : 2
+            >>>   #variables   : 1 (Continuous 1)
+            >>>
+            >>>   C 0, name None, 4-x <= 0
+            >>>   C 1, name None, x-5 <= 0
+            >>>
+            >>>   V 0, name x, Continuous None <= x <= None
+
+            # replace x with x_plus + x_minus
+            x_plus = flopt.Variable("x_plus", lowBound=0)
+            x_minus = flopt.Variable("x_minus", lowBound=0)
+            prob.replace(correspondence_dict={x: x_plus + x_minus})
+            prob.show()
+            >>> Name: None
+            >>>   Type         : Problem
+            >>>   sense        : Minimize
+            >>>   objective    : x_plus+x_minus
+            >>>   #constraints : 2
+            >>>   #variables   : 2 (Continuous 2)
+            >>>
+            >>>   C 0, name None, 4-(x_plus+x_minus) <= 0
+            >>>   C 1, name None, x_plus+x_minus-5 <= 0
+            >>>
+            >>>   V 0, name x_minus, Continuous 0 <= x_minus <= None
+            >>>   V 1, name x_plus, Continuous 0 <= x_plus <= None
+
+        """
+        assert all(isinstance(key, VarElement) for key in correspondence_dict.keys())
+        prob = self.clone()
+
+        var_dict = {var.name: SelfReturn(var) for var in prob.getVariables()}
+        for var, value in correspondence_dict.items():
+            var_dict[var.name] = SelfReturn(value)
+        prob.setObjective(prob.obj.value(var_dict=var_dict), prob.obj_name)
+        for const in prob.constraints:
+            const.expression = const.expression.value(var_dict=var_dict)
+        return prob
+
     def __iadd__(self, other):
         if not isinstance(other, tuple):
             other = (other,)
         if isinstance(other[0], Constraint):
             self.addConstraint(*other)
         elif isinstance(other[0], array_classes):
             self.addConstraints(*other)
         else:
             self.setObjective(*other)
         return self
 
-    def __str__(self):
+    def __str__(self, prefix=""):
         from collections import defaultdict
 
         variables_dict = defaultdict(int)
         for var in self.getVariables():
             variables_dict[var.type()] += 1
         variables_str = ", ".join(
             [
                 f'{str(key).replace("VariableType.", "")} {value}'
                 for key, value in sorted(variables_dict.items())
             ]
         )
-        obj_name = "" if self.obj_name is None else f"{self.obj_name}, "
-        s = f"Name: {self.name}\n"
-        s += f"  Type         : {self.type}\n"
-        s += f"  sense        : {self.sense}\n"
-        s += f"  objective    : {obj_name}{self.obj.name}\n"
-        s += f"  #constraints : {len(self.constraints)}\n"
-        s += f"  #variables   : {len(self.getVariables())} ({variables_str})"
+        obj_name = self.obj.getName() if self.obj_name is None else f"{self.obj_name}, "
+        s = f"{prefix}Name: {self.name}\n"
+        s += f"{prefix}  Type         : {self.type}\n"
+        s += f"{prefix}  sense        : {self.sense}\n"
+        s += f"{prefix}  objective    : {obj_name}\n"
+        s += f"{prefix}  #constraints : {len(self.constraints)}\n"
+        s += f"{prefix}  #variables   : {len(self.getVariables())} ({variables_str})"
         return s
 
-    def show(self):
+    def show(self, to_str=False):
         s = str(self) + "\n\n"
         for ix, const in enumerate(self.constraints):
-            s += f"  C {ix}, name {const.name}, {str(const)}\n"
-        return s
+            s += f"  C {ix}, name {const.name}, {const}\n"
+        s += "\n"
+        for ix, var in enumerate(self.getVariables()):
+            s += f"  V {ix}, name {var.name}, {var.type()} {var.getLb()} <= {var.name} <= {var.getUb()}\n"
+        if to_str:
+            return s
+        print(s)
```

### Comparing `flopt-0.5.5/flopt/solvers/amplify_search.py` & `flopt-0.5.6/flopt/solvers/amplify_search.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,75 +30,73 @@
     Examples
     --------
 
     AmplifySearch can solve the problem whose variables are Spin
 
     .. code-block:: python
 
-        from flopt import Variable, Problem
+        import flopt
 
-        x = Variable('x', cat='Spin')
-        y = Variable('y', cat='Spin')
+        x = flopt.Variable("x", cat="Spin")
+        y = flopt.Variable("y", cat="Spin")
 
-        prob = Problem()
+        prob = flopt.Problem()
         prob += 1 - x * y - x
         prob += x + y >= 0
 
-        print(prob.show())
+        prob.show()
         >>> Name: None
         >>>   Type         : Problem
         >>>   sense        : minimize
         >>>   objective    : 1-(x*y)-x
         >>>   #constraints : 1
         >>>   #variables   : 2 (Spin 2)
         >>>
         >>>   C 0, name None, x+y >= 0
 
     .. code-block:: python
 
-        from flopt import Solver
-
-        solver = Solver('AmplifySearch')
+        solver = flopt.Solver("Amplify")
         solver.setParams(token="xxx")  # your token
         prob.solve(solver, msg=True)
 
         print()
-        print('obj =', Value(prob.obj))
-        print('x =', Value(x))
-        print('y =', Value(y))
+        print("obj =", flopt.Value(prob.obj))
+        print("x =", flopt.Value(x))
+        print("y =", flopt.Value(y))
         >>> obj = -1
         >>> x = 1
         >>> y = 1
 
     In the case, the problem includes the binary variables,
     you should convert them to spin variables.
 
     .. code-block:: python
 
-        from flopt import Variable, Problem
+        import flopt
 
-        x = Variable('x', cat='Binary')
-        y = Variable('y', cat='Binary')
+        x = flopt.Variable("x", cat="Binary")
+        y = flopt.Variable("y", cat="Binary")
 
-        prob = Problem()
+        prob = flopt.Problem()
         prob += (1 - x * y - x).toSpin()
         prob += (x + y >= 0).toSpin()
 
-        print(prob.show())
+        prob.show()
         >>> Name: None
         >>>   Type         : Problem
         >>>   sense        : minimize
         >>>   objective    : -0.25*(x_s*y_s)-(0.75*x_s)-(0.25*y_s)+0.25
         >>>   #constraints : 1
         >>>   #variables   : 2 (Spin 2)
         >>>
         >>>   C 0, name None, 0.5*x_s+(0.5*y_s)+1.0 >= 0
     """
 
-    name = "AmplifySearch"
+    name = "Amplify"
     can_solve_problems = {
         "Variable": VariableType.Spin,
         "Objective": ExpressionType.Quadratic,
         "Constraint": ExpressionType.Linear,
     }
 
     def __init__(self):
@@ -109,25 +107,25 @@
     def search(self, solution, objective, constraints):
         assert (
             self.token is not None
         ), f'token is None, set token as .solve(..., token="xxx")'
 
         self.start_build()
 
-        x = self.prob.getVariables()
+        x = solution
         s = gen_symbols(IsingPoly, len(x))
         np_s = np.array(gen_symbols(IsingPoly, len(x)), dtype=object)
 
         # objective function
-        ising = objective.toIsing()
+        ising = objective.toIsing(x)
         f = -np_s.T.dot(ising.J).dot(np_s) - ising.h.T.dot(np_s) + ising.C
 
         # constraints
         for const in constraints:
-            ising = const.expression.toIsing()
+            ising = const.expression.toIsing(x)
             g = np_s.T.dot(ising.J).dot(np_s) - ising.h.T.dot(np_s) + ising.C
             if const.type() == ConstraintType.Eq:
                 f += equal_to(g, 0)
             else:  # ConstraintType.Le
                 f += less_equal(g, 0)
 
         self.end_build()
```

### Comparing `flopt-0.5.5/flopt/solvers/auto_search/auto_search.py` & `flopt-0.5.6/flopt/solvers/auto_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 
 from flopt.solvers.base import BaseSearch
-from flopt.solvers.auto_search.selector import (
+from flopt.solvers.selector import (
     mip,
     ising,
     qp,
     permutation,
     blackbox,
     blackbox_mip,
     nonlinear,
@@ -55,36 +55,39 @@
 
         >>> # - - - - - - - - - - - - - - #
         >>>   Welcome to the flopt Solver
         >>>   Version 0.5.4
         >>>   Date: September 1, 2022
         >>> # - - - - - - - - - - - - - - #
         >>>
-        >>> Algorithm: ScipySearch
+        >>> Algorithm: Scipy
         >>> Params: {'timelimit': 10}
 
-    See the log, you can see the RandomSearch algorithm is used for this problem.
+    See the log, you can see the Random algorithm is used for this problem.
     Executing .select(), we can check which solver will be select.
 
     .. code-block:: python
 
         solver = Solver(algo="auto")
         solver.setParams({"timelimit": 10})
         solver = solver.select(prob)
         print(solver.name)
-        >>> ScipySearch
+        >>> Scipy
     """
 
     name = "auto"
     can_solve_problems = {
         "Variable": VariableType.Any,
         "Objective": ExpressionType.Any,
         "Constraint": ExpressionType.Any,
     }
 
+    def __init__(self):
+        self.selector_msg = False
+
     def available(self, prob, verbose=False):
         """
         Parameters
         ----------
         prob : Problem
         verbose : bool
 
@@ -134,43 +137,43 @@
             is_problem_class = (
                 problem_type["Variable"].expand() <= problem_class["Variable"].expand()
                 and problem_type["Objective"].expand()
                 <= problem_class["Objective"].expand()
                 and problem_type["Constraint"].expand()
                 <= problem_class["Constraint"].expand()
             )
-            if is_problem_class:
+            if is_problem_class and self.selector_msg:
                 logger.info(f"This problem is identified as {class_str}.")
             return is_problem_class
 
         try:
             if check(problem_type, mip, "MIP"):
                 return MipSelector()
             elif check(problem_type, ising, "Ising"):
                 return IsingSelector()
-            elif check(problem_type, qp, "Qadratic programming"):
+            elif check(problem_type, qp, "Quadratic programming"):
                 return QpSelector()
             elif check(problem_type, permutation, "Permutation programming"):
                 return PermutationSelector()
-            elif check(problem_type, blackbox, "Blackbox optimization"):
-                return BlackBoxSelector()
-            elif check(
-                problem_type,
-                blackbox_mip,
-                "Blackbox optimization with integer variables",
-            ):
-                return BlackBoxMipSelector()
             elif check(problem_type, nonlinear, "Nonlinear optimization"):
                 return NonlinearSelector()
             elif check(
                 problem_type,
                 nonlinear_mip,
                 "Nonlinear optimization with integer variables",
             ):
                 return NonlinearMipSelector()
+            elif check(problem_type, blackbox, "Blackbox optimization"):
+                return BlackBoxSelector()
+            elif check(
+                problem_type,
+                blackbox_mip,
+                "Blackbox optimization with integer variables",
+            ):
+                return BlackBoxMipSelector()
         except ModelNotFound as e:
             logger.warning(e)
             return BaseSelector()
         return BaseSelector()
 
     def solve(self, solution, objective, constraints, prob, *args, **kwargs):
         """
@@ -182,14 +185,16 @@
             solution object
         objective : Expression
             objective object
         constraints : list of Constraint
             list of constriants objects
         prob : Problem
             problem
+        msg :
+            if it is true, message about search is outputed
 
         Returns
         -------
         status, Log
         """
         solver = self.select(prob)
         return solver.solve(solution, objective, constraints, prob, *args, **kwargs)
```

### Comparing `flopt-0.5.5/flopt/solvers/auto_search/selector.py` & `flopt-0.5.6/flopt/solvers/selector.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,21 @@
     logger.info(f"download trained model into {ising_model_path}")
 
 
 # ---------------------------------------------
 #   Optimization Class Definitions
 # ---------------------------------------------
 
+# LP
+lp = {
+    "Variable": VariableType.Continuous,
+    "Objective": ExpressionType.Linear,
+    "Constraint": ExpressionType.Linear,
+}
+
 # MIP
 mip = {
     "Variable": VariableType.Number,
     "Objective": ExpressionType.Linear,
     "Constraint": ExpressionType.Linear,
 }
 
@@ -154,38 +161,38 @@
 
 class NonlinearMipSelector(SklearnSelector):
     model_path = nonlinear_mip_model_path
 
 
 class MipSelector(Selector):
     def __call__(self, prob, solver):
-        return "ScipyMilpSearch"
+        return "ScipyMilp"
 
 
 class QpSelector(Selector):
     def __call__(self, prob, solver):
-        return "CvxoptQpSearch"
+        return "Cvxopt"
 
 
 class PermutationSelector(Selector):
     def __call__(self, prob, solver):
         return "2-Opt"
 
 
 class BaseSelector(Selector):
     algos = [
         "2-Opt",
-        "ScipyMilpSearch",
-        "PulpSearch",
-        "CvxoptQpSearch",
-        "ScipySearch",
+        "ScipyMilp",
+        "Pulp",
+        "Cvxopt",
+        "Scipy",
         "SFLA",
-        "RandomSearch",
-        "HyperoptTPESearch",
-        "OptunaTPESearch",
-        "OptunaCmaEsSearch",
+        "Random",
+        "Hyperopt",
+        "OptunaTPE",
+        "OptunaCmaEs",
     ]
 
     def __call__(self, prob, solver):
         for algo in self.algos:
             if Solver(algo=algo).available(prob):
                 return algo
```

### Comparing `flopt-0.5.5/flopt/solvers/base.py` & `flopt-0.5.6/flopt/solvers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,25 +161,30 @@
         except flopt.error.SolverError:
             status = SolverTerminateState.Error
         except flopt.error.RearchLowerbound:
             status = SolverTerminateState.Lowerbound
         except KeyboardInterrupt:
             print("Get user ctrl-cuser ctrl-c")
             status = SolverTerminateState.Interrupt
+        except Exception as e:
+            print("Exception occures in solver", e)
+            logger.warning("Exception occures in solver", e)
+            status = SolverTerminateState.Abnormal
 
         self.recordLog()
 
         if msg:
             obj_value = self.getObjValue(self.best_solution)
             end_solver_message(
                 status,
                 obj_value,
                 self.build_time,
                 time.time() - self.start_time,
                 self.trial_ix,
+                self.prob.sense,
             )
 
         return status, self.log, time.time() - self.start_time
 
     def start_build(self):
         self.build_time = -time.time()
```

### Comparing `flopt-0.5.5/flopt/solvers/hyperopt_search.py` & `flopt-0.5.6/flopt/solvers/hyperopt_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 for logger in loggers_to_shut_up:
     logging.getLogger(logger).setLevel(logging.ERROR)
 
 
 logger = setup_logger(__name__)
 
 
-class HyperoptTPESearch(BaseSearch):
+class HyperoptSearch(BaseSearch):
     """
     TPE Search using Hyperopt (https://hyperopt.github.io/hyperopt/)
 
     Parameters
     ----------
     n_trial : int
         number of trials
@@ -41,23 +41,22 @@
 
         x = flopt.Variable("x", lowBound=-1, upBound=1, cat="Continuous")
         y = flopt.Variable("y", lowBound=-1, upBound=1, cat="Continuous")
 
         prob = flopt.Problem()
         prob += 2*x*x + x*y + y*y + x + y
 
-        solver = flopt.Solver("HyperoptTPESearch")
-        status, log = prob.solve(solver, msg=True, timelimit=1)
+        status, log = prob.solve(solver="Hyperopt", msg=True, timelimit=1)
 
         print("obj =", flopt.Value(prob.obj))
         print("x =", flopt.Value(x))
         print("y =", flopt.Value(y))
     """
 
-    name = "HyperoptTPESearch"
+    name = "Hyperopt"
     can_solve_problems = {
         "Variable": VariableType.Number,
         "Objective": ExpressionType.Any,
         "Constraint": ExpressionType.Non,
     }
 
     def __init__(self):
@@ -69,19 +68,19 @@
         self.hyperopt_STATUS_OK = STATUS_OK
 
     def search(self, solution, *args):
 
         self.start_build()
 
         # make the search space
-        space = dict()
+        space = {}
         for var in solution:
             name = var.name
-            lb = var.getLb(must_number=True)
-            ub = var.getUb(must_number=True)
+            lb = var.getLb(number=True)
+            ub = var.getUb(number=True)
             if var.type() in {
                 VariableType.Integer,
                 VariableType.Binary,
                 VariableType.Spin,
             }:
                 var_space = hyperopt.hp.quniform(name, lb, ub, 1)
             elif var.type() == VariableType.Continuous:
```

### Comparing `flopt-0.5.5/flopt/solvers/optuna_searches.py` & `flopt-0.5.6/flopt/solvers/optuna_searches.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,39 +48,43 @@
             for var in solution:
                 if var.type() == VariableType.Binary:
                     var.setValue(trial.suggest_int(var.name, 0, 1))
                 elif var.type() == VariableType.Spin:
                     var.toBinary()
                     var.binary.setValue(trial.suggest_int(var.name, 0, 1))
                 elif var.type() == VariableType.Integer:
-                    lb = var.getLb(must_number=True)
-                    ub = var.getUb(must_number=True)
+                    lb = var.getLb(number=True)
+                    ub = var.getUb(number=True)
                     var.setValue(trial.suggest_int(var.name, lb, ub))
                 elif var.type() == VariableType.Continuous:
-                    lb = var.getLb(must_number=True)
-                    ub = var.getUb(must_number=True)
+                    lb = var.getLb(number=True)
+                    ub = var.getUb(number=True)
                     var.setValue(trial.suggest_uniform(var.name, lb, ub))
             obj_value = self.getObjValue(solution)
 
             # update best solution if needed
             self.registerSolution(solution, obj_value)
 
             # callback
             self.callback([solution])
 
             return obj_value
 
         self.end_build()
-        search_timelimit = self.timelimit - self.build_time
+        search_timelimit = max(0, self.timelimit - self.build_time)
 
         @timeout_decorator.timeout(search_timelimit, timeout_exception=TimeoutError)
         def optimize():
             self.study.optimize(objective_func, self.n_trial, timeout=search_timelimit)
 
-        optimize()
+        try:
+            optimize()
+        except ValueError as e:
+            logger.warning(e)
+            raise flopt.error.SolverError()
 
         return SolverTerminateState.Normal
 
 
 class OptunaTPESearch(OptunaSearch):
     """
     Tree-structured Parzen Estimator (TPE) Sampling Search of Optuna.
@@ -107,23 +111,22 @@
 
         x = flopt.Variable("x", lowBound=-1, upBound=1, cat="Continuous")
         y = flopt.Variable("y", lowBound=-1, upBound=1, cat="Continuous")
 
         prob = flopt.Problem()
         prob += 2*x*x + x*y + y*y + x + y
 
-        solver = flopt.Solver("OptunaTPESearch")
-        status, log = prob.solve(solver, msg=True, timelimit=1)
+        status, log = prob.solve(solver="OptunaTPE", msg=True, timelimit=1)
 
         print("obj =", flopt.Value(prob.obj))
         print("x =", flopt.Value(x))
         print("y =", flopt.Value(y))
     """
 
-    name = "OptunaTPESearch"
+    name = "OptunaTPE"
 
     def __init__(self):
         super().__init__()
         self.consider_prior = True
         self.prior_weight = 1.0
         self.consider_magic_clip = True
         self.consider_endpoints = False
@@ -152,15 +155,14 @@
 class OptunaCmaEsSearch(OptunaSearch):
     """
     Covariance Matrix Adaptation Evolution Strategy (CMA-ES) search of Optuna.
     https://optuna.readthedocs.io/en/latest/reference/samplers/generated/optuna.samplers.CmaEsSampler.html
 
     Parameters
     ----------
-    x0
     sigma0
     n_startup_trials
     independent_sampler
     warn_independe_sampling
     seed
 
     Examples
@@ -172,40 +174,42 @@
 
         x = flopt.Variable("x", lowBound=-1, upBound=1, cat="Continuous")
         y = flopt.Variable("y", lowBound=-1, upBound=1, cat="Continuous")
 
         prob = flopt.Problem()
         prob += 2*x*x + x*y + y*y + x + y
 
-        solver = flopt.Solver("OptunaCmaEsSearch")
-        status, log = prob.solve(solver, msg=True, timelimit=1)
+        status, log = prob.solve(solver="OptunaCmaEs", msg=True, timelimit=1)
 
         print("obj =", flopt.Value(prob.obj))
         print("x =", flopt.Value(x))
         print("y =", flopt.Value(y))
         >>> obj = -0.2857142857142857
         >>> x = -0.14285714185152507
         >>> y = -0.4285714299429902
     """
 
-    name = "OptunaCmaEsSearch"
+    name = "OptunaCmaEs"
 
     def __init__(self):
         super().__init__()
-        self.x0 = None
         self.sigma0 = None
         self.n_startup_trials = 1
         self.independent_sampler = None
         self.warn_independent_sampling = False
         self.seed = None
 
     def createStudy(self, solution):
         disable_default_handler()
-        if self.x0 is None:
-            x0 = {var.name: var.value() for var in solution}
+        x0 = dict()
+        for var in solution:
+            if var.type() == VariableType.Spin:
+                x0[var.name] = (var.value() + 1) / 2
+            else:
+                x0[var.name] = var.value()
         sampler = CmaEsSampler(
             x0=x0,
             sigma0=self.sigma0,
             n_startup_trials=self.n_startup_trials,
             independent_sampler=self.independent_sampler,
             warn_independent_sampling=self.warn_independent_sampling,
             seed=self.seed,
```

### Comparing `flopt-0.5.5/flopt/solvers/pulp_search.py` & `flopt-0.5.6/flopt/solvers/pulp_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,31 +49,30 @@
 
         # Problem
         prob = flopt.Problem()
         prob += a + b + c + 2
         prob += a + b >= 2
         prob += b - c >= 3
 
-        solver = flopt.Solver("PulpSearch")
-        prob.solve(solver, msg=True)
+        prob.solve(solver="Pulp", msg=True)
 
     When you use other solvers in pulp, for example GLPK solver, you set solver parameter in PulpSearch object.
 
     .. code-block:: python
 
-        solver = flopt.Solver("PulpSearch")
+        solver = flopt.Solver("Pulp")
 
         import pulp
         glpk_solver = pulp.GLPK_CMD()
         solver.setParams(solver=glpk_solver)
         prob.solve(solver, msg=True)
 
     """
 
-    name = "PulpSearch"
+    name = "Pulp"
     can_solve_problems = {
         "Variable": VariableType.Number,
         "Objective": ExpressionType.Linear,
         "Constraint": ExpressionType.Linear,
     }
 
     def __init__(self):
@@ -85,15 +84,15 @@
         lp_prob, lp_solution = self.createLpProblem(solution, self.prob)
         self.end_build()
 
         if self.solver is not None:
             solver = self.solver
         else:
             solver = pulp.PULP_CBC_CMD(
-                timeLimit=self.timelimit - self.build_time, msg=self.msg
+                timeLimit=max(0, self.timelimit - self.build_time), msg=self.msg
             )
 
         lp_status = lp_prob.solve(solver)
 
         # get result
         for lp_var in lp_solution:
             name = lp_var.getName()
@@ -111,16 +110,15 @@
         logger.info(f"PuLP LpStatus {pulp.constants.LpStatus[lp_status]}")
         if lp_status == -1:
             return SolverTerminateState.Infeasible
         elif lp_status == -2:
             return SolverTerminateState.Unbounded
         elif lp_status == -3:
             return SolverTerminateState.Abnormal
-        else:
-            return SolverTerminateState.Normal
+        return SolverTerminateState.Normal
 
     def createLpProblem(self, solution, prob):
         """Convert Problem into pulp.LpProblem
 
         Parameters
         ----------
         solution : Solution
@@ -141,28 +139,29 @@
                 cat = "Binary"
             else:
                 raise ValueError(var.type())
             lp_var = LpVariable(
                 var.name, lowBound=var.getLb(), upBound=var.getUb(), cat=cat
             )
             lp_variables.append(lp_var)
-        lp_solution = Solution("lp_solution", lp_variables)
+        lp_solution = Solution(lp_variables)
 
         # conver Problem -> pulp.LpProblem
         name = "" if self.name is None else self.name
         sense = (
             pulp.LpMinimize
             if prob.sense in {"minimize", "Minimize"}
             else pulp.LpMaximize
         )
         lp_prob = pulp.LpProblem(name=name, sense=sense)
         if not isinstance(prob.obj, Const):
             lp_prob.setObjective(prob.obj.value(lp_solution))
 
         for const in prob.getConstraints():
-            const_exp = const.expression
-            if const.type() == ConstraintType.Eq:
-                lp_prob.addConstraint(const_exp.value(lp_solution) == 0, const.name)
-            else:  # const.type() == ConstraintType.Le
-                lp_prob.addConstraint(const_exp.value(lp_solution) <= 0, const.name)
+            const_exp = const.expression.value(lp_solution)
+            if not isinstance(const_exp, (int, float)):
+                if const.type() == ConstraintType.Eq:
+                    lp_prob.addConstraint(const_exp == 0, const.name)
+                else:  # const.type() == ConstraintType.Le
+                    lp_prob.addConstraint(const_exp <= 0, const.name)
 
         return lp_prob, lp_solution
```

### Comparing `flopt-0.5.5/flopt/solvers/random_search.py` & `flopt-0.5.6/flopt/solvers/random_search.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,23 +18,22 @@
 
         x = flopt.Variable("x", lowBound=-1, upBound=1, cat="Continuous")
         y = flopt.Variable("y", lowBound=-1, upBound=1, cat="Continuous")
 
         prob = flopt.Problem()
         prob += 2*x*x + x*y + y*y + x + y
 
-        solver = flopt.Solver("RandomSearch")
-        status, log = prob.solve(solver, msg=True, timelimit=1)
+        status, log = prob.solve(solver="Random", msg=True, timelimit=1)
 
         print("obj =", flopt.Value(prob.obj))
         print("x =", flopt.Value(x))
         print("y =", flopt.Value(y))
     """
 
-    name = "RandomSearch"
+    name = "Random"
     can_solve_problems = {
         "Variable": VariableType.Any,
         "Objective": ExpressionType.Any,
         "Constraint": ExpressionType.Non,
     }
 
     def __init__(self):
```

### Comparing `flopt-0.5.5/flopt/solvers/scipy_searches/scipy_milp_search.py` & `flopt-0.5.6/flopt/solvers/scipy_searches/scipy_milp_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from scipy import optimize as scipy_optimize
 import numpy as np
 
 from flopt.solvers.base import BaseSearch
 from flopt.convert import LpStructure
-from flopt.variable import VariableArray
+from flopt.container import FloptNdarray
 from flopt.constants import VariableType, ExpressionType, SolverTerminateState
 from flopt.env import setup_logger
 
 
 logger = setup_logger(__name__)
 
 
@@ -35,37 +35,37 @@
 
         # Problem
         prob = flopt.Problem()
         prob += a + b + c + 2
         prob += a + b >= 2
         prob += b - c >= 3
 
-        solver = flopt.Solver("ScipyMilpSearch")
+        solver = flopt.Solver("ScipyMilp")
         prob.solve(solver, msg=True)
 
     See Also
     --------
     scipy.optimize.milp
     """
 
-    name = "ScipyMilpSearch"
+    name = "ScipyMilp"
     can_solve_problems = {
         "Variable": VariableType.Number,
         "Objective": ExpressionType.Linear,
         "Constraint": ExpressionType.Linear,
     }
 
     def search(self, solution, *args):
         self.start_build()
 
         # lp structure
         lp = LpStructure.fromFlopt(
             self.prob,
-            x=VariableArray(solution.getVariables()),
-            option="all_neq",
+            x=solution,
+            option="ineq",
         )
 
         # bounds
         lbs = [_lb if not np.isnan(_lb) else -np.inf for _lb in lp.lb]
         ubs = [_ub if not np.isnan(_ub) else np.inf for _ub in lp.ub]
         bounds = scipy_optimize.Bounds(lbs, ubs)
 
@@ -79,15 +79,18 @@
             constraints = scipy_optimize.LinearConstraint(lp.G, lb, lp.h)
         else:
             constraints = None
 
         self.end_build()
 
         # options
-        options = {"disp": self.msg, "time_limit": self.timelimit - self.build_time}
+        options = {
+            "disp": self.msg,
+            "time_limit": max(0, self.timelimit - self.build_time),
+        }
 
         # search
         res = scipy_optimize.milp(
             c=lp.c,
             constraints=constraints,
             integrality=integrality,
             bounds=bounds,
@@ -105,9 +108,8 @@
             return SolverTerminateState.Normal
         elif res.status == 1:
             return SolverTerminateState.Timelimit
         elif res.status == 2:
             return SolverTerminateState.Infeasible
         elif res.status == 3:
             return SolverTerminateState.Unbounded
-        else:
-            return SolverTerminateState.Abnormal
+        return SolverTerminateState.Abnormal
```

### Comparing `flopt-0.5.5/flopt/solvers/scipy_searches/scipy_search.py` & `flopt-0.5.6/flopt/solvers/scipy_searches/scipy_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,27 +33,26 @@
 
         # Problem
         prob = flopt.Problem()
         prob += a*a + a*b + b + c + 2
         prob += a + b >= 2
         prob += b - c == 3
 
-        solver = flopt.Solver("ScipySearch")
-        prob.solve(solver, msg=True)
+        prob.solve(solver="Scipy", msg=True)
 
         print(flopt.Value([a, b, c]))
         >>> [0, 2.9999999999999996, 0.0]
 
 
     See Also
     --------
     scipy.optimize.minimize
     """
 
-    name = "ScipySearch"
+    name = "Scipy"
     can_solve_problems = {
         "Variable": VariableType.Number,
         "Objective": ExpressionType.Any,
         "Constraint": ExpressionType.Any,
     }
 
     def __init__(self):
@@ -82,15 +81,15 @@
 
             return func
 
         # initial point
         x0 = [var.value() for var in solution]
 
         # bounds
-        lb, ub = list(), list()
+        lb, ub = [], []
         for var in solution:
             if var.type() == VariableType.Spin:
                 lb.append(0)
                 ub.append(1)
             else:
                 lb.append(l if (l := var.getLb()) is not None else -np.inf)
                 ub.append(u if (u := var.getUb()) is not None else np.inf)
@@ -136,14 +135,20 @@
             args=(),
             method=self.method,
             jac=None,
             hess=None,
             hessp=None,
             tol=None,
         )
+        if self.msg:
+            print()
+            print("-" * 20 + " ScipySearch " + "-" * 20)
+            print(res)
+            print("-" * 20 + "-------------" + "-" * 20)
+            print()
 
         if res.success:
             # get result of solver
             solution.setValuesFromArray(res.x)
             self.registerSolution(solution)
             return SolverTerminateState.Normal
         else:
```

### Comparing `flopt-0.5.5/flopt/solvers/shuffled_frog_leaping_search.py` & `flopt-0.5.6/flopt/solvers/shuffled_frog_leaping_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
             lo = mid + 1
         else:
             hi = mid
     return lo
 
 
 class Frog(Solution):
-    def __init__(self, solution, prob):
-        super().__init__()
-        self._variables = solution._variables
-        self.prob = prob
-        self.obj_value = None
+    def __new__(cls, solution, prob):
+        obj = super().__new__(cls, solution._variables, sort=False)
+        obj.prob = prob
+        obj.obj_value = None
+        return obj
 
     def setObjValue(self):
         self.obj_value = self.prob.getObjValue(self)
 
     def getObjValue(self):
         if self.obj_value is None:
             self.setObjValue()
@@ -40,14 +40,17 @@
         super().random()
         self.obj_value = None
 
     def clip(self):
         super().clip()
         self.obj_value = None
 
+    def clone(self):
+        return Frog(super().clone(), self.prob)
+
 
 class ShuffledFrogLeapingSearch(BaseSearch):
     """
     SFLA (Shuffled Frog Leaping Search)
     It has a incumbent solution anytime.
 
     1. Generate new solutions as frogs at random.
@@ -81,16 +84,15 @@
 
         x = flopt.Variable("x", lowBound=-1, upBound=1, cat="Continuous")
         y = flopt.Variable("y", lowBound=-1, upBound=1, cat="Continuous")
 
         prob = flopt.Problem()
         prob += 2*x*x + x*y + y*y + x + y
 
-        solver = flopt.Solver("SFLA")
-        status, log = prob.solve(solver, msg=True, timelimit=1)
+        status, log = prob.solve(solver="SFLA", msg=True, timelimit=1)
 
         print("obj =", flopt.Value(prob.obj))
         print("x =", flopt.Value(x))
         print("y =", flopt.Value(y))
     """
 
     name = "SFLA"
@@ -143,17 +145,18 @@
     def _memetic_evolution(self, solution):
         """
         memetic evolution
         This function is the key to this method.
         """
         M = self.n_memeplex
         N = self.n_frog_per_memeplex
+        frog = Frog(solution, self)
         if self.frogs[-2].getObjValue() - self.frogs[0].getObjValue() < 1e-9:
             logger.debug(f"reset frogs: #frogs {N} --> {N*2}")
-            new_frogs = [Frog(solution.clone(), self) for _ in range(M * N)]
+            new_frogs = [frog.clone() for _ in range(M * N)]
             self.frogs += new_frogs
             for frog in self.frogs[1:]:
                 frog.setRandom()
             self.frogs.sort(key=lambda frog: frog.getObjValue())
             self.n_frog_per_memeplex *= 2
             N = self.n_frog_per_memeplex
 
@@ -169,24 +172,24 @@
                 worst_frog = self.memeplexes[j][last]
 
                 # move frog which has the worst objective
                 step = best_frog - worst_frog
                 step *= random.random()
                 if (norm := step.norm()) > self.max_step:
                     step *= self.max_step / norm
-                new_frog = Frog(worst_frog + step, self)
+                new_frog = worst_frog + step
                 new_frog.clip()
 
                 # if it does not improve (1)
                 if new_frog.getObjValue() > worst_frog.getObjValue():
                     step = self.best_solution - worst_frog
                     step *= random.random()
                     if (norm := step.norm()) > self.max_step:
                         step *= self.max_step / norm
-                    new_frog = Frog(worst_frog + step, self)
+                    new_frog = worst_frog + step
                     new_frog.clip()
 
                     # if it does not improve (2)
                     if new_frog.getObjValue() > worst_frog.getObjValue():
                         new_frog.setRandom()
 
                 # replace the worst_frog to new frog and sort memeplex
@@ -201,25 +204,26 @@
                     )
 
                 # check time limit
                 self.raiseTimeoutIfNeeded()
 
         # sort entire memeplexes
         self.frogs = [frog for memeplex in self.memeplexes for frog in memeplex]
-        self.frogs.sort(key=lambda frog: self.getObjValue(frog))
+        self.frogs.sort(key=self.getObjValue)
 
     def startProcess(self, solution):
         super().startProcess()
         if self.has_initialized:
             return
         self.start_build()
 
         M = self.n_memeplex
         N = self.n_frog_per_memeplex
-        self.frogs = [Frog(solution.clone(), self) for _ in range(M * N)]
+        frog = Frog(solution.clone(), self)
+        self.frogs = [frog.clone() for _ in range(M * N)]
         for frog in self.frogs:
             frog.setRandom()
         self.frogs.sort(key=lambda frog: frog.getObjValue())
         self.registerSolution(self.frogs[0])
 
         self.end_build()
         self.has_initialized = True
```

### Comparing `flopt-0.5.5/flopt/solvers/solver_utils/common.py` & `flopt-0.5.6/flopt/solvers/solver_utils/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,17 +93,20 @@
         f"{relative_gap_str}",
         f"{abs_gap_str}",
         f"{time:7.2f}",
     )
     print(" ".join(message))
 
 
-def end_solver_message(status, obj_value, build_time, elapsed_time, num_trials):
+def end_solver_message(status, obj_value, build_time, elapsed_time, num_trials, sense):
+    if sense == "Maximize":
+        obj_value = -obj_value
     message = (
         "",
+        f"Sense: {sense}",
         f"Status: {status.__str__()}",
         f"Objective Value: {obj_value}",
         f"Time: {elapsed_time}",
         f"    Build Time: {build_time}",
         f"    Search Time: {elapsed_time - build_time}",
         f"Trials: {num_trials}",
     )
```

### Comparing `flopt-0.5.5/flopt/solvers/solver_utils/solver_log.py` & `flopt-0.5.6/flopt/solvers/solver_utils/solver_log.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 
 logger = setup_logger(__name__)
 
 
 class Log:
     def __init__(self):
-        self.logs = list()
-        self.solutions = list()
+        self.logs = []
+        self.solutions = []
         heapq.heapify(self.solutions)
 
     def append(self, log_dict):
         self.logs.append(log_dict)
 
     def appendSolution(self, solution, obj_value, max_k):
         if len(self.solutions) < max_k:
```

### Comparing `flopt-0.5.5/flopt/solvers/two_opt.py` & `flopt-0.5.6/flopt/solvers/two_opt.py`

 * *Files identical despite different names*

### Comparing `flopt-0.5.5/flopt.egg-info/PKG-INFO` & `flopt-0.5.6/flopt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: flopt
-Version: 0.5.5
+Version: 0.5.6
 Summary: A python Non-Linear Programming API with Heuristic approach
 Home-page: https://flopt.readthedocs.io/en/latest/index.html
 Author: nariaki tateiwa
 Author-email: nariaki3551@gmail.com
 License: MIT
 Keywords: optimization nonliear search heuristics algorithm
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flopt
 
 A Python Flexible Modeler for Optimization Problems.<br><br>
-flopt allows modeling of various problems such as LP, QP, Ising, QUBO, etc.<br>
-Users can also solve the modeled problem using some solvers and obtain the optimal or good solutions.
+
+flopt is a modeling tool for optimization problems such as LP, QP, Ising, QUBO, etc.
+flopt provides various functions for flexible and easy modeling.
+Users can also solve modeled problems with several solvers to obtain optimal or good solutions.
 
 [![Documentation Status](https://readthedocs.org/projects/flopt/badge/?version=latest)](https://flopt.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/flopt.svg)](https://badge.fury.io/py/flopt) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flopt) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 [documentation](https://flopt.readthedocs.io/en/latest/) | [tutorial](https://flopt.readthedocs.io/en/latest/tutorial/index.html) | [case studies](https://flopt.readthedocs.io/en/latest/case_studies/index.html)
 
 <br>
 
@@ -78,27 +79,27 @@
 <br>
 
 ## Simple Example
 
 You  can write codes like PuLP application.
 
 ```python
-from flopt import Variable, Problem, Solver
+from flopt import Variable, Problem
 
 # Variables
 a = Variable('a', lowBound=0, upBound=1, cat='Continuous')
 b = Variable('b', lowBound=1, upBound=2, cat='Continuous')
 c = Variable('c', upBound=3, cat='Continuous')
 
 # Problem
 prob = Problem()
 prob += 2 * (3*a+b) * c**2 + 3 # set the objective function
 prob += a + b * c <= 3         # set the constraint
 
-# Solver
+# Solve
 prob.solve(timelimit=0.5, msg=True) # run solver to solve the problem
 
 # display the result, incumbent solution
 print('obj value', prob.getObjectiveValue())
 print('a', a.value())
 print('b', b.value())
 print('c', c.value())
@@ -115,32 +116,32 @@
 a = Variable('a', lowBound=0, upBound=1, cat='Integer')
 b = Variable('b', lowBound=1, upBound=2, cat='Continuous')
 
 def user_func(a, b):
     from math import sin, cos
     return (0.7*a + 0.3*cos(b)**2 + 0.1*sin(b))*abs(a)
 
-custom_obj = CustomExpression(func=user_func, arg=[a, b])
+custom_obj = CustomExpression(func=user_func, args=[a, b])
 
 prob = Problem(name='CustomExpression')
 prob += custom_obj
 
-# Solver
+# Solve
 prob.solve(timelimit=1, msg=True)  # run solver to solve the problem
 
 # display the result, incumbent solution
 print('obj value', prob.getObjectiveValue())
 ```
 
 <br>
 
 In the case you solve TSP, *Permutation Variable* is useful.
 
 ```python
-from flopt import Variable, Problem, Solver, CustomExpression
+from flopt import Variable, Problem, CustomExpression
 
 N = 4  # Number of city
 D = [[0,1,2,3],  # Distance matrix
      [3,0,2,1],
      [1,2,0,3],
      [2,3,1,0]]
 
@@ -149,21 +150,21 @@
 
 # Object
 def tsp_dist(x):
     distance = 0
     for head, tail in zip(x, x[1:]+[x[0]]):
         distance += D[head][tail]  # D is the distance matrix
     return distance
-tsp_obj = CustomExpression(func=tsp_dist, arg=[x])
+tsp_obj = CustomExpression(func=tsp_dist, args=[x])
 
 # Problem
 prob = Problem(name='TSP')
 prob += tsp_obj
 
-# Solver
+# Solve
 prob.solve(timelimit=10, msg=True)    # run solver to solve the problem
 
 # display the result, incumbent solution
 print('obj value', prob.getObjectiveValue())
 print('x', x.value())
 ```
```

### Comparing `flopt-0.5.5/flopt.egg-info/SOURCES.txt` & `flopt-0.5.6/flopt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 datasets/funcLib/Bukin.py
 datasets/funcLib/Camel.py
 datasets/funcLib/DeJongF3.py
 datasets/funcLib/Easom.py
 datasets/funcLib/Eggholder.py
 datasets/funcLib/Ellipsoid.py
 datasets/funcLib/FiveWell.py
+datasets/funcLib/G1.py
 datasets/funcLib/Goldstain.py
 datasets/funcLib/Griewank.py
 datasets/funcLib/Ktable.py
 datasets/funcLib/Levi.py
 datasets/funcLib/Matyas.py
 datasets/funcLib/McCormick.py
 datasets/funcLib/Michalewicz.py
@@ -24,25 +25,26 @@
 datasets/funcLib/Schaffer2.py
 datasets/funcLib/Schaffer4.py
 datasets/funcLib/Schwefel.py
 datasets/funcLib/Shuberts.py
 datasets/funcLib/SixHump.py
 datasets/funcLib/Sphere.py
 datasets/funcLib/SumDiffPower.py
-datasets/funcLib/WeitedSphere.py
+datasets/funcLib/WeightedSphere.py
 datasets/funcLib/XinShe.py
 datasets/funcLib/Zahkarov.py
 datasets/funcLib/__init__.py
 flopt/__init__.py
+flopt/apis.py
 flopt/constants.py
 flopt/constraint.py
+flopt/container.py
 flopt/env.py
 flopt/error.py
 flopt/expression.py
-flopt/flopt.config
 flopt/polynomial.py
 flopt/problem.py
 flopt/solution.py
 flopt/utils.py
 flopt/variable.py
 flopt.egg-info/PKG-INFO
 flopt.egg-info/SOURCES.txt
@@ -60,25 +62,25 @@
 flopt/performance/func_dataset.py
 flopt/performance/log_visualizer.py
 flopt/performance/mip_dataset.py
 flopt/performance/performance.py
 flopt/performance/tsp_dataset.py
 flopt/solvers/__init__.py
 flopt/solvers/amplify_search.py
+flopt/solvers/auto_search.py
 flopt/solvers/base.py
-flopt/solvers/cvxopt_qp_search.py
+flopt/solvers/cvxopt_search.py
 flopt/solvers/hyperopt_search.py
 flopt/solvers/optuna_searches.py
 flopt/solvers/pulp_search.py
 flopt/solvers/random_search.py
+flopt/solvers/selector.py
 flopt/solvers/shuffled_frog_leaping_search.py
+flopt/solvers/steepest_descent.py
 flopt/solvers/two_opt.py
-flopt/solvers/auto_search/__init__.py
-flopt/solvers/auto_search/auto_search.py
-flopt/solvers/auto_search/selector.py
 flopt/solvers/scipy_searches/__init__.py
 flopt/solvers/scipy_searches/scipy_milp_search.py
 flopt/solvers/scipy_searches/scipy_search.py
 flopt/solvers/solver_utils/__init__.py
 flopt/solvers/solver_utils/common.py
 flopt/solvers/solver_utils/solver_log.py
 tests/__init__.py
@@ -94,13 +96,12 @@
 tests/test_Solution.py
 tests/test_Solver.py
 tests/test_VarBinary.py
 tests/test_VarContinuous.py
 tests/test_VarInteger.py
 tests/test_VarPermutation.py
 tests/test_VarSpin.py
-tests/test_VariableArray.py
 tests/test_VariableFactory.py
 tests/test_example.py
 tests/test_linearize.py
 tests/test_logger.py
 tests/test_utils.py
```

### Comparing `flopt-0.5.5/setup.py` & `flopt-0.5.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,39 +10,39 @@
 setup(
     name="flopt",
     packages=find_packages(),
     package_data={
         "flopt": ["flopt.config"],
     },
     include_package_data=True,
-    version="0.5.5",
+    version="0.5.6",
     license="MIT",
     install_requires=[
         "numpy",
         "sympy",
-        "matplotlib==3.5.2",
+        "matplotlib",
         "pulp",
-        "optuna==2.10.1",
+        "optuna",
         "hyperopt",
         "cvxopt",
         "amplify",
         "pytest",
         "scipy",
         "scikit-learn",
         "dill",
         "pooch",
         "timeout_decorator",
+        "colorlog",
     ],
     author="nariaki tateiwa",
     author_email="nariaki3551@gmail.com",
     url="https://flopt.readthedocs.io/en/latest/index.html",
     description="A python Non-Linear Programming API with Heuristic approach",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="optimization nonliear search heuristics algorithm",
     classifiers=[
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
 )
```

### Comparing `flopt-0.5.5/tests/test_Constraint.py` & `flopt-0.5.6/tests/test_Constraint.py`

 * *Files identical despite different names*

### Comparing `flopt-0.5.5/tests/test_Convert.py` & `flopt-0.5.6/tests/test_Convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,42 @@
 import pytest
 
 import numpy as np
 
 import flopt
+import flopt.convert
 from flopt import Variable, Problem, Solver
 
 
+def test_QuadraticStructure():
+    from flopt.convert import QuadraticStructure
+
+    Q = [[1, 1], [1, 2]]
+    c = [1, 1]
+    C = 0
+    qs = QuadraticStructure(Q, c, C)
+    try:
+        qs.toLinear()
+    except flopt.ConversionError:
+        assert True
+        return True
+    assert False
+
+    Q = None
+    c = [1, 1]
+    C = 0
+    qs = QuadraticStructure(Q, c, C)
+    try:
+        qs.toLinear()
+    except flopt.ConversionError:
+        assert False
+        return True
+    assert True
+
+
 def test_flopt_to_qp1():
     # Variables
     a = Variable("a", cat="Binary")
     b = Variable("b", cat="Binary")
     c = Variable("c", lowBound=-1, upBound=2, cat="Integer")
     d = Variable("d", lowBound=-2, upBound=1, cat="Continuous")
 
@@ -22,16 +49,16 @@
     print(prob)
 
     from flopt.convert import QpStructure
 
     qp = QpStructure.fromFlopt(prob, progress=True)
     print(qp)
 
-    qp.toAllEq()
-    qp.toAllNeq()
+    qp.toEq()
+    qp.toIneq()
     qp.show()
 
 
 def test_flopt_to_qp2():
     # Variables
     a = Variable("a", cat="Binary")
     b = Variable("b", cat="Binary")
@@ -42,16 +69,16 @@
     print(prob)
 
     from flopt.convert import QpStructure
 
     qp = QpStructure.fromFlopt(prob)
     print(qp)
 
-    qp.toAllEq()
-    qp.toAllNeq()
+    qp.toEq()
+    qp.toIneq()
     qp.toLp()
     qp.toIsing()
     qp.toQubo()
 
 
 def test_flopt_to_qp3():
 
@@ -91,16 +118,16 @@
     print(prob)
 
     from flopt.convert import LpStructure
 
     lp = LpStructure.fromFlopt(prob)
     print(lp)
 
-    lp.toAllEq()
-    lp.toAllNeq()
+    lp.toEq()
+    lp.toIneq()
     lp.toQp()
     lp.show()
 
 
 def test_flopt_to_lp2():
     # Variables
     a = Variable("a", cat="Binary")
@@ -112,22 +139,22 @@
     print(prob)
 
     from flopt.convert import LpStructure
 
     lp = LpStructure.fromFlopt(prob)
     print(lp)
 
-    lp.toAllEq()
-    lp.toAllNeq()
+    lp.toEq()
+    lp.toIneq()
     lp.toQp()
     lp.toIsing()
     lp.toQubo()
 
 
-def test_flopt_to_lp_allneq():
+def test_flopt_to_lp_ineq():
     # Variables
     a = Variable("a", cat="Binary")
     b = Variable("b", cat="Binary")
     c = Variable("c", lowBound=-1, upBound=2, cat="Integer")
     d = Variable("d", lowBound=-2, upBound=1, cat="Continuous")
 
     # Problem
@@ -136,18 +163,18 @@
     prob += a + c == 0  # set the constraint
     prob += a + b <= 1  # set the constraint
     prob += a + d >= -1  # set the constraint
     print(prob)
 
     from flopt.convert import LpStructure
 
-    lp = LpStructure.fromFlopt(prob, option="all_neq")
+    lp = LpStructure.fromFlopt(prob, option="ineq")
 
 
-def test_flopt_to_lp_alleq():
+def test_flopt_to_lp_eq():
     # Variables
     a = Variable("a", cat="Binary")
     b = Variable("b", cat="Binary")
     c = Variable("c", lowBound=-1, upBound=2, cat="Integer")
     d = Variable("d", lowBound=-2, upBound=1, cat="Continuous")
 
     # Problem
@@ -156,15 +183,15 @@
     prob += a + c == 0  # set the constraint
     prob += a + b <= 1  # set the constraint
     prob += a + d >= -1  # set the constraint
     print(prob)
 
     from flopt.convert import LpStructure
 
-    lp = LpStructure.fromFlopt(prob, option="all_eq")
+    lp = LpStructure.fromFlopt(prob, option="eq")
 
 
 def test_flopt_to_lp1():
     # Variables
     a = Variable("a", cat="Binary")
     b = Variable("b", cat="Binary")
     c = Variable("c", lowBound=-1, upBound=2, cat="Integer")
@@ -179,16 +206,16 @@
     print(prob)
 
     from flopt.convert import LpStructure
 
     lp = LpStructure.fromFlopt(prob)
     print(lp)
 
-    lp.toAllEq()
-    lp.toAllNeq()
+    lp.toEq()
+    lp.toIneq()
     lp.toQp()
 
 
 def test_flopt_to_lp1():
     # Variables
     a = Variable("a", cat="Binary")
     b = Variable("b", cat="Binary")
@@ -199,16 +226,16 @@
     print(prob)
 
     from flopt.convert import LpStructure
 
     lp = LpStructure.fromFlopt(prob)
     print(lp)
 
-    lp.toAllEq()
-    lp.toAllNeq()
+    lp.toEq()
+    lp.toIneq()
     lp.toQp()
     lp.toIsing()
     lp.toQubo()
 
 
 def test_flopt_to_ising1():
     a = Variable(name="a", ini_value=1, cat="Spin")
@@ -319,15 +346,15 @@
     prob += a + c == 0  # set the constraint
     prob += a + b <= 1  # set the constraint
     prob += a + d >= -1  # set the constraint
 
     print(prob)
 
     # check wheter prob can be converted into pulp modeling
-    assert Solver(algo="PulpSearch").available(prob)
+    assert Solver(algo="Pulp").available(prob)
 
     # convert flopt to pulp
     from flopt.convert import flopt_to_pulp
 
     lp_prob, lp_solution = flopt_to_pulp(prob)
     print(lp_prob)
     print(lp_solution)
@@ -342,27 +369,27 @@
     lb = [0, 0, 0]
     ub = [1, 1, 1]
     var_types = ["Binary", "Binary", "Continuous"]
 
     from flopt.convert import LpStructure
 
     prob = LpStructure(c, C, A=A, b=b, lb=lb, ub=ub, types=var_types).toFlopt()
-    print(prob.show())
+    prob.show()
 
 
 def test_ising_to_flopt():
     # make Ising model
     J = [[1, 2, 1], [0, 1, 1], [0, 0, 3]]
     h = [1, 2, 0]
     C = 0
 
     from flopt.convert import IsingStructure
 
     prob = IsingStructure(J, h, C).toFlopt()
-    print(prob.show())
+    prob.show()
 
 
 def test_qubo_to_flopt():
     # make Qubo model
     Q = [[1, 2, 1], [0, 1, 1], [0, 0, 3]]
     C = 10
 
@@ -388,15 +415,15 @@
     prob += c >= 0  # set the constraint
 
     print(prob)
 
     from flopt.convert import pulp_to_flopt
 
     flopt_prob = pulp_to_flopt(prob)
-    print(flopt_prob.show())
+    flopt_prob.show()
 
 
 def test_pulp_to_flopt2():
     import pulp
 
     # Variables
     a = pulp.LpVariable("a", lowBound=0, upBound=1, cat="Integer")
```

### Comparing `flopt-0.5.5/tests/test_CustomExpression.py` & `flopt-0.5.6/tests/test_CustomExpression.py`

 * *Files identical despite different names*

### Comparing `flopt-0.5.5/tests/test_Expression.py` & `flopt-0.5.6/tests/test_Expression.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pytest
 import numpy as np
 
+import flopt
 from flopt import Variable
-from flopt.expression import Const
+from flopt.polynomial import Monomial, Polynomial
+from flopt.expression import Expression, Const
 from flopt.env import get_variable_lower_bound, get_variable_upper_bound
 
 
 @pytest.fixture(scope="function")
 def a():
     return Variable(name="a", lowBound=1, upBound=5, ini_value=2, cat="Continuous")
 
@@ -100,14 +102,30 @@
     a = Variable(name="a", ini_value=2, cat="Integer")
     b = Variable(name="b", ini_value=1, cat="Integer")
     c = a + b
     assert (c | 1).value() == c.value() | 1
     assert (1 | c).value() == 1 | c.value()
 
 
+def test_Expression_setPolynomial(a, b, c):
+    assert (a + b).setPolynomial() == Polynomial(
+        {Monomial({a: 1}): 1, Monomial({b: 1}): 1}
+    )
+    assert (a + b + c).setPolynomial() == Polynomial(
+        {Monomial({a: 1}): 2, Monomial({b: 1}): 2}
+    )
+    assert (3 * a).setPolynomial() == Polynomial({Monomial({a: 1}): 3})
+    assert (a * 3).setPolynomial() == Polynomial({Monomial({a: 1}): 3})
+    assert (a / 3).setPolynomial() == Polynomial({Monomial({a: 1}): 1.0 / 3})
+    assert (2 * a**3).setPolynomial() == Polynomial({Monomial({a: 3}): 2})
+    assert (a - b).setPolynomial() == Polynomial(
+        {Monomial({a: 1}): 1, Monomial({b: 1}): -1}
+    )
+
+
 def test_Expression_getVariable(a, b, c):
     assert c.getVariables() == {a, b}
 
 
 def test_Expression_constant1(a):
     assert (a + 1).constant() == 1
 
@@ -120,16 +138,44 @@
     assert (2 * a).isMonomial() == True
     assert (2 * a * b).isMonomial() == True
     assert (a + 1).isMonomial() == False
     assert (a / b).isMonomial() == False
 
 
 def test_Expression_isMonomial2(a, b):
-    (2 * a).toMonomial()
-    (2 * a * b).toMonomial()
+    assert (2 * a).toMonomial() == Monomial({a: 1}, coeff=2)
+    assert (2 * a * b).toMonomial() == Monomial({a: 1, b: 1}, coeff=2)
+
+
+def test_Expression_toLinear1(a, b):
+    lp = (a + b + 1).toLinear([a, b])
+    assert lp.C == 1
+    assert np.all(lp.c == [1, 1])
+
+
+def test_Expression_toLinear2(a, b):
+    lp = (a + b + 1).toLinear([a])
+    # assert (lp.C).value() == (b + 1).value()
+    assert lp.C == (b + 1).value()
+    assert np.all(lp.c == [1])
+
+
+def test_Expression_toQuadratic1(a, b):
+    qp = (a * a + a * b + b + 1).toQuadratic([a, b])
+    assert np.all(qp.Q == [[2, 1], [1, 0]])
+    assert np.all(qp.c == [0, 1])
+    assert qp.C == 1
+
+
+def test_Expression_toQuadratic2(a, b):
+    qp = (a * a + a * b + b + 1).toQuadratic([a])
+    assert np.all(qp.Q == [[2]])
+    assert np.all(qp.c == [b])
+    # assert (qp.C).value() == (b + 1).value()
+    assert qp.C == (b + 1).value()
 
 
 def test_Expression_simplify(a, b):
     (a + 1 - a).simplify()
     (a * a + a * b + a).simplify()
 
 
@@ -152,15 +198,15 @@
     s = Variable("ss", cat="Spin")
     i = Variable("ii", lowBound=-1, upBound=1, cat="Integer")
     print((b + 1).toSpin())
     print((s + 1).toSpin())
     print((i + 1).toSpin())
 
 
-def test_Expression_max(a, b, c):
+def test_Expression_max():
     a = Variable(name="a", lowBound=1, upBound=5)
     b = Variable(name="b", lowBound=1, upBound=5)
     c = a + b
     assert np.isclose((a + b + c).max(), 20)
 
     assert np.isclose((a * a).max(), 25)
 
@@ -169,15 +215,15 @@
 
     # unbounded
     z = Variable("z")
     assert np.isclose(z.max(), get_variable_upper_bound())
     assert np.isclose((z + 1.0).max(), get_variable_upper_bound())
 
 
-def test_Expression_min(a, b, c):
+def test_Expression_min():
     a = Variable(name="a", lowBound=1, upBound=5)
     b = Variable(name="b", lowBound=1, upBound=5)
     c = a + b
     assert np.isclose((a + b + c).min(), 4)
 
     assert np.isclose((a * a).min(), 1)
 
@@ -214,14 +260,36 @@
 
 def test_Expression_isLinear(a, b, c):
     assert a.isLinear() == True
     assert c.isLinear() == True
     assert (a * b).isLinear() == False
 
 
+def test_Expression_fromPolynominal():
+    x = Variable("x", cat="Integer")
+    y = Variable("y", cat="Integer")
+    polynomial = Polynomial({Monomial({x: 3}): 1, Monomial({y: 2}): 2})  # x^3 + 2*y^2
+    print(Expression.fromPolynomial(polynomial))
+
+
+def test_Expression_jac1():
+    x = Variable.array("x", 2, cat="Integer")
+    exp = x[0] ** 3 + 2 * x[1] ** 2 + x[0] * x[1]
+    jac = exp.jac(x)
+    assert jac[0] == 3 * x[0] ** 2 + x[1]
+    assert jac[1] == 4 * x[1] + x[0]
+
+
+def test_Expression_jac2():
+    x = Variable.array("x", 2, cat="Integer")
+    exp1 = flopt.Sum(x * x)
+    exp2 = x[0] * x[0] + x[1] * x[1]
+    assert np.all(exp1.jac(x) == exp2.jac(x))
+
+
 def test_Const_constant():
     assert Const(1).constant() == 1
 
 
 def test_Const_setPolynominal():
     Const(0).setPolynomial()
 
@@ -301,7 +369,60 @@
             [1, 2],
             [0, 1],
         ]
     )
     h = np.array([1, 2])
     obj = -(x.T).dot(J).dot(x) - (h.T).dot(x)
     obj.toIsing()
+
+
+def test_Expression_Exp1(a):
+    exp = flopt.exp(a)
+    assert exp.value() == np.exp(a.value())
+    assert exp.getName() == "Exp(a)"
+    assert list(exp.getChildren()) == [a]
+    assert exp.isPolynomial() == False
+    assert exp.getVariables() == {a}
+    assert exp.isNeg() == False
+    assert exp.__repr__()
+
+
+def test_Expression_Exp2():
+    x = flopt.Variable.array("x", 2)
+    exp = flopt.exp(x)
+    assert exp[0] == flopt.exp(x[0])
+    assert exp[1] == flopt.exp(x[1])
+
+
+def test_Expression_Cos(a):
+    exp = flopt.cos(a)
+    assert exp.value() == np.cos(a.value())
+    assert exp.getName() == "Cos(a)"
+
+
+def test_Expression_Sin(a):
+    exp = flopt.sin(a)
+    assert exp.value() == np.sin(a.value())
+    assert exp.getName() == "Sin(a)"
+
+
+def test_Expression_Log(a):
+    exp = flopt.log(a)
+    assert exp.value() == np.log(a.value())
+    assert exp.getName() == "Log(a)"
+
+
+def test_Expression_Abs(a):
+    exp = flopt.abs(a)
+    assert exp.value() == np.abs(a.value())
+    assert exp.getName() == "Abs(a)"
+
+
+def test_Expression_Floor(a):
+    exp = flopt.floor(a)
+    assert exp.value() == np.floor(a.value())
+    assert exp.getName() == "Floor(a)"
+
+
+def test_Expression_Ceil(a):
+    exp = flopt.ceil(a)
+    assert exp.getName() == "Ceil(a)"
```

### Comparing `flopt-0.5.5/tests/test_Performance.py` & `flopt-0.5.6/tests/test_Performance.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 def test_tsp_dataset():
     dataset = flopt.performance.get_dataset("tsp")
     instance = dataset["test8"]
 
     # lp
-    milp = Solver("ScipyMilpSearch")
+    milp = Solver("ScipyMilp")
     solvable, prob = instance.createProblem(milp)
     assert solvable
     prob.solve(milp, msg=True)
     obj_value = prob.getObjectiveValue()
 
     # 2-opt
     two_opt = Solver("2-Opt")
@@ -41,39 +41,39 @@
     prob.solve(two_opt, timelimit=0.5, msg=True)
 
 
 def test_func_dataset():
     dataset = flopt.performance.get_dataset("func")
     instance = dataset["Ackley"]
 
-    scipy_search = Solver("ScipySearch")
+    scipy_search = Solver("Scipy")
     solvable, prob = instance.createProblem(scipy_search)
     assert solvable
     prob.solve(scipy_search, msg=True)
 
 
 def test_mip_dataset():
     dataset = flopt.performance.get_dataset("mip")
     instance = dataset["markshare2"]
-    scipy_search = Solver("ScipyMilpSearch")
+    scipy_search = Solver("ScipyMilp")
     solvable, prob = instance.createProblem(scipy_search)
     assert solvable
-    prob.solve(scipy_search, msg=True)
+    prob.solve(scipy_search, timelimit=0.5, msg=True)
 
 
 def test_Dataset_list():
     flopt.performance.Dataset_list()
 
 
 def test_compute_nosolver(prob):
     logs = flopt.performance.compute(prob, timelimit=0.5, msg=True)
 
 
 def test_compute_RandomSearch(prob):
-    rs_solver = Solver("RandomSearch")
+    rs_solver = Solver("Random")
     logs = flopt.performance.compute(prob, rs_solver, timelimit=0.1, msg=True)
 
 
 def test_CustomDataset(prob):
     cd = CustomDataset(name="user")
     cd += prob  # add problem
```

### Comparing `flopt-0.5.5/tests/test_Polynomial.py` & `flopt-0.5.6/tests/test_Polynomial.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,31 @@
 def test_Monomial_constructer(x, y):
     print(Monomial({x: 1}))
     print(Monomial({x: 2}))
     print(Monomial({x: 2, y: 2}))
     print(Monomial({x: 2, y: 2}, 3))
 
 
-def test_Monomial_mul(x, y):
+def test_Monomial_mul1(x, y):
     a = Monomial({x: 1})  # x
     b = Monomial({y: 2})  # y^2
     assert a * b == Monomial({x: 1, y: 2})
     assert 2 * a == Monomial({x: 1}, coeff=2)
     assert a * 2 == Monomial({x: 1}, coeff=2)
 
 
+def test_Monomial_mul2(x, y):
+    a = Monomial({x: 1})  # x
+    b = Monomial({y: 2})  # y^2
+    a *= 2
+    b *= 2
+    assert a == Monomial({x: 1}, coeff=2)
+    assert b == Monomial({y: 2}, coeff=2)
+
+
 def test_Monomial_pow(x, y):
     a = Monomial({x: 1})  # x
     b = Monomial({y: 2})  # y^2
     assert (2 * a * b * b) ** 3 == Monomial({x: 3, y: 12}, coeff=8)
 
 
 def test_Monomial_toPolynomial(x, y):
@@ -129,14 +138,15 @@
     assert p.coeff(x, x) == 1
     assert p.coeff(x, x, x) == 0
 
 
 def test_Polynomial_isConstant(x, y, a, b):
     assert Polynomial(constant=2).isConstant() == True
     assert Polynomial(constant=2).constant() == 2
+    assert Polynomial(constant=2).toMonomial() == Monomial(coeff=2)
     assert a.isConstant() == False
 
 
 def test_Polynomial_str(a):
     print(a)
     print(b)
```

### Comparing `flopt-0.5.5/tests/test_Problem.py` & `flopt-0.5.6/tests/test_Problem.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 import numpy as np
 
 from flopt import Variable, Problem, CustomExpression, Solver, Sum
+import flopt.constants
 
 
 def test_Problem_obj():
     a = Variable("a", ini_value=1, cat="Integer")
     b = Variable("b", ini_value=1, cat="Continuous")
 
     prob = Problem()
@@ -24,29 +25,74 @@
 
 def test_Problem_obj3():
     prob = Problem()
     prob += 1
     assert prob.getObjectiveValue() == 1
 
 
+def test_Problem_clone():
+    a = Variable("a", ini_value=1, cat="Integer")
+    b = Variable("b", ini_value=1, cat="Continuous")
+
+    prob = Problem()
+    prob += a + 2 * b
+    prob += a + b >= 3
+    cloned_prob = prob.clone()
+    assert cloned_prob.sense == prob.sense
+    assert cloned_prob.obj == prob.obj
+    assert cloned_prob.constraints == prob.constraints
+
+
+def test_Problem_toEq():
+    a = Variable("a", ini_value=1, cat="Integer")
+    b = Variable("b", ini_value=1, cat="Continuous")
+
+    prob = Problem()
+    prob += a + 2 * b
+    prob += a + b >= 3
+    eq_prob = prob.toEq()
+    assert len(eq_prob.getVariables()) == 3
+    assert len(prob.getVariables()) == 2
+    assert all(
+        const.type() == flopt.constants.ConstraintType.Eq
+        for const in eq_prob.constraints
+    )
+
+
+def test_Problem_toIneq():
+    a = Variable("a", ini_value=1, cat="Integer")
+    b = Variable("b", ini_value=1, cat="Continuous")
+
+    prob = Problem()
+    prob += a + 2 * b
+    prob += a + b == 3
+    eq_prob = prob.toIneq()
+    assert len(eq_prob.constraints) == 2
+    assert len(prob.constraints) == 1
+    assert all(
+        const.type() == flopt.constants.ConstraintType.Le
+        for const in eq_prob.constraints
+    )
+
+
 def test_Problem_getSolution():
     # Variables
     a = Variable("a", lowBound=0, upBound=1, cat="Integer")
     b = Variable("b", lowBound=1, upBound=2, cat="Continuous")
     c = Variable("c", lowBound=1, upBound=3, cat="Continuous")
 
     # Problem
     prob = Problem(name="Test")
     x = np.array([a, b, c], dtype=object)
     J = np.array([[1, 2, 1], [0, 1, 1], [0, 0, 3]])
     h = np.array([1, 2, 0])
     prob += -(x.T).dot(J).dot(x) - (h.T).dot(x)
 
     # Solver
-    solver = Solver("RandomSearch")
+    solver = Solver("Random")
     solver.setParams(max_k=2, timelimit=1)  # set max_k > 1
 
     # solve
     prob.solve(solver, msg=True)
 
     from itertools import count
```

### Comparing `flopt-0.5.5/tests/test_ProblemType.py` & `flopt-0.5.6/tests/test_ProblemType.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def test_toProblemType3():
     x = flopt.Variable("x", cat="Continuous")
     prob = flopt.Problem()
     prob += x * x * x
     problem_type = prob.toProblemType()
     assert problem_type == {
         "Variable": VariableType.Continuous,
-        "Objective": ExpressionType.Any,
+        "Objective": ExpressionType.Polynomial,
         "Constraint": ExpressionType.Non,
     }
 
 
 def test_toProblemType4():
     x = flopt.Variable("x", cat="Continuous")
     prob = flopt.Problem()
@@ -70,15 +70,15 @@
 def test_toProblemType6():
     x = flopt.Variable("x", lowBound=0, upBound=10, cat="Permutation")
     prob = flopt.Problem()
     prob += x
     problem_type = prob.toProblemType()
     assert problem_type == {
         "Variable": VariableType.Permutation,
-        "Objective": ExpressionType.Any,
+        "Objective": ExpressionType.Permutation,
         "Constraint": ExpressionType.Non,
     }
 
 
 def test_toProblemType7():
     x = flopt.Variable.array("x", 1, cat="Spin")
     prob = flopt.Problem()
@@ -106,15 +106,15 @@
 def test_toProblemType9():
     x = flopt.Variable.array("x", 10, cat="Spin")
     prob = flopt.Problem()
     prob += flopt.Prod(x)
     problem_type = prob.toProblemType()
     assert problem_type == {
         "Variable": VariableType.Binary,
-        "Objective": ExpressionType.Any,
+        "Objective": ExpressionType.Polynomial,
         "Constraint": ExpressionType.Non,
     }
 
 
 def test_toProblemType10():
     x = flopt.Variable.array("x", 10, cat="Spin")
     prob = flopt.Problem()
```

### Comparing `flopt-0.5.5/tests/test_VarBinary.py` & `flopt-0.5.6/tests/test_VarBinary.py`

 * *Files identical despite different names*

### Comparing `flopt-0.5.5/tests/test_VarContinuous.py` & `flopt-0.5.6/tests/test_VarContinuous.py`

 * *Files identical despite different names*

### Comparing `flopt-0.5.5/tests/test_VarInteger.py` & `flopt-0.5.6/tests/test_VarInteger.py`

 * *Files identical despite different names*

### Comparing `flopt-0.5.5/tests/test_VarPermutation.py` & `flopt-0.5.6/tests/test_VarPermutation.py`

 * *Files identical despite different names*

### Comparing `flopt-0.5.5/tests/test_VarSpin.py` & `flopt-0.5.6/tests/test_VarSpin.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,41 +47,41 @@
     assert ((-a) * b).name == (a * (-b)).name
     assert (a * b).name == ((-a) * (-b)).name
     assert (a * (a * b)).name == b.name
     assert ((a * b) * b).name == a.name
 
 
 def test_VarSpin_selfmul(a):
-    assert (a * a).value() == 1
+    assert a * a == 1
 
 
 def test_VarSpin_div(a):
     assert (a / 2).value() == 0.5
     assert (1 / a).value() == 1
     assert (a / 2.0).value() == 0.5
     assert (1.0 / a).value() == 1
     assert (a / np.float64(2.0)).value() == 0.5
     assert (np.float64(1.0) / a).value() == 1
 
 
 def test_VarSpin_pow(a):
-    assert (a**2).value() == 1
+    assert a**2 == 1
     assert (2**a).value() == 2
     assert (a**2.1).value() == 1
     assert (2.1**a).value() == 2.1
     assert (a ** np.float64(2.1)).value() == 1
     assert (np.float64(2.1) ** a).value() == 2.1
 
 
 def test_VarSpin_intpow(a):
-    assert (a**0).value() == 1
+    assert a**0 == 1
     assert (a**1) == a
-    assert (a**2).value() == 1
+    assert a**2 == 1
     assert (a**3).value() == a
-    assert (a**4).value() == 1
+    assert a**4 == 1
 
 
 def test_VarSpin_mod(a):
     assert (a % 2).value() == 1
 
 
 def test_VarSpin_abs(a):
```

### Comparing `flopt-0.5.5/tests/test_VariableFactory.py` & `flopt-0.5.6/tests/test_VariableFactory.py`

 * *Files identical despite different names*

### Comparing `flopt-0.5.5/tests/test_logger.py` & `flopt-0.5.6/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `flopt-0.5.5/tests/test_utils.py` & `flopt-0.5.6/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     a = Variable("a", lowBound=0, upBound=1, cat="Continuous")
     b = Variable("b", lowBound=1, upBound=2, cat="Continuous")
     c = Variable("c", upBound=3, cat="Continuous")
 
     def custom(a, b, c):
         return a + b * c
 
-    z = CustomExpression(func=custom, arg=[a, b, c])
+    z = CustomExpression(func=custom, args=[a, b, c])
 
     path = tmpdir.mkdir("save").join("tmp2.txt")
     get_dot_graph(z, path)
 
 
 def test_dot_graph_Sum(tmpdir):
     x = Variable.array("x", 6)
```

