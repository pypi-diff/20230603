# Comparing `tmp/chaospy-4.3.9.tar.gz` & `tmp/chaospy-4.3.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/chaospy/chaospy/dist/tmpx369ybgn/chaospy-4.3.9.tar", last modified: Thu Nov 10 13:20:50 2022, max compression
+gzip compressed data, was "/home/runner/work/chaospy/chaospy/dist/tmpetb340xi/chaospy-4.3.9.post1.tar", last modified: Thu Nov 10 14:59:34 2022, max compression
```

## Comparing `chaospy-4.3.9.tar` & `chaospy-4.3.9.post1.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-11-10 13:15:58.000000 chaospy-4.3.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-11-10 13:15:58.000000 chaospy-4.3.9/.github/ISSUE_TEMPLATE/functionality_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-11-10 13:15:58.000000 chaospy-4.3.9/.github/ISSUE_TEMPLATE/usage_question.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-11-10 13:15:58.000000 chaospy-4.3.9/.github/workflows/pipe.yml
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-10 13:15:58.000000 chaospy-4.3.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-11-10 13:15:58.000000 chaospy-4.3.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    26655 2022-11-10 13:15:58.000000 chaospy-4.3.9/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3780 2022-11-10 13:15:58.000000 chaospy-4.3.9/CITATIONS.bib
--rw-r--r--   0 runner    (1001) docker     (121)     3349 2022-11-10 13:15:58.000000 chaospy-4.3.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     3126 2022-11-10 13:15:58.000000 chaospy-4.3.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-11-10 13:15:58.000000 chaospy-4.3.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-10 13:15:58.000000 chaospy-4.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4589 2022-11-10 13:20:50.000000 chaospy-4.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4009 2022-11-10 13:15:58.000000 chaospy-4.3.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/descriptives/
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2748 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/conditional.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/descriptives/correlation/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/correlation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/correlation/auto_correlation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/correlation/pearson.py
--rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/correlation/spearman.py
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/covariance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/expected.py
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/kurtosis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1975 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/percentile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/quantity_of_interest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/descriptives/sensitivity/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/sensitivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/sensitivity/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/sensitivity/main2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/sensitivity/total.py
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/skewness.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/standard_deviation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/descriptives/variance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/distributions/
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9969 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/approximation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/distributions/baseclass/
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/baseclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/baseclass/copula.py
--rw-r--r--   0 runner    (1001) docker     (121)    33546 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/baseclass/distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     3984 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/baseclass/lower_upper.py
--rw-r--r--   0 runner    (1001) docker     (121)     8303 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/baseclass/mean_covariance.py
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/baseclass/operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4810 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/baseclass/shift_scale.py
--rw-r--r--   0 runner    (1001) docker     (121)     4386 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/baseclass/simple.py
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/baseclass/slice_.py
--rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/baseclass/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     9629 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/baseclass/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/distributions/collection/
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/alpha.py
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/anglit.py
--rw-r--r--   0 runner    (1001) docker     (121)     8880 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/beta.py
--rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/binomial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/bradford.py
--rw-r--r--   0 runner    (1001) docker     (121)     2473 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/burr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/cauchy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4285 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/chi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/chi_squared.py
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/discrete_uniform.py
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/double_gamma.py
--rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/double_weibull.py
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/exponential_power.py
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/exponential_weibull.py
--rw-r--r--   0 runner    (1001) docker     (121)     2726 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/f.py
--rw-r--r--   0 runner    (1001) docker     (121)     2226 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/fatigue_life.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/fisk.py
--rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/folded_cauchy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/folded_normal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1867 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/frechet.py
--rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/gamma.py
--rw-r--r--   0 runner    (1001) docker     (121)     2757 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/generalized_exponential.py
--rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/generalized_extreme.py
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/generalized_gamma.py
--rw-r--r--   0 runner    (1001) docker     (121)     2100 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/generalized_half_logistic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/gompertz.py
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/hyperbolic_secant.py
--rw-r--r--   0 runner    (1001) docker     (121)     2159 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/inverse_gamma.py
--rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/kumaraswamy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/laplace.py
--rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/levy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/log_gamma.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/log_laplace.py
--rw-r--r--   0 runner    (1001) docker     (121)     4098 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/log_normal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2147 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/log_uniform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/log_weibull.py
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/logistic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/mielke.py
--rw-r--r--   0 runner    (1001) docker     (121)     5862 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/mv_log_normal.py
--rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/mv_normal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/mv_student_t.py
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/nakagami.py
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/normal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/pareto1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/pareto2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/power_log_normal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/power_normal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2146 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/reciprocal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/student_t.py
--rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/triangle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/trunc_exponential.py
--rw-r--r--   0 runner    (1001) docker     (121)     3728 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/trunc_normal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2407 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/tukey_lambda.py
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/uniform.py
--rw-r--r--   0 runner    (1001) docker     (121)     2557 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/wald.py
--rw-r--r--   0 runner    (1001) docker     (121)     1933 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/weibull.py
--rw-r--r--   0 runner    (1001) docker     (121)     2640 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/collection/wrapped_cauchy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/distributions/copulas/
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/copulas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5209 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/copulas/archimedean.py
--rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/copulas/clayton.py
--rw-r--r--   0 runner    (1001) docker     (121)     5218 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/copulas/gumbel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3889 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/copulas/joe.py
--rw-r--r--   0 runner    (1001) docker     (121)     4159 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/copulas/nataf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4445 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/copulas/t_copula.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/distributions/kernel/
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7269 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/kernel/baseclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     3283 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/kernel/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/kernel/mixture.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/distributions/operators/
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7500 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/operators/addition.py
--rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/operators/iid.py
--rw-r--r--   0 runner    (1001) docker     (121)     8434 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/operators/joint.py
--rw-r--r--   0 runner    (1001) docker     (121)     3192 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/operators/logarithm.py
--rw-r--r--   0 runner    (1001) docker     (121)    11041 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/operators/multiply.py
--rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/operators/negative.py
--rw-r--r--   0 runner    (1001) docker     (121)    10072 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/operators/power.py
--rw-r--r--   0 runner    (1001) docker     (121)     8221 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/operators/truncation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/distributions/sampler/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/antithetic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3550 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/latin_hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/distributions/sampler/sequences/
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/sequences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/sequences/additive_recursion.py
--rw-r--r--   0 runner    (1001) docker     (121)     2853 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/sequences/chebyshev.py
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/sequences/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/sequences/halton.py
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/sequences/hammersley.py
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/sequences/korobov.py
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/sequences/primes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4235 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/sequences/sobol.py
--rw-r--r--   0 runner    (1001) docker     (121)   248116 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/sequences/sobol_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1747 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/distributions/sampler/sequences/van_der_corput.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/expansion/
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/expansion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3426 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/expansion/chebyshev.py
--rw-r--r--   0 runner    (1001) docker     (121)     6575 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/expansion/cholesky.py
--rw-r--r--   0 runner    (1001) docker     (121)     4467 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/expansion/frontend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/expansion/gegenbauer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3317 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/expansion/gram_schmidt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/expansion/hermite.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/expansion/jacobi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3588 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/expansion/lagrange.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/expansion/laguerre.py
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/expansion/legendre.py
--rw-r--r--   0 runner    (1001) docker     (121)     5695 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/expansion/stieltjes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/external/
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6165 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/external/openturns_.py
--rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/external/scipy_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/quadrature/
--rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3938 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/chebyshev.py
--rw-r--r--   0 runner    (1001) docker     (121)     3887 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/clenshaw_curtis.py
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/discrete.py
--rw-r--r--   0 runner    (1001) docker     (121)     3152 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/fejer_1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/fejer_2.py
--rw-r--r--   0 runner    (1001) docker     (121)     9694 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/frontend.py
--rw-r--r--   0 runner    (1001) docker     (121)     3542 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/gegenbauer.py
--rw-r--r--   0 runner    (1001) docker     (121)    16534 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/genz_keister.py
--rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/hermite.py
--rw-r--r--   0 runner    (1001) docker     (121)    16264 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/hypercube.py
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/jacobi.py
--rw-r--r--   0 runner    (1001) docker     (121)     9694 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/kronrod.py
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/laguerre.py
--rw-r--r--   0 runner    (1001) docker     (121)     5427 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/legendre.py
--rw-r--r--   0 runner    (1001) docker     (121)     4394 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/leja.py
--rw-r--r--   0 runner    (1001) docker     (121)     5502 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/lobatto.py
--rw-r--r--   0 runner    (1001) docker     (121)     4354 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/newton_cotes.py
--rw-r--r--   0 runner    (1001) docker     (121)    85484 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/patterson.py
--rw-r--r--   0 runner    (1001) docker     (121)     6475 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/radau.py
--rw-r--r--   0 runner    (1001) docker     (121)     5429 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/sparse_grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     2397 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/quadrature/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy/recurrence/
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/recurrence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/recurrence/chebyshev.py
--rw-r--r--   0 runner    (1001) docker     (121)     4656 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/recurrence/frontend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/recurrence/jacobi.py
--rw-r--r--   0 runner    (1001) docker     (121)     4073 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/recurrence/lanczos.py
--rw-r--r--   0 runner    (1001) docker     (121)     6540 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/recurrence/stieltjes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3099 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     8039 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/saltelli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2525 2022-11-10 13:15:58.000000 chaospy-4.3.9/chaospy/spectral.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4589 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11684 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-10 13:20:50.000000 chaospy-4.3.9/chaospy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 13:17:26.000000 chaospy-4.3.9/chaospy.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-10 13:15:58.000000 chaospy-4.3.9/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-11-10 13:15:58.000000 chaospy-4.3.9/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)    29164 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/_static/chaospy_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     3849 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/_static/chaospy_logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)    74756 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/_static/chaospy_logo2.png
--rw-r--r--   0 runner    (1001) docker     (121)     7659 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/_static/chaospy_logo2.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/_templates/distribution.rst
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/_templates/ndpoly.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4948 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/about_us.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3329 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/bibliography.bib
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/docs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/docs/reference/descriptive/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/descriptive/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/descriptive/miscellaneous.rst
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/descriptive/sensitivity_indices.rst
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/descriptive/statistical_moment.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/docs/reference/distribution/
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/distribution/advanced.rst
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/distribution/baseclass.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/distribution/collection.rst
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/distribution/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/distribution/operator.rst
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/distribution/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/high_level_interface.rst
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/docs/reference/polynomial/
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/polynomial/baseclass.rst
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/polynomial/constructor.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2678 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/polynomial/helper_function.rst
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/polynomial/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/docs/reference/quadrature/
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/quadrature/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/recurrence.rst
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/reference/sampling.rst
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/docs/user_guide/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/docs/user_guide/advanced_topics/
--rw-r--r--   0 runner    (1001) docker     (121)   151234 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/advanced_topics/advanced_regression_method.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    66076 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/advanced_topics/gaussian_mixture_model.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    83466 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/advanced_topics/generalized_polynomial_chaos.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/advanced_topics/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)   201077 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/advanced_topics/kernel_density_estimation.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   251704 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/advanced_topics/polynomial_chaos_kriging.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/advanced_topics/problem_formulation.py
--rw-r--r--   0 runner    (1001) docker     (121)    74698 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/advanced_topics/seir_model.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    75904 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/advanced_topics/stochastic_dependencies.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (121)      255 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/fill_notebooks.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/docs/user_guide/fundamentals/
--rw-r--r--   0 runner    (1001) docker     (121)    15602 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/fundamentals/descriptive_statistics.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/fundamentals/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)   258964 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/fundamentals/probability_distributions.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/fundamentals/problem_formulation.py
--rw-r--r--   0 runner    (1001) docker     (121)   124782 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/fundamentals/quadrature_integration.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   138826 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/fundamentals/quasi_random_samples.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/docs/user_guide/main_usage/
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/main_usage/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    40399 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/main_usage/intrusive_galerkin.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    45047 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/main_usage/lagrange_polynomials.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   427058 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/main_usage/monte_carlo_integration.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/main_usage/monte_carlo_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)   283293 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/main_usage/point_collocation.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   162189 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/main_usage/problem_formulation.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/main_usage/problem_formulation.py
--rw-r--r--   0 runner    (1001) docker     (121)   366315 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/main_usage/pseudo_spectral_projection.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/main_usage/pseudo_spectral_projection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/docs/user_guide/polynomial/
--rw-r--r--   0 runner    (1001) docker     (121)     4975 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/polynomial/comparison_operators.rst
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/polynomial/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5159 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/polynomial/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3809 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/polynomial/numpy_functions.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13399 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/polynomial/orthogonality.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/polynomial/polynomial_division.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2910 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/polynomial/polynomial_evaluation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3018 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/polynomial/polynomial_expansion.rst
--rw-r--r--   0 runner    (1001) docker     (121)    53355 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/polynomial/truncation_scheme.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   212998 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/quick_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-10 13:15:58.000000 chaospy-4.3.9/docs/user_guide/zbibliography.rst
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-11-10 13:15:58.000000 chaospy-4.3.9/polychaos.md
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-10 13:15:58.000000 chaospy-4.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-11-10 13:15:58.000000 chaospy-4.3.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-11-10 13:15:58.000000 chaospy-4.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-11-10 13:20:50.000000 chaospy-4.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4653 2022-11-10 13:15:58.000000 chaospy-4.3.9/tasks.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/tests/distributions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/tests/distributions/collection/
--rw-r--r--   0 runner    (1001) docker     (121)     6278 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/distributions/collection/test_mv_normal.py
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/distributions/collection/test_triangle.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/distributions/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/tests/distributions/copulas/
--rw-r--r--   0 runner    (1001) docker     (121)     6121 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/distributions/copulas/test_nataf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/tests/distributions/kernel/
--rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/distributions/kernel/test_gaussian_kde.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/tests/distributions/operators/
--rw-r--r--   0 runner    (1001) docker     (121)     7450 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/distributions/operators/test_addition.py
--rw-r--r--   0 runner    (1001) docker     (121)     6659 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/distributions/operators/test_multiply.py
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/distributions/operators/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/distributions/operators/test_truncation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/distributions/test_1d_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/distributions/test_2d_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/distributions/test_approximation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1731 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/distributions/test_arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/distributions/test_baseclass.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/tests/poly/
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/poly/test_numpoly.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 13:20:50.000000 chaospy-4.3.9/tests/recurrence/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/recurrence/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/recurrence/test_quadrature_creation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/recurrence/test_stieltjes_method.py
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/test_intrusive_galerkin.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/test_lagrange_polynomials.py
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/test_monte_carlo_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/test_orthogonal_expansion.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/test_point_collocation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/test_pseudo_spectral_projection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/test_regression_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-11-10 13:15:58.000000 chaospy-4.3.9/tests/test_stress.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      883 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/.github/ISSUE_TEMPLATE/functionality_request.md
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/.github/ISSUE_TEMPLATE/usage_question.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/.github/workflows/pipe.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    26655 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3780 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/CITATIONS.bib
+-rw-r--r--   0 runner    (1001) docker     (121)     3349 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3126 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4009 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/
+-rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/descriptives/
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2748 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/conditional.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/descriptives/correlation/
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/correlation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/correlation/auto_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/correlation/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/correlation/spearman.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/covariance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/expected.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/kurtosis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1975 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/percentile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/quantity_of_interest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/descriptives/sensitivity/
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/sensitivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/sensitivity/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/sensitivity/main2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/sensitivity/total.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/skewness.py
+-rw-r--r--   0 runner    (1001) docker     (121)      928 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/standard_deviation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/descriptives/variance.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/distributions/
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9969 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/approximation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/distributions/baseclass/
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/baseclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/baseclass/copula.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33546 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/baseclass/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3984 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/baseclass/lower_upper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8303 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/baseclass/mean_covariance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/baseclass/operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4810 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/baseclass/shift_scale.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4386 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/baseclass/simple.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/baseclass/slice_.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4230 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/baseclass/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9629 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/baseclass/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/
+-rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/alpha.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1498 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/anglit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8880 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/beta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/binomial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/bradford.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2473 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/burr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/cauchy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4285 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/chi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/chi_squared.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/discrete_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/double_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/double_weibull.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/exponential_power.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/exponential_weibull.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2726 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/f.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2226 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/fatigue_life.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/fisk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/folded_cauchy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/folded_normal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1867 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/frechet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2757 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/generalized_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/generalized_extreme.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/generalized_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2100 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/generalized_half_logistic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/gompertz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/hyperbolic_secant.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2159 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/inverse_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/kumaraswamy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/laplace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/levy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/log_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/log_laplace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4098 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/log_normal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2147 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/log_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/log_weibull.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/logistic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/mielke.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5862 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/mv_log_normal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/mv_normal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/mv_student_t.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/nakagami.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/normal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/pareto1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/pareto2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/power_log_normal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/power_normal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2146 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/reciprocal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/student_t.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/trunc_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3590 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/trunc_normal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2407 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/tukey_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2557 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/wald.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1933 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/weibull.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2640 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/collection/wrapped_cauchy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/distributions/copulas/
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/copulas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5209 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/copulas/archimedean.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/copulas/clayton.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5218 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/copulas/gumbel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3889 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/copulas/joe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4159 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/copulas/nataf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4445 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/copulas/t_copula.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/distributions/kernel/
+-rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7269 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/kernel/baseclass.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3283 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/kernel/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/kernel/mixture.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/distributions/operators/
+-rw-r--r--   0 runner    (1001) docker     (121)      410 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7500 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/operators/addition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/operators/iid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8434 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/operators/joint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3192 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/operators/logarithm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11041 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/operators/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/operators/negative.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10072 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/operators/power.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8221 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/operators/truncation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/antithetic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3550 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      885 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/latin_hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2317 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/additive_recursion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2853 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/chebyshev.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/halton.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/hammersley.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/korobov.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/primes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4235 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/sobol.py
+-rw-r--r--   0 runner    (1001) docker     (121)   248116 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/sobol_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1747 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/van_der_corput.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/expansion/
+-rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/expansion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3426 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/expansion/chebyshev.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6575 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/expansion/cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4467 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/expansion/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/expansion/gegenbauer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3317 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/expansion/gram_schmidt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/expansion/hermite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/expansion/jacobi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3588 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/expansion/lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/expansion/laguerre.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/expansion/legendre.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5695 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/expansion/stieltjes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/external/
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6165 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/external/openturns_.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/external/scipy_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3938 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/chebyshev.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3887 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/clenshaw_curtis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3152 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/fejer_1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/fejer_2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9694 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3542 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/gegenbauer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16534 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/genz_keister.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/hermite.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16264 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/hypercube.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/jacobi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9694 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/kronrod.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/laguerre.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5427 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/legendre.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4394 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/leja.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5502 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/lobatto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4354 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/newton_cotes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    85484 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/patterson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6475 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/radau.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5429 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/sparse_grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2397 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/quadrature/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy/recurrence/
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/recurrence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1786 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/recurrence/chebyshev.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4656 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/recurrence/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/recurrence/jacobi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4073 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/recurrence/lanczos.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6540 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/recurrence/stieltjes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3099 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/regression.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8039 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/saltelli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2525 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/chaospy/spectral.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11684 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/chaospy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 14:56:50.000000 chaospy-4.3.9.post1/chaospy.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)    29164 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/_static/chaospy_logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3849 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/_static/chaospy_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    74756 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/_static/chaospy_logo2.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7659 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/_static/chaospy_logo2.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      652 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/_templates/distribution.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      658 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/_templates/ndpoly.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4948 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/about_us.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3329 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/bibliography.bib
+-rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/docs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/docs/reference/descriptive/
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/descriptive/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/descriptive/miscellaneous.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/descriptive/sensitivity_indices.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      485 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/descriptive/statistical_moment.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/docs/reference/distribution/
+-rw-r--r--   0 runner    (1001) docker     (121)      428 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/distribution/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/distribution/baseclass.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/distribution/collection.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/distribution/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/distribution/operator.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/distribution/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/high_level_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/docs/reference/polynomial/
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/polynomial/baseclass.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/polynomial/constructor.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2678 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/polynomial/helper_function.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/polynomial/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/docs/reference/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (121)      883 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/quadrature/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/recurrence.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/reference/sampling.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/docs/user_guide/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/docs/user_guide/advanced_topics/
+-rw-r--r--   0 runner    (1001) docker     (121)   151234 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/advanced_topics/advanced_regression_method.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    66076 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/advanced_topics/gaussian_mixture_model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    83466 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/advanced_topics/generalized_polynomial_chaos.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/advanced_topics/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)   201077 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/advanced_topics/kernel_density_estimation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   251704 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/advanced_topics/polynomial_chaos_kriging.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/advanced_topics/problem_formulation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    74698 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/advanced_topics/seir_model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    75904 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/advanced_topics/stochastic_dependencies.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (121)      255 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/fill_notebooks.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/docs/user_guide/fundamentals/
+-rw-r--r--   0 runner    (1001) docker     (121)    15602 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/fundamentals/descriptive_statistics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/fundamentals/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)   258964 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/fundamentals/probability_distributions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/fundamentals/problem_formulation.py
+-rw-r--r--   0 runner    (1001) docker     (121)   124782 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/fundamentals/quadrature_integration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   138826 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/fundamentals/quasi_random_samples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/docs/user_guide/main_usage/
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/main_usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    40399 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/main_usage/intrusive_galerkin.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    45047 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/main_usage/lagrange_polynomials.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   427058 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/main_usage/monte_carlo_integration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/main_usage/monte_carlo_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)   283293 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/main_usage/point_collocation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   162189 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/main_usage/problem_formulation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/main_usage/problem_formulation.py
+-rw-r--r--   0 runner    (1001) docker     (121)   366315 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/main_usage/pseudo_spectral_projection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/main_usage/pseudo_spectral_projection.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/docs/user_guide/polynomial/
+-rw-r--r--   0 runner    (1001) docker     (121)     4975 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/polynomial/comparison_operators.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/polynomial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5159 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/polynomial/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3809 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/polynomial/numpy_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13399 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/polynomial/orthogonality.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     2679 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/polynomial/polynomial_division.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2910 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/polynomial/polynomial_evaluation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3018 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/polynomial/polynomial_expansion.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    53355 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/polynomial/truncation_scheme.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   212998 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/quick_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/docs/user_guide/zbibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/polychaos.md
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4653 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tasks.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/tests/distributions/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/tests/distributions/collection/
+-rw-r--r--   0 runner    (1001) docker     (121)     6278 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/distributions/collection/test_mv_normal.py
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/distributions/collection/test_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/distributions/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/tests/distributions/copulas/
+-rw-r--r--   0 runner    (1001) docker     (121)     6121 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/distributions/copulas/test_nataf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/tests/distributions/kernel/
+-rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/distributions/kernel/test_gaussian_kde.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/tests/distributions/operators/
+-rw-r--r--   0 runner    (1001) docker     (121)     7450 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/distributions/operators/test_addition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6659 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/distributions/operators/test_multiply.py
+-rw-r--r--   0 runner    (1001) docker     (121)      824 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/distributions/operators/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2218 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/distributions/operators/test_truncation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/distributions/test_1d_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/distributions/test_2d_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/distributions/test_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1731 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/distributions/test_arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/distributions/test_baseclass.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/tests/poly/
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/poly/test_numpoly.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 14:59:34.000000 chaospy-4.3.9.post1/tests/recurrence/
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/recurrence/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/recurrence/test_quadrature_creation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/recurrence/test_stieltjes_method.py
+-rw-r--r--   0 runner    (1001) docker     (121)      996 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/test_intrusive_galerkin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/test_lagrange_polynomials.py
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/test_monte_carlo_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/test_orthogonal_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/test_point_collocation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/test_pseudo_spectral_projection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/test_regression_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-11-10 14:55:45.000000 chaospy-4.3.9.post1/tests/test_stress.py
```

### Comparing `chaospy-4.3.9/.github/ISSUE_TEMPLATE/bug_report.md` & `chaospy-4.3.9.post1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/.github/ISSUE_TEMPLATE/functionality_request.md` & `chaospy-4.3.9.post1/.github/ISSUE_TEMPLATE/functionality_request.md`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/.github/workflows/pipe.yml` & `chaospy-4.3.9.post1/.github/workflows/pipe.yml`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/CHANGELOG.rst` & `chaospy-4.3.9.post1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/CITATIONS.bib` & `chaospy-4.3.9.post1/CITATIONS.bib`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/CODE_OF_CONDUCT.md` & `chaospy-4.3.9.post1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/CONTRIBUTING.rst` & `chaospy-4.3.9.post1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/LICENSE.txt` & `chaospy-4.3.9.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/PKG-INFO` & `chaospy-4.3.9.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaospy
-Version: 4.3.9
+Version: 4.3.9.post1
 Summary: "Numerical tool for performing uncertainty quantification"
 Home-page: https://github.com/jonathf/chaospy/
 Author: Jonathan Feinberg
 Author-email: jonathf@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `chaospy-4.3.9/README.rst` & `chaospy-4.3.9.post1/README.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/__init__.py` & `chaospy-4.3.9.post1/chaospy/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     """Configure logging for Chaospy."""
     logpath = os.environ.get("CHAOSPY_LOGPATH", os.devnull)
     logging.basicConfig(level=logging.DEBUG, filename=logpath, filemode="w")
     streamer = logging.StreamHandler()
     loglevel = (
         logging.DEBUG if os.environ.get("CHAOSPY_DEBUG", "") == "1" else logging.WARNING
     )
+    loglevel = logging.DEBUG
     streamer.setLevel(loglevel)
 
     logger = logging.getLogger("chaospy")
     logger.addHandler(streamer)
     logger = logging.getLogger("numpoly")
     logger.addHandler(streamer)
```

### Comparing `chaospy-4.3.9/chaospy/descriptives/conditional.py` & `chaospy-4.3.9.post1/chaospy/descriptives/conditional.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/descriptives/correlation/auto_correlation.py` & `chaospy-4.3.9.post1/chaospy/descriptives/correlation/auto_correlation.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/descriptives/correlation/pearson.py` & `chaospy-4.3.9.post1/chaospy/descriptives/correlation/pearson.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/descriptives/correlation/spearman.py` & `chaospy-4.3.9.post1/chaospy/descriptives/correlation/spearman.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/descriptives/covariance.py` & `chaospy-4.3.9.post1/chaospy/descriptives/covariance.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/descriptives/expected.py` & `chaospy-4.3.9.post1/chaospy/descriptives/expected.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/descriptives/kurtosis.py` & `chaospy-4.3.9.post1/chaospy/descriptives/kurtosis.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/descriptives/percentile.py` & `chaospy-4.3.9.post1/chaospy/descriptives/percentile.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/descriptives/quantity_of_interest.py` & `chaospy-4.3.9.post1/chaospy/descriptives/quantity_of_interest.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/descriptives/sensitivity/main.py` & `chaospy-4.3.9.post1/chaospy/descriptives/sensitivity/main.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/descriptives/sensitivity/main2.py` & `chaospy-4.3.9.post1/chaospy/descriptives/sensitivity/main2.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/descriptives/sensitivity/total.py` & `chaospy-4.3.9.post1/chaospy/descriptives/sensitivity/total.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/descriptives/skewness.py` & `chaospy-4.3.9.post1/chaospy/descriptives/skewness.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/descriptives/standard_deviation.py` & `chaospy-4.3.9.post1/chaospy/descriptives/standard_deviation.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/descriptives/variance.py` & `chaospy-4.3.9.post1/chaospy/descriptives/variance.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/approximation.py` & `chaospy-4.3.9.post1/chaospy/distributions/approximation.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/baseclass/copula.py` & `chaospy-4.3.9.post1/chaospy/distributions/baseclass/copula.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/baseclass/distribution.py` & `chaospy-4.3.9.post1/chaospy/distributions/baseclass/distribution.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/baseclass/lower_upper.py` & `chaospy-4.3.9.post1/chaospy/distributions/baseclass/lower_upper.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/baseclass/mean_covariance.py` & `chaospy-4.3.9.post1/chaospy/distributions/baseclass/mean_covariance.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/baseclass/operator.py` & `chaospy-4.3.9.post1/chaospy/distributions/baseclass/operator.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/baseclass/shift_scale.py` & `chaospy-4.3.9.post1/chaospy/distributions/baseclass/shift_scale.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/baseclass/simple.py` & `chaospy-4.3.9.post1/chaospy/distributions/baseclass/simple.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/baseclass/slice_.py` & `chaospy-4.3.9.post1/chaospy/distributions/baseclass/slice_.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/baseclass/user.py` & `chaospy-4.3.9.post1/chaospy/distributions/baseclass/user.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/baseclass/utils.py` & `chaospy-4.3.9.post1/chaospy/distributions/baseclass/utils.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/__init__.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/alpha.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/alpha.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/anglit.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/anglit.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/beta.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/beta.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/binomial.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/binomial.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/bradford.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/bradford.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/burr.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/burr.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/cauchy.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/cauchy.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/chi.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/chi.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/chi_squared.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/chi_squared.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/discrete_uniform.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/discrete_uniform.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/double_gamma.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/double_gamma.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/double_weibull.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/double_weibull.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/exponential_power.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/exponential_power.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/exponential_weibull.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/exponential_weibull.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/f.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/f.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/fatigue_life.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/fatigue_life.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/fisk.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/fisk.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/folded_cauchy.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/folded_cauchy.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/folded_normal.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/folded_normal.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/frechet.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/frechet.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/gamma.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/gamma.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/generalized_exponential.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/generalized_exponential.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/generalized_extreme.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/generalized_extreme.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/generalized_gamma.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/generalized_gamma.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/generalized_half_logistic.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/generalized_half_logistic.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/gompertz.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/gompertz.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/hyperbolic_secant.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/hyperbolic_secant.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/inverse_gamma.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/inverse_gamma.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/kumaraswamy.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/kumaraswamy.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/laplace.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/laplace.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/levy.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/levy.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/log_gamma.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/log_gamma.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/log_laplace.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/log_laplace.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/log_normal.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/log_normal.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/log_uniform.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/log_uniform.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/log_weibull.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/log_weibull.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/logistic.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/logistic.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/mielke.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/mielke.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/mv_log_normal.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/mv_log_normal.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/mv_normal.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/mv_normal.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/mv_student_t.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/mv_student_t.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/nakagami.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/nakagami.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/normal.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/normal.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/pareto1.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/pareto1.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/pareto2.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/pareto2.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/power_log_normal.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/power_log_normal.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/power_normal.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/power_normal.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/reciprocal.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/reciprocal.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/student_t.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/student_t.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/triangle.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/triangle.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/trunc_exponential.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/trunc_exponential.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/trunc_normal.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/trunc_normal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Truncated normal distribution."""
 import numpy
 from scipy import special
-from scipy.stats import truncnorm
+from scipy.stats import truncnorm, norm
 import chaospy
 
 from .normal import normal
 from ..baseclass import SimpleDistribution, ShiftScaleDistribution
 
 
 class trunc_normal(SimpleDistribution):
@@ -16,30 +16,29 @@
                 "lower=%s" % lower,
                 "upper=%s" % upper,
                 "mu=%s" % mu,
                 "sigma=%s" % sigma,
             ],
         )
 
-    def get_parameters(self, idx, cache, assert_numerical=True):
-        parameters = super().get_parameters(
-            idx, cache, assert_numerical=assert_numerical
-        )
-        parameters["a"] = (parameters["a"] - parameters["mu"]) / parameters["sigma"]
-        parameters["b"] = (parameters["b"] - parameters["mu"]) / parameters["sigma"]
-        return parameters
-
     def _pdf(self, x, a, b, mu, sigma):
+        a = (a - mu) / sigma
+        b = (b - mu) / sigma
         return truncnorm.pdf(x, a, b, loc=mu, scale=sigma)
 
     def _cdf(self, x, a, b, mu, sigma):
+        a = (a - mu) / sigma
+        b = (b - mu) / sigma
         return truncnorm.cdf(x, a, b, loc=mu, scale=sigma)
 
     def _ppf(self, q, a, b, mu, sigma):
-        return truncnorm.ppf(q, a, b, loc=mu, scale=sigma)
+        a = norm.cdf(a, loc=mu, scale=sigma)
+        b = norm.cdf(b, loc=mu, scale=sigma)
+        q = (b - a) * q + a
+        return norm.ppf(q, mu, sigma)
 
     def _lower(self, a, b, mu, sigma):
         del b
         lower = normal()._lower() * sigma + mu
         return numpy.where(a < lower, lower, a)
 
     def _upper(self, a, b, mu, sigma):
@@ -82,17 +81,17 @@
         array([0.354, 0.506, 0.576, 0.576, 0.506, 0.354])
         >>> half_trunc.pdf(xloc).round(3)
         array([0.288, 0.41 , 0.467, 0.467, 0.41 , 0.288])
         >>> full_trunc.sample(4).round(3)
         array([ 0.266, -0.715,  0.868, -0.03 ])
         >>> half_trunc.sample(4).round(3)
         array([ 0.625, -0.921, -1.822, -0.428])
-        >>> full_trunc.mom([1, 2, 3])
+        >>> full_trunc.mom([1, 2, 3]).round(8)
         array([0.        , 0.29112509, 0.        ])
-        >>> half_trunc.mom([1, 2, 3])
+        >>> half_trunc.mom([1, 2, 3]).round(8)
         array([-0.28759997,  0.71240003, -0.86279991])
 
     """
 
     def __init__(self, lower=-numpy.inf, upper=numpy.inf, mu=0, sigma=1):
         super(TruncNormal, self).__init__(
             trunc_normal(lower=lower, upper=upper, mu=mu, sigma=sigma)
```

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/tukey_lambda.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/tukey_lambda.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/uniform.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/uniform.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/wald.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/wald.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/weibull.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/weibull.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/collection/wrapped_cauchy.py` & `chaospy-4.3.9.post1/chaospy/distributions/collection/wrapped_cauchy.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/copulas/__init__.py` & `chaospy-4.3.9.post1/chaospy/distributions/copulas/__init__.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/copulas/archimedean.py` & `chaospy-4.3.9.post1/chaospy/distributions/copulas/archimedean.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/copulas/clayton.py` & `chaospy-4.3.9.post1/chaospy/distributions/copulas/clayton.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/copulas/gumbel.py` & `chaospy-4.3.9.post1/chaospy/distributions/copulas/gumbel.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/copulas/joe.py` & `chaospy-4.3.9.post1/chaospy/distributions/copulas/joe.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/copulas/nataf.py` & `chaospy-4.3.9.post1/chaospy/distributions/copulas/nataf.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/copulas/t_copula.py` & `chaospy-4.3.9.post1/chaospy/distributions/copulas/t_copula.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/kernel/__init__.py` & `chaospy-4.3.9.post1/chaospy/distributions/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/kernel/baseclass.py` & `chaospy-4.3.9.post1/chaospy/distributions/kernel/baseclass.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/kernel/gaussian.py` & `chaospy-4.3.9.post1/chaospy/distributions/kernel/gaussian.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/kernel/mixture.py` & `chaospy-4.3.9.post1/chaospy/distributions/kernel/mixture.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/operators/addition.py` & `chaospy-4.3.9.post1/chaospy/distributions/operators/addition.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/operators/iid.py` & `chaospy-4.3.9.post1/chaospy/distributions/operators/iid.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/operators/joint.py` & `chaospy-4.3.9.post1/chaospy/distributions/operators/joint.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/operators/logarithm.py` & `chaospy-4.3.9.post1/chaospy/distributions/operators/logarithm.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/operators/multiply.py` & `chaospy-4.3.9.post1/chaospy/distributions/operators/multiply.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/operators/negative.py` & `chaospy-4.3.9.post1/chaospy/distributions/operators/negative.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/operators/power.py` & `chaospy-4.3.9.post1/chaospy/distributions/operators/power.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/operators/truncation.py` & `chaospy-4.3.9.post1/chaospy/distributions/operators/truncation.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/sampler/antithetic.py` & `chaospy-4.3.9.post1/chaospy/distributions/sampler/antithetic.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/sampler/generator.py` & `chaospy-4.3.9.post1/chaospy/distributions/sampler/generator.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/sampler/latin_hypercube.py` & `chaospy-4.3.9.post1/chaospy/distributions/sampler/latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/sampler/sequences/additive_recursion.py` & `chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/additive_recursion.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/sampler/sequences/chebyshev.py` & `chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/chebyshev.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/sampler/sequences/grid.py` & `chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/grid.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/sampler/sequences/halton.py` & `chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/halton.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/sampler/sequences/hammersley.py` & `chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/hammersley.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/sampler/sequences/korobov.py` & `chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/korobov.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/sampler/sequences/primes.py` & `chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/primes.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/sampler/sequences/sobol.py` & `chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/sobol.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/sampler/sequences/sobol_constants.py` & `chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/sobol_constants.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/distributions/sampler/sequences/van_der_corput.py` & `chaospy-4.3.9.post1/chaospy/distributions/sampler/sequences/van_der_corput.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/expansion/__init__.py` & `chaospy-4.3.9.post1/chaospy/expansion/__init__.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/expansion/chebyshev.py` & `chaospy-4.3.9.post1/chaospy/expansion/chebyshev.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/expansion/cholesky.py` & `chaospy-4.3.9.post1/chaospy/expansion/cholesky.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/expansion/frontend.py` & `chaospy-4.3.9.post1/chaospy/expansion/frontend.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/expansion/gegenbauer.py` & `chaospy-4.3.9.post1/chaospy/expansion/gegenbauer.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/expansion/gram_schmidt.py` & `chaospy-4.3.9.post1/chaospy/expansion/gram_schmidt.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/expansion/hermite.py` & `chaospy-4.3.9.post1/chaospy/expansion/hermite.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/expansion/jacobi.py` & `chaospy-4.3.9.post1/chaospy/expansion/jacobi.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/expansion/lagrange.py` & `chaospy-4.3.9.post1/chaospy/expansion/lagrange.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/expansion/laguerre.py` & `chaospy-4.3.9.post1/chaospy/expansion/laguerre.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/expansion/legendre.py` & `chaospy-4.3.9.post1/chaospy/expansion/legendre.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/expansion/stieltjes.py` & `chaospy-4.3.9.post1/chaospy/expansion/stieltjes.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/external/openturns_.py` & `chaospy-4.3.9.post1/chaospy/external/openturns_.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/external/scipy_stats.py` & `chaospy-4.3.9.post1/chaospy/external/scipy_stats.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/__init__.py` & `chaospy-4.3.9.post1/chaospy/quadrature/__init__.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/chebyshev.py` & `chaospy-4.3.9.post1/chaospy/quadrature/chebyshev.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/clenshaw_curtis.py` & `chaospy-4.3.9.post1/chaospy/quadrature/clenshaw_curtis.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/discrete.py` & `chaospy-4.3.9.post1/chaospy/quadrature/discrete.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/fejer_1.py` & `chaospy-4.3.9.post1/chaospy/quadrature/fejer_1.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/fejer_2.py` & `chaospy-4.3.9.post1/chaospy/quadrature/fejer_2.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/frontend.py` & `chaospy-4.3.9.post1/chaospy/quadrature/frontend.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/gaussian.py` & `chaospy-4.3.9.post1/chaospy/quadrature/gaussian.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/gegenbauer.py` & `chaospy-4.3.9.post1/chaospy/quadrature/gegenbauer.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/genz_keister.py` & `chaospy-4.3.9.post1/chaospy/quadrature/genz_keister.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/grid.py` & `chaospy-4.3.9.post1/chaospy/quadrature/grid.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/hermite.py` & `chaospy-4.3.9.post1/chaospy/quadrature/hermite.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/hypercube.py` & `chaospy-4.3.9.post1/chaospy/quadrature/hypercube.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/jacobi.py` & `chaospy-4.3.9.post1/chaospy/quadrature/jacobi.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/kronrod.py` & `chaospy-4.3.9.post1/chaospy/quadrature/kronrod.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/laguerre.py` & `chaospy-4.3.9.post1/chaospy/quadrature/laguerre.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/legendre.py` & `chaospy-4.3.9.post1/chaospy/quadrature/legendre.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/leja.py` & `chaospy-4.3.9.post1/chaospy/quadrature/leja.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/lobatto.py` & `chaospy-4.3.9.post1/chaospy/quadrature/lobatto.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/newton_cotes.py` & `chaospy-4.3.9.post1/chaospy/quadrature/newton_cotes.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/patterson.py` & `chaospy-4.3.9.post1/chaospy/quadrature/patterson.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/radau.py` & `chaospy-4.3.9.post1/chaospy/quadrature/radau.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/sparse_grid.py` & `chaospy-4.3.9.post1/chaospy/quadrature/sparse_grid.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/quadrature/utils.py` & `chaospy-4.3.9.post1/chaospy/quadrature/utils.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/recurrence/chebyshev.py` & `chaospy-4.3.9.post1/chaospy/recurrence/chebyshev.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/recurrence/frontend.py` & `chaospy-4.3.9.post1/chaospy/recurrence/frontend.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/recurrence/jacobi.py` & `chaospy-4.3.9.post1/chaospy/recurrence/jacobi.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/recurrence/lanczos.py` & `chaospy-4.3.9.post1/chaospy/recurrence/lanczos.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/recurrence/stieltjes.py` & `chaospy-4.3.9.post1/chaospy/recurrence/stieltjes.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/regression.py` & `chaospy-4.3.9.post1/chaospy/regression.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/saltelli.py` & `chaospy-4.3.9.post1/chaospy/saltelli.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy/spectral.py` & `chaospy-4.3.9.post1/chaospy/spectral.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/chaospy.egg-info/PKG-INFO` & `chaospy-4.3.9.post1/chaospy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaospy
-Version: 4.3.9
+Version: 4.3.9.post1
 Summary: "Numerical tool for performing uncertainty quantification"
 Home-page: https://github.com/jonathf/chaospy/
 Author: Jonathan Feinberg
 Author-email: jonathf@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `chaospy-4.3.9/chaospy.egg-info/SOURCES.txt` & `chaospy-4.3.9.post1/chaospy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/conftest.py` & `chaospy-4.3.9.post1/conftest.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/Makefile` & `chaospy-4.3.9.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/_static/chaospy_logo.png` & `chaospy-4.3.9.post1/docs/_static/chaospy_logo.png`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/_static/chaospy_logo.svg` & `chaospy-4.3.9.post1/docs/_static/chaospy_logo.svg`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/_static/chaospy_logo2.png` & `chaospy-4.3.9.post1/docs/_static/chaospy_logo2.png`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/_static/chaospy_logo2.svg` & `chaospy-4.3.9.post1/docs/_static/chaospy_logo2.svg`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/_templates/distribution.rst` & `chaospy-4.3.9.post1/docs/_templates/distribution.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/_templates/ndpoly.rst` & `chaospy-4.3.9.post1/docs/_templates/ndpoly.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/about_us.rst` & `chaospy-4.3.9.post1/docs/about_us.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/bibliography.bib` & `chaospy-4.3.9.post1/docs/bibliography.bib`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/conf.py` & `chaospy-4.3.9.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/index.rst` & `chaospy-4.3.9.post1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/reference/distribution/collection.rst` & `chaospy-4.3.9.post1/docs/reference/distribution/collection.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/reference/high_level_interface.rst` & `chaospy-4.3.9.post1/docs/reference/high_level_interface.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/reference/polynomial/constructor.rst` & `chaospy-4.3.9.post1/docs/reference/polynomial/constructor.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/reference/polynomial/helper_function.rst` & `chaospy-4.3.9.post1/docs/reference/polynomial/helper_function.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/reference/quadrature/index.rst` & `chaospy-4.3.9.post1/docs/reference/quadrature/index.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/reference/sampling.rst` & `chaospy-4.3.9.post1/docs/reference/sampling.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/advanced_topics/advanced_regression_method.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/advanced_topics/advanced_regression_method.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/advanced_topics/gaussian_mixture_model.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/advanced_topics/gaussian_mixture_model.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/advanced_topics/generalized_polynomial_chaos.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/advanced_topics/generalized_polynomial_chaos.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/advanced_topics/kernel_density_estimation.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/advanced_topics/kernel_density_estimation.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/advanced_topics/polynomial_chaos_kriging.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/advanced_topics/polynomial_chaos_kriging.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/advanced_topics/problem_formulation.py` & `chaospy-4.3.9.post1/docs/user_guide/advanced_topics/problem_formulation.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/advanced_topics/seir_model.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/advanced_topics/seir_model.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/advanced_topics/stochastic_dependencies.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/advanced_topics/stochastic_dependencies.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/fundamentals/descriptive_statistics.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/fundamentals/descriptive_statistics.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/fundamentals/probability_distributions.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/fundamentals/probability_distributions.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/fundamentals/problem_formulation.py` & `chaospy-4.3.9.post1/docs/user_guide/fundamentals/problem_formulation.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/fundamentals/quadrature_integration.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/fundamentals/quadrature_integration.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/fundamentals/quasi_random_samples.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/fundamentals/quasi_random_samples.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/main_usage/intrusive_galerkin.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/main_usage/intrusive_galerkin.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/main_usage/lagrange_polynomials.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/main_usage/lagrange_polynomials.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/main_usage/monte_carlo_integration.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/main_usage/monte_carlo_integration.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/main_usage/point_collocation.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/main_usage/point_collocation.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/main_usage/problem_formulation.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/main_usage/problem_formulation.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/main_usage/problem_formulation.py` & `chaospy-4.3.9.post1/docs/user_guide/main_usage/problem_formulation.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/main_usage/pseudo_spectral_projection.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/main_usage/pseudo_spectral_projection.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/polynomial/comparison_operators.rst` & `chaospy-4.3.9.post1/docs/user_guide/polynomial/comparison_operators.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/polynomial/introduction.rst` & `chaospy-4.3.9.post1/docs/user_guide/polynomial/introduction.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/polynomial/numpy_functions.rst` & `chaospy-4.3.9.post1/docs/user_guide/polynomial/numpy_functions.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/polynomial/orthogonality.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/polynomial/orthogonality.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/polynomial/polynomial_division.rst` & `chaospy-4.3.9.post1/docs/user_guide/polynomial/polynomial_division.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/polynomial/polynomial_evaluation.rst` & `chaospy-4.3.9.post1/docs/user_guide/polynomial/polynomial_evaluation.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/polynomial/polynomial_expansion.rst` & `chaospy-4.3.9.post1/docs/user_guide/polynomial/polynomial_expansion.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/polynomial/truncation_scheme.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/polynomial/truncation_scheme.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/docs/user_guide/quick_tutorial.ipynb` & `chaospy-4.3.9.post1/docs/user_guide/quick_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/setup.cfg` & `chaospy-4.3.9.post1/setup.cfg`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tasks.rst` & `chaospy-4.3.9.post1/tasks.rst`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/conftest.py` & `chaospy-4.3.9.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/distributions/collection/test_mv_normal.py` & `chaospy-4.3.9.post1/tests/distributions/collection/test_mv_normal.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/distributions/collection/test_triangle.py` & `chaospy-4.3.9.post1/tests/distributions/collection/test_triangle.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/distributions/copulas/test_nataf.py` & `chaospy-4.3.9.post1/tests/distributions/copulas/test_nataf.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/distributions/kernel/test_gaussian_kde.py` & `chaospy-4.3.9.post1/tests/distributions/kernel/test_gaussian_kde.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/distributions/operators/test_addition.py` & `chaospy-4.3.9.post1/tests/distributions/operators/test_addition.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/distributions/operators/test_multiply.py` & `chaospy-4.3.9.post1/tests/distributions/operators/test_multiply.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/distributions/operators/test_operators.py` & `chaospy-4.3.9.post1/tests/distributions/operators/test_operators.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/distributions/operators/test_truncation.py` & `chaospy-4.3.9.post1/tests/distributions/operators/test_truncation.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/distributions/test_1d_dependencies.py` & `chaospy-4.3.9.post1/tests/distributions/test_1d_dependencies.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/distributions/test_2d_dependencies.py` & `chaospy-4.3.9.post1/tests/distributions/test_2d_dependencies.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/distributions/test_approximation.py` & `chaospy-4.3.9.post1/tests/distributions/test_approximation.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/distributions/test_arithmetics.py` & `chaospy-4.3.9.post1/tests/distributions/test_arithmetics.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/distributions/test_baseclass.py` & `chaospy-4.3.9.post1/tests/distributions/test_baseclass.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/recurrence/conftest.py` & `chaospy-4.3.9.post1/tests/recurrence/conftest.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/recurrence/test_quadrature_creation.py` & `chaospy-4.3.9.post1/tests/recurrence/test_quadrature_creation.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/recurrence/test_stieltjes_method.py` & `chaospy-4.3.9.post1/tests/recurrence/test_stieltjes_method.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/test_intrusive_galerkin.py` & `chaospy-4.3.9.post1/tests/test_intrusive_galerkin.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/test_lagrange_polynomials.py` & `chaospy-4.3.9.post1/tests/test_lagrange_polynomials.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/test_orthogonal_expansion.py` & `chaospy-4.3.9.post1/tests/test_orthogonal_expansion.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/test_point_collocation.py` & `chaospy-4.3.9.post1/tests/test_point_collocation.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/test_pseudo_spectral_projection.py` & `chaospy-4.3.9.post1/tests/test_pseudo_spectral_projection.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/test_regression_models.py` & `chaospy-4.3.9.post1/tests/test_regression_models.py`

 * *Files identical despite different names*

### Comparing `chaospy-4.3.9/tests/test_stress.py` & `chaospy-4.3.9.post1/tests/test_stress.py`

 * *Files identical despite different names*

