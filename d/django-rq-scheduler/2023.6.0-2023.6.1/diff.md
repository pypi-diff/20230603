# Comparing `tmp/django_rq_scheduler-2023.6.0.tar.gz` & `tmp/django_rq_scheduler-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rq_scheduler-2023.6.0.tar", max compression
+gzip compressed data, was "django_rq_scheduler-2023.6.1.tar", max compression
```

## Comparing `django_rq_scheduler-2023.6.0.tar` & `django_rq_scheduler-2023.6.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1107 2023-05-12 14:29:26.090261 django_rq_scheduler-2023.6.0/LICENSE
--rw-r--r--   0        0        0     1558 2023-05-12 14:29:26.090261 django_rq_scheduler-2023.6.0/README.md
--rw-r--r--   0        0        0     1769 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/pyproject.toml
--rw-r--r--   0        0        0      134 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/__init__.py
--rw-r--r--   0        0        0      147 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/admin/__init__.py
--rw-r--r--   0        0        0     5661 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/admin/job.py
--rw-r--r--   0        0        0     1641 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/admin/redis_models.py
--rw-r--r--   0        0        0      281 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/apps.py
--rw-r--r--   0        0        0     1214 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/decorators.py
--rw-r--r--   0        0        0        0 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/commands/__init__.py
--rw-r--r--   0        0        0     1189 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/commands/delete_failed_executions.py
--rw-r--r--   0        0        0     1908 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/commands/export.py
--rw-r--r--   0        0        0     3417 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/commands/import.py
--rw-r--r--   0        0        0     3602 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/commands/rqstats.py
--rw-r--r--   0        0        0     3176 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/commands/rqworker.py
--rw-r--r--   0        0        0     1374 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/commands/run_job.py
--rw-r--r--   0        0        0     7162 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
--rw-r--r--   0        0        0      898 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
--rw-r--r--   0        0        0     4196 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0003_auto_20220329_2107.py
--rw-r--r--   0        0        0      791 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0      896 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0      728 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0006_auto_20230118_1640.py
--rw-r--r--   0        0        0     1302 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0007_add_result_ttl.py
--rw-r--r--   0        0        0     1982 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
--rw-r--r--   0        0        0     1362 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
--rw-r--r--   0        0        0      661 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0010_queue.py
--rw-r--r--   0        0        0     7643 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
--rw-r--r--   0        0        0      934 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py
--rw-r--r--   0        0        0     1320 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0013_alter_cronjob_queue_alter_repeatablejob_queue_and_more.py
--rw-r--r--   0        0        0        0 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/__init__.py
--rw-r--r--   0        0        0      187 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/models/__init__.py
--rw-r--r--   0        0        0     3102 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/models/args.py
--rw-r--r--   0        0        0      364 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/models/queue.py
--rw-r--r--   0        0        0    15332 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/models/scheduled_job.py
--rw-r--r--   0        0        0      366 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/models/worker.py
--rw-r--r--   0        0        0        0 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/py.typed
--rw-r--r--   0        0        0     5048 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/queues.py
--rw-r--r--   0        0        0     9041 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/rq_classes.py
--rw-r--r--   0        0        0     1073 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/settings.py
--rw-r--r--   0        0        0      163 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/change_form.html
--rw-r--r--   0        0        0      127 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/change_list.html
--rw-r--r--   0        0        0     1595 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/confirm_action.html
--rw-r--r--   0        0        0     7822 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/job_detail.html
--rw-r--r--   0        0        0     2697 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/jobs-list.partial.html
--rw-r--r--   0        0        0     6360 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/jobs.html
--rw-r--r--   0        0        0      915 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/queue_workers.html
--rw-r--r--   0        0        0      568 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/scheduler_base.html
--rw-r--r--   0        0        0     1324 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/single_job_action.html
--rw-r--r--   0        0        0     4224 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/stats.html
--rw-r--r--   0        0        0     3032 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/worker_details.html
--rw-r--r--   0        0        0     1879 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/workers-list.partial.html
--rw-r--r--   0        0        0      935 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/workers.html
--rw-r--r--   0        0        0        0 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/templatetags/__init__.py
--rw-r--r--   0        0        0     1546 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/templatetags/scheduler_tags.py
--rw-r--r--   0        0        0        0 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/__init__.py
--rw-r--r--   0        0        0      502 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/jobs.py
--rw-r--r--   0        0        0      668 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_internals.py
--rw-r--r--   0        0        0     5887 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_job_arg_models.py
--rw-r--r--   0        0        0     2349 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_job_decorator.py
--rw-r--r--   0        0        0     4920 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_mgmt_cmds.py
--rw-r--r--   0        0        0    27724 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_models.py
--rw-r--r--   0        0        0      807 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_redis_models.py
--rw-r--r--   0        0        0     2317 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_settings.py
--rw-r--r--   0        0        0    18728 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_views.py
--rw-r--r--   0        0        0     1577 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_worker.py
--rw-r--r--   0        0        0     3399 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/testtools.py
--rw-r--r--   0        0        0     2677 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tools.py
--rw-r--r--   0        0        0     1121 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/urls.py
--rw-r--r--   0        0        0    15854 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/views.py
--rw-r--r--   0        0        0     3304 1970-01-01 00:00:00.000000 django_rq_scheduler-2023.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1107 2023-06-03 14:51:51.030081 django_rq_scheduler-2023.6.1/LICENSE
+-rw-r--r--   0        0        0     1366 2023-06-03 14:51:51.030081 django_rq_scheduler-2023.6.1/README.md
+-rw-r--r--   0        0        0     1860 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/__init__.py
+-rw-r--r--   0        0        0      104 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/admin/__init__.py
+-rw-r--r--   0        0        0     5613 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/admin/job.py
+-rw-r--r--   0        0        0     1468 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/admin/redis_models.py
+-rw-r--r--   0        0        0      281 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/apps.py
+-rw-r--r--   0        0        0     1214 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/decorators.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/commands/__init__.py
+-rw-r--r--   0        0        0     1303 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/commands/delete_failed_executions.py
+-rw-r--r--   0        0        0     1907 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/commands/export.py
+-rw-r--r--   0        0        0     3835 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/commands/import.py
+-rw-r--r--   0        0        0     3438 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/commands/rqstats.py
+-rw-r--r--   0        0        0     3176 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/commands/rqworker.py
+-rw-r--r--   0        0        0     1374 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/management/commands/run_job.py
+-rw-r--r--   0        0        0     6402 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
+-rw-r--r--   0        0        0      898 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
+-rw-r--r--   0        0        0     4196 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0003_auto_20220329_2107.py
+-rw-r--r--   0        0        0      791 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0      896 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0      728 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0006_auto_20230118_1640.py
+-rw-r--r--   0        0        0     1302 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0007_add_result_ttl.py
+-rw-r--r--   0        0        0     1982 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
+-rw-r--r--   0        0        0     1362 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
+-rw-r--r--   0        0        0      661 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0010_queue.py
+-rw-r--r--   0        0        0     7643 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
+-rw-r--r--   0        0        0      934 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py
+-rw-r--r--   0        0        0     1320 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/0013_alter_cronjob_queue_alter_repeatablejob_queue_and_more.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/migrations/__init__.py
+-rw-r--r--   0        0        0      187 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/models/__init__.py
+-rw-r--r--   0        0        0     3113 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/models/args.py
+-rw-r--r--   0        0        0      364 2023-06-03 14:51:51.034081 django_rq_scheduler-2023.6.1/scheduler/models/queue.py
+-rw-r--r--   0        0        0    14803 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/models/scheduled_job.py
+-rw-r--r--   0        0        0      366 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/models/worker.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/py.typed
+-rw-r--r--   0        0        0     5056 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/queues.py
+-rw-r--r--   0        0        0     9124 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/rq_classes.py
+-rw-r--r--   0        0        0     1073 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/settings.py
+-rw-r--r--   0        0        0      163 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/change_form.html
+-rw-r--r--   0        0        0      127 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/change_list.html
+-rw-r--r--   0        0        0     1595 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/confirm_action.html
+-rw-r--r--   0        0        0     7823 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/job_detail.html
+-rw-r--r--   0        0        0     2697 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/jobs-list.partial.html
+-rw-r--r--   0        0        0     6360 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/jobs.html
+-rw-r--r--   0        0        0      915 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/queue_workers.html
+-rw-r--r--   0        0        0      568 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/scheduler_base.html
+-rw-r--r--   0        0        0     1324 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/single_job_action.html
+-rw-r--r--   0        0        0     4224 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/stats.html
+-rw-r--r--   0        0        0     3032 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/worker_details.html
+-rw-r--r--   0        0        0     1879 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/workers-list.partial.html
+-rw-r--r--   0        0        0      935 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/workers.html
+-rw-r--r--   0        0        0        0 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templatetags/__init__.py
+-rw-r--r--   0        0        0     1652 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/templatetags/scheduler_tags.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/__init__.py
+-rw-r--r--   0        0        0      502 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/jobs.py
+-rw-r--r--   0        0        0      668 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_internals.py
+-rw-r--r--   0        0        0     5887 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_job_arg_models.py
+-rw-r--r--   0        0        0     2349 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_job_decorator.py
+-rw-r--r--   0        0        0    10967 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_mgmt_cmds.py
+-rw-r--r--   0        0        0    27724 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_models.py
+-rw-r--r--   0        0        0      807 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_redis_models.py
+-rw-r--r--   0        0        0     2317 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_settings.py
+-rw-r--r--   0        0        0    20065 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_views.py
+-rw-r--r--   0        0        0     1577 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/test_worker.py
+-rw-r--r--   0        0        0     3399 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tests/testtools.py
+-rw-r--r--   0        0        0     2742 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/tools.py
+-rw-r--r--   0        0        0     1121 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/urls.py
+-rw-r--r--   0        0        0    16239 2023-06-03 14:51:51.038081 django_rq_scheduler-2023.6.1/scheduler/views.py
+-rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 django_rq_scheduler-2023.6.1/PKG-INFO
```

### Comparing `django_rq_scheduler-2023.6.0/LICENSE` & `django_rq_scheduler-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/README.md` & `django_rq_scheduler-2023.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -19,12 +19,7 @@
 # Sponsor
 
 django-rq-scheduler is developed for free.
 
 You can support this project by becoming a sponsor using [this link](https://github.com/sponsors/cunla).
 
 
-## Security contact information
-
-To report a security vulnerability, please use the
-[Tidelift security contact](https://tidelift.com/security).
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `django_rq_scheduler-2023.6.0/pyproject.toml` & `django_rq_scheduler-2023.6.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-rq-scheduler"
 packages = [
     { include = "scheduler" },
 ]
-version = "2023.6.0"
+version = "2023.6.1"
 description = "An async job scheduler for django using redis"
 readme = "README.md"
 keywords = ["redis", "django", "background-jobs", "job-queue", "task-queue", "redis-queue", "scheduled-jobs"]
 authors = [
-    "Daniel Moran <daniel.maruani@gmail.com>",
+    "Daniel Moran <daniel@moransoftware.ca>",
 ]
 maintainers = [
-    "Daniel Moran <daniel.maruani@gmail.com>",
+    "Daniel Moran <daniel@moransoftware.ca>",
 ]
 license = "MIT"
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
@@ -29,35 +29,39 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Framework :: Django',
     'Framework :: Django :: 4',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
     'Framework :: Django :: 4.2',
+    'Framework :: Django :: 3',
     'Framework :: Django :: 3.2',
 ]
 homepage = "https://github.com/dsoftwareinc/django-rq-scheduler"
 documentation = "https://django-rq-scheduler.readthedocs.io/en/latest/"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/dsoftwareinc/django-rq-scheduler/issues"
 "Funding" = "https://github.com/sponsors/cunla"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 django = ">=3.2"
-django-model-utils = "^4.3"
 croniter = "^1.3"
 click = "^8.1"
-rq = "^1.14"
+rq = "^1.15"
+pyyaml = { version = "^6.0", optional = true }
 
 [tool.poetry.dev-dependencies]
-poetry = "^1.4"
+poetry = "^1.5"
 coverage = "^7"
-fakeredis = { version = "^2.12", extras=['lua'] }
+fakeredis = { version = "^2.13", extras = ['lua'] }
 Flake8-pyproject = "^1.2"
 
+[tool.poetry.extras]
+yaml = ["pyyaml"]
+
 [tool.flake8]
 max-line-length = 119
 exclude = [
     'scheduler/migrations',
 ]
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/admin/job.py` & `django_rq_scheduler-2023.6.1/scheduler/admin/job.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,26 @@
     fieldsets = (
         (None, {
             'fields': (('key',), ('arg_type', 'val',),),
         }),
     )
 
 
+@admin.register(CronJob, ScheduledJob, RepeatableJob)
 class JobAdmin(admin.ModelAdmin):
+    LIST_DISPLAY_EXTRA = dict(
+        CronJob=('cron_string', 'next_run',),
+        ScheduledJob=('scheduled_time',),
+        RepeatableJob=('scheduled_time', 'interval_display'),
+    )
+    FIELDSET_EXTRA = dict(
+        CronJob=('cron_string', 'repeat', 'timeout', 'result_ttl',),
+        ScheduledJob=('scheduled_time', 'timeout', 'result_ttl'),
+        RepeatableJob=('scheduled_time', ('interval', 'interval_unit',), 'repeat', 'timeout', 'result_ttl',),
+    )
     """BaseJob admin class"""
     save_on_top = True
     change_form_template = 'admin/scheduler/change_form.html'
     actions = ['disable_selected', 'enable_selected', 'enqueue_job_now', ]
     inlines = [JobArgInline, JobKwargInline, ]
     list_filter = ('enabled',)
     list_display = ('enabled', 'name', 'job_id', 'function_string', 'is_scheduled', 'queue',)
@@ -49,14 +60,30 @@
             'fields': ('name', 'callable', 'enabled', 'at_front',),
         }),
         (_('RQ Settings'), {
             'fields': ('queue', 'job_id',),
         }),
     )
 
+    def get_list_display(self, request):
+        if self.model.__name__ not in JobAdmin.LIST_DISPLAY_EXTRA:
+            raise ValueError(f'Unrecognized model {self.model}')
+        return JobAdmin.list_display + JobAdmin.LIST_DISPLAY_EXTRA[self.model.__name__]
+
+    def get_fieldsets(self, request, obj=None):
+        if self.model.__name__ not in JobAdmin.FIELDSET_EXTRA:
+            raise ValueError(f'Unrecognized model {self.model}')
+        return JobAdmin.fieldsets + ((_('Scheduling'), {
+            'fields': JobAdmin.FIELDSET_EXTRA[self.model.__name__],
+        }),)
+
+    @admin.display(description='Next run')
+    def next_run(self, o: CronJob):
+        return tools.get_next_cron_time(o.cron_string)
+
     def change_view(self, request, object_id, form_url='', extra_context=None):
         extra = extra_context or {}
         obj = self.get_object(request, object_id)
         try:
             execution_list = get_job_executions(obj.queue, obj)
         except redis.ConnectionError as e:
             logger.warn(f'Could not get job executions: {e}')
@@ -113,59 +140,7 @@
     @admin.action(description="Enqueue now", permissions=('change',))
     def enqueue_job_now(self, request, queryset):
         job_names = []
         for job in queryset:
             job.enqueue_to_run()
             job_names.append(job.name)
         self.message_user(request, f"The following jobs have been enqueued: {', '.join(job_names)}", )
-
-
-@admin.register(ScheduledJob)
-class ScheduledJobAdmin(JobAdmin):
-    list_display = JobAdmin.list_display + ('scheduled_time',)
-
-    fieldsets = JobAdmin.fieldsets + (
-        (_('Scheduling'), {
-            'fields': (
-                'scheduled_time',
-                'timeout',
-                'result_ttl'
-            ),
-        }),
-    )
-
-
-@admin.register(RepeatableJob)
-class RepeatableJobAdmin(JobAdmin):
-    list_display = JobAdmin.list_display + ('scheduled_time', 'interval_display')
-
-    fieldsets = JobAdmin.fieldsets + (
-        (_('Scheduling'), {
-            'fields': (
-                'scheduled_time',
-                ('interval', 'interval_unit',),
-                'repeat',
-                'timeout',
-                'result_ttl',
-            ),
-        }),
-    )
-
-
-@admin.register(CronJob)
-class CronJobAdmin(JobAdmin):
-    list_display = JobAdmin.list_display + ('cron_string', 'next_run')
-
-    fieldsets = JobAdmin.fieldsets + (
-        (_('Scheduling'), {
-            'fields': (
-                'cron_string',
-                'repeat',
-                'timeout',
-                'result_ttl',
-            ),
-        }),
-    )
-
-    @admin.display(description='Next run')
-    def next_run(self, o):
-        return tools.get_next_cron_time(o.cron_string)
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/admin/redis_models.py` & `django_rq_scheduler-2023.6.1/scheduler/admin/redis_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from django.contrib import admin
 
-from scheduler import settings
 from scheduler import views
 from scheduler.models import Queue
 from scheduler.models.worker import Worker
 
-QUEUES = [(key, key) for key in settings.QUEUES.keys()]
-
 
 class ImmutableAdmin(admin.ModelAdmin):
     def has_add_permission(self, request):
         return False  # Hide the admin "+ Add" link for Queues
 
     def has_change_permission(self, request, obj=None):
         return True
@@ -27,23 +24,21 @@
         `ModelAdmin.has_(add|change|delete)_permission` for that.
         """
         return request.user.has_module_perms('django-rq-scheduler')
 
 
 @admin.register(Queue)
 class QueueAdmin(ImmutableAdmin):
-    """Admin View for Django-RQ Queue"""
+    """Admin View for queues"""
 
     def changelist_view(self, request, extra_context=None):
         """The 'change list' admin view for this model."""
-        # proxy request to stats view
         return views.stats(request)
 
 
 @admin.register(Worker)
 class WorkerAdmin(ImmutableAdmin):
     """Admin View for workers"""
 
     def changelist_view(self, request, extra_context=None):
         """The 'change list' admin view for this model."""
-        # proxy request to stats view
         return views.workers(request)
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/decorators.py` & `django_rq_scheduler-2023.6.1/scheduler/decorators.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/management/commands/delete_failed_executions.py` & `django_rq_scheduler-2023.6.1/scheduler/management/commands/delete_failed_executions.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,20 +12,20 @@
         parser.add_argument(
             '--queue', '-q', dest='queue', default='default',
             help='Specify the queue [default]')
         parser.add_argument('-f', '--func', help='optional job function name, e.g. "app.tasks.func"')
         parser.add_argument('--dry-run', action='store_true', help='Do not actually delete failed jobs')
 
     def handle(self, *args, **options):
-        queue = get_queue(options['queue'])
+        queue = get_queue(options.get('queue', 'default'))
         job_ids = queue.failed_job_registry.get_job_ids()
-        jobs = [JobExecution.fetch(job_id) for job_id in job_ids]
+        jobs = [JobExecution.fetch(job_id, connection=queue.connection) for job_id in job_ids]
         func_name = options.get('func', None)
         if func_name is not None:
             jobs = [job for job in jobs if job.func_name == func_name]
-        if options['dry_run']:
-            click.echo(f'Found {len(jobs)} failed jobs')
-            return
-
+        dry_run = options.get('dry_run', False)
+        click.echo(f'Found {len(jobs)} failed jobs')
         for job in jobs:
-            job.delete()
+            click.echo(f'Deleting {job.id}')
+            if not dry_run:
+                job.delete()
         click.echo(f'Deleted {len(jobs)} failed jobs')
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/management/commands/export.py` & `django_rq_scheduler-2023.6.1/scheduler/management/commands/export.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,26 +39,26 @@
     def handle(self, *args, **options):
         file = open(options.get('filename'), 'w') if options.get("filename") else sys.stdout
         res = list()
         for model_name in MODEL_NAMES:
             model = apps.get_model(app_label='scheduler', model_name=model_name)
             jobs = model.objects.all()
             if options.get('enabled'):
-                jobs = jobs.filtered(enabled=True)
+                jobs = jobs.filter(enabled=True)
             for job in jobs:
                 res.append(job.to_dict())
 
         if options.get("format") == 'json':
             import json
             click.echo(json.dumps(res, indent=2), file=file)
             return
 
         if options.get("format") == 'yaml':
             try:
                 import yaml
             except ImportError:
                 click.echo("Aborting. LibYAML is not installed.")
-                return
+                exit(1)
             # Disable YAML alias
             yaml.Dumper.ignore_aliases = lambda *x: True
             click.echo(yaml.dump(res, default_flow_style=False), file=file)
             return
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/management/commands/import.py` & `django_rq_scheduler-2023.6.1/scheduler/management/commands/import.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sys
-from datetime import datetime
 
 import click
 from django.apps import apps
+from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.core.management.base import BaseCommand
+from django.utils import timezone
 
 from scheduler.models import JobArg, JobKwarg
 from scheduler.tools import MODEL_NAMES
 
 
 def create_job_from_dict(job_dict, update):
     model = apps.get_model(app_label='scheduler', model_name=job_dict['model'])
@@ -20,17 +21,22 @@
         else:
             click.echo(f'Found existing job "{existing_job}", skipping')
             return
     kwargs = dict(job_dict)
     del kwargs['model']
     del kwargs['callable_args']
     del kwargs['callable_kwargs']
-    if 'scheduled_time' in kwargs:
-        kwargs['scheduled_time'] = datetime.fromisoformat(kwargs['scheduled_time'])
-
+    if kwargs.get('scheduled_time', None):
+        kwargs['scheduled_time'] = timezone.datetime.fromisoformat(kwargs['scheduled_time'])
+        if not settings.USE_TZ:
+            kwargs['scheduled_time'] = timezone.make_naive(kwargs['scheduled_time'])
+    model_fields = set(map(lambda field: field.attname, model._meta.get_fields()))
+    keys_to_ignore = list(filter(lambda k: k not in model_fields, kwargs.keys()))
+    for k in keys_to_ignore:
+        del kwargs[k]
     scheduled_job = model.objects.create(**kwargs)
     click.echo(f'Created job {scheduled_job}')
     content_type = ContentType.objects.get_for_model(scheduled_job)
 
     for arg in job_dict['callable_args']:
         JobArg.objects.create(
             content_type=content_type, object_id=scheduled_job.id, **arg, )
@@ -79,25 +85,25 @@
         jobs = list()
         if options.get("format") == 'json':
             import json
             try:
                 jobs = json.load(file)
             except json.decoder.JSONDecodeError:
                 click.echo('Error decoding json', err=True)
-
-        if options.get("format") == 'yaml':
+                exit(1)
+        elif options.get("format") == 'yaml':
             try:
                 import yaml
             except ImportError:
                 click.echo("Aborting. LibYAML is not installed.")
-                return
+                exit(1)
             # Disable YAML alias
             yaml.Dumper.ignore_aliases = lambda *x: True
             jobs = yaml.load(file, yaml.SafeLoader)
 
         if options.get('reset'):
             for model_name in MODEL_NAMES:
                 model = apps.get_model(app_label='scheduler', model_name=model_name)
-                model.objects.delete()
+                model.objects.all().delete()
 
         for job in jobs:
             create_job_from_dict(job, update=options.get('update'))
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/management/commands/rqstats.py` & `django_rq_scheduler-2023.6.1/scheduler/management/commands/rqstats.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import time
 
 import click
 from django.core.management.base import BaseCommand
-
 from scheduler.views import get_statistics
 
 ANSI_LIGHT_GREEN = "\033[1;32m"
 ANSI_LIGHT_WHITE = "\033[1;37m"
 ANSI_RESET = "\033[0m"
 
 KEYS = ('jobs', 'started_jobs', 'deferred_jobs', 'finished_jobs', 'canceled_jobs', 'workers')
@@ -49,19 +48,16 @@
         click.echo()
         self._print_separator()
         click.echo(f'| {"Name":<16} |    Queued |    Active |  Deferred |'
                    f'  Finished |'
                    f'  Canceled |'
                    f'   Workers |')
         self._print_separator()
-
         for ind, queue in enumerate(statistics["queues"]):
-            vals = (queue[k] for k in KEYS)
-            vals = (queue["jobs"], queue["started_jobs"], queue["deferred_jobs"],
-                    queue["finished_jobs"], queue['canceled_jobs'], queue["workers"])
+            vals = list((queue[k] for k in KEYS))
             # Deal with colors
             if prev_stats and len(prev_stats['queues']) > ind:
                 prev = prev_stats["queues"][ind]
                 prev_vals = (prev[k] for k in KEYS)
                 colors = [ANSI_LIGHT_GREEN
                           if vals[i] != prev_vals[i] else ANSI_LIGHT_WHITE
                           for i in range(len(prev_vals))
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/management/commands/rqworker.py` & `django_rq_scheduler-2023.6.1/scheduler/management/commands/rqworker.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/management/commands/run_job.py` & `django_rq_scheduler-2023.6.1/scheduler/management/commands/run_job.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py` & `django_rq_scheduler-2023.6.1/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # Generated by Django 4.0.1 on 2022-01-06 20:34
 
-import django.utils.timezone
-import model_utils.fields
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-    replaces = [('scheduler', '0001_initial'), ('scheduler', '0002_add_timeout'),
-                ('scheduler', '0003_remove_queue_choices'), ('scheduler', '0004_add_cron_jobs'),
-                ('scheduler', '0005_added_result_ttl')]
+    # replaces = [('scheduler', '0001_initial'), ('scheduler', '0002_add_timeout'),
+    #             ('scheduler', '0003_remove_queue_choices'), ('scheduler', '0004_add_cron_jobs'),
+    #             ('scheduler', '0005_added_result_ttl')]
 
     dependencies = [
     ]
 
     operations = [
         migrations.CreateModel(
             name='CronJob',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('created', model_utils.fields.AutoCreatedField(default=django.utils.timezone.now, editable=False,
-                                                                verbose_name='created')),
-                ('modified', model_utils.fields.AutoLastModifiedField(default=django.utils.timezone.now, editable=False,
-                                                                      verbose_name='modified')),
+                ('created', models.DateTimeField(auto_now_add=True, verbose_name='created')),
+                ('modified', models.DateTimeField(auto_now=True, verbose_name='modified')),
                 ('name', models.CharField(max_length=128, unique=True, verbose_name='name')),
                 ('callable', models.CharField(max_length=2048, verbose_name='callable')),
                 ('enabled', models.BooleanField(default=True, verbose_name='enabled')),
                 ('queue', models.CharField(max_length=16, verbose_name='queue')),
                 ('job_id',
                  models.CharField(blank=True, editable=False, max_length=128, null=True, verbose_name='job id')),
                 ('timeout', models.IntegerField(blank=True,
@@ -42,18 +38,16 @@
                 'verbose_name_plural': 'Cron Jobs',
             },
         ),
         migrations.CreateModel(
             name='RepeatableJob',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('created', model_utils.fields.AutoCreatedField(default=django.utils.timezone.now, editable=False,
-                                                                verbose_name='created')),
-                ('modified', model_utils.fields.AutoLastModifiedField(default=django.utils.timezone.now, editable=False,
-                                                                      verbose_name='modified')),
+                ('created', models.DateTimeField(auto_now_add=True, verbose_name='created')),
+                ('modified', models.DateTimeField(auto_now=True, verbose_name='modified')),
                 ('name', models.CharField(max_length=128, unique=True, verbose_name='name')),
                 ('callable', models.CharField(max_length=2048, verbose_name='callable')),
                 ('enabled', models.BooleanField(default=True, verbose_name='enabled')),
                 ('queue', models.CharField(max_length=16, verbose_name='queue')),
                 ('job_id',
                  models.CharField(blank=True, editable=False, max_length=128, null=True, verbose_name='job id')),
                 ('scheduled_time', models.DateTimeField(verbose_name='scheduled time')),
@@ -75,18 +69,16 @@
                 'verbose_name_plural': 'Repeatable Jobs',
             },
         ),
         migrations.CreateModel(
             name='ScheduledJob',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('created', model_utils.fields.AutoCreatedField(default=django.utils.timezone.now, editable=False,
-                                                                verbose_name='created')),
-                ('modified', model_utils.fields.AutoLastModifiedField(default=django.utils.timezone.now, editable=False,
-                                                                      verbose_name='modified')),
+                ('created', models.DateTimeField(auto_now_add=True, verbose_name='created')),
+                ('modified', models.DateTimeField(auto_now=True, verbose_name='modified')),
                 ('name', models.CharField(max_length=128, unique=True, verbose_name='name')),
                 ('callable', models.CharField(max_length=2048, verbose_name='callable')),
                 ('enabled', models.BooleanField(default=True, verbose_name='enabled')),
                 ('queue', models.CharField(max_length=16, verbose_name='queue')),
                 ('job_id',
                  models.CharField(blank=True, editable=False, max_length=128, null=True, verbose_name='job id')),
                 ('scheduled_time', models.DateTimeField(verbose_name='scheduled time')),
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py` & `django_rq_scheduler-2023.6.1/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/migrations/0003_auto_20220329_2107.py` & `django_rq_scheduler-2023.6.1/scheduler/migrations/0003_auto_20220329_2107.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py` & `django_rq_scheduler-2023.6.1/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py` & `django_rq_scheduler-2023.6.1/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/migrations/0006_auto_20230118_1640.py` & `django_rq_scheduler-2023.6.1/scheduler/migrations/0006_auto_20230118_1640.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/migrations/0007_add_result_ttl.py` & `django_rq_scheduler-2023.6.1/scheduler/migrations/0007_add_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py` & `django_rq_scheduler-2023.6.1/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py` & `django_rq_scheduler-2023.6.1/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/migrations/0010_queue.py` & `django_rq_scheduler-2023.6.1/scheduler/migrations/0010_queue.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py` & `django_rq_scheduler-2023.6.1/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py` & `django_rq_scheduler-2023.6.1/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/migrations/0013_alter_cronjob_queue_alter_repeatablejob_queue_and_more.py` & `django_rq_scheduler-2023.6.1/scheduler/migrations/0013_alter_cronjob_queue_alter_repeatablejob_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/models/args.py` & `django_rq_scheduler-2023.6.1/scheduler/models/args.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,37 +2,36 @@
 from typing import Callable
 
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-from model_utils import Choices
 
 from scheduler import tools
 
 ARG_TYPE_TYPES_DICT = {
     'str': str,
     'int': int,
     'bool': bool,
     'datetime': datetime,
     'callable': Callable,
 }
 
 
 class BaseJobArg(models.Model):
-    ARG_TYPE = Choices(
-        ('str', _('string')),
-        ('int', _('int')),
-        ('bool', _('boolean')),
-        ('datetime', _('datetime')),
-        ('callable', _('callable')),
-    )
+    class ArgType(models.TextChoices):
+        STR = 'str', _('string')
+        INT = 'int', _('int')
+        BOOL = 'bool', _('boolean')
+        DATETIME = 'datetime', _('datetime')
+        CALLABLE = 'callable', _('callable')
+
     arg_type = models.CharField(
-        _('Argument Type'), max_length=12, choices=ARG_TYPE, default=ARG_TYPE.str
+        _('Argument Type'), max_length=12, choices=ArgType.choices, default=ArgType.STR,
     )
     val = models.CharField(_('Argument Value'), blank=True, max_length=255)
     content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
     object_id = models.PositiveIntegerField()
     content_object = GenericForeignKey()
 
     def clean(self):
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/models/scheduled_job.py` & `django_rq_scheduler-2023.6.1/scheduler/models/scheduled_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.templatetags.tz import utc
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
-from model_utils import Choices
-from model_utils.models import TimeStampedModel
 
 from scheduler import settings
 from scheduler import tools
 from scheduler.models.args import JobArg, JobKwarg
 from scheduler.queues import get_queue, logger
 from scheduler.rq_classes import DjangoQueue
 
@@ -33,15 +31,17 @@
     model = apps.get_model(app_label='scheduler', model_name=model_name)
     scheduled_job = model.objects.filter(job_id=job.id).first()
     if scheduled_job is not None:
         scheduled_job.unschedule()
         scheduled_job.schedule()
 
 
-class BaseJob(TimeStampedModel):
+class BaseJob(models.Model):
+    created = models.DateTimeField(auto_now_add=True)
+    modified = models.DateTimeField(auto_now=True)
     QUEUES = [(key, key) for key in settings.QUEUES.keys()]
     JOB_TYPE = 'BaseJob'
     name = models.CharField(
         _('name'), max_length=128, unique=True,
         help_text='Name of the job.', )
     callable = models.CharField(_('callable'), max_length=2048)
     callable_args = GenericRelation(JobArg, related_query_name='args')
@@ -205,20 +205,20 @@
             queue.remove(self.job_id)
             queue.scheduled_job_registry.remove(self.job_id)
         self.job_id = None
         super(BaseJob, self).save()
         return True
 
     def _schedule_time(self):
-        raise NotImplementedError
+        return utc(self.scheduled_time)
 
     def to_dict(self) -> Dict:
         """Export model to dictionary, so it can be saved as external file backup
         """
-        return dict(
+        res = dict(
             model=self.JOB_TYPE,
             name=self.name,
             callable=self.callable,
             callable_args=[
                 dict(arg_type=arg.arg_type, val=arg.val, )
                 for arg in self.callable_args.all()],
             callable_kwargs=[
@@ -226,26 +226,34 @@
                 for arg in self.callable_kwargs.all()],
             enabled=self.enabled,
             queue=self.queue,
             repeat=self.repeat,
             at_front=self.at_front,
             timeout=self.timeout,
             result_ttl=self.result_ttl,
+            cron_string=getattr(self, 'cron_string', None),
+            scheduled_time=self._schedule_time().isoformat(),
+            interval=getattr(self, 'interval', None),
+            interval_unit=getattr(self, 'interval_unit', None),
         )
+        return res
 
     def get_absolute_url(self):
         model = self._meta.model.__name__.lower()
         return reverse(f'admin:scheduler_{model}_change', args=[self.id, ])
 
     def __str__(self):
         func = self.function_string()
         return f'{self.JOB_TYPE}[{self.name}={func}]'
 
     def save(self, **kwargs):
         schedule_job = kwargs.pop('schedule_job', True)
+        update_fields = kwargs.get('update_fields', None)
+        if update_fields:
+            kwargs['update_fields'] = set(update_fields).union({'modified'})
         super(BaseJob, self).save(**kwargs)
         if schedule_job:
             self.schedule()
             super(BaseJob, self).save()
 
     def delete(self, **kwargs):
         self.unschedule()
@@ -276,66 +284,47 @@
     class Meta:
         abstract = True
 
 
 class ScheduledTimeMixin(models.Model):
     scheduled_time = models.DateTimeField(_('scheduled time'))
 
-    def _schedule_time(self):
-        return utc(self.scheduled_time)
-
     class Meta:
         abstract = True
 
 
 class ScheduledJob(ScheduledTimeMixin, BaseJob):
     repeat = None
     JOB_TYPE = 'ScheduledJob'
 
     def ready_for_schedule(self) -> bool:
         return (super(ScheduledJob, self).ready_for_schedule()
                 and (self.scheduled_time is None
                      or self.scheduled_time >= timezone.now()))
 
-    def to_dict(self) -> Dict:
-        res = super(ScheduledJob, self).to_dict()
-        res['scheduled_time'] = self.scheduled_time.isoformat()
-        del res['repeat']
-        return res
-
     class Meta:
         verbose_name = _('Scheduled Job')
         verbose_name_plural = _('Scheduled Jobs')
         ordering = ('name',)
 
 
 class RepeatableJob(ScheduledTimeMixin, BaseJob):
-    UNITS = Choices(
-        ('seconds', _('seconds')),
-        ('minutes', _('minutes')),
-        ('hours', _('hours')),
-        ('days', _('days')),
-        ('weeks', _('weeks')),
-    )
+    class TimeUnits(models.TextChoices):
+        SECONDS = 'seconds', _('seconds')
+        MINUTES = 'minutes', _('minutes')
+        HOURS = 'hours', _('hours')
+        DAYS = 'days', _('days')
+        WEEKS = 'weeks', _('weeks')
 
     interval = models.PositiveIntegerField(_('interval'))
     interval_unit = models.CharField(
-        _('interval unit'), max_length=12, choices=UNITS, default=UNITS.hours
+        _('interval unit'), max_length=12, choices=TimeUnits.choices, default=TimeUnits.HOURS
     )
     JOB_TYPE = 'RepeatableJob'
 
-    def to_dict(self) -> Dict:
-        res = super(RepeatableJob, self).to_dict()
-        res.update(dict(
-            scheduled_time=self.scheduled_time.isoformat(),
-            interval=self.interval,
-            interval_unit=self.interval_unit,
-        ))
-        return res
-
     def clean(self):
         super(RepeatableJob, self).clean()
         self.clean_interval_unit()
         self.clean_result_ttl()
 
     def clean_interval_unit(self):
         if SCHEDULER_INTERVAL > self.interval_seconds():
@@ -365,22 +354,14 @@
     def interval_display(self):
         return '{} {}'.format(self.interval, self.get_interval_unit_display())
 
     def interval_seconds(self):
         kwargs = {self.interval_unit: self.interval, }
         return timedelta(**kwargs).total_seconds()
 
-    def _prevent_duplicate_runs(self):
-        """
-        Counts the number of repeats lapsed between scheduled time and now
-        and decrements that amount from the repeats remaining and updates the scheduled time to the next repeat.
-
-        self.repeat is None ==> Run forever.
-        """
-
     def _enqueue_args(self):
         res = super(RepeatableJob, self)._enqueue_args()
         res['meta']['interval'] = self.interval_seconds()
         return res
 
     def ready_for_schedule(self):
         if super(RepeatableJob, self).ready_for_schedule() is False:
@@ -407,31 +388,23 @@
     cron_string = models.CharField(
         _('cron string'), max_length=64,
         help_text=mark_safe(
             '''Define the schedule in a crontab like syntax.
             Times are in UTC. Use <a href="https://crontab.guru/">crontab.guru</a> to create a cron string.''')
     )
 
-    def to_dict(self) -> Dict:
-        res = super(CronJob, self).to_dict()
-        res['cron_string'] = self.cron_string
-        return res
-
     def clean(self):
         super(CronJob, self).clean()
         self.clean_cron_string()
 
     def clean_cron_string(self):
         try:
             croniter.croniter(self.cron_string)
         except ValueError as e:
-            raise ValidationError({
-                'cron_string': ValidationError(
-                    _(str(e)), code='invalid')
-            })
+            raise ValidationError({'cron_string': ValidationError(_(str(e)), code='invalid')})
 
     def _schedule_time(self):
         return tools.get_next_cron_time(self.cron_string)
 
     class Meta:
         verbose_name = _('Cron Job')
         verbose_name_plural = _('Cron Jobs')
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/queues.py` & `django_rq_scheduler-2023.6.1/scheduler/queues.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import List, Dict
 
-import fakeredis
 import redis
 from redis.sentinel import Sentinel
 
 from .rq_classes import JobExecution, DjangoQueue, DjangoWorker
 from .settings import get_config
 from .settings import logger
 
@@ -29,14 +28,15 @@
 
 
 def _get_redis_connection(config, use_strict_redis=False):
     """
     Returns a redis connection from a connection config
     """
     if get_config('FAKEREDIS'):
+        import fakeredis
         redis_cls = fakeredis.FakeRedis if use_strict_redis else fakeredis.FakeStrictRedis
     else:
         redis_cls = redis.StrictRedis if use_strict_redis else redis.Redis
     logger.debug(f'Getting connection for {config}')
     if 'URL' in config:
         if config.get('SSL') or config.get('URL').startswith('rediss://'):
             return redis_cls.from_url(
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/rq_classes.py` & `django_rq_scheduler-2023.6.1/scheduler/rq_classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,16 @@
     elif isinstance(v, str):
         return v
     else:
         raise ValueError('Unknown type %r' % type(v))
 
 
 def compact(lst: List[Any]) -> List[Any]:
-    """Excludes `None` values from a list-like object.
-
+    """Remove `None` values from an iterable object.
     :param lst: A list (or list-like) object
-
     :returns: The list without None values
     """
     return [item for item in lst if item is not None]
 
 
 class JobExecution(Job):
     def __eq__(self, other):
@@ -150,39 +148,37 @@
 
     def scheduler_pid(self) -> int:
         pid = self.connection.get(RQScheduler.get_locking_key(self.queues[0].name))
         return int(pid.decode()) if pid is not None else None
 
 
 class DjangoQueue(Queue):
+    REGISTRIES = dict(
+        finished='finished_job_registry',
+        failed='failed_job_registry',
+        scheduled='scheduled_job_registry',
+        started='started_job_registry',
+        deferred='deferred_job_registry',
+        canceled='canceled_job_registry',
+    )
     """
     A subclass of RQ's QUEUE that allows jobs to be stored temporarily to be
     enqueued later at the end of Django's request/response cycle.
     """
 
     def __init__(self, *args, **kwargs):
         kwargs['job_class'] = JobExecution
         super(DjangoQueue, self).__init__(*args, **kwargs)
 
     def get_registry(self, name: str) -> Union[None, BaseRegistry, 'DjangoQueue']:
         name = name.lower()
         if name == 'queued':
             return self
-        elif name == 'finished':
-            return self.finished_job_registry
-        elif name == 'failed':
-            return self.failed_job_registry
-        elif name == 'scheduled':
-            return self.scheduled_job_registry
-        elif name == 'started':
-            return self.started_job_registry
-        elif name == 'deferred':
-            return self.deferred_job_registry
-        elif name == 'canceled':
-            return self.canceled_job_registry
+        elif name in DjangoQueue.REGISTRIES:
+            return getattr(self, DjangoQueue.REGISTRIES[name])
         return None
 
     @property
     def finished_job_registry(self):
         return FinishedJobRegistry(self.name, self.connection)
 
     @property
@@ -221,14 +217,20 @@
         return compact([self.fetch_job(job_id) for job_id in job_ids])
 
     def clean_registries(self):
         self.started_job_registry.cleanup()
         self.failed_job_registry.cleanup()
         self.finished_job_registry.cleanup()
 
+    def remove_job_id(self, job_id: str):
+        self.connection.lrem(self.key, 0, job_id)
+
+    def last_job_id(self):
+        return self.connection.lindex(self.key, 0)
+
 
 class DjangoScheduler(RQScheduler):
     def __init__(self, *args, **kwargs):
         kwargs.setdefault('interval', settings.SCHEDULER_CONFIG['SCHEDULER_INTERVAL'])
         super(DjangoScheduler, self).__init__(*args, **kwargs)
 
     @staticmethod
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/settings.py` & `django_rq_scheduler-2023.6.1/scheduler/settings.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/confirm_action.html` & `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/confirm_action.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/job_detail.html` & `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/job_detail.html`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     <h2>Job {{ job.id }}
         {% if job.is_scheduled_job %}
             <small>
                 <a href="{{ job|scheduled_job }}">Link to scheduled job</a>
             </small>
         {% endif %}
     </h2>
-
 {% endblock %}
 
 {% block content %}
     <div id="content-main">
         <fieldset class="module aligned ">
             <div class="form-row">
                 <label>Queue:</label>
@@ -86,26 +85,25 @@
                         {% endfor %})
                     {% else %}
                         Unpickling Error
                     {% endif %}
                 </div>
             </div>
             <div class="form-row">
-
-                <label>Scheduler callable</label>
+                <label>Scheduler callable:</label>
                 <div class="data">{{ job | show_func_name }}</div>
             </div>
 
             <div class="form-row">
                 <label>Meta:</label>
                 <div class="data">
                     {% for k in job.meta %}
                         <div class="form-row">
                             <label>{{ k }}</label>
-                            <div class="data">{{ job.meta|get_item:k }}</div>
+                            <div class="data">{{ job.meta | get_item:k }}</div>
                         </div>
                     {% endfor %}
                 </div>
             </div>
 
 
             <div class="form-row">
```

#### html2text {}

```diff
@@ -23,20 +23,20 @@
 Status:
 {{ job.get_status }}
 Direct callable:
 {% if data_is_valid %} {{ job.func_name }}( {% if job.args %} {% for arg in
 job.args %} {{ arg|force_escape }}, {% endfor %} {% endif %} {% for key, value
 in job.kwargs.items %} {{ key }}={{ value|force_escape }}, {% endfor %}) {%
 else %} Unpickling Error {% endif %}
-Scheduler callable
+Scheduler callable:
 {{ job | show_func_name }}
 Meta:
 {% for k in job.meta %}
 {{ k }}
-{{ job.meta|get_item:k }}
+{{ job.meta | get_item:k }}
 {% endfor %}
 Depends On:
 {% if dependency_id %} {{_dependency_id_}} {% endif %}
 {% if exc_info %}
 Exception:
 {% if job.exc_info %}{{ job.exc_info|linebreaks }}{% endif %}
 {% endif %}
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/jobs-list.partial.html` & `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/jobs-list.partial.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/jobs.html` & `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/jobs.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/queue_workers.html` & `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/queue_workers.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/scheduler_base.html` & `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/scheduler_base.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/single_job_action.html` & `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/single_job_action.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/stats.html` & `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/stats.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/worker_details.html` & `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/worker_details.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/workers-list.partial.html` & `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/workers-list.partial.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/workers.html` & `django_rq_scheduler-2023.6.1/scheduler/templates/admin/scheduler/workers.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/templatetags/scheduler_tags.py` & `django_rq_scheduler-2023.6.1/scheduler/templatetags/scheduler_tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,39 @@
+from typing import Dict
+
 from django import template
+from django.utils.safestring import mark_safe
 
 from scheduler.rq_classes import JobExecution, DjangoQueue
 from scheduler.tools import get_scheduled_job
 
 register = template.Library()
 
 
 @register.filter
 def show_func_name(rq_job: JobExecution) -> str:
     try:
-        if rq_job.func_name == 'scheduler.tools.run_job':
+        res = rq_job.func_name
+        if res == 'scheduler.tools.run_job':
             job = get_scheduled_job(*rq_job.args)
-            return job.function_string()
-        return rq_job.func_name
+            res = job.function_string()
+        return mark_safe(res)
     except Exception as e:
         return repr(e)
 
 
 @register.filter
-def get_item(dictionary, key):
+def get_item(dictionary: Dict, key):
     return dictionary.get(key)
 
 
 @register.filter
 def scheduled_job(job: JobExecution):
-    scheduled_job = get_scheduled_job(*job.args)
-    return scheduled_job.get_absolute_url()
+    django_scheduled_job = get_scheduled_job(*job.args)
+    return django_scheduled_job.get_absolute_url()
 
 
 @register.filter
 def worker_scheduler_pid(worker):
     return worker.scheduler_pid()
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/tests/test_internals.py` & `django_rq_scheduler-2023.6.1/scheduler/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/tests/test_job_arg_models.py` & `django_rq_scheduler-2023.6.1/scheduler/tests/test_job_arg_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/tests/test_job_decorator.py` & `django_rq_scheduler-2023.6.1/scheduler/tests/test_job_decorator.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/tests/test_models.py` & `django_rq_scheduler-2023.6.1/scheduler/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/tests/test_redis_models.py` & `django_rq_scheduler-2023.6.1/scheduler/tests/test_redis_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/tests/test_settings.py` & `django_rq_scheduler-2023.6.1/scheduler/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/tests/test_views.py` & `django_rq_scheduler-2023.6.1/scheduler/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from django.test.client import Client
 from django.urls import reverse
 
 from scheduler.queues import get_queue
 from scheduler.tools import create_worker
 from . import test_settings  # noqa
 from .jobs import failing_job, long_job, test_job
-from .testtools import assert_message_in_response
+from .testtools import assert_message_in_response, job_factory, _get_job_from_scheduled_registry
+from ..models import ScheduledJob
 from ..rq_classes import JobExecution, ExecutionStatus
 
 
 class BaseTestCase(TestCase):
     def setUp(self):
         self.user = User.objects.create_superuser('user', password='pass')
         self.client = Client()
@@ -108,14 +109,35 @@
         self.assertEqual(200, res.status_code)
         tmp = queue.fetch_job(job_list[-1].id)
         self.assertEqual(tmp.get_status(), ExecutionStatus.QUEUED)
         self.assertIsNotNone(tmp.enqueued_at)
 
 
 class JobListActionViewsTest(BaseTestCase):
+    def test_job_list_action_delete_jobs__with_bad_next_url(self):
+        queue = get_queue('django_rq_scheduler_test')
+
+        # enqueue some jobs
+        job_ids = []
+        for _ in range(0, 3):
+            job = queue.enqueue(test_job)
+            job_ids.append(job.id)
+
+        # remove those jobs using view
+        res = self.client.post(
+            reverse('queue_actions', args=[queue.name, ]), {
+                'action': 'delete', 'job_ids': job_ids,
+                'next_url': 'bad_url',
+            }, follow=True)
+        assert_message_in_response(res, 'Bad followup URL')
+        # check if jobs are removed
+        self.assertEqual(200, res.status_code)
+        for job_id in job_ids:
+            self.assertFalse(JobExecution.exists(job_id, connection=queue.connection))
+            self.assertNotIn(job_id, queue.job_ids)
 
     def test_job_list_action_delete_jobs(self):
         queue = get_queue('django_rq_scheduler_test')
 
         # enqueue some jobs
         job_ids = []
         for _ in range(0, 3):
@@ -303,14 +325,24 @@
         self.assertIn('DeserializationError', res.content.decode())
 
         # Bad job-id should return 404
         url = reverse('job_details', args=['bad_job_id', ])
         res = self.client.get(url)
         self.assertEqual(400, res.status_code)
 
+    def test_scheduled_job_details(self):
+        """Job data is displayed properly"""
+        scheduled_job = job_factory(ScheduledJob, enabled=True)
+        job = _get_job_from_scheduled_registry(scheduled_job)
+
+        url = reverse('job_details', args=[job.id, ])
+        res = self.client.get(url, follow=True)
+        self.assertIn('job', res.context)
+        self.assertEqual(res.context['job'], job)
+
     def test_job_details_on_deleted_dependency(self):
         """Page doesn't crash even if job.dependency has been deleted"""
         queue = get_queue('default')
 
         job = queue.enqueue(test_job)
         second_job = queue.enqueue(test_job, depends_on=job)
         job.delete()
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/tests/test_worker.py` & `django_rq_scheduler-2023.6.1/scheduler/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/tests/testtools.py` & `django_rq_scheduler-2023.6.1/scheduler/tests/testtools.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/tools.py` & `django_rq_scheduler-2023.6.1/scheduler/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import importlib
 import os
 
 import croniter
 from django.apps import apps
+from django.templatetags.tz import utc
 from django.utils import timezone
 
 from scheduler.queues import get_queues, logger, get_queue
 from scheduler.rq_classes import DjangoWorker, MODEL_NAMES
 from scheduler.settings import get_config
 
 
@@ -15,20 +16,20 @@
     module = importlib.import_module('.'.join(path[:-1]))
     func = getattr(module, path[-1])
     if callable(func) is False:
         raise TypeError("'{}' is not callable".format(callable_str))
     return func
 
 
-def get_next_cron_time(cron_string):
+def get_next_cron_time(cron_string) -> timezone.datetime:
     """Calculate the next scheduled time by creating a crontab object
     with a cron string"""
     now = timezone.now()
     itr = croniter.croniter(cron_string, now)
-    return itr.get_next(timezone.datetime)
+    return utc(itr.get_next(timezone.datetime))
 
 
 def get_scheduled_job(task_model: str, task_id: int):
     if task_model not in MODEL_NAMES:
         raise ValueError(f'Job Model {task_model} does not exist, choices are {MODEL_NAMES}')
     model = apps.get_model(app_label='scheduler', model_name=task_model)
     task = model.objects.filter(id=task_id).first()
```

### Comparing `django_rq_scheduler-2023.6.0/scheduler/urls.py` & `django_rq_scheduler-2023.6.1/scheduler/urls.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.6.0/scheduler/views.py` & `django_rq_scheduler-2023.6.1/scheduler/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+from html import escape
 from math import ceil
 from typing import Tuple, Optional
 
 import redis
 from django.contrib import admin, messages
 from django.contrib.admin.views.decorators import staff_member_required
 from django.core.paginator import Paginator
 from django.http import JsonResponse
 from django.http.response import HttpResponseNotFound, Http404, HttpResponseBadRequest
 from django.shortcuts import redirect
 from django.shortcuts import render
-from django.urls import reverse
+from django.urls import reverse, resolve
 from django.views.decorators.cache import never_cache
 from redis.exceptions import ResponseError
 
 from .queues import get_all_workers, get_connection, logger, QueueNotFoundError
 from .queues import get_queue as get_queue_base
 from .rq_classes import JobExecution, DjangoWorker, DjangoQueue, InvalidJobOperation
 from .settings import SCHEDULER_CONFIG
@@ -69,15 +70,15 @@
                 queue.clean_registries()
 
             # Raw access to the first item from left of the redis list.
             # This might not be accurate since new job can be added from the left
             # with `at_front` parameters.
             # Ideally rq should supports Queue.oldest_job
 
-            last_job_id = connection.lindex(queue.key, 0)
+            last_job_id = queue.last_job_id()
             last_job = queue.fetch_job(last_job_id.decode('utf-8')) if last_job_id else None
             if last_job and last_job.enqueued_at:
                 oldest_job_timestamp = last_job.enqueued_at.strftime('%Y-%m-%d, %H:%M:%S')
             else:
                 oldest_job_timestamp = "-"
 
             # parse_class and connection_pool are not needed and not JSON serializable
@@ -229,15 +230,15 @@
 
 
 @never_cache
 @staff_member_required
 def job_detail(request, job_id: str):
     queue, job = _find_job(job_id)
     if job is None:
-        return HttpResponseBadRequest(f'Job {job_id} does not exist, maybe its TTL has passed')
+        return HttpResponseBadRequest(f'Job {escape(job_id)} does not exist, maybe its TTL has passed')
     try:
         job.func_name
         data_is_valid = True
     except Exception:
         data_is_valid = False
 
     try:
@@ -329,14 +330,19 @@
 
 
 @never_cache
 @staff_member_required
 def confirm_action(request, queue_name):
     queue = get_queue(queue_name)
     next_url = request.META.get('HTTP_REFERER') or reverse('queue_registry_jobs', args=[queue_name, 'queued'])
+    try:
+        resolve(next_url)
+    except Exception:
+        messages.warning(request, 'Bad followup URL')
+        next_url = reverse('queue_registry_jobs', args=[queue_name, 'queued'])
 
     if request.method == 'POST' and request.POST.get('action', False):
         # confirm action
         if request.POST.get('_selected_action', False):
             job_id_list = request.POST.getlist('_selected_action')
             context_data = {
                 **admin.site.each_context(request),
@@ -353,25 +359,30 @@
 
 
 @never_cache
 @staff_member_required
 def actions(request, queue_name):
     queue = get_queue(queue_name)
     next_url = request.POST.get('next_url') or reverse('queue_registry_jobs', args=[queue_name, 'queued'])
+    try:
+        resolve(next_url)
+    except Exception:
+        messages.warning(request, 'Bad followup URL')
+        next_url = reverse('queue_registry_jobs', args=[queue_name, 'queued'])
 
     action = request.POST.get('action', False)
     job_ids = request.POST.get('job_ids', False)
     if request.method != 'POST' or not action or not job_ids:
         return redirect(next_url)
     job_ids = request.POST.getlist('job_ids')
     if action == 'delete':
         for job_id in job_ids:
             job = JobExecution.fetch(job_id, connection=queue.connection)
             # Remove job id from queue and delete the actual job
-            queue.connection.lrem(queue.key, 0, job.id)
+            queue.remove_job_id(job.id)
             job.delete()
         messages.info(request, f'You have successfully deleted {len(job_ids)} jobs!')
     elif action == 'requeue':
         for job_id in job_ids:
             job = JobExecution.fetch(job_id, connection=queue.connection)
             job.requeue()
         messages.info(request, f'You have successfully re-queued {len(job_ids)}  jobs!')
@@ -394,15 +405,15 @@
 
 
 @never_cache
 @staff_member_required
 def job_action(request, job_id: str, action: str):
     queue, job = _find_job(job_id)
     if job is None:
-        return HttpResponseBadRequest(f'Job {job_id} does not exist, maybe its TTL has passed')
+        return HttpResponseBadRequest(f'Job {escape(job_id)} does not exist, maybe its TTL has passed')
     if action not in SUPPORTED_JOB_ACTIONS:
         return HttpResponseNotFound()
 
     if request.method != 'POST':
         context_data = {
             **admin.site.each_context(request),
             'job': job,
@@ -414,15 +425,15 @@
     try:
         if action == 'requeue':
             job.requeue()
             messages.info(request, f'You have successfully re-queued {job.id}')
             return redirect('job_details', job_id)
         elif action == 'delete':
             # Remove job id from queue and delete the actual job
-            queue.connection.lrem(queue.key, 0, job.id)
+            queue.remove_job_id(job.id)
             job.delete()
             messages.info(request, 'You have successfully deleted %s' % job.id)
             return redirect('queue_registry_jobs', queue.name, 'queued')
         elif action == 'enqueue':
             job.delete(remove_from_queue=False)
             queue._enqueue_job(job)
             messages.info(request, 'You have successfully enqueued %s' % job.id)
```

### Comparing `django_rq_scheduler-2023.6.0/PKG-INFO` & `django_rq_scheduler-2023.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: django-rq-scheduler
-Version: 2023.6.0
+Version: 2023.6.1
 Summary: An async job scheduler for django using redis
 Home-page: https://github.com/dsoftwareinc/django-rq-scheduler
 License: MIT
 Keywords: redis,django,background-jobs,job-queue,task-queue,redis-queue,scheduled-jobs
 Author: Daniel Moran
-Author-email: daniel.maruani@gmail.com
+Author-email: daniel@moransoftware.ca
 Maintainer: Daniel Moran
-Maintainer-email: daniel.maruani@gmail.com
+Maintainer-email: daniel@moransoftware.ca
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: yaml
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: croniter (>=1.3,<2.0)
 Requires-Dist: django (>=3.2)
-Requires-Dist: django-model-utils (>=4.3,<5.0)
-Requires-Dist: rq (>=1.14,<2.0)
+Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "yaml"
+Requires-Dist: rq (>=1.15,<2.0)
 Project-URL: Bug Tracker, https://github.com/dsoftwareinc/django-rq-scheduler/issues
 Project-URL: Documentation, https://django-rq-scheduler.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/cunla
 Description-Content-Type: text/markdown
 
 Django RQ Scheduler
 ===================
@@ -60,12 +59,8 @@
 # Sponsor
 
 django-rq-scheduler is developed for free.
 
 You can support this project by becoming a sponsor using [this link](https://github.com/sponsors/cunla).
 
 
-## Security contact information
 
-To report a security vulnerability, please use the
-[Tidelift security contact](https://tidelift.com/security).
-Tidelift will coordinate the fix and disclosure.
```

