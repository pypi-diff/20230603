# Comparing `tmp/most_queue-1.20.tar.gz` & `tmp/most_queue-1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "most_queue-1.20.tar", last modified: Fri Jun  2 20:11:58 2023, max compression
+gzip compressed data, was "most_queue-1.21.tar", last modified: Sat Jun  3 07:33:16 2023, max compression
```

## Comparing `most_queue-1.20.tar` & `most_queue-1.21.tar`

### file list

```diff
@@ -1,92 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.170381 most_queue-1.20/
--rw-rw-rw-   0        0        0     1091 2022-09-15 10:35:18.000000 most_queue-1.20/LICENSE
--rw-rw-rw-   0        0        0     6337 2023-06-02 20:11:58.170381 most_queue-1.20/PKG-INFO
--rw-rw-rw-   0        0        0     4545 2023-05-17 17:25:06.000000 most_queue-1.20/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.123708 most_queue-1.20/most_queue/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.20/most_queue/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.135935 most_queue-1.20/most_queue/sim/
--rw-rw-rw-   0        0        0       78 2023-05-17 17:58:01.000000 most_queue-1.20/most_queue/sim/__init__.py
--rw-rw-rw-   0        0        0    13931 2023-06-02 19:10:20.000000 most_queue-1.20/most_queue/sim/fj_delta_im.py
--rw-rw-rw-   0        0        0    11089 2023-06-02 19:12:14.000000 most_queue-1.20/most_queue/sim/fj_im.py
--rw-rw-rw-   0        0        0    10084 2023-05-17 17:54:25.000000 most_queue-1.20/most_queue/sim/flow_sum_im.py
--rw-rw-rw-   0        0        0     9307 2023-06-02 19:38:06.000000 most_queue-1.20/most_queue/sim/network_im_prty.py
--rw-rw-rw-   0        0        0    12328 2023-06-02 19:38:06.000000 most_queue-1.20/most_queue/sim/queue_finite_source_sim.py
--rw-rw-rw-   0        0        0    37275 2023-05-17 17:54:25.000000 most_queue-1.20/most_queue/sim/rand_destribution.py
--rw-rw-rw-   0        0        0     3800 2023-05-17 17:54:25.000000 most_queue-1.20/most_queue/sim/smo_batch_sim.py
--rw-rw-rw-   0        0        0    31076 2023-06-02 19:34:00.000000 most_queue-1.20/most_queue/sim/smo_im.py
--rw-rw-rw-   0        0        0    37990 2023-06-02 20:04:15.000000 most_queue-1.20/most_queue/sim/smo_im_prty.py
--rw-rw-rw-   0        0        0     7658 2023-05-17 17:57:13.000000 most_queue-1.20/most_queue/sim/smo_impatient_im.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.148321 most_queue-1.20/most_queue/tests/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.20/most_queue/tests/__init__.py
--rw-rw-rw-   0        0        0     3826 2023-05-17 17:18:04.000000 most_queue-1.20/most_queue/tests/ek_d_n.py
--rw-rw-rw-   0        0        0     5090 2023-05-17 18:17:47.000000 most_queue-1.20/most_queue/tests/fj_calc.py
--rw-rw-rw-   0        0        0     5539 2022-09-16 07:43:39.000000 most_queue-1.20/most_queue/tests/fj_im.py
--rw-rw-rw-   0        0        0     4278 2023-05-11 04:35:32.000000 most_queue-1.20/most_queue/tests/flow_sum.py
--rw-rw-rw-   0        0        0     5122 2022-09-16 08:17:30.000000 most_queue-1.20/most_queue/tests/gi_m_1_calc.py
--rw-rw-rw-   0        0        0     5258 2022-09-16 08:17:30.000000 most_queue-1.20/most_queue/tests/gi_m_n_calc.py
--rw-rw-rw-   0        0        0     2255 2022-09-16 08:20:45.000000 most_queue-1.20/most_queue/tests/m_d_n_calc.py
--rw-rw-rw-   0        0        0     3644 2023-05-17 18:41:32.000000 most_queue-1.20/most_queue/tests/m_h2_h2warm.py
--rw-rw-rw-   0        0        0     6712 2022-09-16 08:52:49.000000 most_queue-1.20/most_queue/tests/m_ph_n_prty.py
--rw-rw-rw-   0        0        0     5267 2022-09-20 18:59:53.000000 most_queue-1.20/most_queue/tests/mg1_calc.py
--rw-rw-rw-   0        0        0      982 2022-09-15 18:04:48.000000 most_queue-1.20/most_queue/tests/mg1_warm_calc.py
--rw-rw-rw-   0        0        0     4747 2023-05-08 07:36:11.000000 most_queue-1.20/most_queue/tests/mgn_tt.py
--rw-rw-rw-   0        0        0     3337 2022-09-15 18:04:48.000000 most_queue-1.20/most_queue/tests/mmn3_pnz_cox_approx.py
--rw-rw-rw-   0        0        0     2830 2022-09-15 18:04:48.000000 most_queue-1.20/most_queue/tests/mmn_prty_pnz_approx.py
--rw-rw-rw-   0        0        0     8149 2022-09-23 20:18:42.000000 most_queue-1.20/most_queue/tests/network_im_prty.py
--rw-rw-rw-   0        0        0    17534 2022-09-15 18:04:48.000000 most_queue-1.20/most_queue/tests/passage_time.py
--rw-rw-rw-   0        0        0     2744 2022-09-23 19:56:01.000000 most_queue-1.20/most_queue/tests/smo_im.py
--rw-rw-rw-   0        0        0     6545 2022-09-23 20:18:42.000000 most_queue-1.20/most_queue/tests/smo_im_prty.py
--rw-rw-rw-   0        0        0      967 2022-09-16 08:52:49.000000 most_queue-1.20/most_queue/tests/weibull.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.163872 most_queue-1.20/most_queue/theory/
--rw-rw-rw-   0        0        0       76 2023-05-17 17:43:06.000000 most_queue-1.20/most_queue/theory/__init__.py
--rw-rw-rw-   0        0        0     2360 2022-11-30 18:00:26.000000 most_queue-1.20/most_queue/theory/batch_mm1.py
--rw-rw-rw-   0        0        0     1304 2022-09-15 11:45:51.000000 most_queue-1.20/most_queue/theory/diff5dots.py
--rw-rw-rw-   0        0        0     6001 2023-06-02 19:50:03.000000 most_queue-1.20/most_queue/theory/ek_d_n_calc.py
--rw-rw-rw-   0        0        0     4741 2023-06-02 19:50:03.000000 most_queue-1.20/most_queue/theory/engset_model.py
--rw-rw-rw-   0        0        0    19289 2023-05-17 17:46:45.000000 most_queue-1.20/most_queue/theory/fj_calc.py
--rw-rw-rw-   0        0        0    10650 2023-05-17 17:35:09.000000 most_queue-1.20/most_queue/theory/flow_sum.py
--rw-rw-rw-   0        0        0     1626 2022-11-30 19:52:32.000000 most_queue-1.20/most_queue/theory/generate_pareto_noise.py
--rw-rw-rw-   0        0        0     4231 2023-06-02 19:52:43.000000 most_queue-1.20/most_queue/theory/gi_m_1_calc.py
--rw-rw-rw-   0        0        0     6171 2023-06-02 19:55:05.000000 most_queue-1.20/most_queue/theory/gi_m_n_calc.py
--rw-rw-rw-   0        0        0     2135 2022-11-29 13:43:22.000000 most_queue-1.20/most_queue/theory/impatience_calc.py
--rw-rw-rw-   0        0        0     4199 2023-06-02 19:56:01.000000 most_queue-1.20/most_queue/theory/m_d_n_calc.py
--rw-rw-rw-   0        0        0    27804 2023-06-02 20:00:16.000000 most_queue-1.20/most_queue/theory/m_h2_h2warm.py
--rw-rw-rw-   0        0        0    29730 2023-05-17 17:54:25.000000 most_queue-1.20/most_queue/theory/m_ph_n_prty.py
--rw-rw-rw-   0        0        0     4672 2023-06-02 20:00:16.000000 most_queue-1.20/most_queue/theory/mg1_calc.py
--rw-rw-rw-   0        0        0     1354 2023-06-02 20:02:08.000000 most_queue-1.20/most_queue/theory/mg1_warm_calc.py
--rw-rw-rw-   0        0        0    17357 2023-06-02 20:02:08.000000 most_queue-1.20/most_queue/theory/mgn_tt.py
--rw-rw-rw-   0        0        0    18821 2023-06-02 20:03:36.000000 most_queue-1.20/most_queue/theory/mmn3_pnz_cox_approx.py
--rw-rw-rw-   0        0        0    26711 2023-06-02 20:05:31.000000 most_queue-1.20/most_queue/theory/mmn_prty_pnz_approx.py
--rw-rw-rw-   0        0        0     1987 2023-05-17 17:54:25.000000 most_queue-1.20/most_queue/theory/mmnr_calc.py
--rw-rw-rw-   0        0        0     5777 2023-05-17 17:54:25.000000 most_queue-1.20/most_queue/theory/network_calc.py
--rw-rw-rw-   0        0        0     1066 2022-12-04 16:14:36.000000 most_queue-1.20/most_queue/theory/network_viewer.py
--rw-rw-rw-   0        0        0    40877 2023-05-18 21:35:04.000000 most_queue-1.20/most_queue/theory/passage_time.py
--rw-rw-rw-   0        0        0    17662 2023-05-17 17:54:25.000000 most_queue-1.20/most_queue/theory/prty_calc.py
--rw-rw-rw-   0        0        0     2174 2022-09-15 17:05:30.000000 most_queue-1.20/most_queue/theory/q_poisson_arrival_calc.py
--rw-rw-rw-   0        0        0     5396 2022-09-15 11:45:51.000000 most_queue-1.20/most_queue/theory/student_stat.py
--rw-rw-rw-   0        0        0      632 2022-09-15 11:45:51.000000 most_queue-1.20/most_queue/theory/sv_sum_calc.py
--rw-rw-rw-   0        0        0     4079 2022-09-15 12:02:16.000000 most_queue-1.20/most_queue/theory/weibull.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.165871 most_queue-1.20/most_queue/utils/
--rw-rw-rw-   0        0        0        0 2023-05-17 17:19:33.000000 most_queue-1.20/most_queue/utils/__init__.py
--rw-rw-rw-   0        0        0     2078 2023-05-17 17:18:48.000000 most_queue-1.20/most_queue/utils/approx_cdf_make.py
--rw-rw-rw-   0        0        0      319 2023-05-18 16:11:27.000000 most_queue-1.20/most_queue/utils/binom_probs.py
--rw-rw-rw-   0        0        0       62 2023-05-18 20:41:30.000000 most_queue-1.20/most_queue/utils/difstir.py
--rw-rw-rw-   0        0        0     2761 2023-06-02 20:11:23.000000 most_queue-1.20/most_queue/utils/tables.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.165871 most_queue-1.20/most_queue/visualisation/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.20/most_queue/visualisation/__init__.py
--rw-rw-rw-   0        0        0    35629 2022-09-30 18:59:24.000000 most_queue-1.20/most_queue/visualisation/smo_im_vis.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.169383 most_queue-1.20/most_queue/visualisation/utils/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.20/most_queue/visualisation/utils/__init__.py
--rw-rw-rw-   0        0        0     3169 2022-06-17 16:46:09.000000 most_queue-1.20/most_queue/visualisation/utils/result_table.py
--rw-rw-rw-   0        0        0    14872 2022-08-16 20:24:21.000000 most_queue-1.20/most_queue/visualisation/utils/settings_window.py
--rw-rw-rw-   0        0        0     1432 2022-06-03 20:22:54.000000 most_queue-1.20/most_queue/visualisation/utils/splash_screen.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:11:58.127303 most_queue-1.20/most_queue.egg-info/
--rw-rw-rw-   0        0        0     6337 2023-06-02 20:11:58.000000 most_queue-1.20/most_queue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2594 2023-06-02 20:11:58.000000 most_queue-1.20/most_queue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 20:11:58.000000 most_queue-1.20/most_queue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-25 20:28:16.000000 most_queue-1.20/most_queue.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      114 2023-06-02 20:11:58.000000 most_queue-1.20/most_queue.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-02 20:11:58.000000 most_queue-1.20/most_queue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      508 2023-06-02 20:11:38.000000 most_queue-1.20/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 20:11:58.170381 most_queue-1.20/setup.cfg
--rw-rw-rw-   0        0        0     1000 2023-06-02 20:11:32.000000 most_queue-1.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.269953 most_queue-1.21/
+-rw-rw-rw-   0        0        0     1091 2022-09-15 10:35:18.000000 most_queue-1.21/LICENSE
+-rw-rw-rw-   0        0        0     6337 2023-06-03 07:33:16.268981 most_queue-1.21/PKG-INFO
+-rw-rw-rw-   0        0        0     4545 2023-05-17 17:25:06.000000 most_queue-1.21/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.198447 most_queue-1.21/most_queue/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.21/most_queue/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.215939 most_queue-1.21/most_queue/sim/
+-rw-rw-rw-   0        0        0       78 2023-05-17 17:58:01.000000 most_queue-1.21/most_queue/sim/__init__.py
+-rw-rw-rw-   0        0        0     3853 2023-06-03 06:16:25.000000 most_queue-1.21/most_queue/sim/batch_sim.py
+-rw-rw-rw-   0        0        0    13909 2023-06-03 06:25:11.000000 most_queue-1.21/most_queue/sim/fj_delta_sim.py
+-rw-rw-rw-   0        0        0    11136 2023-06-03 06:21:42.000000 most_queue-1.21/most_queue/sim/fj_sim.py
+-rw-rw-rw-   0        0        0    10039 2023-06-03 06:30:19.000000 most_queue-1.21/most_queue/sim/flow_sum_sim.py
+-rw-rw-rw-   0        0        0     7702 2023-06-03 06:35:08.000000 most_queue-1.21/most_queue/sim/impatient_queue_sim.py
+-rw-rw-rw-   0        0        0     9329 2023-06-03 06:35:08.000000 most_queue-1.21/most_queue/sim/priority_network.py
+-rw-rw-rw-   0        0        0    38069 2023-06-03 06:30:19.000000 most_queue-1.21/most_queue/sim/priority_queue_sim.py
+-rw-rw-rw-   0        0        0    31166 2023-06-03 06:16:25.000000 most_queue-1.21/most_queue/sim/qs_sim.py
+-rw-rw-rw-   0        0        0    12393 2023-06-03 06:35:08.000000 most_queue-1.21/most_queue/sim/queue_finite_source_sim.py
+-rw-rw-rw-   0        0        0    37275 2023-05-17 17:54:25.000000 most_queue-1.21/most_queue/sim/rand_destribution.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.241586 most_queue-1.21/most_queue/tests/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.21/most_queue/tests/__init__.py
+-rw-rw-rw-   0        0        0     3571 2023-06-03 07:00:47.000000 most_queue-1.21/most_queue/tests/ek_d_n.py
+-rw-rw-rw-   0        0        0     5109 2023-06-03 07:00:47.000000 most_queue-1.21/most_queue/tests/fj_calc.py
+-rw-rw-rw-   0        0        0     5554 2023-06-03 07:02:09.000000 most_queue-1.21/most_queue/tests/fj_im.py
+-rw-rw-rw-   0        0        0     4292 2023-06-03 07:03:43.000000 most_queue-1.21/most_queue/tests/flow_sum.py
+-rw-rw-rw-   0        0        0     5166 2023-06-03 07:07:00.000000 most_queue-1.21/most_queue/tests/gi_m_1_calc.py
+-rw-rw-rw-   0        0        0     5302 2023-06-03 07:08:42.000000 most_queue-1.21/most_queue/tests/gi_m_n_calc.py
+-rw-rw-rw-   0        0        0     2287 2023-06-03 07:09:19.000000 most_queue-1.21/most_queue/tests/m_d_n_calc.py
+-rw-rw-rw-   0        0        0     3148 2023-06-03 07:12:12.000000 most_queue-1.21/most_queue/tests/m_h2_h2warm.py
+-rw-rw-rw-   0        0        0     6737 2023-06-03 07:16:26.000000 most_queue-1.21/most_queue/tests/m_ph_n_prty.py
+-rw-rw-rw-   0        0        0     2779 2023-06-03 07:16:26.000000 most_queue-1.21/most_queue/tests/mg1_calc.py
+-rw-rw-rw-   0        0        0      792 2023-06-03 07:17:42.000000 most_queue-1.21/most_queue/tests/mg1_warm_calc.py
+-rw-rw-rw-   0        0        0     4248 2023-06-03 07:19:07.000000 most_queue-1.21/most_queue/tests/mgn_tt.py
+-rw-rw-rw-   0        0        0     3358 2023-06-03 07:23:03.000000 most_queue-1.21/most_queue/tests/mmn3_pnz_cox_approx.py
+-rw-rw-rw-   0        0        0     2860 2023-06-03 07:23:03.000000 most_queue-1.21/most_queue/tests/mmn_prty_pnz_approx.py
+-rw-rw-rw-   0        0        0     6535 2023-06-03 07:23:03.000000 most_queue-1.21/most_queue/tests/network_im_prty.py
+-rw-rw-rw-   0        0        0     2207 2023-06-03 07:25:02.000000 most_queue-1.21/most_queue/tests/smo_im.py
+-rw-rw-rw-   0        0        0     4974 2023-06-03 07:31:47.000000 most_queue-1.21/most_queue/tests/smo_im_prty.py
+-rw-rw-rw-   0        0        0      967 2022-09-16 08:52:49.000000 most_queue-1.21/most_queue/tests/weibull.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.262405 most_queue-1.21/most_queue/theory/
+-rw-rw-rw-   0        0        0       76 2023-05-17 17:43:06.000000 most_queue-1.21/most_queue/theory/__init__.py
+-rw-rw-rw-   0        0        0     2360 2022-11-30 18:00:26.000000 most_queue-1.21/most_queue/theory/batch_mm1.py
+-rw-rw-rw-   0        0        0      632 2022-09-15 11:45:51.000000 most_queue-1.21/most_queue/theory/convolution_sum_calc.py
+-rw-rw-rw-   0        0        0     1304 2022-09-15 11:45:51.000000 most_queue-1.21/most_queue/theory/diff5dots.py
+-rw-rw-rw-   0        0        0     6030 2023-06-03 06:39:46.000000 most_queue-1.21/most_queue/theory/ek_d_n_calc.py
+-rw-rw-rw-   0        0        0     4741 2023-06-02 19:50:03.000000 most_queue-1.21/most_queue/theory/engset_model.py
+-rw-rw-rw-   0        0        0    19297 2023-06-03 06:39:46.000000 most_queue-1.21/most_queue/theory/fj_calc.py
+-rw-rw-rw-   0        0        0    10652 2023-06-03 06:43:21.000000 most_queue-1.21/most_queue/theory/flow_sum.py
+-rw-rw-rw-   0        0        0     1626 2022-11-30 19:52:32.000000 most_queue-1.21/most_queue/theory/generate_pareto_noise.py
+-rw-rw-rw-   0        0        0     4285 2023-06-03 07:04:51.000000 most_queue-1.21/most_queue/theory/gi_m_1_calc.py
+-rw-rw-rw-   0        0        0     6205 2023-06-03 06:46:05.000000 most_queue-1.21/most_queue/theory/gi_m_n_calc.py
+-rw-rw-rw-   0        0        0     2135 2022-11-29 13:43:22.000000 most_queue-1.21/most_queue/theory/impatience_calc.py
+-rw-rw-rw-   0        0        0     4228 2023-06-03 06:46:46.000000 most_queue-1.21/most_queue/theory/m_d_n_calc.py
+-rw-rw-rw-   0        0        0    27856 2023-06-03 06:48:34.000000 most_queue-1.21/most_queue/theory/m_h2_h2warm.py
+-rw-rw-rw-   0        0        0    29755 2023-06-03 06:50:55.000000 most_queue-1.21/most_queue/theory/m_ph_n_prty.py
+-rw-rw-rw-   0        0        0     4708 2023-06-03 06:52:44.000000 most_queue-1.21/most_queue/theory/mg1_calc.py
+-rw-rw-rw-   0        0        0     1383 2023-06-03 06:52:44.000000 most_queue-1.21/most_queue/theory/mg1_warm_calc.py
+-rw-rw-rw-   0        0        0    17386 2023-06-03 06:53:31.000000 most_queue-1.21/most_queue/theory/mgn_tt.py
+-rw-rw-rw-   0        0        0    18846 2023-06-03 06:54:14.000000 most_queue-1.21/most_queue/theory/mmn3_pnz_cox_approx.py
+-rw-rw-rw-   0        0        0    26736 2023-06-03 06:54:45.000000 most_queue-1.21/most_queue/theory/mmn_prty_pnz_approx.py
+-rw-rw-rw-   0        0        0     1994 2023-06-03 07:29:46.000000 most_queue-1.21/most_queue/theory/mmnr_calc.py
+-rw-rw-rw-   0        0        0     5777 2023-05-17 17:54:25.000000 most_queue-1.21/most_queue/theory/network_calc.py
+-rw-rw-rw-   0        0        0     1066 2022-12-04 16:14:36.000000 most_queue-1.21/most_queue/theory/network_viewer.py
+-rw-rw-rw-   0        0        0    40877 2023-05-18 21:35:04.000000 most_queue-1.21/most_queue/theory/passage_time.py
+-rw-rw-rw-   0        0        0    17662 2023-05-17 17:54:25.000000 most_queue-1.21/most_queue/theory/priority_calc.py
+-rw-rw-rw-   0        0        0     2174 2022-09-15 17:05:30.000000 most_queue-1.21/most_queue/theory/q_poisson_arrival_calc.py
+-rw-rw-rw-   0        0        0     5396 2022-09-15 11:45:51.000000 most_queue-1.21/most_queue/theory/student_stat.py
+-rw-rw-rw-   0        0        0     4079 2022-09-15 12:02:16.000000 most_queue-1.21/most_queue/theory/weibull.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.265409 most_queue-1.21/most_queue/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-17 17:19:33.000000 most_queue-1.21/most_queue/utils/__init__.py
+-rw-rw-rw-   0        0        0     2078 2023-05-17 17:18:48.000000 most_queue-1.21/most_queue/utils/approx_cdf_make.py
+-rw-rw-rw-   0        0        0      319 2023-05-18 16:11:27.000000 most_queue-1.21/most_queue/utils/binom_probs.py
+-rw-rw-rw-   0        0        0     2761 2023-06-02 20:11:23.000000 most_queue-1.21/most_queue/utils/tables.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.265946 most_queue-1.21/most_queue/visualisation/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.21/most_queue/visualisation/__init__.py
+-rw-rw-rw-   0        0        0    35629 2022-09-30 18:59:24.000000 most_queue-1.21/most_queue/visualisation/smo_im_vis.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.268981 most_queue-1.21/most_queue/visualisation/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.21/most_queue/visualisation/utils/__init__.py
+-rw-rw-rw-   0        0        0     3169 2022-06-17 16:46:09.000000 most_queue-1.21/most_queue/visualisation/utils/result_table.py
+-rw-rw-rw-   0        0        0    14872 2022-08-16 20:24:21.000000 most_queue-1.21/most_queue/visualisation/utils/settings_window.py
+-rw-rw-rw-   0        0        0     1432 2022-06-03 20:22:54.000000 most_queue-1.21/most_queue/visualisation/utils/splash_screen.py
+drwxrwxrwx   0        0        0        0 2023-06-03 07:33:16.205174 most_queue-1.21/most_queue.egg-info/
+-rw-rw-rw-   0        0        0     6337 2023-06-03 07:33:16.000000 most_queue-1.21/most_queue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2556 2023-06-03 07:33:16.000000 most_queue-1.21/most_queue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 07:33:16.000000 most_queue-1.21/most_queue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-25 20:28:16.000000 most_queue-1.21/most_queue.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      114 2023-06-03 07:33:16.000000 most_queue-1.21/most_queue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-03 07:33:16.000000 most_queue-1.21/most_queue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      508 2023-06-03 07:33:06.000000 most_queue-1.21/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 07:33:16.269953 most_queue-1.21/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2023-06-03 07:32:58.000000 most_queue-1.21/setup.py
```

### Comparing `most_queue-1.20/LICENSE` & `most_queue-1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/PKG-INFO` & `most_queue-1.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: most_queue
-Version: 1.20
+Version: 1.21
 Summary: Software package for calculation and simulation of queuing systems
 Home-page: https://github.com/xabarov/mps
 Author: Xabarov Roman
 Author-email: Xabarov Roman <xabarov1985@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `most_queue-1.20/README.md` & `most_queue-1.21/README.md`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/sim/fj_delta_im.py` & `most_queue-1.21/most_queue/sim/fj_delta_sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import rand_destribution as rd
-from fj_im import SmoFJ as SmoFJ
-from fj_im import SubTask as SubTask
-from fj_im import Task as Task
-from smo_im import Server
+from fj_sim import ForkJoinSim
+from fj_sim import SubTask as SubTask
+from fj_sim import Task as Task
+from qs_sim import Server
 from most_queue.theory import sv_sum_calc
 
+import rand_destribution as rd
+
 
 class ServerWarmUp(Server):
     """
     Канал обслуживания
     """
     id = 0
 
@@ -52,25 +53,25 @@
     """
 
     def __init__(self, arr_time, task_id):
         SubTask.__init__(self, arr_time, task_id)
         self.future_arr_time = 0
 
 
-class SmoFJDelta(SmoFJ):
+class ForkJoinSimDelta(ForkJoinSim):
     """
     Имитационная модель СМО Fork-Join, Split-Join
     """
 
     def __init__(self, num_of_channels, num_of_parts, delta, is_SJ=False, buffer=None):
         """
         num_of_channels - количество каналов СМО
         buffer - максимальная длина очереди
         """
-        SmoFJ.__init__(self, num_of_channels, num_of_parts, is_SJ, buffer)
+        ForkJoinSim.__init__(self, num_of_channels, num_of_parts, is_SJ, buffer)
         self.delta = delta
         self.subtask_arr_queue = []
         self.serv_task_id = -1
         self.first_subtask_arr_time = {}
 
     def task_arrival(self):
         """
@@ -297,15 +298,14 @@
             res += "\nQueue Count " + str(len(self.queue)) + "\n"
 
         return res
 
 
 if __name__ == '__main__':
 
-    from most_queue.theory import mg1_calc
     from most_queue.theory import fj_calc
     from most_queue.theory import mg1_warm_calc
     from most_queue.utils.tables import times_print
 
     n = 3
     l = 1.0
     b1 = 0.35
@@ -313,19 +313,19 @@
     b1_delta = 0.1
     b_params = rd.H2_dist.get_params_by_mean_and_coev(b1, coev)
 
     delta_params = rd.H2_dist.get_params_by_mean_and_coev(b1_delta, coev)
     b_delta = rd.H2_dist.calc_theory_moments(*delta_params)
     b = rd.H2_dist.calc_theory_moments(*b_params, 4)
 
-    smo = SmoFJDelta(n, n, b_delta, True)
-    smo.set_sources(l, 'M')
-    smo.set_servers(b_params, 'H')
-    smo.run(100000)
-    v_im = smo.v
+    qs = ForkJoinSimDelta(n, n, b_delta, True)
+    qs.set_sources(l, 'M')
+    qs.set_servers(b_params, 'H')
+    qs.run(100000)
+    v_im = qs.v
 
     b_max_warm = fj_calc.getMaxMomentsDelta(n, b, 4, b_delta)
     b_max = fj_calc.getMaxMoments(n, b, 4)
     ro = l * b_max[0]
     v_ch = mg1_warm_calc.get_v(l, b_max, b_max_warm)
 
     print("\n")
@@ -345,19 +345,19 @@
     b1_delta = 0.1
     delta_params = rd.Erlang_dist.get_params_by_mean_and_coev(b1_delta, coev)
     b_delta = rd.Erlang_dist.calc_theory_moments(*delta_params)
 
     b_params = rd.Erlang_dist.get_params_by_mean_and_coev(b1, coev)
     b = rd.Erlang_dist.calc_theory_moments(*b_params, 4)
 
-    smo = SmoFJDelta(n, n, b_delta, True)
-    smo.set_sources(l, 'M')
-    smo.set_servers(b_params, 'E')
-    smo.run(100000)
-    v_im = smo.v
+    qs = ForkJoinSimDelta(n, n, b_delta, True)
+    qs.set_sources(l, 'M')
+    qs.set_servers(b_params, 'E')
+    qs.run(100000)
+    v_im = qs.v
 
     b_max_warm = fj_calc.getMaxMomentsDelta(n, b, 4, b_delta)
     b_max = fj_calc.getMaxMoments(n, b, 4)
     ro = l * b_max[0]
     v_ch = mg1_warm_calc.get_v(l, b_max, b_max_warm)
 
     print("\n\nКоэфф вариации времени обслуживания: ", coev)
```

### Comparing `most_queue-1.20/most_queue/sim/fj_im.py` & `most_queue-1.21/most_queue/sim/fj_sim.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import rand_destribution as rd
-from most_queue.sim import smo_im
+from qs_sim import QueueingSystemSimulator
 import math
 import sys
 from tqdm import tqdm
 
 from colorama import init
 from colorama import Fore, Style
 
@@ -44,25 +44,25 @@
 
     def __str__(self):
         res = "\tTask #" + str(self.id) + "\n"
         res += "\t\tArrival time: " + str(self.arr_time) + "\n"
         return res
 
 
-class SmoFJ(smo_im.SmoIm):
+class ForkJoinSim(QueueingSystemSimulator):
     """
     Имитационная модель СМО Fork-Join, Split-Join
     """
 
     def __init__(self, num_of_channels, k, is_SJ=False, is_Purge=False, buffer=None):
         """
         num_of_channels - количество каналов СМО
         buffer - максимальная длина очереди
         """
-        smo_im.SmoIm.__init__(self, num_of_channels, buffer)
+        QueueingSystemSimulator.__init__(self, num_of_channels, buffer)
         self.k = k
         self.is_SJ = is_SJ
         self.is_Purge = is_Purge
         self.served_subtask_in_task = {}
         self.sub_task_in_sys = 0
 
         self.queues = []
@@ -268,15 +268,15 @@
             for c in range(self.n):
                 res += str(self.servers[c])
             res += "\nQueue Count " + str(len(self.queue)) + "\n"
 
         return res
 
 
-class SetSmoException(Exception):
+class QueueingSystemException(Exception):
 
     def __str__(self, text):
         return text
 
 
 if __name__ == '__main__':
 
@@ -287,19 +287,19 @@
     n = 3
     l = 1.0
     b1 = 0.37
     coev = 1.5
     params = rd.H2_dist.get_params_by_mean_and_coev(b1, coev)
     b = rd.H2_dist.calc_theory_moments(*params, 4)
 
-    smo = SmoFJ(n, n, True)
-    smo.set_sources(l, 'M')
-    smo.set_servers(params, 'H')
-    smo.run(100000)
-    v_im = smo.v
+    qs = ForkJoinSim(n, n, True)
+    qs.set_sources(l, 'M')
+    qs.set_servers(params, 'H')
+    qs.run(100000)
+    v_im = qs.v
 
     b_max = fj_calc.getMaxMoments(n, b, 4)
     ro = l * b_max[0]
     v_ch = mg1_calc.get_v(l, b_max)
 
     print("\n")
     print("-" * 60)
@@ -310,19 +310,19 @@
     times_print(v_im, v_ch, is_w=False)
 
     coev = 0.8
     b1 = 0.5
     params = rd.Erlang_dist.get_params_by_mean_and_coev(b1, coev)
     b = rd.Erlang_dist.calc_theory_moments(*params, 4)
 
-    smo = SmoFJ(n, n, True)
-    smo.set_sources(l, 'M')
-    smo.set_servers(params, 'E')
-    smo.run(100000)
-    v_im = smo.v
+    qs = ForkJoinSim(n, n, True)
+    qs.set_sources(l, 'M')
+    qs.set_servers(params, 'E')
+    qs.run(100000)
+    v_im = qs.v
 
     b_max = fj_calc.getMaxMoments(n, b, 4)
     ro = l * b_max[0]
     v_ch = mg1_calc.get_v(l, b_max)
 
     print("\n\nКоэфф вариации времени обслуживания: ", coev)
     print("Коэффициент загрузки: {:4.3f}".format(ro))
```

### Comparing `most_queue-1.20/most_queue/sim/flow_sum_im.py` & `most_queue-1.21/most_queue/sim/flow_sum_sim.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import rand_destribution as rd
 from tqdm import tqdm
 import copy
 import math
 
 
-class SummatorIM:
+class FlowSumSim:
 
     def __init__(self, a, distr="Gamma", verbose=True, num_of_moments=4, num_of_jobs=1000000):
         self.n = len(a)
         self.a = a
         self.distr = distr
         self.verbose = verbose
         self.num_of_moments = num_of_moments
@@ -39,25 +39,25 @@
             return 0
 
         for i in range(n - 1):
             if self.verbose:
                 print("Summation of flows. Start simulation {0} from {1}. Distribution: {2}".format(i + 1, n - 1,
                                                                                                     distr_str))
             if self.distr == "Gamma":
-                f1 = SummatorIM.sum_2_Gamma_flows_im(self.a[0], self.a[1], num_of_sim=self.num_of_jobs,
-                                                     num_of_moments=self.num_of_moments)
-            elif self.distr == "H":
-                f1 = SummatorIM.sum_2_H2_flows_im(self.a[0], self.a[1], num_of_sim=self.num_of_jobs,
+                f1 = FlowSumSim.sum_2_Gamma_flows(self.a[0], self.a[1], num_of_sim=self.num_of_jobs,
                                                   num_of_moments=self.num_of_moments)
+            elif self.distr == "H":
+                f1 = FlowSumSim.sum_2_H2_flows(self.a[0], self.a[1], num_of_sim=self.num_of_jobs,
+                                               num_of_moments=self.num_of_moments)
             elif self.distr == "Pa":
-                f1 = SummatorIM.sum_2_Pa_flows_im(self.a[0], self.a[1], num_of_sim=self.num_of_jobs,
-                                                  num_of_moments=self.num_of_moments)
+                f1 = FlowSumSim.sum_2_Pa_flows(self.a[0], self.a[1], num_of_sim=self.num_of_jobs,
+                                               num_of_moments=self.num_of_moments)
             else:
-                f1 = SummatorIM.sum_2_Erlang_flows_im(self.a[0], self.a[1], num_of_sim=self.num_of_jobs,
-                                                      num_of_moments=self.num_of_moments)
+                f1 = FlowSumSim.sum_2_Erlang_flows(self.a[0], self.a[1], num_of_sim=self.num_of_jobs,
+                                                   num_of_moments=self.num_of_moments)
 
             self.flows_.append(f1)
             self.coevs.append(self.get_coev(f1))
             f = []
             f.append(f1)
 
             for j in range(len(self.a) - 2):
@@ -68,15 +68,15 @@
         for i in range(len(self.flows_)):
             self.a1_sum.append(self.flows_[i][0])
             self.a2_sum.append(self.flows_[i][1])
 
         self.result_flow = self.a[0]
 
     @staticmethod
-    def sum_2_H2_flows_im(a1, a2, num_of_moments=4, num_of_sim=1000000):
+    def sum_2_H2_flows(a1, a2, num_of_moments=4, num_of_sim=1000000):
         """
         суммирование двух потоков c коэффициентами вариации > 1
         Аппроксимация H2-распределением
         a1 - список из начальных моментов интервалов между соседникми заявками первого потока
         a2 - список из начальных моментов интервалов между соседникми заявками второго потока
         """
 
@@ -114,15 +114,15 @@
     @staticmethod
     def get_coev(a):
         D = a[1] - pow(a[0], 2)
         coev = math.sqrt(D) / a[0]
         return coev
 
     @staticmethod
-    def sum_2_Pa_flows_im(a1, a2, num_of_moments=4, num_of_sim=1000000):
+    def sum_2_Pa_flows(a1, a2, num_of_moments=4, num_of_sim=1000000):
         """
         суммирование двух потоков
         Аппроксимация Pa-распределением
         a1 - список из начальных моментов интервалов между соседникми заявками первого потока
         a2 - список из начальных моментов интервалов между соседникми заявками второго потока
         """
 
@@ -154,15 +154,15 @@
             for i in range(num_of_sim):
                 summ += pow(arrivals[i], k + 1)
             f[k] = summ / num_of_sim
 
         return f
 
     @staticmethod
-    def sum_2_Erlang_flows_im(a1, a2, num_of_moments=4, num_of_sim=1000000):
+    def sum_2_Erlang_flows(a1, a2, num_of_moments=4, num_of_sim=1000000):
 
         params1 = rd.Erlang_dist.get_params(a1)
         arr1 = rd.Erlang_dist(params1)
         params2 = rd.Erlang_dist.get_params(a2)
         arr2 = rd.Erlang_dist(params2)
         arrivals = []
         time1 = arr1.generate()
@@ -188,15 +188,15 @@
             for i in range(num_of_sim):
                 summ += pow(arrivals[i], k + 1)
             f[k] = summ / num_of_sim
 
         return f
 
     @staticmethod
-    def sum_2_Gamma_flows_im(a1, a2, num_of_moments=4, num_of_sim=1000000):
+    def sum_2_Gamma_flows(a1, a2, num_of_moments=4, num_of_sim=1000000):
         """
         суммирование двух потоков c коэффициентами вариации > 1
         Аппроксимация H2-распределением
         a1 - список из начальных моментов интервалов между соседникми заявками первого потока
         a2 - список из начальных моментов интервалов между соседникми заявками второго потока
         """
 
@@ -251,19 +251,19 @@
 
         for i in range(n - 1):
             if verbose:
                 print("Summation of flows. Start simulation {0} from {1}. Distribution: {2}".format(i + 1, n - 1,
                                                                                                     distr_str))
 
             if disr == "Gamma":
-                f1 = SummatorIM.sum_2_Gamma_flows_im(a[0], a[1])
+                f1 = FlowSumSim.sum_2_Gamma_flows(a[0], a[1])
             elif disr == "H":
-                f1 = SummatorIM.sum_2_H2_flows_im(a[0], a[1])
+                f1 = FlowSumSim.sum_2_H2_flows(a[0], a[1])
             else:
-                f1 = SummatorIM.sum_2_Erlang_flows_im(a[0], a[1])
+                f1 = FlowSumSim.sum_2_Erlang_flows(a[0], a[1])
 
             f = []
             for j in range(len(a) - 2):
                 f.append(a[j + 2])
             f.append(f1)
             a = copy.deepcopy(f)
```

### Comparing `most_queue-1.20/most_queue/sim/network_im_prty.py` & `most_queue-1.21/most_queue/sim/priority_network.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from smo_im_prty import SmoImPrty
+from priority_queue_sim import PriorityQueueSimulator
 import rand_destribution as rd
 import numpy as np
 import math
-from smo_im_prty import Task
+from priority_queue_sim import Task
 from most_queue.theory import network_calc
 import time
 from tqdm import tqdm
 import sys
 
 from colorama import init
 from colorama import Fore, Style
 
 init()
 
-class NetworkPrty:
+class PriorityNetwork:
     """
     Имитационная модель СеМО с многоканальными узлами и приоритетами
     """
 
     def __init__(self, k_num, L, R, n, prty, serv_params, nodes_prty):
 
         self.k_num = k_num  # число классов
@@ -30,15 +30,15 @@
         # serv_params[node][k][{'params':[...], 'type':'...'}]
         self.nodes_prty = nodes_prty  # [node][prty_numbers_in_new_order] перестановки исходных
         # номеров приоритетов по узлам
 
         self.smos = []
 
         for m in range(self.n_num):
-            self.smos.append(SmoImPrty(n[m], k_num, prty[m]))
+            self.smos.append(PriorityQueueSimulator(n[m], k_num, prty[m]))
             param_serv_reset = []  # из-за смены порядка приоритетов в узле
             # для расчета необходимо преобразовать список с параметрами вр обслуживания в узле
             for k in range(k_num):
                 param_serv_reset.append(serv_params[m][nodes_prty[m][k]])
 
             self.smos[m].set_servers(param_serv_reset)
             time.sleep(0.1)
@@ -196,19 +196,19 @@
 
     for k in range(k_num):
         b.append([])
         for m in range(n_num):
             b[k].append(rd.H2_dist.calc_theory_moments(*h2_params[m], 4))
 
     prty = ['NP'] * n_num
-    semo_im = NetworkPrty(k_num, L, R, n, prty, serv_params, nodes_prty)
+    qn = PriorityNetwork(k_num, L, R, n, prty, serv_params, nodes_prty)
 
-    semo_im.run(jobs_num)
+    qn.run(jobs_num)
 
-    v_im = semo_im.v_semo
+    v_im = qn.v_semo
 
     semo_calc = network_calc.network_prty_calc(R, b, n, L, prty, nodes_prty)
     v_ch = semo_calc['v']
     loads = semo_calc['loads']
 
     print("\n")
     print("-" * 60)
@@ -225,19 +225,19 @@
     print("-" * 60)
     print("{0:^60s}".format("Относительный приоритет"))
 
     print("-" * 60)
     times_print_with_classes(v_im, v_ch, is_w=False)
 
     prty = ['PR'] * n_num
-    semo_im = NetworkPrty(k_num, L, R, n, prty, serv_params, nodes_prty)
+    qn = PriorityNetwork(k_num, L, R, n, prty, serv_params, nodes_prty)
 
-    semo_im.run(jobs_num)
+    qn.run(jobs_num)
 
-    v_im = semo_im.v_semo
+    v_im = qn.v_semo
 
     semo_calc = network_calc.network_prty_calc(R, b, n, L, prty, nodes_prty)
     v_ch = semo_calc['v']
 
     print("-" * 60)
     print("{0:^60s}".format("Абсолютный приоритет"))
     print("-" * 60)
```

### Comparing `most_queue-1.20/most_queue/sim/queue_finite_source_sim.py` & `most_queue-1.21/most_queue/sim/queue_finite_source_sim.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import rand_destribution as rd
-from smo_im import SmoIm, SetSmoException, Task
+from qs_sim import QueueingSystemSimulator, QueueSystemException, Task
 
 
-class QueueFiniteSourceSim(SmoIm):
+class QueueingFiniteSourceSim(QueueingSystemSimulator):
     """
     Имитационная модель СМО GI/G/n/r и GI/G/n с конечным числом источников заявок
     """
 
     def __init__(self, num_of_channels, m, buffer=None, verbose=True, calc_next_event_time=False, cuda=False):
         """
         num_of_channels - количество каналов СМО
@@ -15,17 +15,17 @@
         verbose - вывод комментариев в процессе ИМ
         calc_next_event_time - нужно ли осуществлять расчет времени для след события (используется для визуализации)
         cuda - нужно ли использовать ускорение GPU при генерации заявок. Прирост в скорости небольшой, поэтому
         по умолчанию cuda=False
 
         Для запуска ИМ необходимо:
         - вызвать конструктор с параметрами
-        - задать вх поток с помощью метода set_sorces() экземпляра созданного класса SmoIm
-        - задать распределение обслуживания с помощью метода set_servers() экземпляра созданного класса SmoIm
-        - запустить ИМ с помощью метода run() экземпляра созданного класса SmoIm,
+        - задать вх поток с помощью метода set_sorces() экземпляра созданного класса QueueingFiniteSourceSim
+        - задать распределение обслуживания с помощью метода set_servers() экземпляра QueueingFiniteSourceSim
+        - запустить ИМ с помощью метода run() экземпляра созданного класса QueueingFiniteSourceSim,
         которому нужно передать число требуемых к обслуживанию заявок
 
         """
         self.m = m
         self.sources_left = m  # сколько источников готовы посылать заявки
 
         super().__init__(num_of_channels, buffer=buffer, verbose=verbose, calc_next_event_time=calc_next_event_time,
@@ -70,15 +70,15 @@
         elif self.source_types == "Uniform":
             self.source = rd.Uniform_dist(self.source_params)
         elif self.source_types == "Norm":
             self.source = rd.Normal_dist(self.source_params)
         elif self.source_types == "D":
             self.source = rd.Det_dist(self.source_params)
         else:
-            raise SetSmoException(
+            raise QueueSystemException(
                 "Неправильно задан тип распределения источника. Варианты М, Н, Е, С, Pa, Norm, Uniform")
 
         self.arrival_times = [self.source.generate() for i in range(self.m)]
 
     def arrival(self):
 
         """
@@ -282,22 +282,22 @@
     n = 1
 
     num_of_jobs = 1000000
 
     engset = Engset(lam, mu, m)
     v = engset.get_v()
 
-    smo = QueueFiniteSourceSim(n, m)
+    qs = QueueingFiniteSourceSim(n, m)
 
-    smo.set_sources(lam, 'M')
-    smo.set_servers(mu, 'M')
+    qs.set_sources(lam, 'M')
+    qs.set_servers(mu, 'M')
 
-    smo.run(num_of_jobs)
+    qs.run(num_of_jobs)
 
-    v_im = smo.v
-    p_im = smo.get_p()
+    v_im = qs.v
+    p_im = qs.get_p()
     p_ch = engset.get_p()
 
     probs_print(p_im, p_ch, 10)
 
-    print("Time spent ", smo.time_spent)
+    print("Time spent ", qs.time_spent)
     times_print(v_im, v, is_w=False)
```

### Comparing `most_queue-1.20/most_queue/sim/rand_destribution.py` & `most_queue-1.21/most_queue/sim/rand_destribution.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/sim/smo_batch_sim.py` & `most_queue-1.21/most_queue/sim/batch_sim.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from smo_im import SmoIm, Task
+from qs_sim import QueueingSystemSimulator, Task
 
 import numpy as np
 
 
-class SmoBatchSim(SmoIm):
+class QueueingSystemBatchSim(QueueingSystemSimulator):
     def __init__(self, num_of_channels, batch_prob, buffer=None, verbose=True):
         super().__init__(num_of_channels, buffer, verbose)
 
         self.batch_prob = batch_prob
         self.calc_cdf_prob()
 
     def calc_cdf_prob(self):
@@ -97,21 +97,21 @@
     mu = lam * moments[0] / ro
     n_jobs = 1000000
 
     batch_calc = BatchMM1(lam, mu, ls)
 
     v1 = batch_calc.get_v1()
 
-    smo = SmoBatchSim(n, ls)
+    qs = QueueingSystemBatchSim(n, ls)
 
-    smo.set_sources(lam, 'M')
-    smo.set_servers(mu, 'M')
+    qs.set_sources(lam, 'M')
+    qs.set_servers(mu, 'M')
 
-    smo.run(n_jobs)
+    qs.run(n_jobs)
 
-    v1_im = smo.v[0]
+    v1_im = qs.v[0]
 
     print("\nЗначения среднего времени пребывания заявок в системе:\n")
 
     print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
     print("-" * 45)
     print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(1, v1, v1_im))
```

### Comparing `most_queue-1.20/most_queue/sim/smo_im.py` & `most_queue-1.21/most_queue/sim/qs_sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from colorama import init
 from colorama import Fore, Style
 
 init()
 
 
-class SmoIm:
+class QueueingSystemSimulator:
     """
     Имитационная модель СМО GI/G/n/r и GI/G/n
     """
 
     def __init__(self, num_of_channels, buffer=None, verbose=True, calc_next_event_time=False, cuda=False):
         """
         Конструктор
@@ -25,17 +25,17 @@
         verbose - вывод комментариев в процессе ИМ
         calc_next_event_time - нужно ли осуществлять расчет времени для след события (используется для визуализации)
         cuda - нужно ли использовать ускорение GPU при генерации заявок. Прирост в скорости небольшой, поэтому
         по умолчанию cuda=False
 
         Для запуска ИМ необходимо:
         - вызвать конструктор с параметрами
-        - задать вх поток с помощью метода set_sorces() экземпляра созданного класса SmoIm
-        - задать распределение обслуживания с помощью метода set_servers() экземпляра созданного класса SmoIm
-        - запустить ИМ с помощью метода run() экземпляра созданного класса SmoIm,
+        - задать вх поток с помощью метода set_sorces() экземпляра созданного класса QueueSystemSimulator
+        - задать распределение обслуживания с помощью метода set_servers() экземпляра класса QueueSystemSimulator
+        - запустить ИМ с помощью метода run() экземпляра созданного класса QueueSystemSimulator,
         которому нужно передать число требуемых к обслуживанию заявок
 
         """
         self.n = num_of_channels
         self.buffer = buffer
         self.verbose = verbose  # выводить ли текстовые сообщения о работе
         self.cuda = cuda  # использование CUDA при ИМ для генерации ПСЧ
@@ -123,15 +123,15 @@
             elif types == "Unifrorm":
                 self.warm_dist = rd.Uniform_dist(params)
             elif types == "Norm":
                 self.warm_dist = rd.Normal_dist(params)
             elif types == "D":
                 self.warm_dist = rd.Det_dist(params)
             else:
-                raise SetSmoException(
+                raise QueueSystemException(
                     "Неправильно задан тип распределения времени обсл с разогревом. Варианты М, Н, Е, С, Pa, Uniform, Norm, D")
 
         self.is_set_warm = True
 
         self.is_only_first = is_only_first
 
     def set_sources(self, params, types):
@@ -169,15 +169,15 @@
         elif self.source_types == "Uniform":
             self.source = rd.Uniform_dist(self.source_params)
         elif self.source_types == "Norm":
             self.source = rd.Normal_dist(self.source_params)
         elif self.source_types == "D":
             self.source = rd.Det_dist(self.source_params)
         else:
-            raise SetSmoException(
+            raise QueueSystemException(
                 "Неправильно задан тип распределения источника. Варианты М, Н, Е, С, Pa, Norm, Uniform")
         self.arrival_time = self.source.generate()
 
     def set_servers(self, params, types):
         """
         Задает тип и параметры распределения времени обслуживания.
         Вид распределения                   Тип[types]     Параметры [params]
@@ -585,15 +585,15 @@
             for c in range(self.n):
                 res += str(self.servers[c])
             res += "\nQueue Count " + str(len(self.queue)) + "\n"
 
         return res
 
 
-class SetSmoException(Exception):
+class QueueSystemException(Exception):
 
     def __str__(self, text):
         return text
 
 
 class Task:
     """
@@ -646,15 +646,15 @@
         elif types == "Uniform":
             self.dist = rd.Uniform_dist(params)
         elif types == "Norm":
             self.dist = rd.Normal_dist(params)
         elif types == "D":
             self.dist = rd.Det_dist(params)
         else:
-            raise SetSmoException(
+            raise QueueSystemException(
                 "Неправильно задан тип распределения сервера. Варианты М, Н, Е, С, Pa, Norm, Uniform, D")
         self.time_to_end_service = 1e10
         self.is_free = True
         self.tsk_on_service = None
         Server.id += 1
         self.id = Server.id
 
@@ -679,15 +679,15 @@
         elif types == "Unifrorm":
             self.warm_dist = rd.Uniform_dist(params)
         elif types == "Norm":
             self.warm_dist = rd.Normal_dist(params)
         elif types == "D":
             self.warm_dist = rd.Det_dist(params)
         else:
-            raise SetSmoException(
+            raise QueueSystemException(
                 "Неправильно задан тип распределения времени обсл с разогревом. Варианты М, Н, Е, С, Pa, Uniform, Norm, D")
 
     def start_service(self, ts, ttek, is_warm=False):
 
         self.tsk_on_service = ts
         self.is_free = False
         if not is_warm:
@@ -723,41 +723,41 @@
     r = 100
     ro = 0.8
     num_of_jobs = 300000
     is_cuda = False
 
     mu = l / (ro * n)
 
-    smo = SmoIm(n, buffer=r, cuda=is_cuda)
+    qs = QueueingSystemSimulator(n, buffer=r, cuda=is_cuda)
 
-    smo.set_sources(l, 'M')
-    smo.set_servers(mu, 'M')
+    qs.set_sources(l, 'M')
+    qs.set_servers(mu, 'M')
 
-    smo.run(num_of_jobs)
+    qs.run(num_of_jobs)
 
     w = mmnr_calc.M_M_n_formula.get_w(l, mu, n, r)
 
-    w_im = smo.w
+    w_im = qs.w
 
-    print("Time spent ", smo.time_spent)
+    print("Time spent ", qs.time_spent)
 
     times_print(w_im, w)
 
     print("\n\nДанные ИМ::\n")
-    print(smo)
+    print(qs)
 
     print(f"M/D/{n}")
 
-    smo = SmoIm(n)
+    qs = QueueingSystemSimulator(n)
 
-    smo.set_sources(l, 'M')
-    smo.set_servers(1.0 / mu, 'D')
+    qs.set_sources(l, 'M')
+    qs.set_servers(1.0 / mu, 'D')
 
-    smo.run(num_of_jobs, is_real_served=False)
+    qs.run(num_of_jobs, is_real_served=False)
 
     mdn = m_d_n_calc.M_D_n(l, 1 / mu, n)
     p_ch = mdn.calc_p()
-    p_im = smo.get_p()
+    p_im = qs.get_p()
 
-    print("Time spent ", smo.time_spent)
+    print("Time spent ", qs.time_spent)
 
     probs_print(p_im, p_ch, 10)
```

### Comparing `most_queue-1.20/most_queue/sim/smo_im_prty.py` & `most_queue-1.21/most_queue/sim/priority_queue_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from colorama import Fore, Style
 
 import math
 
 init()
 
 
-class SmoImPrty:
+class PriorityQueueSimulator:
     """
     Имитационная модель СМО GI/G/n/r и GI/G/n с приоритетами
     """
 
     def __init__(self, num_of_channels, num_of_classes, prty_type='No', buffer=None, calc_next_event_time=False):
         """
         num_of_channels - количество каналов СМО
@@ -27,17 +27,17 @@
             RS  -  preemptive repeat with resampling, обслуживание заново с новой случайной длительностью
             RW  - preemptive repeat without resampling, обслуживание заново с прежней длительностью
             NP  - non preemptive, относиттельный приоритет
         buffer - максимальная длина очереди
 
         Для запуска ИМ необходимо:
         - вызвать конструктор с параметрами
-        - задать вх поток с помощью метода set_sorces() экземпляра созданного класса SmoImPrty
-        - задать распределение обслуживания с помощью метода set_servers() экземпляра созданного класса SmoImPrty
-        - запустить ИМ с помощью метода run() экземпляра созданного класса SmoImPrty,
+        - задать вх поток с помощью метода set_sorces() экземпляра созданного класса PriorityQueueSimulator
+        - задать распределение обслуживания с помощью метода set_servers() экземпляра класса PriorityQueueSimulator
+        - запустить ИМ с помощью метода run() экземпляра созданного класса PriorityQueueSimulator,
         которому нужно передать число требуемых к обслуживанию заявок
 
         """
         self.n = num_of_channels
         self.k = num_of_classes
         self.buffer = buffer
         self.prty_type = prty_type
@@ -130,15 +130,15 @@
             elif source_type == "Pa":
                 self.sources.append(rd.Pareto_dist(params))
             elif source_type == "Uniform":
                 self.sources.append(rd.Uniform_dist(params))
             elif self.source_types == "D":
                 self.sources.append(rd.Det_dist(params))
             else:
-                raise SetSmoException(
+                raise QueueingSystemException(
                     "Неправильно задан тип распределения источника. Варианты М, Н, Е, С, Pa, Uniform, D")
             self.arrival_time[i] = self.sources[i].generate()
             time.sleep(0.1)
 
     def set_servers(self, servers_params):
         """
         Задает тип и параметры распределения времени обслуживания.
@@ -197,15 +197,15 @@
             elif warm_up_type == "Pa":
                 self.warm_up.append(rd.Pareto_dist(params))
             elif warm_up_type == "Uniform":
                 self.warm_up.append(rd.Uniform_dist(params))
             elif warm_up_type == "D":
                 self.warm_up.append(rd.Det_dist(params))
             else:
-                raise SetSmoException(
+                raise QueueingSystemException(
                     "Неправильно задан тип распределения разогрева. Варианты М, Н, Е, С, Pa, Uniform, D")
 
     def calc_load(self):
 
         """
         Вычисляет коэффициент загрузки СМО
         """
@@ -681,15 +681,15 @@
                 res += str(self.servers[c]) + "\n"
                 for kk in range(self.k):
                     res += "Queue # " + str(kk + 1) + " count " + str(len(self.queue[kk])) + "\n"
 
         return res
 
 
-class SetSmoException(Exception):
+class QueueingSystemException(Exception):
 
     def __str__(self, text):
         return text
 
 
 class Task:
     """
@@ -752,15 +752,15 @@
             elif dist_type == "C":
                 self.dist.append(rd.Cox_dist(params))
             elif dist_type == "Pa":
                 self.dist.append(rd.Pareto_dist(params))
             elif dist_type == "Uniform":
                 self.dist.append(rd.Uniform_dist(params))
             else:
-                raise SetSmoException(
+                raise QueueingSystemException(
                     "Неправильно задан тип распределения сервера. Варианты М, Н, Е, С, Gamma, Pa, Uniform")
         self.time_to_end_service = 1e10
         self.total_time_to_serve = 0
         # Сохранение типа дисциплины обслуживания необходимо для
         # корректного назначения времени обслуживания после прерывания
         self.prty_type = prty_type
         self.is_free = True
@@ -839,44 +839,44 @@
 
     print("\nСравнение данных ИМ и результатов расчета методом инвариантов отношения (Р) \n"
           "времени пребывания в многоканальной СМО с приоритетами")
     print("Число каналов: " + str(n) + "\nЧисло классов: " + str(k) + "\nКоэффициент загрузки: {0:<1.2f}".format(ro) +
           "\nКоэффициент вариации времени обслуживания: " + str(coev) + "\n")
     print("Абсолютный приоритет")
 
-    smo = SmoImPrty(n, k, "PR")
+    qs = PriorityQueueSimulator(n, k, "PR")
     sources = []
     servers_params = []
     for j in range(k):
         sources.append({'type': 'M', 'params': l[j]})
         servers_params.append({'type': 'Gamma', 'params': params[j]})
 
-    smo.set_sources(sources)
-    smo.set_servers(servers_params)
+    qs.set_sources(sources)
+    qs.set_servers(servers_params)
 
-    smo.run(num_of_jobs)
+    qs.run(num_of_jobs)
 
-    v_im = smo.v
+    v_im = qs.v
 
     v_teor = prty_calc.get_v_prty_invar(l, b, n, 'PR')
 
     times_print_with_classes(v_im, v_teor, is_w=False)
 
     print("Относительный приоритет")
 
-    smo = SmoImPrty(n, k, "NP")
+    qs = PriorityQueueSimulator(n, k, "NP")
     sources = []
     servers_params = []
     for j in range(k):
         sources.append({'type': 'M', 'params': l[j]})
         servers_params.append({'type': 'Gamma', 'params': params[j]})
 
-    smo.set_sources(sources)
-    smo.set_servers(servers_params)
+    qs.set_sources(sources)
+    qs.set_servers(servers_params)
 
-    smo.run(num_of_jobs)
+    qs.run(num_of_jobs)
 
-    v_im = smo.v
+    v_im = qs.v
 
     v_teor = prty_calc.get_v_prty_invar(l, b, n, 'NP')
 
     times_print_with_classes(v_im, v_teor, is_w=False)
```

### Comparing `most_queue-1.20/most_queue/sim/smo_impatient_im.py` & `most_queue-1.21/most_queue/sim/impatient_queue_sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import rand_destribution as rd
-from smo_im import SmoIm, SetSmoException, Task
+from qs_sim import QueueingSystemSimulator, QueueSystemException, Task
 
 
 class ImpatientTask(Task):
     def __init__(self, arr_time, moment_to_leave):
         super().__init__(arr_time)
         self.moment_to_leave = moment_to_leave
 
     def __str__(self):
         return f'Task # {self.id}\nArrival moment: {self.arr_time:8.3f}\nMoment to leave: {self.moment_to_leave:8.3f}'
 
 
-class SmoImpatientSim(SmoIm):
+class ImpatientQueueSim(QueueingSystemSimulator):
     def __init__(self, num_of_channels, buffer=None, verbose=True):
         super().__init__(num_of_channels, buffer, verbose)
 
         self.impatience_params = None
         self.impatience_types = None
 
     def set_impatiens(self, params, types):
@@ -49,15 +49,15 @@
         elif self.impatience_types == "Gamma":
             self.impatience = rd.Gamma(self.impatience_params)
         elif self.impatience_types == "Uniform":
             self.impatience = rd.Uniform_dist(self.impatience_params)
         elif self.impatience_types == "D":
             self.impatience = rd.Det_dist(self.impatience_params)
         else:
-            raise SetSmoException(
+            raise QueueSystemException(
                 "Неправильно задан тип распределения нетерпения заявок. Варианты М, Н, Е, С, D, Pa, Uniform")
 
     def arrival(self):
 
         """
         Действия по прибытию заявки в СМО.
         """
@@ -171,22 +171,22 @@
     ro = 0.8
     n_jobs = 300000
     mu = l / (ro * n)
     gamma = 0.2
 
     v1 = impatience_calc.get_v1(l, mu, gamma)
 
-    smo = SmoImpatientSim(n)
+    qs = ImpatientQueueSim(n)
 
-    smo.set_sources(l, 'M')
-    smo.set_servers(mu, 'M')
-    smo.set_impatiens(gamma, 'M')
+    qs.set_sources(l, 'M')
+    qs.set_servers(mu, 'M')
+    qs.set_impatiens(gamma, 'M')
 
-    smo.run(n_jobs)
+    qs.run(n_jobs)
 
-    v1_im = smo.v[0]
+    v1_im = qs.v[0]
 
     print("\nЗначения среднего времени пребывания заявок в системе:\n")
 
     print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
     print("-" * 45)
     print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(1, v1, v1_im))
```

### Comparing `most_queue-1.20/most_queue/tests/ek_d_n.py` & `most_queue-1.21/most_queue/tests/ek_d_n.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from most_queue.sim import smo_im
+from most_queue.sim.qs_sim import QueueingSystemSimulator
 from most_queue.sim import rand_destribution as rd
 from most_queue.theory.ek_d_n_calc import Ek_D_n
+from most_queue.utils.tables import probs_print
 
 
 def test():
     """
     Тестирование численного расчета многоканальной системы Ek/D/n
     с детерминированным обслуживанием
 
@@ -39,34 +40,27 @@
     ekdn = Ek_D_n(l, k, b, n)
 
     # запускаем расчет вероятностей состояний СМО
     p_ch = ekdn.calc_p()
 
     # для верификации используем ИМ.
     # создаем экземпляр класса ИМ, передаем число каналов обслуживания
-    smo = smo_im.SmoIm(n)
+    qs = QueueingSystemSimulator(n)
 
     # задаем входной поток. Методу нужно передать параметры распределения списком и тип распределения. E - Эрланг
-    smo.set_sources([k, l], "E")
+    qs.set_sources([k, l], "E")
     # задаем каналы обслуживания. На вход время обслуживания и тип распределения - D.
-    smo.set_servers(b, "D")
+    qs.set_servers(b, "D")
 
     # запускаем ИМ:
-    smo.run(num_of_jobs)
+    qs.run(num_of_jobs)
 
     # получаем параметры - начальные моменты времени пребывания и распределение веротяностей состояния системы
-    v_im = smo.v
-    p_im = smo.get_p()
+    v_sim = qs.v
+    p_sim = qs.get_p()
 
     # выводим полученные значения:
-    print("-" * 36)
-    print("{0:^36s}".format("Вероятности состояний СМО E{0:d}/D/{1:d}".format(k, n)))
-    print("-" * 36)
-    print("{0:^4s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
-    print("-" * 36)
-    for i in range(11):
-        print("{0:^4d}|{1:^15.5g}|{2:^15.5g}".format(i, p_ch[i], p_im[i]))
-    print("-" * 36)
+    probs_print(p_sim, p_ch, 10)
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `most_queue-1.20/most_queue/tests/fj_calc.py` & `most_queue-1.21/most_queue/tests/fj_calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from most_queue.theory import fj_calc
-from most_queue.sim.fj_im import SmoFJ
+from most_queue.sim.fj_sim import ForkJoinSim
 import matplotlib.pyplot as plt
 
 
 def test():
     """
     Тестирование аппроксимаций для системы Fork-Join
     В пакете most_queue.theory.fj_calc модержатся следующие методы:
@@ -28,60 +28,60 @@
     # интенсивность обслуживания и начальные моменты
     mu = 1.0
     b = [1 / mu, 2 / pow(mu, 2), 6 / pow(mu, 3)]
 
     l = ro / b[0]  # интенсивность вх потока
 
     # массивы для накопления средних времен пребывания в СМО
-    v_im = []
+    v_sim = []
     v_varma = []
     v_varki = []
     v_nelson = []
 
     str_f = "{0:^15s}|{1:^15s}|{2:^15s}|{3:^15s}"
     str_f_v = "\n{0:^15.3f}|{1:^15.3f}|{2:^15.3f}|{3:^15.3f}"
     print(str_f.format("ИМ", "Varki", "Varma", "Nelson"))
 
     for i, nn in enumerate(n):
         # для верификации используем ИМ.
         # создаем экземпляр класса ИМ, передаем число каналов обслуживания
         # ИМ поддерживает СМО типа Fork-Join (n, k). В нашем случае k = n
 
-        smo = SmoFJ(nn, nn, False)
+        qs = ForkJoinSim(nn, nn, False)
 
         # задаем входной поток. Методу нужно передать параметры распределения и тип распределения. М - экспоненциальное
-        smo.set_sources(l, 'M')
+        qs.set_sources(l, 'M')
 
         # задаем каналы обслуживания. Методу нужно передать параметры распределения и тип распределения. М - экспоненциальное
-        smo.set_servers(mu, 'M')
+        qs.set_servers(mu, 'M')
 
         # запускаем ИМ
-        smo.run(num_of_jobs)
+        qs.run(num_of_jobs)
 
         # получаем список начальных моментов времени пребывания заявок в СМО и сохраняем
         # в массив только среднее (первый нач момент)
-        v = smo.v
-        v_im.append(v[0])
+        v = qs.v
+        v_sim.append(v[0])
 
         # расчет средних времен пребывания с помощью аппроксимаций. \
         # На вход каждого из методов - l, mu, nn (число каналов СМО)
 
         v_varki.append(fj_calc.get_v1_fj_varki_merchant(l, mu, nn))
         v_varma.append(fj_calc.get_v1_fj_varma(l, mu, nn))
         v_nelson.append(fj_calc.get_v1_fj_nelson_tantawi(l, mu, nn))
 
-        print(str_f_v.format(v_im[i], v_varki[i], v_varma[i], v_nelson[i]))
+        print(str_f_v.format(v_sim[i], v_varki[i], v_varma[i], v_nelson[i]))
 
     # строим графики и сохраняем в текущую директорию:
 
     fig, ax = plt.subplots()
 
     linestyles = ["solid", "dotted", "dashed", "dashdot"]
 
-    ax.plot(n, v_im, label="ИМ", linestyle=linestyles[0])
+    ax.plot(n, v_sim, label="ИМ", linestyle=linestyles[0])
     ax.plot(n, v_varki, label="Varki", linestyle=linestyles[1])
     ax.plot(n, v_varma, label="Varma", linestyle=linestyles[2])
     ax.plot(n, v_nelson, label="Nelson", linestyle=linestyles[3])
 
     ax.set_ylabel("v1")
     ax.set_xlabel("n")
 
@@ -89,18 +89,18 @@
     plt.savefig("v1_from_n_with_ro = {0:^4.2f}.png".format(ro), dpi=300)
 
     # errors
     v_nelson_err = []
     v_varma_err = []
     v_varki_err = []
 
-    for i in range(len(v_im)):
-        v_varma_err.append(100 * (v_varma[i] - v_im[i]) / v_im[i])
-        v_varki_err.append(100 * (v_varki[i] - v_im[i]) / v_im[i])
-        v_nelson_err.append(100 * (v_nelson[i] - v_im[i]) / v_im[i])
+    for i in range(len(v_sim)):
+        v_varma_err.append(100 * (v_varma[i] - v_sim[i]) / v_sim[i])
+        v_varki_err.append(100 * (v_varki[i] - v_sim[i]) / v_sim[i])
+        v_nelson_err.append(100 * (v_nelson[i] - v_sim[i]) / v_sim[i])
 
     fig, ax = plt.subplots()
     ax.plot(n, v_varki_err, label="Varki", linestyle=linestyles[0])
     ax.plot(n, v_varma_err, label="Varma", linestyle=linestyles[1])
     ax.plot(n, v_nelson_err, label="Nelson", linestyle=linestyles[2])
 
     ax.set_ylabel("error, %")
```

### Comparing `most_queue-1.20/most_queue/tests/fj_im.py` & `most_queue-1.21/most_queue/tests/fj_im.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from most_queue.theory import mg1_calc
 from most_queue.theory import fj_calc
-from most_queue.sim.fj_im import SmoFJ
+from most_queue.sim.fj_sim import ForkJoinSim
 from most_queue.sim import rand_destribution as rd
 
 
 def test():
     """
     Тестирование расчета системы Split-Join
         | Рыжиков, Ю. И. Метод расчета длительности обработки задач в системе массового обслуживания
@@ -31,28 +31,28 @@
 
 
     # для верификации используем ИМ.
     # создаем экземпляр класса ИМ, передаем число каналов обслуживания
     # ИМ поддерживает СМО типа Fork-Join (n, k). В нашем случае k = n
     # Для задания СМО Split-Join необходимо передать третий параметр True, иначе по умаолчанию - Fork-Join
 
-    smo = SmoFJ(n, n, True)
+    qs = ForkJoinSim(n, n, True)
 
     # задаем входной поток. Методу нужно передать параметры распределения и тип распределения. М - экспоненциальное
-    smo.set_sources(l, 'M')
+    qs.set_sources(l, 'M')
 
     # задаем каналы обслуживания. Методу нужно передать параметры распределения и тип распределения.
     # H - гиперэкспоненциальное второго параядка
-    smo.set_servers(params, 'H')
+    qs.set_servers(params, 'H')
 
     # запускаем ИМ
-    smo.run(num_of_jobs)
+    qs.run(num_of_jobs)
 
     # получаем список начальных моментов времени пребывания заявок в СМО
-    v_im = smo.v
+    v_sim = qs.v
 
     # расчет начальных моментов распределения максимума с помощью метода fj_calc.getMaxMoments.
     # На вход число каналов, список начальных моментов
     b_max = fj_calc.getMaxMoments(n, b)
     ro = l * b_max[0]
 
     # далее расчет как обычной СМО M/G/1 начальными моментами распределения максимума СВ
@@ -64,40 +64,40 @@
     print("-" * 60)
     print("Коэфф вариации времени обслуживания: ", coev)
     print("Коэффициент загрузки: {:4.3f}".format(ro))
     print("Начальные моменты времени пребывания заявок в системе:")
     print("-" * 60)
     print("{0:^15s}|{1:^20s}|{2:^20s}".format("№ момента", "Числ", "ИМ"))
     print("-" * 60)
-    for j in range(min(len(v_ch), len(v_im))):
-        print("{0:^16d}|{1:^20.5g}|{2:^20.5g}".format(j + 1, v_ch[j], v_im[j]))
+    for j in range(min(len(v_ch), len(v_sim))):
+        print("{0:^16d}|{1:^20.5g}|{2:^20.5g}".format(j + 1, v_ch[j], v_sim[j]))
     print("-" * 60)
 
     # тоже для коэфф вариации < 1 (аппроксимируем распределением Эрланга)
     coev = 0.8
     b1 = 0.5
     params = rd.Erlang_dist.get_params_by_mean_and_coev(b1, coev)
     b = rd.Erlang_dist.calc_theory_moments(*params, 4)
 
-    smo = SmoFJ(n, n, True)
-    smo.set_sources(l, 'M')
-    smo.set_servers(params, 'E')
-    smo.run(num_of_jobs)
-    v_im = smo.v
+    qs = ForkJoinSim(n, n, True)
+    qs.set_sources(l, 'M')
+    qs.set_servers(params, 'E')
+    qs.run(num_of_jobs)
+    v_sim = qs.v
 
     b_max = fj_calc.getMaxMoments(n, b)
     ro = l * b_max[0]
     v_ch = mg1_calc.get_v(l, b_max)
 
     print("\n\nКоэфф вариации времени обслуживания: ", coev)
     print("Коэффициент загрузки: {:4.3f}".format(ro))
     print("Начальные моменты времени пребывания заявок в системе:")
     print("-" * 60)
     print("{0:^15s}|{1:^20s}|{2:^20s}".format("№ момента", "Числ", "ИМ"))
     print("-" * 60)
-    for j in range(min(len(v_ch), len(v_im))):
-        print("{0:^16d}|{1:^20.5g}|{2:^20.5g}".format(j + 1, v_ch[j], v_im[j]))
+    for j in range(min(len(v_ch), len(v_sim))):
+        print("{0:^16d}|{1:^20.5g}|{2:^20.5g}".format(j + 1, v_ch[j], v_sim[j]))
     print("-" * 60)
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `most_queue-1.20/most_queue/tests/flow_sum.py` & `most_queue-1.21/most_queue/tests/flow_sum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from most_queue.theory.flow_sum import SummatorNumeric
-from most_queue.sim import flow_sum_im
+from most_queue.sim.flow_sum_sim import FlowSumSim
 from most_queue.sim import rand_destribution as rd
 import matplotlib.pyplot as plt
 
 
 def test():
     """
     Тестирование суммирования потоков
@@ -29,46 +29,46 @@
 
     # Численный расчет
     s = SummatorNumeric(a, is_semi=is_semi)
     s.sum_flows()  # в  s._flows[i][j] содержатся начальные моменты суммируемых потокоы,
     # i - кол-во суммируемых потоков, j - номер начального момента
 
     # ИМ
-    s_im = flow_sum_im.SummatorIM(a, distr=distr_im, num_of_jobs=num_of_jobs)
-    s_im.sum_flows()  # в  s_im._flows[i][j] содержатся начальные моменты суммируемых потокоы,
+    s_sim = FlowSumSim(a, distr=distr_im, num_of_jobs=num_of_jobs)
+    s_sim.sum_flows()  # в  s_sim._flows[i][j] содержатся начальные моменты суммируемых потокоы,
     # i - кол-во суммируемых потоков, j - номер начального момента
 
     # Расчет ошибок и отображение результатов
-    coevs_im = s_im.coevs
+    coevs_sim = s_sim.coevs
     coevs_num = s.coevs
     errors1 = []
     errors2 = []
     errors_coev = []
 
     str_f = "{0:^18s}|{1:^10.3f}|{2:^10.3f}|{3:^10.3f}|{4:^10.3f}|{5:^10.3f}"
     print("{0:^18s}|{1:^10s}|{2:^10s}|{3:^10s}|{4:^10s}|{5:^10s}".format("-", "a1", "a2", "a3", "a4", "coev"))
     print("-" * 80)
 
     for i in range(n_nums - 1):
         print("{0:^80s}".format("Сумма " + str(i + 2) + " потоков"))
         print("-" * 80)
-        print(str_f.format("ИМ", s_im.flows_[i][0], s_im.flows_[i][1], s_im.flows_[i][2], s_im.flows_[i][3],
+        print(str_f.format("ИМ", s_sim.flows_[i][0], s_sim.flows_[i][1], s_sim.flows_[i][2], s_sim.flows_[i][3],
                            coevs_num[i]))
         print("-" * 80)
         print(str_f.format("Числ", s.flows_[i][0].real, s.flows_[i][1].real, s.flows_[i][2].real, s.flows_[i][3].real,
-                           coevs_im[i]))
+                           coevs_sim[i]))
         print("-" * 80)
-        errors1.append(SummatorNumeric.get_error(s.flows_[i][0].real, s_im.flows_[i][0]))
-        errors2.append(SummatorNumeric.get_error(s.flows_[i][1].real, s_im.flows_[i][1]))
-        errors_coev.append(SummatorNumeric.get_error(coevs_num[i], coevs_im[i]))
+        errors1.append(SummatorNumeric.get_error(s.flows_[i][0].real, s_sim.flows_[i][0]))
+        errors2.append(SummatorNumeric.get_error(s.flows_[i][1].real, s_sim.flows_[i][1]))
+        errors_coev.append(SummatorNumeric.get_error(coevs_num[i], coevs_sim[i]))
 
     fig, ax = plt.subplots()
     linestyles = ["solid", "dotted", "dashed", "dashdot"]
 
-    ax.plot(ns, s_im.a1_sum, label="ИМ a1", linestyle=linestyles[0])
+    ax.plot(ns, s_sim.a1_sum, label="ИМ a1", linestyle=linestyles[0])
     ax.plot(ns, s.a1_sum, label="Числ a1", linestyle=linestyles[1])
 
     plt.legend()
     str_title = "Среднее сумм-х потоков, %"
     if is_semi:
         str_title += ". Метод семиинвариантов"
     else:
```

### Comparing `most_queue-1.20/most_queue/tests/gi_m_1_calc.py` & `most_queue-1.21/most_queue/tests/gi_m_n_calc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,110 +1,113 @@
-from most_queue.theory.gi_m_1_calc import *
+from most_queue.theory.gi_m_n_calc import *
 from most_queue.sim import rand_destribution as rd
-from most_queue.sim import smo_im
+from most_queue.sim.qs_sim import QueueingSystemSimulator
 
 
 def test():
     """
-    Тестирование расчета СМО GI/M/1
+    Тестирование расчета СМО GI/M/n
     Для верификации используем имитационное моделирование (ИМ).
     """
 
-    l = 1  # интенсивность вх потока
-    a1 = 1 / l  # средний интревал между заявками
-    b1 = 0.9  # среднее время обслуживания
+    l = 1.0  # интенсивность вх потока
+    a1 = 1.0 / l  # средний интревал между заявками
+    n = 4   # число каналов
+    ro = 0.8  # коэффициент загрузки СМО
+    b1 = ro * n / l  # среднее время обслуживания из заданного ro
     mu = 1 / b1  # интенсивность обслуживания
     a_coev = 1.6  # коэфф вариации вх потока
+
     num_of_jobs = 800000  # количество заявок для ИМ. Чем больше, тем выше точночть ИМ
 
     # расчет параметров аппроксимирующего Гамма-распределения для вх птокоа по заданным среднему и коэфф вариации
     v, alpha = rd.Gamma.get_mu_alpha_by_mean_and_coev(a1, a_coev)
     a = rd.Gamma.calc_theory_moments(v, alpha)
 
     # расчет начальных моментов времени пребывания и ожидания в СМО
-    v_ch = get_v(a, mu)
-    w_ch = get_w(a, mu)
+    v_ch = get_v(a, mu, n)
+    w_ch = get_w(a, mu, n)
 
     # расчет вероятностей состояний СМО
-    p_ch = get_p(a, mu)
+    p_ch = get_p(a, mu, n)
 
     # для верификации используем ИМ.
     # создаем экземпляр класса ИМ, передаем число каналов обслуживания
-    smo = smo_im.SmoIm(1)
+    qs = QueueingSystemSimulator(n)
 
     # задаем входной поток. Методу нужно передать параметры распределения списком и тип распределения.
-    smo.set_sources([v, alpha], "Gamma")
+    qs.set_sources([v, alpha], "Gamma")
 
     # задаем каналы обслуживания. На вход параметры (в нашем случае интенсивность обслуживания)
     # и тип распределения - М (экспоненциальное).
-    smo.set_servers(mu, "M")
+    qs.set_servers(mu, "M")
 
     # запускаем ИМ:
-    smo.run(num_of_jobs)
+    qs.run(num_of_jobs)
 
     # получаем список начальных моментов времени пребывания и ожидания в СМО
-    v_im = smo.v
-    w_im = smo.w
+    v_sim = qs.v
+    w_sim = qs.w
 
     # получаем распределение вероятностей состояний СМО
-    p_im = smo.get_p()
+    p_sim = qs.get_p()
 
     # Вывод результатов
     print("\nGamma. Значения начальных моментов времени пребывания заявок в системе:\n")
 
     print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
     print("-" * 45)
     for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_sim[j]))
 
     print("\nЗначения начальных моментов времени ожидания заявок в системе:\n")
 
     print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
     print("-" * 45)
     for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_im[j]))
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_sim[j]))
 
     print("{0:^25s}".format("Вероятности состояний СМО"))
     print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
     print("-" * 32)
     for i in range(11):
-        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_im[i]))
-
-    # Тоже для распределения Парето
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_sim[i]))
 
+    # Тоже для Парето
     alpha, K = rd.Pareto_dist.get_a_k_by_mean_and_coev(a1, a_coev)
     a = rd.Pareto_dist.calc_theory_moments(alpha, K)
-    v_ch = get_v(a, mu, approx_distr="Pa")
-    w_ch = get_w(a, mu, approx_distr="Pa")
-    p_ch = get_p(a, mu, approx_distr="Pa")
-
-    smo = smo_im.SmoIm(1)
-    smo.set_sources([alpha, K], "Pa")
-    smo.set_servers(mu, "M")
-    smo.run(num_of_jobs)
-    v_im = smo.v
-    w_im = smo.w
-    p_im = smo.get_p()
+    v_ch = get_v(a, mu, n, approx_distr="Pa")
+    p_ch = get_p(a, mu, n, approx_distr="Pa")
+
+    qs = QueueingSystemSimulator(n)
+    qs.set_sources([alpha, K], "Pa")
+    qs.set_servers(mu, "M")
+    qs.run(num_of_jobs)
+    v_sim = qs.v
+    p_sim = qs.get_p()
 
     print("\nPareto. Значения начальных моментов времени пребывания заявок в системе:\n")
 
     print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
     print("-" * 45)
     for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_sim[j]))
+
+    w_ch = get_w(a, mu, n, approx_distr="Pa")
+    w_sim = qs.w
 
     print("\nЗначения начальных моментов времени ожидания заявок в системе:\n")
 
     print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
     print("-" * 45)
     for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_im[j]))
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_sim[j]))
 
     print("{0:^25s}".format("Вероятности состояний СМО"))
     print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
     print("-" * 32)
     for i in range(11):
-        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_im[i]))
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_sim[i]))
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `most_queue-1.20/most_queue/tests/gi_m_n_calc.py` & `most_queue-1.21/most_queue/tests/smo_im_prty.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,113 +1,105 @@
-from most_queue.theory.gi_m_n_calc import *
+from most_queue.sim.priority_queue_sim import PriorityQueueSimulator
+from most_queue.theory import prty_calc
 from most_queue.sim import rand_destribution as rd
-from most_queue.sim import smo_im
-
+from most_queue.utils.tables import probs_print, times_print_with_classes
 
 def test():
     """
-    Тестирование расчета СМО GI/M/n
-    Для верификации используем имитационное моделирование (ИМ).
+    Тестирование имитационной модели СМО с приоритетами
+    Для верификации - сравнение с результатами расчета СМО с методом инвариантов отношения:
+        Рыжиков Ю.И., Хомоненко А.Д. Расчет многоканальных систем обслуживания с абсолютным и
+        относительным приоритетами на основе инвариантов отношения // Интеллектуальные технологии
+        на транспорте. 2015. №3
     """
+    n = 5  # число каналов
+    k = 3  # число классов заявок
+    l = [0.2, 0.3, 0.4]  # интенсивности пребытия заявок по классам
+    lsum = sum(l)
+    num_of_jobs = 1000000  # количество заявок для ИМ
+
+    # Зададим параметры обслуживания по начальным моментам.
+    # Зададим средние времена обслуживания по классам
+    b1 = [0.45 * n, 0.9 * n, 1.35 * n]
+
+    # Коэфф вариации времени обслуживания пусть будет одинаковый для всех классов
+    coev = 0.577
+
+    # вторые начальные моменты
+    b2 = [0] * k #
+    for i in range(k):
+        b2[i] = (b1[i] ** 2) * (1 + coev ** 2)
+
+    b_sr = sum(b1) / k
+
+    # получим коэфф загрузки
+    ro = lsum * b_sr / n
+
+    # теперь по заданным двум нач моментам подберем параметры аппроксимирующего Гамма-распределения
+    # и добавим в список параметров params
+    params = []
+    for i in range(k):
+        params.append(rd.Gamma.get_mu_alpha([b1[i], b2[i]]))
+
+    b = []
+    for j in range(k):
+        b.append(rd.Gamma.calc_theory_moments(params[j][0], params[j][1], 4))
+
+    print("\nСравнение данных ИМ и результатов расчета методом инвариантов отношения (Р) \n"
+          "времени пребывания в многоканальной СМО с приоритетами")
+    print("Число каналов: " + str(n) + "\nЧисло классов: " + str(k) + "\nКоэффициент загрузки: {0:<1.2f}".format(ro) +
+          "\nКоэффициент вариации времени обслуживания: " + str(coev) + "\n")
+    print("Абсолютный приоритет")
+
+    # при создании ИМ передаем число каналов, число классов и тип приоритета.
+    # PR - абсолютный с дообслуживанием заявок
+    qs = PriorityQueueSimulator(n, k, "PR")
+
+    # для задания источников заявок и каналов обслуживания нужно задать набор словарей с полями
+    # type - тип распределения,
+    # params - его параметры.
+    # Число таких словарей в списках sources и servers_params соответствует числу классов
+
+    sources = []
+    servers_params = []
+    for j in range(k):
+        sources.append({'type': 'M', 'params': l[j]})
+        servers_params.append({'type': 'Gamma', 'params': params[j]})
+
+    qs.set_sources(sources)
+    qs.set_servers(servers_params)
+
+    # запуск ИМ
+    qs.run(num_of_jobs)
+
+    # получение начальных моментов времени пребывания
+
+    v_sim = qs.v
+
+    # расчет их же методом инвариантов отношения (для сравнения)
+    v_teor = prty_calc.get_v_prty_invar(l, b, n, 'PR')
+
+    times_print_with_classes(v_sim, v_teor, False)
+
+    print("Относительный приоритет")
+
+    # Тоже самое для относительного приоритета (NP)
+    qs = PriorityQueueSimulator(n, k, "NP")
+    sources = []
+    servers_params = []
+    for j in range(k):
+        sources.append({'type': 'M', 'params': l[j]})
+        servers_params.append({'type': 'Gamma', 'params': params[j]})
+
+    qs.set_sources(sources)
+    qs.set_servers(servers_params)
+
+    qs.run(num_of_jobs)
+
+    v_sim = qs.v
 
-    l = 1.0  # интенсивность вх потока
-    a1 = 1.0 / l  # средний интревал между заявками
-    n = 4   # число каналов
-    ro = 0.8  # коэффициент загрузки СМО
-    b1 = ro * n / l  # среднее время обслуживания из заданного ro
-    mu = 1 / b1  # интенсивность обслуживания
-    a_coev = 1.6  # коэфф вариации вх потока
-
-    num_of_jobs = 800000  # количество заявок для ИМ. Чем больше, тем выше точночть ИМ
-
-    # расчет параметров аппроксимирующего Гамма-распределения для вх птокоа по заданным среднему и коэфф вариации
-    v, alpha = rd.Gamma.get_mu_alpha_by_mean_and_coev(a1, a_coev)
-    a = rd.Gamma.calc_theory_moments(v, alpha)
-
-    # расчет начальных моментов времени пребывания и ожидания в СМО
-    v_ch = get_v(a, mu, n)
-    w_ch = get_w(a, mu, n)
-
-    # расчет вероятностей состояний СМО
-    p_ch = get_p(a, mu, n)
-
-    # для верификации используем ИМ.
-    # создаем экземпляр класса ИМ, передаем число каналов обслуживания
-    smo = smo_im.SmoIm(n)
-
-    # задаем входной поток. Методу нужно передать параметры распределения списком и тип распределения.
-    smo.set_sources([v, alpha], "Gamma")
-
-    # задаем каналы обслуживания. На вход параметры (в нашем случае интенсивность обслуживания)
-    # и тип распределения - М (экспоненциальное).
-    smo.set_servers(mu, "M")
-
-    # запускаем ИМ:
-    smo.run(num_of_jobs)
-
-    # получаем список начальных моментов времени пребывания и ожидания в СМО
-    v_im = smo.v
-    w_im = smo.w
-
-    # получаем распределение вероятностей состояний СМО
-    p_im = smo.get_p()
-
-    # Вывод результатов
-    print("\nGamma. Значения начальных моментов времени пребывания заявок в системе:\n")
-
-    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
-    print("-" * 45)
-    for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
-
-    print("\nЗначения начальных моментов времени ожидания заявок в системе:\n")
-
-    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
-    print("-" * 45)
-    for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_im[j]))
-
-    print("{0:^25s}".format("Вероятности состояний СМО"))
-    print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
-    print("-" * 32)
-    for i in range(11):
-        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_im[i]))
-
-    # Тоже для Парето
-    alpha, K = rd.Pareto_dist.get_a_k_by_mean_and_coev(a1, a_coev)
-    a = rd.Pareto_dist.calc_theory_moments(alpha, K)
-    v_ch = get_v(a, mu, n, approx_distr="Pa")
-    p_ch = get_p(a, mu, n, approx_distr="Pa")
-
-    smo = smo_im.SmoIm(n)
-    smo.set_sources([alpha, K], "Pa")
-    smo.set_servers(mu, "M")
-    smo.run(num_of_jobs)
-    v_im = smo.v
-    p_im = smo.get_p()
-
-    print("\nPareto. Значения начальных моментов времени пребывания заявок в системе:\n")
-
-    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
-    print("-" * 45)
-    for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
-
-    w_ch = get_w(a, mu, n, approx_distr="Pa")
-    w_im = smo.w
-
-    print("\nЗначения начальных моментов времени ожидания заявок в системе:\n")
-
-    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
-    print("-" * 45)
-    for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_im[j]))
-
-    print("{0:^25s}".format("Вероятности состояний СМО"))
-    print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
-    print("-" * 32)
-    for i in range(11):
-        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_im[i]))
+    v_teor = prty_calc.get_v_prty_invar(l, b, n, 'NP')
 
+    times_print_with_classes(v_sim, v_teor, False)
 
 if __name__ == "__main__":
     test()
```

### Comparing `most_queue-1.20/most_queue/tests/m_d_n_calc.py` & `most_queue-1.21/most_queue/tests/m_d_n_calc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from most_queue.sim import smo_im
+from most_queue.sim.qs_sim import QueueingSystemSimulator
 from most_queue.theory.m_d_n_calc import M_D_n
 
 
 def test():
     """
     Тестирование расчета СМО M/D/n
     Для верификации используем имитационное моделирование (ИМ).
@@ -16,37 +16,37 @@
 
     # расчет вероятностей состояний СМО
     mdn = M_D_n(l, b, n)
     p_ch = mdn.calc_p()
 
     # для верификации используем ИМ.
     # создаем экземпляр класса ИМ, передаем число каналов обслуживания
-    smo = smo_im.SmoIm(n)
+    qs = QueueingSystemSimulator(n)
 
     # задаем входной поток. Методу нужно передать параметры распределения и тип распределения.
-    smo.set_sources(l, "M")
+    qs.set_sources(l, "M")
 
     # задаем каналы обслуживания. На вход параметры (в нашем случае время обслуживания)
     # и тип распределения - D (детерминированное).
-    smo.set_servers(b, "D")
+    qs.set_servers(b, "D")
 
     # запускаем ИМ:
-    smo.run(num_of_jobs)
+    qs.run(num_of_jobs)
 
     # получаем список начальных моментов времени пребывания в СМО
-    v_im = smo.v
+    v_sim = qs.v
     # получаем распределение вероятностей состояний СМО
-    p_im = smo.get_p()
+    p_sim = qs.get_p()
 
     # Вывод результатов
     print("-" * 36)
     print("{0:^36s}".format("Вероятности состояний СМО M/D/{0:d}".format(n)))
     print("-" * 36)
     print("{0:^4s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
     print("-" * 36)
     for i in range(11):
-        print("{0:^4d}|{1:^15.5g}|{2:^15.5g}".format(i, p_ch[i], p_im[i]))
+        print("{0:^4d}|{1:^15.5g}|{2:^15.5g}".format(i, p_ch[i], p_sim[i]))
     print("-" * 36)
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `most_queue-1.20/most_queue/tests/m_h2_h2warm.py` & `most_queue-1.21/most_queue/tests/m_h2_h2warm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from most_queue.theory.m_h2_h2warm import Mh2h2Warm
-from most_queue.sim import smo_im
+from most_queue.sim.qs_sim import QueueingSystemSimulator
 from most_queue.sim import rand_destribution as rd
 
+from most_queue.utils.tables import probs_print, times_print
+
 import math
 import time
 
 
 def test():
-    n = 3  # число каналов
+    n = 5  # число каналов
     l = 1.0  # интенсивность вх потока
     ro = 0.7  # коэфф загрузки
     b1 = n * 0.7  # ср время обслуживания
-    b1_warm = n * 0.9  # ср время разогрева
+    b1_warm = n * 0.1  # ср время разогрева
     num_of_jobs = 1000000  # число обсл заявок ИМ
     b_coev = [0.8, 1.5]  # коэфф вариации времени обсл
     b_coev_warm = 1.2  # коэфф вариации времени разогрева
     buff = None  # очередь - неограниченная
     verbose = False  # не выводить пояснения при расчетах
 
     for k in range(len(b_coev)):
@@ -28,24 +30,24 @@
         b_w = [0.0] * 3
         b_w[0] = b1_warm
         alpha = 1 / (b_coev_warm ** 2)
         b_w[1] = math.pow(b_w[0], 2) * (math.pow(b_coev_warm, 2) + 1)
         b_w[2] = b_w[1] * b_w[0] * (1.0 + 2 / alpha)
 
         im_start = time.process_time()
-        smo = smo_im.SmoIm(n, buffer=buff)
-        smo.set_sources(l, 'M')
+        qs = QueueingSystemSimulator(n, buffer=buff)
+        qs.set_sources(l, 'M')
 
         gamma_params = rd.Gamma.get_mu_alpha(b)
         gamma_params_warm = rd.Gamma.get_mu_alpha(b_w)
-        smo.set_servers(gamma_params, 'Gamma')
-        smo.set_warm(gamma_params_warm, 'Gamma')
-        smo.run(num_of_jobs)
-        p = smo.get_p()
-        v_im = smo.v
+        qs.set_servers(gamma_params, 'Gamma')
+        qs.set_warm(gamma_params_warm, 'Gamma')
+        qs.run(num_of_jobs)
+        p = qs.get_p()
+        v_sim = qs.v
         im_time = time.process_time() - im_start
 
         tt_start = time.process_time()
         tt = Mh2h2Warm(l, b, b_w, n, buffer=buff, verbose=verbose)
 
         tt.run()
         p_tt = tt.get_p()
@@ -59,23 +61,13 @@
               "с комплексными параметрами\n"
               "Коэффициент загрузки: {1:^1.2f}".format(n, ro))
         print(f'Коэффициент вариации времени обслуживания {b_coev[k]:0.3f}')
         print(f'Коэффициент вариации времени разогрева {b_coev_warm:0.3f}')
         print("Количество итераций алгоритма Такахаси-Таками: {0:^4d}".format(num_of_iter))
         print("Время работы алгоритма Такахаси-Таками: {0:^5.3f} c".format(tt_time))
         print("Время ИМ: {0:^5.3f} c".format(im_time))
-        print("{0:^25s}".format("Первые 10 вероятностей состояний СМО"))
-        print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
-        print("-" * 32)
-        for i in range(11):
-            print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], p[i]))
-
-        print("\n")
-        print("{0:^25s}".format("Начальные моменты времени ожидания в СМО"))
-        print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
-        print("-" * 32)
-        for i in range(3):
-            print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i + 1, v_tt[i], v_im[i]))
+        probs_print(p, p_tt, 10)
+        times_print(v_sim, v_tt, False)
 
 
 if __name__ == '__main__':
     test()
```

### Comparing `most_queue-1.20/most_queue/tests/m_ph_n_prty.py` & `most_queue-1.21/most_queue/tests/m_ph_n_prty.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import math
-from most_queue.sim import smo_im_prty
+from most_queue.sim.priority_queue_sim import PriorityQueueSimulator
 from most_queue.sim import rand_destribution as rd
 from most_queue.theory import prty_calc
 import time
 from most_queue.theory.m_ph_n_prty import m_ph_n_prty
 
 
 def test():
@@ -94,33 +94,33 @@
         invar_times.append(time.process_time() - invar_start)
 
         im_start = time.process_time()
 
         for i in range(iteration):
             print("Start IM iteration: {0:d}".format(i + 1))
 
-            smo = smo_im_prty.SmoImPrty(n, K, "PR")
+            qs = PriorityQueueSimulator(n, K, "PR")
             sources = []
             servers_params = []
             l = [l_H, l_L]
 
             sources.append({'type': 'M', 'params': l_H})
             sources.append({'type': 'M', 'params': l_L})
             servers_params.append({'type': 'Gamma', 'params': gamma_params})
             servers_params.append({'type': 'M', 'params': mu_L})
 
-            smo.set_sources(sources)
-            smo.set_servers(servers_params)
+            qs.set_sources(sources)
+            qs.set_servers(servers_params)
 
             # запуск ИМ:
-            smo.run(num_of_jobs)
+            qs.run(num_of_jobs)
 
             # получение результатов ИМ:
-            p = smo.get_p()
-            v_im = smo.v
+            p = qs.get_p()
+            v_im = qs.v
             v1_sum += v_im[0][0]
             v2_sum += v_im[1][0]
 
         v1 = v1_sum / iteration
         v2 = v2_sum / iteration
         # расчет численным методом:
         v2_im_mass.append(v2)
```

### Comparing `most_queue-1.20/most_queue/tests/mg1_calc.py` & `most_queue-1.21/most_queue/tests/gi_m_1_calc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,127 +1,110 @@
-from most_queue.theory.mg1_calc import *
+from most_queue.theory.gi_m_1_calc import *
+from most_queue.sim import rand_destribution as rd
+from most_queue.sim.qs_sim import QueueingSystemSimulator
 
 
 def test():
     """
-    Тестирование расчета СМО M/G/1
+    Тестирование расчета СМО GI/M/1
     Для верификации используем имитационное моделирование (ИМ).
     """
-    l = 1  # интенсивность входного потока
+
+    l = 1  # интенсивность вх потока
+    a1 = 1 / l  # средний интревал между заявками
     b1 = 0.9  # среднее время обслуживания
-    coev = 1.6  # коэфф вариации времени обслуживания
-    num_of_jobs = 800000  # количество заявок для ИМ
+    mu = 1 / b1  # интенсивность обслуживания
+    a_coev = 1.6  # коэфф вариации вх потока
+    num_of_jobs = 800000  # количество заявок для ИМ. Чем больше, тем выше точночть ИМ
 
-    # подбор параметров аппроксимирующего H2-распределения для времени обслуживания [y1, mu1, mu2]:
-    params = rd.H2_dist.get_params_by_mean_and_coev(b1, coev)
-    b = rd.H2_dist.calc_theory_moments(*params, 4)
-
-    # вычисление численными методами
-    w_ch = get_w(l, b)
-    p_ch = get_p(l, b, 100)
-    v_ch = get_v(l, b)
-
-    # запуск ИМ для верификации результатов
-    smo = smo_im.SmoIm(1)
-    smo.set_servers(params, "H")
-    smo.set_sources(l, "M")
-    smo.run(num_of_jobs)
-    w_im = smo.w
-    p_im = smo.get_p()
-    v_im = smo.v
+    # расчет параметров аппроксимирующего Гамма-распределения для вх птокоа по заданным среднему и коэфф вариации
+    v, alpha = rd.Gamma.get_mu_alpha_by_mean_and_coev(a1, a_coev)
+    a = rd.Gamma.calc_theory_moments(v, alpha)
 
-    # вывод результатов
+    # расчет начальных моментов времени пребывания и ожидания в СМО
+    v_ch = get_v(a, mu)
+    w_ch = get_w(a, mu)
 
-    print("\nH2. Значения начальных моментов времени ожидания заявок в системе:\n")
+    # расчет вероятностей состояний СМО
+    p_ch = get_p(a, mu)
 
-    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
-    print("-" * 45)
-    for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_im[j]))
+    # для верификации используем ИМ.
+    # создаем экземпляр класса ИМ, передаем число каналов обслуживания
+    qs = QueueingSystemSimulator(1)
 
-    print("\nЗначения начальных моментов времени пребывания заявок в системе:\n")
+    # задаем входной поток. Методу нужно передать параметры распределения списком и тип распределения.
+    qs.set_sources([v, alpha], "Gamma")
 
-    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
-    print("-" * 45)
-    for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
+    # задаем каналы обслуживания. На вход параметры (в нашем случае интенсивность обслуживания)
+    # и тип распределения - М (экспоненциальное).
+    qs.set_servers(mu, "M")
 
-    print("{0:^25s}".format("Вероятности состояний СМО"))
-    print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
-    print("-" * 32)
-    for i in range(11):
-        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_im[i]))
+    # запускаем ИМ:
+    qs.run(num_of_jobs)
 
+    # получаем список начальных моментов времени пребывания и ожидания в СМО
+    v_sim = qs.v
+    w_sim = qs.w
 
-    # Тоже самое, но для других распределений времени обслуживания
-    params = rd.Uniform_dist.get_params_by_mean_and_coev(b1, coev)
-    b = rd.Uniform_dist.calc_theory_moments(*params, 4)
-    w_ch = get_w(l, b)
-    p_ch = get_p(l, b, 100, dist_type="Uniform")
-    v_ch = get_v(l, b)
-
-    smo = smo_im.SmoIm(1)
-    smo.set_servers(params, "Uniform")
-    smo.set_sources(l, "M")
-    smo.run(num_of_jobs)
-    w_im = smo.w
-    p_im = smo.get_p()
-    v_im = smo.v
+    # получаем распределение вероятностей состояний СМО
+    p_sim = qs.get_p()
 
-    print("\nUniform. Значения начальных моментов времени ожидания заявок в системе:\n")
+    # Вывод результатов
+    print("\nGamma. Значения начальных моментов времени пребывания заявок в системе:\n")
 
     print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
     print("-" * 45)
     for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_im[j]))
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_sim[j]))
 
-    print("\nЗначения начальных моментов времени пребывания заявок в системе:\n")
+    print("\nЗначения начальных моментов времени ожидания заявок в системе:\n")
 
     print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
     print("-" * 45)
     for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_sim[j]))
 
     print("{0:^25s}".format("Вероятности состояний СМО"))
     print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
     print("-" * 32)
     for i in range(11):
-        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_im[i]))
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_sim[i]))
+
+    # Тоже для распределения Парето
 
-    a, K = rd.Pareto_dist.get_a_k_by_mean_and_coev(b1, coev)
-    b = rd.Pareto_dist.calc_theory_moments(a, K, 4)
-    w_ch = get_w(l, b)
-    p_ch = get_p(l, b, 100, dist_type="Pa")
-    v_ch = get_v(l, b)
-
-    smo = smo_im.SmoIm(1)
-    smo.set_servers([a, K], "Pa")
-    smo.set_sources(l, "M")
-    smo.run(num_of_jobs)
-    w_im = smo.w
-    p_im = smo.get_p()
-    v_im = smo.v
+    alpha, K = rd.Pareto_dist.get_a_k_by_mean_and_coev(a1, a_coev)
+    a = rd.Pareto_dist.calc_theory_moments(alpha, K)
+    v_ch = get_v(a, mu, approx_distr="Pa")
+    w_ch = get_w(a, mu, approx_distr="Pa")
+    p_ch = get_p(a, mu, approx_distr="Pa")
+
+    qs = QueueingSystemSimulator(1)
+    qs.set_sources([alpha, K], "Pa")
+    qs.set_servers(mu, "M")
+    qs.run(num_of_jobs)
+    v_sim = qs.v
+    w_sim = qs.w
+    p_sim = qs.get_p()
 
-    print("\nPareto. Значения начальных моментов времени ожидания заявок в системе:\n")
+    print("\nPareto. Значения начальных моментов времени пребывания заявок в системе:\n")
 
     print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
     print("-" * 45)
-    for j in range(len(w_ch)):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_im[j]))
-
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_sim[j]))
 
-    print("\nЗначения начальных моментов времени пребывания заявок в системе:\n")
+    print("\nЗначения начальных моментов времени ожидания заявок в системе:\n")
 
     print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
     print("-" * 45)
-    for j in range(len(w_ch)):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
+    for j in range(3):
+        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w_ch[j], w_sim[j]))
 
     print("{0:^25s}".format("Вероятности состояний СМО"))
     print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
     print("-" * 32)
     for i in range(11):
-        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_im[i]))
+        print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_ch[i], p_sim[i]))
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `most_queue-1.20/most_queue/tests/mg1_warm_calc.py` & `most_queue-1.21/most_queue/tests/mg1_warm_calc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 from most_queue.theory.mg1_warm_calc import *
-
+from most_queue.sim.qs_sim import QueueingSystemSimulator
+from most_queue.utils.tables import probs_print, times_print
 
 def test():
     l = 1
     b1 = 0.8
     b1_warm = 0.9
     coev = 1.3
     b_params = rd.H2_dist.get_params_by_mean_and_coev(b1, coev)
     b = rd.H2_dist.calc_theory_moments(*b_params, 4)
 
-    b_warm_params = rd.H2_dist.get_params_by_mean_and_coev(b1, coev)
+    b_warm_params = rd.H2_dist.get_params_by_mean_and_coev(b1_warm, coev)
     b_warm = rd.H2_dist.calc_theory_moments(*b_params, 4)
 
-    smo = smo_im.SmoIm(1)
-    smo.set_servers(b_params, "H")
-    smo.set_warm(b_warm_params, "H")
-    smo.set_sources(l, "M")
-    smo.run(100000)
+    qs = QueueingSystemSimulator(1)
+    qs.set_servers(b_params, "H")
+    qs.set_warm(b_warm_params, "H")
+    qs.set_sources(l, "M")
+    qs.run(100000)
 
     v_ch = get_v(l, b, b_warm)
-    v_im = smo.v
-
-    print("\nЗначения начальных моментов времени пребывания заявок в системе:\n")
+    v_sim = qs.v
 
-    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
-    print("-" * 45)
-    for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, v_ch[j], v_im[j]))
+    times_print(v_sim, v_ch, False)
 
 
 if __name__ == "__main__":
     test()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `most_queue-1.20/most_queue/tests/mgn_tt.py` & `most_queue-1.21/most_queue/tests/mgn_tt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
-from most_queue.sim import smo_im
+from most_queue.sim.qs_sim import QueueingSystemSimulator
 from most_queue.sim import rand_destribution as rd
 import time
 from most_queue.theory.mgn_tt import MGnCalc
+from most_queue.utils.tables import probs_print, times_print
 
 
 def test():
     """
     Тестирование метода Такахаси-Таками для расчета СМО М/H2/n
 
     При коэфф вариации времени обслуживания < 1 параметры аппроксимирующего Н2-распределения
@@ -41,52 +42,43 @@
         tt_time = time.process_time() - tt_start
         # также можно узнать сколько итераций потребовалось
         num_of_iter = tt.num_of_iter_
 
         # запуск ИМ для верификации результатов
         im_start = time.process_time()
 
-        smo = smo_im.SmoIm(n)
+        qs = QueueingSystemSimulator(n)
 
         # задаем вх поток заявок. М - экспоненциальный с интенсивностью l
-        smo.set_sources(l, 'M')
+        qs.set_sources(l, 'M')
 
         # задаем параметры каналов обслуживания Гамма-распределением.
         # Параметры распределения подбираем с помощью метода библиотеки random_distribution
         gamma_params = rd.Gamma.get_mu_alpha([b[0], b[1]])
-        smo.set_servers(gamma_params, 'Gamma')
+        qs.set_servers(gamma_params, 'Gamma')
 
         # Запуск ИМ
-        smo.run(num_of_jobs)
+        qs.run(num_of_jobs)
 
         # Получение результатов
-        p = smo.get_p()
-        v_im = smo.v
+        p = qs.get_p()
+        v_sim = qs.v
         im_time = time.process_time() - im_start
 
         # вывод результатов
 
         print("\nСравнение результатов расчета методом Такахаси-Таками и ИМ.\n"
               "ИМ - M/Gamma/{0:^2d}\nТакахаси-Таками - M/H2/{0:^2d}"
               "с комплексными параметрами\n"
               "Коэффициент загрузки: {1:^1.2f}\nКоэффициент вариации времени обслуживания: {2:^1.2f}\n".format(n, ro,
                                                                                                                b_coev[
                                                                                                                    k]))
         print("Количество итераций алгоритма Такахаси-Таками: {0:^4d}".format(num_of_iter))
         print("Время работы алгоритма Такахаси-Таками: {0:^5.3f} c".format(tt_time))
         print("Время работы ИМ: {0:^5.3f} c".format(im_time))
-        print("{0:^25s}".format("Первые 10 вероятностей состояний СМО"))
-        print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
-        print("-" * 32)
-        for i in range(11):
-            print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], p[i]))
-
-        print("\n")
-        print("{0:^25s}".format("Начальные моменты времени пребывания в СМО"))
-        print("{0:^3s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
-        print("-" * 32)
-        for i in range(3):
-            print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i + 1, v_tt[i], v_im[i]))
+        probs_print(p, p_tt, 10)
+
+        times_print(v_sim, v_tt, False)
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `most_queue-1.20/most_queue/tests/mmn3_pnz_cox_approx.py` & `most_queue-1.21/most_queue/tests/mmn3_pnz_cox_approx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from most_queue.sim import smo_im_prty
+from most_queue.sim.priority_queue_sim import PriorityQueueSimulator
 from most_queue.theory import mmn_prty_pnz_approx
-from most_queue.theory.mmnr_calc import M_M_n_formula
+from most_queue.theory.mmnr_calc import MMnr_calc
 from most_queue.theory.mmn3_pnz_cox_approx import Mmn3_pnz_cox
 
 
 def test():
     num_of_jobs = 200000
     n = 2  # количество каналов
     K = 3  # количество классов
@@ -19,44 +19,44 @@
     b1_H = 1 / mu_H
     b1_L = 1 / mu_L
     b1_M = 1 / mu_M
     b_ave = (l_L / l_sum) * b1_L + (l_H / l_sum) * b1_H + (l_M / l_sum) * b1_M
     ro = l_sum * b_ave / n
 
     # задание ИМ:
-    smo = smo_im_prty.SmoImPrty(n, K, "PR")
+    qs = PriorityQueueSimulator(n, K, "PR")
     sources = []
     servers_params = []
     l = [l_H, l_M, l_L]
     mu = [mu_H, mu_M, mu_L]
     for j in range(K):
         sources.append({'type': 'M', 'params': l[j]})
         servers_params.append({'type': 'M', 'params': mu[j]})
 
-    smo.set_sources(sources)
-    smo.set_servers(servers_params)
+    qs.set_sources(sources)
+    qs.set_servers(servers_params)
 
     # запуск ИМ:
-    smo.run(num_of_jobs)
+    qs.run(num_of_jobs)
 
     # получение результатов ИМ:
-    p = smo.get_p()
-    v_im = smo.v
+    p = qs.get_p()
+    v_sim = qs.v
 
     # расчет численным методом:
     tt = Mmn3_pnz_cox(mu_L, mu_M, mu_H, l_L, l_M, l_H)
     tt_for_second = mmn_prty_pnz_approx.MMn_PRTY_PNZ_Cox_approx(2, mu_M, mu_H, l_M, l_H)
     tt_for_second.run()
 
     tt.run()
     p_tt = tt.get_p()
     v_tt = tt.get_low_class_v1()
     v_2 = tt_for_second.get_second_class_v1()
 
-    v_1 = M_M_n_formula.get_v(l_H, mu_H, 2, 100)[0]
+    v_1 = MMnr_calc.get_v(l_H, mu_H, 2, 100)[0]
 
     print("\nСравнение результатов расчета численным методом с аппроксимацией ПНЗ "
           "\nраспределением Кокса второго порядка и ИМ.")
     print("Коэффициент загрузки: {0:^1.2f}".format(ro))
     print("Количество обслуженных заявок для ИМ: {0:d}\n".format(num_of_jobs))
 
     print("{0:^25s}".format("Вероятности состояний для заявок 3-го класса"))
@@ -66,14 +66,14 @@
         print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], p[2][i]))
 
     print("\n")
     print("{0:^35s}".format("Средние времена пребывания в СМО"))
     print("-" * 38)
     print("{0:^10s}|{1:^15s}|{2:^15s}".format("N класса", "Числ", "ИМ"))
     print("-" * 38)
-    print("{0:^10d}|{1:^15.3g}|{2:^15.3g}".format(0, v_1, v_im[0][0]))
-    print("{0:^10d}|{1:^15.3g}|{2:^15.3g}".format(1, v_2, v_im[1][0]))
-    print("{0:^10d}|{1:^15.3g}|{2:^15.3g}".format(2, v_tt, v_im[2][0]))
+    print("{0:^10d}|{1:^15.3g}|{2:^15.3g}".format(0, v_1, v_sim[0][0]))
+    print("{0:^10d}|{1:^15.3g}|{2:^15.3g}".format(1, v_2, v_sim[1][0]))
+    print("{0:^10d}|{1:^15.3g}|{2:^15.3g}".format(2, v_tt, v_sim[2][0]))
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `most_queue-1.20/most_queue/tests/mmn_prty_pnz_approx.py` & `most_queue-1.21/most_queue/tests/mmn_prty_pnz_approx.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from most_queue.theory.mmn_prty_pnz_approx import MMn_PRTY_PNZ_Cox_approx
-from most_queue.sim import smo_im_prty
+from most_queue.sim.priority_queue_sim import PriorityQueueSimulator
 
 
 def test():
     num_of_jobs = 100000
     n = 3  # количество каналов
     K = 2  # количество классов
     mu_L = 1.3  # интенсивность обслуживания заявок 2-го класса
@@ -13,32 +13,32 @@
     ro = 0.8
     b1_H = 1 / mu_H
     b1_L = (ro * n - l_H * b1_H) / l_L
     l_sum = l_H + l_L
     # b_ave = (l_L / l_sum) * b1_L + (l_H / l_sum) * b1_H
 
     # задание ИМ:
-    smo = smo_im_prty.SmoImPrty(n, K, "PR")
+    qs = PriorityQueueSimulator(n, K, "PR")
     sources = []
     servers_params = []
     l = [l_H, l_L]
     mu = [mu_H, mu_L]
     for j in range(K):
         sources.append({'type': 'M', 'params': l[j]})
         servers_params.append({'type': 'M', 'params': mu[j]})
 
-    smo.set_sources(sources)
-    smo.set_servers(servers_params)
+    qs.set_sources(sources)
+    qs.set_servers(servers_params)
 
     # запуск ИМ:
-    smo.run(num_of_jobs)
+    qs.run(num_of_jobs)
 
     # получение результатов ИМ:
-    p = smo.get_p()
-    v_im = smo.v
+    p = qs.get_p()
+    v_sim = qs.v
 
     # расчет численным методом:
     tt = MMn_PRTY_PNZ_Cox_approx(n, mu_L, mu_H, l_L, l_H)
     tt.run()
     p_tt = tt.get_p()
     v_tt = tt.get_second_class_v1()
     # v = tt.calculate_v()
@@ -54,15 +54,15 @@
     for i in range(11):
         print("{0:^4d}|{1:^15.3g}|{2:^15.3g}".format(i, p_tt[i], p[1][i]))
 
     print("\n")
     print("{0:^25s}".format("Среднее время пребывания в СМО заявок 2-го класса"))
     print("{0:^15s}|{1:^15s}".format("Числ", "ИМ"))
     print("-" * 32)
-    print("{0:^15.3g}|{1:^15.3g}".format(v_tt, v_im[1][0]))
-    # print("{0:^15.3g}|{1:^15.3g}".format(v[0].real, v_im[1][0]))
-    # print("{0:^15.3g}|{1:^15.3g}".format(v[1].real, v_im[1][1]))
-    # print("{0:^15.3g}|{1:^15.3g}".format(v[2].real, v_im[1][2]))
+    print("{0:^15.3g}|{1:^15.3g}".format(v_tt, v_sim[1][0]))
+    # print("{0:^15.3g}|{1:^15.3g}".format(v[0].real, v_sim[1][0]))
+    # print("{0:^15.3g}|{1:^15.3g}".format(v[1].real, v_sim[1][1]))
+    # print("{0:^15.3g}|{1:^15.3g}".format(v[2].real, v_sim[1][2]))
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `most_queue-1.20/most_queue/tests/network_im_prty.py` & `most_queue-1.21/most_queue/tests/network_im_prty.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import most_queue.sim.rand_destribution as rd
 import numpy as np
 from most_queue.theory import network_calc
-from most_queue.sim.network_im_prty import NetworkPrty
+from most_queue.sim.priority_network import PriorityNetwork
 
+from most_queue.utils.tables import probs_print, times_print_with_classes
 
 def test():
     """
     Тестирование ИМ СеМО с приоритетами в узлах
     Сравнение с численным расчетом методом декомпозиции
     """
     k_num = 3  # число классов
@@ -69,21 +70,21 @@
         for m in range(n_num):
             b[k].append(rd.H2_dist.calc_theory_moments(*h2_params[m], 4))
 
     prty = ['NP'] * n_num  # список, содержащий тип приоритета для каждого узла сети.
     # "NP" - относительный приоритет. Также доступны абсолютные ("PR", "RW", "RS") и без приоритета "No"
 
     # Создаем экземпляр модели СеМО
-    semo_im = NetworkPrty(k_num, L, R, n, prty, serv_params, nodes_prty)
+    qn = PriorityNetwork(k_num, L, R, n, prty, serv_params, nodes_prty)
 
     #  Запуск ИМ:
-    semo_im.run(jobs_num)
+    qn.run(jobs_num)
 
     #  Получение нач. моментов пребывания в СеМО
-    v_im = semo_im.v_semo
+    v_im = qn.v_semo
 
     #  Получение нач. моментов пребывания в СеМО с помощью метода инвариантов отношения
     semo_calc = network_calc.network_prty_calc(R, b, n, L, prty, nodes_prty)
     v_ch = semo_calc['v']
 
     #  получения коэфф загрузки каждого узла
     loads = semo_calc['loads']
@@ -100,82 +101,27 @@
     print("\nКоэффициенты загрузки узлов :")
     for load in loads:
         print("{0:^1.3f}".format(load), end=" ")
     print("\n")
     print("-" * 60)
     print("{0:^60s}".format("Относительный приоритет"))
 
-    print("-" * 60)
-    print("{0:^11s}|{1:^47s}|".format('', 'Номер начального момента'))
-    print("{0:^10s}| ".format('№ кл'), end="")
-    print("-" * 45 + " |")
-
-    print(" " * 11 + "|", end="")
-    for j in range(3):
-        s = str(j + 1)
-        print("{:^15s}|".format(s), end="")
-    print("")
-    print("-" * 60)
-
-    for i in range(k_num):
-        print(" " * 5 + "|", end="")
-        print("{:^5s}|".format("ИМ"), end="")
-        for j in range(3):
-            print("{:^15.3g}|".format(v_im[i][j]), end="")
-        print("")
-        print("{:^5s}".format(str(i + 1)) + "|" + "-" * 54)
-
-        print(" " * 5 + "|", end="")
-        print("{:^5s}|".format("Р"), end="")
-        for j in range(3):
-            print("{:^15.3g}|".format(v_ch[i][j]), end="")
-        print("")
-        print("-" * 60)
-
-    print("\n")
-
+    times_print_with_classes(v_im, v_ch, False)
     #  Теперь для абсолютного приоритета:
     prty = ['PR'] * n_num
-    semo_im = NetworkPrty(k_num, L, R, n, prty, serv_params, nodes_prty)
+    qn = PriorityNetwork(k_num, L, R, n, prty, serv_params, nodes_prty)
 
-    semo_im.run(jobs_num)
+    qn.run(jobs_num)
 
-    v_im = semo_im.v_semo
+    v_im = qn.v_semo
 
     semo_calc = network_calc.network_prty_calc(R, b, n, L, prty, nodes_prty)
     v_ch = semo_calc['v']
 
     print("-" * 60)
     print("{0:^60s}".format("Абсолютный приоритет"))
 
-    print("-" * 60)
-    print("{0:^11s}|{1:^47s}|".format('', 'Номер начального момента'))
-    print("{0:^10s}| ".format('№ кл'), end="")
-    print("-" * 45 + " |")
-
-    print(" " * 11 + "|", end="")
-    for j in range(3):
-        s = str(j + 1)
-        print("{:^15s}|".format(s), end="")
-    print("")
-    print("-" * 60)
-
-    for i in range(k_num):
-        print(" " * 5 + "|", end="")
-        print("{:^5s}|".format("ИМ"), end="")
-        for j in range(3):
-            print("{:^15.3g}|".format(v_im[i][j]), end="")
-        print("")
-        print("{:^5s}".format(str(i + 1)) + "|" + "-" * 54)
-
-        print(" " * 5 + "|", end="")
-        print("{:^5s}|".format("Р"), end="")
-        for j in range(3):
-            print("{:^15.3g}|".format(v_ch[i][j]), end="")
-        print("")
-        print("-" * 60)
-
-    print("\n")
+    times_print_with_classes(v_im, v_ch, False)
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `most_queue-1.20/most_queue/tests/smo_im.py` & `most_queue-1.21/most_queue/theory/q_poisson_arrival_calc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,60 @@
-from most_queue.sim.smo_im import SmoIm
-from most_queue.theory import mmnr_calc
-from most_queue.theory import m_d_n_calc
+import math
+from most_queue.sim import rand_destribution as rd
+import scipy.spatial as sc
 
 
-def test():
+def get_q_Gamma(l, mu, alpha, num=100):
     """
-    Тестирование имитационной модели СМО
-    Для верификации - сравнение с результатами расчета СМО M/M/3, M/D/3
+    Гамма-распределение
+    l - интенсивность входного потока
+    mu и alpha параметры Гамма-распределения
+    num - число возвращаемых q[j]
     """
-    n = 3  # число каналов
-    l = 1.0  # интенсивность вх потока
-    r = 30  # длина очереди
-    ro = 0.8  # коэфф загрузки
-    mu = l / (ro * n)  # интенсивность обслуживания
+    q = [0.0] * num
+    q[0] = math.pow(mu / (mu + l), alpha)
+    for j in range(1, num):
+        q[j] = q[j - 1] * l * (alpha + j - 1) / ((l + mu) * j)
 
-    # создвем экземпляр класса ИМ
-    smo = SmoIm(n, buffer=r)
+    return q
 
-    # задаем вх поток - параметры и тип распределения.
-    smo.set_sources(l, 'M')
-    # задаем распределение обслуживания - параметры и тип распределения.
-    smo.set_servers(mu, 'M')
 
-    # запуск ИМ - передаем кол-во заявок для обслуживания
-    smo.run(1000000)
-    # получаем начальные моменты времени ожидания. Также можно получить время пребывания .v,
-    # вероятности состояний .get_p(), периоды непрерывной занятости .pppz
-    w_im = smo.w
-
-    # для сравнения расчитаем теже начальные моменты численно
-    w = mmnr_calc.M_M_n_formula.get_w(l, mu, n, r)
-
-    # вывод результатов
-
-    print("\nЗначения начальных моментов времени ожидания заявок в системе:\n")
-
-    print("{0:^15s}|{1:^15s}|{2:^15s}".format("№ момента", "Числ", "ИМ"))
-    print("-" * 45)
-    for j in range(3):
-        print("{0:^16d}|{1:^15.5g}|{2:^15.5g}".format(j + 1, w[j], w_im[j]))
-    print("\n\nДанные ИМ::\n")
-    print(smo)
-
-    # тоже для детерминированного обслуживания
-
-    smo = SmoIm(n)
-
-    smo.set_sources(l, 'M')
-    smo.set_servers(1.0 / mu, 'D')
-
-    smo.run(1000000)
+def get_q_uniform(l, mean, half_interval, num=100):
+    """
+    Равномерное распределение на отрезке [mean-half_interval, mean+half_interval
+    l - интенсивность входного потока
+    mean - среднее
+    half_interval - полуинтервал влево и вправо от среднего значения
+    num - число возвращаемых q[j]
+    """
+    q = [0.0] * num
+    for j in range(num):
+        summ1 = 0
+        for i in range(j + 1):
+            summ1 += l * pow(mean - half_interval, i) * math.exp(-l * (mean - half_interval)) / math.factorial(i)
+        summ2 = 0
+        for i in range(j + 1):
+            summ2 += l * pow(mean + half_interval, i) * math.exp(-l * (mean + half_interval)) / math.factorial(i)
+        q[j] = (1.0 / (2 * l * half_interval)) * (summ1 - summ2)
 
-    mdn = m_d_n_calc.M_D_n(l, 1 / mu, n)
-    p_ch = mdn.calc_p()
-    p_im = smo.get_p()
+    return q
 
-    print("-" * 36)
-    print("{0:^36s}".format("Вероятности состояний СМО M/D/{0:d}".format(n)))
-    print("-" * 36)
-    print("{0:^4s}|{1:^15s}|{2:^15s}".format("№", "Числ", "ИМ"))
-    print("-" * 36)
-    for i in range(11):
-        print("{0:^4d}|{1:^15.5g}|{2:^15.5g}".format(i, p_ch[i], p_im[i]))
-    print("-" * 36)
 
+def get_q_Pareto(l, alpha, K, num=100):
+    """
+    Распределение Парето
+    l - интенсивность входного потока
+    K, alpha - параметры распределения Парето
+    num - число возвращаемых q[j]
+    """
+    q = [0.0] * num
+    gammas = [0.0] * num
+    z = l * K
+    gammas[0] = rd.Gamma.get_minus_gamma(alpha) - rd.Gamma.get_gamma_small(-alpha, z)
+
+    for j in range(1, num):
+        gammas[j] = (j - alpha - 1) * gammas[j - 1] + pow(z, j - alpha - 1) * math.exp(-z)
+    forw = alpha * pow(z, alpha)
+    for j in range(num):
+        q[j] = forw * gammas[j] / math.factorial(j)
 
-if __name__ == "__main__":
-    test()
+    return q
```

### Comparing `most_queue-1.20/most_queue/tests/weibull.py` & `most_queue-1.21/most_queue/tests/weibull.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/batch_mm1.py` & `most_queue-1.21/most_queue/theory/batch_mm1.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/diff5dots.py` & `most_queue-1.21/most_queue/theory/diff5dots.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/ek_d_n_calc.py` & `most_queue-1.21/most_queue/theory/ek_d_n_calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,33 +144,33 @@
                     is_close = True
                 z_old = z_new
             z[m] = z_old
         self.z_ = z
 
 
 if __name__ == "__main__":
-    from most_queue.sim import smo_im
+    from most_queue.sim.qs_sim import QueueingSystemSimulator
     from most_queue.sim import rand_destribution as rd
     from most_queue.utils.tables import probs_print
 
     ro = 0.8  # коэффициент загрузки
     a1 = 1  # среднее время между заявками вх потока
     n = 4  # число каналов
     coev_a = 0.56  # коэффициент вариации вх потока
     num_of_jobs = 800000  # количество заявок для ИМ
 
     k, l = rd.Erlang_dist.get_params_by_mean_and_coev(a1, coev_a)
     b = a1 * n * ro
     ekdn = Ek_D_n(l, k, b, n)
     p_ch = ekdn.calc_p()
 
-    smo = smo_im.SmoIm(n)
-    smo.set_sources([k, l], "E")
-    smo.set_servers(b, "D")
-    smo.run(num_of_jobs)
-    v_im = smo.v
-    p_im = smo.get_p()
+    qs = QueueingSystemSimulator(n)
+    qs.set_sources([k, l], "E")
+    qs.set_servers(b, "D")
+    qs.run(num_of_jobs)
+    v_im = qs.v
+    p_im = qs.get_p()
 
     print("-" * 36)
     print("{0:^36s}".format("СМО E{0:d}/D/{1:d}".format(k, n)))
 
     probs_print(p_im, p_ch, 10)
```

### Comparing `most_queue-1.20/most_queue/theory/engset_model.py` & `most_queue-1.21/most_queue/theory/engset_model.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/fj_calc.py` & `most_queue-1.21/most_queue/theory/fj_calc.py`

 * *Files 7% similar despite different names*

```diff
@@ -403,21 +403,21 @@
             b[0] = 1
             alpha = 1 / (coevs[j] ** 2)
             b[1] = math.pow(b[0], 2) * (math.pow(coevs[j], 2) + 1)
             b[2] = b[1] * b[0] * (1.0 + 2 / alpha)
             l = get_1ambda_max(b, ns[nn])
 
             t_im_start = time.process_time()
-            smo = SmoFJ(ns[nn], ns[nn], False)
+            qs = ForkJoinSim(ns[nn], ns[nn], False)
             params = rd.Gamma.get_mu_alpha(b)
-            smo.set_sources(l, 'M')
-            smo.set_servers(params, 'Gamma')
-            smo.run(num_of_jobs)
-            v = smo.v
-            v1_im[nn].append(smo.v[moment])
+            qs.set_sources(l, 'M')
+            qs.set_servers(params, 'Gamma')
+            qs.run(num_of_jobs)
+            v = qs.v
+            v1_im[nn].append(qs.v[moment])
             im_times[nn].append(time.process_time() - t_im_start)
 
             t_fj_start = time.process_time()
             v_fj = get_v_fj_invar_tt(l, b, ns[nn])[moment]
             fj_times[nn][j] = time.process_time() - t_fj_start
             fj_errors[nn][j] = calc_error_percentage(v1_im[nn][j], v_fj)
 
@@ -501,21 +501,21 @@
             b[0] = 1
             alpha = 1 / (coevs[j] ** 2)
             b[1] = math.pow(b[0], 2) * (math.pow(coevs[j], 2) + 1)
             b[2] = b[1] * b[0] * (1.0 + 2 / alpha)
             l = get_1ambda_max(b, ns[nn])
 
             t_im_start = time.process_time()
-            smo = SmoFJ(ns[nn], ns[nn], False)
+            qs = ForkJoinSim(ns[nn], ns[nn], False)
             params = rd.Gamma.get_mu_alpha(b)
-            smo.set_sources(l, 'M')
-            smo.set_servers(params, 'Gamma')
-            smo.run(num_of_jobs)
-            v = smo.v
-            v1_im[nn].append(smo.v[moment])
+            qs.set_sources(l, 'M')
+            qs.set_servers(params, 'Gamma')
+            qs.run(num_of_jobs)
+            v = qs.v
+            v1_im[nn].append(qs.v[moment])
             im_times[nn].append(time.process_time() - t_im_start)
 
             t_fj_start = time.process_time()
             v_fj = get_v_fj_invar_tt(l, b, ns[nn])[moment]
             fj_times[nn][j] = time.process_time() - t_fj_start
             fj_errors[nn][j] = calc_error_percentage(v1_im[nn][j], v_fj)
 
@@ -572,15 +572,15 @@
             file.write(data_str)
 
         file.close()
 
 
 if __name__ == "__main__":
     import numpy as np
-    from most_queue.sim.fj_im import SmoFJ
+    from most_queue.sim.fj_sim import ForkJoinSim
 
     n = [x for x in range(2, 15)]
     mu = 1.0
     b = [1 / mu, 2 / pow(mu, 2), 6 / pow(mu, 3)]
 
     ro = 0.8
 
@@ -594,20 +594,20 @@
 
     str_f = "{0:^15s}|{1:^15s}|{2:^15s}|{3:^15s}|{4:^15s}"
     str_f_v = "{0:^15.3f}|{1:^15.3f}|{2:^15.3f}|{3:^15.3f}|{4:^15.3f}"
 
     print(str_f.format("ИМ", "Инвар", "Varki", "Varma", "Nelson"))
     i = 0
     for nn in n:
-        smo = SmoFJ(nn, nn, False)
+        qs = ForkJoinSim(nn, nn, False)
 
-        smo.set_sources(l, 'M')
-        smo.set_servers(mu, 'M')
-        smo.run(num_of_jobs)
-        v = smo.v
+        qs.set_sources(l, 'M')
+        qs.set_servers(mu, 'M')
+        qs.run(num_of_jobs)
+        v = qs.v
         v1_inv = get_v1_fj_invar(l, mu, nn, 100)
         v_im.append(v[0])
         v_inv.append(v1_inv)
         v_varki.append(get_v1_fj_varki_merchant(l, mu, nn))
         v_varma.append(get_v1_fj_varma(l, mu, nn))
         v_nelson.append(get_v1_fj_nelson_tantawi(l, mu, nn))
         print(str_f_v.format(v_im[i], v_inv[i], v_varki[i], v_varma[i], v_nelson[i]))
```

### Comparing `most_queue-1.20/most_queue/theory/flow_sum.py` & `most_queue-1.21/most_queue/theory/flow_sum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from most_queue.sim import flow_sum_im
+from most_queue.sim import flow_sum_sim
 
 import copy
 import matplotlib.pyplot as plt
 import most_queue.sim.rand_destribution as rd
 import math
 
 class SummatorNumeric:
@@ -237,15 +237,15 @@
     a = []
     for i in range(n_nums):
         params1 = rd.Gamma.get_mu_alpha_by_mean_and_coev(mean, coev)
         a1 = rd.Gamma.calc_theory_moments(*params1, 4)
         a.append(a1)
 
     s = SummatorNumeric(a, is_semi=is_semi)
-    s_im = flow_sum_im.SummatorIM(a, distr=distr_im, num_of_jobs=num_of_jobs)
+    s_im = flow_sum_sim.FlowSumSim(a, distr=distr_im, num_of_jobs=num_of_jobs)
 
     s.sum_flows()
     s_im.sum_flows()
 
     coevs_im = s_im.coevs
     coevs_num = s.coevs
     errors1 = []
```

### Comparing `most_queue-1.20/most_queue/theory/generate_pareto_noise.py` & `most_queue-1.21/most_queue/theory/generate_pareto_noise.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/gi_m_1_calc.py` & `most_queue-1.21/most_queue/theory/gi_m_1_calc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 from most_queue.sim import rand_destribution as rd
 import q_poisson_arrival_calc
-import sv_sum_calc
+from most_queue.theory import convolution_sum_calc
 
 
 def get_pi(a, mu, num=100, e=1e-10, approx_distr="Gamma"):
     """
     Вычисление вероятностей состояний СМО
     a - список начальных моментов распределения интервало рекуррентного вх потока заявок
     mu - интенсивность обслуживания
@@ -85,63 +85,63 @@
         print("w_param calc. Unknown type of distr_type")
 
     return 0
 
 
 if __name__ == '__main__':
 
-    from most_queue.sim import smo_im
+    from most_queue.sim import qs_sim
     from most_queue.utils.tables import times_print, probs_print
 
     l = 1
     a1 = 1 / l
     b1 = 0.9
     mu = 1 / b1
     a_coev = 1.6
     num_of_jobs = 800000
 
     v, alpha = rd.Gamma.get_mu_alpha_by_mean_and_coev(a1, a_coev)
     a = rd.Gamma.calc_theory_moments(v, alpha)
     v_ch = get_v(a, mu)
     p_ch = get_p(a, mu)
 
-    smo = smo_im.SmoIm(1)
-    smo.set_sources([v, alpha], "Gamma")
-    smo.set_servers(mu, "M")
-    smo.run(num_of_jobs)
-    v_im = smo.v
-    p_im = smo.get_p()
+    qs = qs_sim.QueueingSystemSimulator(1)
+    qs.set_sources([v, alpha], "Gamma")
+    qs.set_servers(mu, "M")
+    qs.run(num_of_jobs)
+    v_im = qs.v
+    p_im = qs.get_p()
 
     print("\nGamma\n")
 
     times_print(v_im, v_ch, is_w=False)
 
     w_ch = get_w(a, mu)
-    w_im = smo.w
+    w_im = qs.w
 
     times_print(w_im, w_ch, is_w=True)
 
     probs_print(p_im, p_ch, 10)
 
     # Pareto test
     alpha, K = rd.Pareto_dist.get_a_k_by_mean_and_coev(a1, a_coev)
     a = rd.Pareto_dist.calc_theory_moments(alpha, K)
     v_ch = get_v(a, mu, approx_distr="Pa")
     p_ch = get_p(a, mu, approx_distr="Pa")
 
-    smo = smo_im.SmoIm(1)
-    smo.set_sources([alpha, K], "Pa")
-    smo.set_servers(mu, "M")
-    smo.run(num_of_jobs)
-    v_im = smo.v
-    p_im = smo.get_p()
+    qs = qs_sim.QueueingSystemSimulator(1)
+    qs.set_sources([alpha, K], "Pa")
+    qs.set_servers(mu, "M")
+    qs.run(num_of_jobs)
+    v_im = qs.v
+    p_im = qs.get_p()
 
     print("\nPareto\n")
 
     times_print(v_im, v_ch, is_w=False)
 
     w_ch = get_w(a, mu, approx_distr="Pa")
-    w_im = smo.w
+    w_im = qs.w
 
     times_print(w_im, w_ch, is_w=True)
 
     probs_print(p_im, p_ch, 10)
```

### Comparing `most_queue-1.20/most_queue/theory/gi_m_n_calc.py` & `most_queue-1.21/most_queue/theory/gi_m_n_calc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from most_queue.sim import rand_destribution as rd
+
 import numpy as np
 import math
-from most_queue.sim import rand_destribution as rd
+
 import q_poisson_arrival_calc
 import sv_sum_calc
 import diff5dots
 
 
 def get_pi(a, mu, n, num=100, e=1e-10, approx_distr="Gamma"):
     """
@@ -142,16 +144,15 @@
     else:
         print("w_param calc. Unknown type of distr_type")
 
     return 0
 
 
 if __name__ == '__main__':
-
-    from most_queue.sim import smo_im
+    from most_queue.sim.qs_sim import QueueingSystemSimulator
     from most_queue.utils.tables import times_print, probs_print
 
     l = 1.0
     a1 = 1.0 / l
     n = 4
     ro = 0.8
     b1 = ro * n / l
@@ -161,48 +162,48 @@
     num_of_jobs = 800000
 
     v, alpha = rd.Gamma.get_mu_alpha_by_mean_and_coev(a1, a_coev)
     a = rd.Gamma.calc_theory_moments(v, alpha)
     v_ch = get_v(a, mu, n)
     p_ch = get_p(a, mu, n)
 
-    smo = smo_im.SmoIm(n)
-    smo.set_sources([v, alpha], "Gamma")
-    smo.set_servers(mu, "M")
-    smo.run(num_of_jobs)
-    v_im = smo.v
-    p_im = smo.get_p()
+    qs = QueueingSystemSimulator(n)
+    qs.set_sources([v, alpha], "Gamma")
+    qs.set_servers(mu, "M")
+    qs.run(num_of_jobs)
+    v_im = qs.v
+    p_im = qs.get_p()
 
     print("Gamma\n")
 
     times_print(v_im, v_ch, is_w=False)
 
     w_ch = get_w(a, mu, n)
-    w_im = smo.w
+    w_im = qs.w
 
     times_print(w_im, w_ch, is_w=True)
 
     probs_print(p_im, p_ch, 10)
 
     # Pareto test
     alpha, K = rd.Pareto_dist.get_a_k_by_mean_and_coev(a1, a_coev)
     a = rd.Pareto_dist.calc_theory_moments(alpha, K)
     v_ch = get_v(a, mu, n, approx_distr="Pa")
     p_ch = get_p(a, mu, n, approx_distr="Pa")
 
-    smo = smo_im.SmoIm(n)
-    smo.set_sources([alpha, K], "Pa")
-    smo.set_servers(mu, "M")
-    smo.run(num_of_jobs)
-    v_im = smo.v
-    p_im = smo.get_p()
+    qs = QueueingSystemSimulator(n)
+    qs.set_sources([alpha, K], "Pa")
+    qs.set_servers(mu, "M")
+    qs.run(num_of_jobs)
+    v_im = qs.v
+    p_im = qs.get_p()
 
     print("Pareto\n")
 
     times_print(v_im, v_ch, is_w=False)
 
     w_ch = get_w(a, mu, n, approx_distr="Pa")
-    w_im = smo.w
+    w_im = qs.w
 
     times_print(w_im, w_ch, is_w=True)
 
     probs_print(p_im, p_ch, 10)
```

### Comparing `most_queue-1.20/most_queue/theory/impatience_calc.py` & `most_queue-1.21/most_queue/theory/impatience_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/m_d_n_calc.py` & `most_queue-1.21/most_queue/theory/m_d_n_calc.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,27 +107,27 @@
                 z_old = z_new
             z[m] = z_old
         self.z_ = z
 
 
 if __name__ == "__main__":
 
-    from most_queue.sim import smo_im
+    from most_queue.sim.qs_sim import QueueingSystemSimulator
     from most_queue.utils.tables import probs_print
 
     l = 1.0  # интенсивность входного потока
     ro = 0.8  # коэффициент загрузки
     n = 2  # количество каналов обслуживания
     num_of_jobs = 800000  # количество заявок для ИМ
 
     b = ro * n / l
     mdn = M_D_n(l, b, n)
     p_ch = mdn.calc_p()
 
-    smo = smo_im.SmoIm(n)
-    smo.set_sources(l, "M")
-    smo.set_servers(b, "D")
-    smo.run(num_of_jobs)
-    v_im = smo.v
-    p_im = smo.get_p()
+    qs = QueueingSystemSimulator(n)
+    qs.set_sources(l, "M")
+    qs.set_servers(b, "D")
+    qs.run(num_of_jobs)
+    v_im = qs.v
+    p_im = qs.get_p()
 
     probs_print(p_im, p_ch, 10)
```

### Comparing `most_queue-1.20/most_queue/theory/m_h2_h2warm.py` & `most_queue-1.21/most_queue/theory/m_h2_h2warm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-import numpy as np
-import math
 from tqdm import tqdm
-from most_queue.sim import rand_destribution as rd
 from scipy import special
+from scipy.misc import derivative
+
 from most_queue.utils.binom_probs import calc_binom_probs
+from most_queue.sim import rand_destribution as rd
 from diff5dots import diff5dots
-from scipy.misc import derivative
+
+import numpy as np
+import math
 
 
 class Mh2h2Warm:
     """
     Расчет СМО M/H2/n с H2-разогревом численным методом Такахаси-Таками.
     Используются комплексные параметры, которые позволяют аппроксимировать распределение времени обслуживания
     с произвольными коэффициентами вариации (>1, <=1)
@@ -672,15 +674,15 @@
             output[i, i] = sumA + sumB + sumC
 
         return output
 
 
 if __name__ == "__main__":
 
-    import smo_im
+    from most_queue.sim.qs_sim import QueueingSystemSimulator
     from most_queue.sim import rand_destribution as rd
     import time
     from most_queue.utils.tables import times_print, probs_print
 
     n = 3
     # число каналов
     l = 1.0  # интенсивность вх потока
@@ -705,24 +707,24 @@
         alpha = 1 / (b_coev_warm[k] ** 2)
         b_w[1] = math.pow(b_w[0], 2) * (math.pow(b_coev_warm[k], 2) + 1)
         b_w[2] = b_w[1] * b_w[0] * (1.0 + 2 / alpha)
 
         h2_params = rd.H2_dist.get_params_clx(b)
 
         im_start = time.process_time()
-        smo = smo_im.SmoIm(n, buffer=buff)
-        smo.set_sources(l, 'M')
+        qs = QueueingSystemSimulator(n, buffer=buff)
+        qs.set_sources(l, 'M')
 
         gamma_params = rd.Gamma.get_mu_alpha(b)
         gamma_params_warm = rd.Gamma.get_mu_alpha(b_w)
-        smo.set_servers(gamma_params, 'Gamma')
-        smo.set_warm(gamma_params_warm, 'Gamma')
-        smo.run(num_of_jobs)
-        p = smo.get_p()
-        v_im = smo.v  # .w -> wait times
+        qs.set_servers(gamma_params, 'Gamma')
+        qs.set_warm(gamma_params_warm, 'Gamma')
+        qs.run(num_of_jobs)
+        p = qs.get_p()
+        v_im = qs.v  # .w -> wait times
         im_time = time.process_time() - im_start
 
         tt_start = time.process_time()
         tt = Mh2h2Warm(l, b, b_w, n, buffer=buff, verbose=verbose)
 
         tt.run()
         p_tt = tt.get_p()
```

### Comparing `most_queue-1.20/most_queue/theory/m_ph_n_prty.py` & `most_queue-1.21/most_queue/theory/m_ph_n_prty.py`

 * *Files 0% similar despite different names*

```diff
@@ -644,15 +644,15 @@
 
             output[i, i] = sumA + sumB + sumC
 
         return output
 
 
 if __name__ == "__main__":
-    from most_queue.sim import smo_im_prty
+    from most_queue.sim.priority_queue_sim import PriorityQueueSimulator
     from most_queue.sim import rand_destribution as rd
     import prty_calc
     import time
 
     num_of_jobs = 800000  # число обсл заявок ИМ
 
     is_cox = False  # использовать для аппроксимации ПНЗ распределение Кокса или Н2-распределение
@@ -734,33 +734,33 @@
         invar_times.append(time.process_time() - invar_start)
 
         im_start = time.process_time()
 
         for i in range(iteration):
             print("Start IM iteration: {0:d}".format(i + 1))
 
-            smo = smo_im_prty.SmoImPrty(n, K, "PR")
+            qs = PriorityQueueSimulator(n, K, "PR")
             sources = []
             servers_params = []
             l = [l_H, l_L]
 
             sources.append({'type': 'M', 'params': l_H})
             sources.append({'type': 'M', 'params': l_L})
             servers_params.append({'type': 'Gamma', 'params': gamma_params})
             servers_params.append({'type': 'M', 'params': mu_L})
 
-            smo.set_sources(sources)
-            smo.set_servers(servers_params)
+            qs.set_sources(sources)
+            qs.set_servers(servers_params)
 
             # запуск ИМ:
-            smo.run(num_of_jobs)
+            qs.run(num_of_jobs)
 
             # получение результатов ИМ:
-            p = smo.get_p()
-            v_im = smo.v
+            p = qs.get_p()
+            v_im = qs.v
             v1_sum += v_im[0][0]
             v2_sum += v_im[1][0]
 
         v1 = v1_sum / iteration
         v2 = v2_sum / iteration
         # расчет численным методом:
         v2_im_mass.append(v2)
```

### Comparing `most_queue-1.20/most_queue/theory/mg1_calc.py` & `most_queue-1.21/most_queue/theory/mg1_calc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 from most_queue.sim import rand_destribution as rd
-from most_queue.sim import smo_im
+from most_queue.sim.qs_sim import QueueingSystemSimulator
 import q_poisson_arrival_calc as q_calc
 
 
 def get_w(l, b, num=3):
     """
     Расчет начальных моментов времени ожидания для СМО M/G/1
     :param l: интенсивность поступления заявок в СМО
@@ -85,65 +85,65 @@
     num_of_jobs = 800000
 
     params = rd.H2_dist.get_params_by_mean_and_coev(b1, coev)
     b = rd.H2_dist.calc_theory_moments(*params, 4)
     w_ch = get_w(l, b)
     p_ch = get_p(l, b, 100)
 
-    smo = smo_im.SmoIm(1)
-    smo.set_servers(params, "H")
-    smo.set_sources(l, "M")
-    smo.run(num_of_jobs)
-    w_im = smo.w
-    p_im = smo.get_p()
+    qs = QueueingSystemSimulator(1)
+    qs.set_servers(params, "H")
+    qs.set_sources(l, "M")
+    qs.run(num_of_jobs)
+    w_im = qs.w
+    p_im = qs.get_p()
 
     times_print(w_im, w_ch, True)
 
     v_ch = get_v(l, b)
-    v_im = smo.v
+    v_im = qs.v
 
     times_print(v_im, v_ch, False)
 
     probs_print(p_im, p_ch, 10)
 
     params = rd.Uniform_dist.get_params_by_mean_and_coev(b1, coev)
     b = rd.Uniform_dist.calc_theory_moments(*params, 4)
     w_ch = get_w(l, b)
     p_ch = get_p(l, b, 100, dist_type="Uniform")
 
-    smo = smo_im.SmoIm(1)
-    smo.set_servers(params, "Uniform")
-    smo.set_sources(l, "M")
-    smo.run(num_of_jobs)
-    w_im = smo.w
-    p_im = smo.get_p()
+    qs = QueueingSystemSimulator(1)
+    qs.set_servers(params, "Uniform")
+    qs.set_sources(l, "M")
+    qs.run(num_of_jobs)
+    w_im = qs.w
+    p_im = qs.get_p()
 
     times_print(w_im, w_ch, True)
 
     v_ch = get_v(l, b)
-    v_im = smo.v
+    v_im = qs.v
 
     times_print(v_im, v_ch, False)
 
     probs_print(p_im, p_ch, 10)
 
     a, K = rd.Pareto_dist.get_a_k_by_mean_and_coev(b1, coev)
     b = rd.Pareto_dist.calc_theory_moments(a, K, 4)
     w_ch = get_w(l, b)
     p_ch = get_p(l, b, 100, dist_type="Pa")
 
-    smo = smo_im.SmoIm(1)
-    smo.set_servers([a, K], "Pa")
-    smo.set_sources(l, "M")
-    smo.run(num_of_jobs)
-    w_im = smo.w
-    p_im = smo.get_p()
+    qs = QueueingSystemSimulator(1)
+    qs.set_servers([a, K], "Pa")
+    qs.set_sources(l, "M")
+    qs.run(num_of_jobs)
+    w_im = qs.w
+    p_im = qs.get_p()
 
     times_print(w_im, w_ch, True)
 
     v_ch = get_v(l, b)
-    v_im = smo.v
+    v_im = qs.v
 
     times_print(v_im, v_ch, False)
 
     probs_print(p_im, p_ch, 10)
```

### Comparing `most_queue-1.20/most_queue/theory/mg1_warm_calc.py` & `most_queue-1.21/most_queue/theory/mg1_warm_calc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from most_queue.sim import rand_destribution as rd
 from diff5dots import diff5dots
-from most_queue.sim import smo_im
+from most_queue.sim.qs_sim import QueueingSystemSimulator
 
 
 def get_v(l, b, b_warm):
     tv = b_warm[0] / (1 - l * b[0])
     p0_star = 1 / (1 + l * tv)
 
     b_param = rd.Gamma.get_mu_alpha(b)
@@ -37,17 +37,17 @@
     coev = 1.3
     b_params = rd.H2_dist.get_params_by_mean_and_coev(b1, coev)
     b = rd.H2_dist.calc_theory_moments(*b_params, 4)
 
     b_warm_params = rd.H2_dist.get_params_by_mean_and_coev(b1, coev)
     b_warm = rd.H2_dist.calc_theory_moments(*b_params, 4)
 
-    smo = smo_im.SmoIm(1)
-    smo.set_servers(b_params, "H")
-    smo.set_warm(b_warm_params, "H")
-    smo.set_sources(l, "M")
-    smo.run(100000)
+    qs = QueueingSystemSimulator(1)
+    qs.set_servers(b_params, "H")
+    qs.set_warm(b_warm_params, "H")
+    qs.set_sources(l, "M")
+    qs.run(100000)
 
     v_ch = get_v(l, b, b_warm)
-    v_im = smo.v
+    v_im = qs.v
 
     times_print(v_im, v_ch, False)
```

### Comparing `most_queue-1.20/most_queue/theory/mgn_tt.py` & `most_queue-1.21/most_queue/theory/mgn_tt.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,15 +446,15 @@
             else:
                 output[i, i] = self.l + (num - i) * self.mu[0] + i * self.mu[1]
 
         return output
 
 
 if __name__ == "__main__":
-    from most_queue.sim import smo_im
+    from most_queue.sim.qs_sim import QueueingSystemSimulator
     from most_queue.sim import rand_destribution as rd
     from most_queue.utils.tables import times_print, probs_print
     import time
 
     n = 3  # число каналов
     l = 1.0  # интенсивность вх потока
     ro = 0.8  # коэфф загрузки
@@ -469,21 +469,21 @@
         b = [0.0] * 3
         alpha = 1 / (b_coev[k] ** 2)
         b[0] = b1
         b[1] = math.pow(b[0], 2) * (math.pow(b_coev[k], 2) + 1)
         b[2] = b[1] * b[0] * (1.0 + 2 / alpha)
 
         im_start = time.process_time()
-        smo = smo_im.SmoIm(n, buffer=buff)
-        smo.set_sources(l, 'M')
+        qs = QueueingSystemSimulator(n, buffer=buff)
+        qs.set_sources(l, 'M')
         gamma_params = rd.Gamma.get_mu_alpha([b[0], b[1]])
-        smo.set_servers(gamma_params, 'Gamma')
-        smo.run(num_of_jobs)
-        p = smo.get_p()
-        v_im = smo.v
+        qs.set_servers(gamma_params, 'Gamma')
+        qs.run(num_of_jobs)
+        p = qs.get_p()
+        v_im = qs.v
         im_time = time.process_time() - im_start
 
         h2_params = rd.H2_dist.get_params_clx(b)
 
         tt_start = time.process_time()
         tt = MGnCalc(n, l, b, buffer=buff, verbose=verbose)
         tt.run()
```

### Comparing `most_queue-1.20/most_queue/theory/mmn3_pnz_cox_approx.py` & `most_queue-1.21/most_queue/theory/mmn3_pnz_cox_approx.py`

 * *Files 4% similar despite different names*

```diff
@@ -455,15 +455,15 @@
 
             output[i, i] = sumA + sumB + sumC
 
         return output
 
 
 if __name__ == "__main__":
-    from most_queue.sim import smo_im_prty
+    from most_queue.sim.priority_queue_sim import PriorityQueueSimulator
     import mmn_prty_pnz_approx
     from mmnr_calc import M_M_n_formula
     from most_queue.sim import rand_destribution as rd
     from most_queue.utils.tables import times_print, probs_print
 
     num_of_jobs = 200000
     n = 2  # количество каналов
@@ -479,32 +479,32 @@
     b1_H = 1 / mu_H
     b1_L = 1 / mu_L
     b1_M = 1 / mu_M
     b_ave = (l_L / l_sum) * b1_L + (l_H / l_sum) * b1_H + (l_M / l_sum) * b1_M
     ro = l_sum * b_ave / n
 
     # задание ИМ:
-    smo = smo_im_prty.SmoImPrty(n, K, "PR")
+    qs = PriorityQueueSimulator(n, K, "PR")
     sources = []
     servers_params = []
     l = [l_H, l_M, l_L]
     mu = [mu_H, mu_M, mu_L]
     for j in range(K):
         sources.append({'type': 'M', 'params': l[j]})
         servers_params.append({'type': 'M', 'params': mu[j]})
 
-    smo.set_sources(sources)
-    smo.set_servers(servers_params)
+    qs.set_sources(sources)
+    qs.set_servers(servers_params)
 
     # запуск ИМ:
-    smo.run(num_of_jobs)
+    qs.run(num_of_jobs)
 
     # получение результатов ИМ:
-    p = smo.get_p()
-    v_im = smo.v
+    p = qs.get_p()
+    v_im = qs.v
 
     # расчет численным методом:
     tt = Mmn3_pnz_cox(mu_L, mu_M, mu_H, l_L, l_M, l_H)
     tt_for_second = mmn_prty_pnz_approx.MMn_PRTY_PNZ_Cox_approx(2, mu_M, mu_H, l_M, l_H)
     tt_for_second.run()
 
     tt.run()
```

### Comparing `most_queue-1.20/most_queue/theory/mmn_prty_pnz_approx.py` & `most_queue-1.21/most_queue/theory/mmn_prty_pnz_approx.py`

 * *Files 0% similar despite different names*

```diff
@@ -595,15 +595,15 @@
             output[i, i] = sumA + sumB + sumC
 
         return output
 
 
 if __name__ == "__main__":
     from most_queue.sim import rand_destribution as rd
-    from most_queue.sim import smo_im_prty
+    from most_queue.sim.priority_queue_sim import PriorityQueueSimulator
     from most_queue.utils.tables import probs_print, times_print
 
 
     num_of_jobs = 100000
     n = 3  # количество каналов
     K = 2  # количество классов
     mu_L = 1.3  # интенсивность обслуживания заявок 2-го класса
@@ -613,32 +613,32 @@
     ro = 0.8
     b1_H = 1 / mu_H
     b1_L = (ro * n - l_H * b1_H) / l_L
     l_sum = l_H + l_L
     # b_ave = (l_L / l_sum) * b1_L + (l_H / l_sum) * b1_H
 
     # задание ИМ:
-    smo = smo_im_prty.SmoImPrty(n, K, "PR")
+    qs = PriorityQueueSimulator(n, K, "PR")
     sources = []
     servers_params = []
     l = [l_H, l_L]
     mu = [mu_H, mu_L]
     for j in range(K):
         sources.append({'type': 'M', 'params': l[j]})
         servers_params.append({'type': 'M', 'params': mu[j]})
 
-    smo.set_sources(sources)
-    smo.set_servers(servers_params)
+    qs.set_sources(sources)
+    qs.set_servers(servers_params)
 
     # запуск ИМ:
-    smo.run(num_of_jobs)
+    qs.run(num_of_jobs)
 
     # получение результатов ИМ:
-    p = smo.get_p()
-    v_im = smo.v
+    p = qs.get_p()
+    v_im = qs.v
 
     # расчет численным методом:
     tt = MMn_PRTY_PNZ_Cox_approx(n, mu_L, mu_H, l_L, l_H)
     tt.run()
     p_tt = tt.get_p()
     v_tt = tt.get_second_class_v1()
     # v = tt.calculate_v()
```

### Comparing `most_queue-1.20/most_queue/theory/mmnr_calc.py` & `most_queue-1.21/most_queue/theory/mmnr_calc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 import math
-import sv_sum_calc
+from most_queue.theory import convolution_sum_calc as csc
 from most_queue.sim import rand_destribution as rd
 
-class M_M_n_formula:
+class MMnr_calc:
 
     @staticmethod
     def getPI(l, mu, n, r):
 
         ro = l / mu
-        p = M_M_n_formula.get_p(l, mu, n, r)
+        p = MMnr_calc.get_p(l, mu, n, r)
 
         chisl = math.pow(ro, n + r) * p[0]
         znam = math.factorial(n) * math.pow(n, r)
         return chisl / znam
 
     @staticmethod
     def getQ(l, mu, n, r):
         ro = l / mu
-        p = M_M_n_formula.get_p(l, mu, n, r)
+        p = MMnr_calc.get_p(l, mu, n, r)
         sum = 0
         for i in range(1, r + 1):
             sum += i * math.pow(ro / n, i)
         return p[n] * sum
 
     @staticmethod
     def get_qs(l, mu, n, r, q_num=3):
-        p = M_M_n_formula.get_p(l, mu, n, r)
+        p = MMnr_calc.get_p(l, mu, n, r)
         q_s = []
         for k in range(1, q_num + 1):
             summ = 0
             for nn in range(k, r + 1):
                 summ += (math.factorial(nn) / math.factorial(nn - k)) * p[nn+n]
             q_s.append(summ)
         return q_s
 
     @staticmethod
     def get_w(l, mu, n, r, num=3):
-        qs = M_M_n_formula.get_qs(l, mu, n, r, q_num=num)
+        qs = MMnr_calc.get_qs(l, mu, n, r, q_num=num)
         w = [0] * num
         for k in range(num):
             w[k] = qs[k] / pow(l, k + 1)
         return w
 
     @staticmethod
     def get_v(l, mu, n, r):
-        w = M_M_n_formula.get_w(l, mu, n, r)
+        w = MMnr_calc.get_w(l, mu, n, r)
         b = rd.Exp_dist.calc_theory_moments(mu)
-        v = sv_sum_calc.get_moments(w, b)
+        v = csc.get_moments(w, b)
         return v
 
     @staticmethod
     def get_p(l, mu, n, r):
 
         p = [0] * (n + r + 1)
         ro = l / mu
```

### Comparing `most_queue-1.20/most_queue/theory/network_calc.py` & `most_queue-1.21/most_queue/theory/network_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/network_viewer.py` & `most_queue-1.21/most_queue/theory/network_viewer.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/passage_time.py` & `most_queue-1.21/most_queue/theory/passage_time.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/prty_calc.py` & `most_queue-1.21/most_queue/theory/priority_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/student_stat.py` & `most_queue-1.21/most_queue/theory/student_stat.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/sv_sum_calc.py` & `most_queue-1.21/most_queue/theory/convolution_sum_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/theory/weibull.py` & `most_queue-1.21/most_queue/theory/weibull.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/utils/approx_cdf_make.py` & `most_queue-1.21/most_queue/utils/approx_cdf_make.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/utils/tables.py` & `most_queue-1.21/most_queue/utils/tables.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/visualisation/smo_im_vis.py` & `most_queue-1.21/most_queue/visualisation/smo_im_vis.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/visualisation/utils/result_table.py` & `most_queue-1.21/most_queue/visualisation/utils/result_table.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/visualisation/utils/settings_window.py` & `most_queue-1.21/most_queue/visualisation/utils/settings_window.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue/visualisation/utils/splash_screen.py` & `most_queue-1.21/most_queue/visualisation/utils/splash_screen.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.20/most_queue.egg-info/PKG-INFO` & `most_queue-1.21/most_queue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: most-queue
-Version: 1.20
+Version: 1.21
 Summary: Software package for calculation and simulation of queuing systems
 Home-page: https://github.com/xabarov/mps
 Author: Xabarov Roman
 Author-email: Xabarov Roman <xabarov1985@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `most_queue-1.20/most_queue.egg-info/SOURCES.txt` & `most_queue-1.21/most_queue.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 most_queue.egg-info/PKG-INFO
 most_queue.egg-info/SOURCES.txt
 most_queue.egg-info/dependency_links.txt
 most_queue.egg-info/not-zip-safe
 most_queue.egg-info/requires.txt
 most_queue.egg-info/top_level.txt
 most_queue/sim/__init__.py
-most_queue/sim/fj_delta_im.py
-most_queue/sim/fj_im.py
-most_queue/sim/flow_sum_im.py
-most_queue/sim/network_im_prty.py
+most_queue/sim/batch_sim.py
+most_queue/sim/fj_delta_sim.py
+most_queue/sim/fj_sim.py
+most_queue/sim/flow_sum_sim.py
+most_queue/sim/impatient_queue_sim.py
+most_queue/sim/priority_network.py
+most_queue/sim/priority_queue_sim.py
+most_queue/sim/qs_sim.py
 most_queue/sim/queue_finite_source_sim.py
 most_queue/sim/rand_destribution.py
-most_queue/sim/smo_batch_sim.py
-most_queue/sim/smo_im.py
-most_queue/sim/smo_im_prty.py
-most_queue/sim/smo_impatient_im.py
 most_queue/tests/__init__.py
 most_queue/tests/ek_d_n.py
 most_queue/tests/fj_calc.py
 most_queue/tests/fj_im.py
 most_queue/tests/flow_sum.py
 most_queue/tests/gi_m_1_calc.py
 most_queue/tests/gi_m_n_calc.py
@@ -32,20 +32,20 @@
 most_queue/tests/m_ph_n_prty.py
 most_queue/tests/mg1_calc.py
 most_queue/tests/mg1_warm_calc.py
 most_queue/tests/mgn_tt.py
 most_queue/tests/mmn3_pnz_cox_approx.py
 most_queue/tests/mmn_prty_pnz_approx.py
 most_queue/tests/network_im_prty.py
-most_queue/tests/passage_time.py
 most_queue/tests/smo_im.py
 most_queue/tests/smo_im_prty.py
 most_queue/tests/weibull.py
 most_queue/theory/__init__.py
 most_queue/theory/batch_mm1.py
+most_queue/theory/convolution_sum_calc.py
 most_queue/theory/diff5dots.py
 most_queue/theory/ek_d_n_calc.py
 most_queue/theory/engset_model.py
 most_queue/theory/fj_calc.py
 most_queue/theory/flow_sum.py
 most_queue/theory/generate_pareto_noise.py
 most_queue/theory/gi_m_1_calc.py
@@ -59,23 +59,21 @@
 most_queue/theory/mgn_tt.py
 most_queue/theory/mmn3_pnz_cox_approx.py
 most_queue/theory/mmn_prty_pnz_approx.py
 most_queue/theory/mmnr_calc.py
 most_queue/theory/network_calc.py
 most_queue/theory/network_viewer.py
 most_queue/theory/passage_time.py
-most_queue/theory/prty_calc.py
+most_queue/theory/priority_calc.py
 most_queue/theory/q_poisson_arrival_calc.py
 most_queue/theory/student_stat.py
-most_queue/theory/sv_sum_calc.py
 most_queue/theory/weibull.py
 most_queue/utils/__init__.py
 most_queue/utils/approx_cdf_make.py
 most_queue/utils/binom_probs.py
-most_queue/utils/difstir.py
 most_queue/utils/tables.py
 most_queue/visualisation/__init__.py
 most_queue/visualisation/smo_im_vis.py
 most_queue/visualisation/utils/__init__.py
 most_queue/visualisation/utils/result_table.py
 most_queue/visualisation/utils/settings_window.py
 most_queue/visualisation/utils/splash_screen.py
```

### Comparing `most_queue-1.20/setup.py` & `most_queue-1.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='most-queue',
-      version='1.20',
+      version='1.21',
       description="Software package for calculation and simulation of queuing systems",
       author='Xabarov Roman',
       author_email='xabarov1985@gmail.com',
       url='https://github.com/xabarov/mps',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
```

