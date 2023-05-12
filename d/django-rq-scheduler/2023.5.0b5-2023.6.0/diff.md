# Comparing `tmp/django_rq_scheduler-2023.5.0b5.tar.gz` & `tmp/django_rq_scheduler-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rq_scheduler-2023.5.0b5.tar", max compression
+gzip compressed data, was "django_rq_scheduler-2023.6.0.tar", max compression
```

## Comparing `django_rq_scheduler-2023.5.0b5.tar` & `django_rq_scheduler-2023.6.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
--rw-r--r--   0        0        0     1107 2023-04-18 20:24:54.707516 django_rq_scheduler-2023.5.0b5/LICENSE
--rw-r--r--   0        0        0     1558 2023-04-18 20:24:54.707516 django_rq_scheduler-2023.5.0b5/README.md
--rw-r--r--   0        0        0     1741 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/pyproject.toml
--rw-r--r--   0        0        0      134 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/__init__.py
--rw-r--r--   0        0        0      147 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/admin/__init__.py
--rw-r--r--   0        0        0     5661 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/admin/job.py
--rw-r--r--   0        0        0     1641 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/admin/redis_models.py
--rw-r--r--   0        0        0      281 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/apps.py
--rw-r--r--   0        0        0     1207 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/decorators.py
--rw-r--r--   0        0        0        0 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/commands/__init__.py
--rw-r--r--   0        0        0     1189 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/commands/delete_failed_executions.py
--rw-r--r--   0        0        0     1908 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/commands/export.py
--rw-r--r--   0        0        0     3417 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/commands/import.py
--rw-r--r--   0        0        0     3602 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/commands/rqstats.py
--rw-r--r--   0        0        0     3090 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/commands/rqworker.py
--rw-r--r--   0        0        0     1374 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/management/commands/run_job.py
--rw-r--r--   0        0        0     7162 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
--rw-r--r--   0        0        0      898 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
--rw-r--r--   0        0        0     4196 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0003_auto_20220329_2107.py
--rw-r--r--   0        0        0      791 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0      896 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
--rw-r--r--   0        0        0      728 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0006_auto_20230118_1640.py
--rw-r--r--   0        0        0     1302 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0007_add_result_ttl.py
--rw-r--r--   0        0        0     1982 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
--rw-r--r--   0        0        0     1362 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
--rw-r--r--   0        0        0      661 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0010_queue.py
--rw-r--r--   0        0        0     7643 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
--rw-r--r--   0        0        0      935 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py
--rw-r--r--   0        0        0        0 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/migrations/__init__.py
--rw-r--r--   0        0        0      187 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/models/__init__.py
--rw-r--r--   0        0        0     3102 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/models/args.py
--rw-r--r--   0        0        0      364 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/models/queue.py
--rw-r--r--   0        0        0    15140 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/models/scheduled_job.py
--rw-r--r--   0        0        0      366 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/models/worker.py
--rw-r--r--   0        0        0        0 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/py.typed
--rw-r--r--   0        0        0     4858 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/queues.py
--rw-r--r--   0        0        0     7780 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/rq_classes.py
--rw-r--r--   0        0        0      932 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/settings.py
--rw-r--r--   0        0        0      163 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/change_form.html
--rw-r--r--   0        0        0      127 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/change_list.html
--rw-r--r--   0        0        0     1559 2023-04-18 20:24:54.711516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/confirm_action.html
--rw-r--r--   0        0        0     1282 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/delete_job.html
--rw-r--r--   0        0        0     7124 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/job_detail.html
--rw-r--r--   0        0        0     2697 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/jobs-list.partial.html
--rw-r--r--   0        0        0     6297 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/jobs.html
--rw-r--r--   0        0        0     1055 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/queue_workers.html
--rw-r--r--   0        0        0      568 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/scheduler_base.html
--rw-r--r--   0        0        0     4120 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/stats.html
--rw-r--r--   0        0        0     3032 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/worker_details.html
--rw-r--r--   0        0        0     1875 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/workers-list.partial.html
--rw-r--r--   0        0        0      935 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/workers.html
--rw-r--r--   0        0        0        0 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templatetags/__init__.py
--rw-r--r--   0        0        0     1396 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/templatetags/scheduler_tags.py
--rw-r--r--   0        0        0        0 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/__init__.py
--rw-r--r--   0        0        0      535 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/jobs.py
--rw-r--r--   0        0        0      668 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_internals.py
--rw-r--r--   0        0        0     5887 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_job_arg_models.py
--rw-r--r--   0        0        0     2349 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_job_decorator.py
--rw-r--r--   0        0        0     4816 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_mgmt_cmds.py
--rw-r--r--   0        0        0    27529 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_models.py
--rw-r--r--   0        0        0      807 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_redis_models.py
--rw-r--r--   0        0        0     2211 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_settings.py
--rw-r--r--   0        0        0    14933 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_views.py
--rw-r--r--   0        0        0     1577 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/test_worker.py
--rw-r--r--   0        0        0     3311 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tests/testtools.py
--rw-r--r--   0        0        0     2572 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/tools.py
--rw-r--r--   0        0        0     1736 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/urls.py
--rw-r--r--   0        0        0    16009 2023-04-18 20:24:54.715516 django_rq_scheduler-2023.5.0b5/scheduler/views.py
--rw-r--r--   0        0        0     3306 1970-01-01 00:00:00.000000 django_rq_scheduler-2023.5.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1107 2023-05-12 14:29:26.090261 django_rq_scheduler-2023.6.0/LICENSE
+-rw-r--r--   0        0        0     1558 2023-05-12 14:29:26.090261 django_rq_scheduler-2023.6.0/README.md
+-rw-r--r--   0        0        0     1769 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/__init__.py
+-rw-r--r--   0        0        0      147 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/admin/__init__.py
+-rw-r--r--   0        0        0     5661 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/admin/job.py
+-rw-r--r--   0        0        0     1641 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/admin/redis_models.py
+-rw-r--r--   0        0        0      281 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/apps.py
+-rw-r--r--   0        0        0     1214 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/decorators.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/commands/__init__.py
+-rw-r--r--   0        0        0     1189 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/commands/delete_failed_executions.py
+-rw-r--r--   0        0        0     1908 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/commands/export.py
+-rw-r--r--   0        0        0     3417 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/commands/import.py
+-rw-r--r--   0        0        0     3602 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/commands/rqstats.py
+-rw-r--r--   0        0        0     3176 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/commands/rqworker.py
+-rw-r--r--   0        0        0     1374 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/management/commands/run_job.py
+-rw-r--r--   0        0        0     7162 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py
+-rw-r--r--   0        0        0      898 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py
+-rw-r--r--   0        0        0     4196 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0003_auto_20220329_2107.py
+-rw-r--r--   0        0        0      791 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0      896 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py
+-rw-r--r--   0        0        0      728 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0006_auto_20230118_1640.py
+-rw-r--r--   0        0        0     1302 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0007_add_result_ttl.py
+-rw-r--r--   0        0        0     1982 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py
+-rw-r--r--   0        0        0     1362 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py
+-rw-r--r--   0        0        0      661 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0010_queue.py
+-rw-r--r--   0        0        0     7643 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py
+-rw-r--r--   0        0        0      934 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py
+-rw-r--r--   0        0        0     1320 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/0013_alter_cronjob_queue_alter_repeatablejob_queue_and_more.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/migrations/__init__.py
+-rw-r--r--   0        0        0      187 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/models/__init__.py
+-rw-r--r--   0        0        0     3102 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/models/args.py
+-rw-r--r--   0        0        0      364 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/models/queue.py
+-rw-r--r--   0        0        0    15332 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/models/scheduled_job.py
+-rw-r--r--   0        0        0      366 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/models/worker.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/py.typed
+-rw-r--r--   0        0        0     5048 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/queues.py
+-rw-r--r--   0        0        0     9041 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/rq_classes.py
+-rw-r--r--   0        0        0     1073 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/settings.py
+-rw-r--r--   0        0        0      163 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/change_form.html
+-rw-r--r--   0        0        0      127 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/change_list.html
+-rw-r--r--   0        0        0     1595 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/confirm_action.html
+-rw-r--r--   0        0        0     7822 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/job_detail.html
+-rw-r--r--   0        0        0     2697 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/jobs-list.partial.html
+-rw-r--r--   0        0        0     6360 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/jobs.html
+-rw-r--r--   0        0        0      915 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/queue_workers.html
+-rw-r--r--   0        0        0      568 2023-05-12 14:29:26.098261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/scheduler_base.html
+-rw-r--r--   0        0        0     1324 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/single_job_action.html
+-rw-r--r--   0        0        0     4224 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/stats.html
+-rw-r--r--   0        0        0     3032 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/worker_details.html
+-rw-r--r--   0        0        0     1879 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/workers-list.partial.html
+-rw-r--r--   0        0        0      935 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/workers.html
+-rw-r--r--   0        0        0        0 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/templatetags/__init__.py
+-rw-r--r--   0        0        0     1546 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/templatetags/scheduler_tags.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/__init__.py
+-rw-r--r--   0        0        0      502 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/jobs.py
+-rw-r--r--   0        0        0      668 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_internals.py
+-rw-r--r--   0        0        0     5887 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_job_arg_models.py
+-rw-r--r--   0        0        0     2349 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_job_decorator.py
+-rw-r--r--   0        0        0     4920 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_mgmt_cmds.py
+-rw-r--r--   0        0        0    27724 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_models.py
+-rw-r--r--   0        0        0      807 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_redis_models.py
+-rw-r--r--   0        0        0     2317 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_settings.py
+-rw-r--r--   0        0        0    18728 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_views.py
+-rw-r--r--   0        0        0     1577 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/test_worker.py
+-rw-r--r--   0        0        0     3399 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tests/testtools.py
+-rw-r--r--   0        0        0     2677 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/tools.py
+-rw-r--r--   0        0        0     1121 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/urls.py
+-rw-r--r--   0        0        0    15854 2023-05-12 14:29:26.102261 django_rq_scheduler-2023.6.0/scheduler/views.py
+-rw-r--r--   0        0        0     3304 1970-01-01 00:00:00.000000 django_rq_scheduler-2023.6.0/PKG-INFO
```

### Comparing `django_rq_scheduler-2023.5.0b5/LICENSE` & `django_rq_scheduler-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/README.md` & `django_rq_scheduler-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/pyproject.toml` & `django_rq_scheduler-2023.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-rq-scheduler"
 packages = [
     { include = "scheduler" },
 ]
-version = "2023.5.0b5"
+version = "2023.6.0"
 description = "An async job scheduler for django using redis"
 readme = "README.md"
 keywords = ["redis", "django", "background-jobs", "job-queue", "task-queue", "redis-queue", "scheduled-jobs"]
 authors = [
     "Daniel Moran <daniel.maruani@gmail.com>",
 ]
 maintainers = [
@@ -44,20 +44,20 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 django = ">=3.2"
 django-model-utils = "^4.3"
 croniter = "^1.3"
 click = "^8.1"
-rq = "^1.13"
+rq = "^1.14"
 
 [tool.poetry.dev-dependencies]
 poetry = "^1.4"
 coverage = "^7"
-fakeredis = "^2.10"
+fakeredis = { version = "^2.12", extras=['lua'] }
 Flake8-pyproject = "^1.2"
 
 [tool.flake8]
 max-line-length = 119
 exclude = [
     'scheduler/migrations',
 ]
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/admin/job.py` & `django_rq_scheduler-2023.6.0/scheduler/admin/job.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/admin/redis_models.py` & `django_rq_scheduler-2023.6.0/scheduler/admin/redis_models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from scheduler import settings
 from django.contrib import admin
 
+from scheduler import settings
 from scheduler import views
 from scheduler.models import Queue
 from scheduler.models.worker import Worker
 
 QUEUES = [(key, key) for key in settings.QUEUES.keys()]
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/decorators.py` & `django_rq_scheduler-2023.6.0/scheduler/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-
-from rq.decorators import job as _rq_job
-
 from scheduler import settings
 from .queues import get_queue, QueueNotFoundError
+from .rq_classes import rq_job_decorator
 
 
 def job(*args, **kwargs):
     """
     The same as rq package's job decorator, but it automatically works out
     the ``connection`` argument from SCHEDULER_QUEUES.
 
@@ -35,11 +33,11 @@
             raise QueueNotFoundError(f'Queue {queue} does not exist')
 
     config = settings.SCHEDULER_CONFIG
 
     kwargs.setdefault('result_ttl', config.get('DEFAULT_RESULT_TTL'))
     kwargs.setdefault('timeout', config.get('DEFAULT_TIMEOUT'))
 
-    decorator = _rq_job(queue, *args, **kwargs)
+    decorator = rq_job_decorator(queue, *args, **kwargs)
     if func:
         return decorator(func)
     return decorator
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/management/commands/delete_failed_executions.py` & `django_rq_scheduler-2023.6.0/scheduler/management/commands/delete_failed_executions.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/management/commands/export.py` & `django_rq_scheduler-2023.6.0/scheduler/management/commands/export.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/management/commands/import.py` & `django_rq_scheduler-2023.6.0/scheduler/management/commands/import.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/management/commands/rqstats.py` & `django_rq_scheduler-2023.6.0/scheduler/management/commands/rqstats.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/management/commands/rqworker.py` & `django_rq_scheduler-2023.6.0/scheduler/management/commands/rqworker.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import sys
 
 import click
 from django.core.management.base import BaseCommand
 from django.db import connections
 from redis.exceptions import ConnectionError
-from rq import use_connection
 from rq.logutils import setup_loghandlers
 
 from scheduler.tools import create_worker
 
 VERBOSITY_TO_LOG_LEVEL = {
     0: logging.CRITICAL,
     1: logging.WARNING,
@@ -42,14 +41,16 @@
                             default=False, help='Run worker in burst mode')
         parser.add_argument('--name', action='store', dest='name',
                             default=None, help='Name of the worker')
         parser.add_argument('--worker-ttl', action='store', type=int, dest='worker_ttl', default=420,
                             help='Default worker timeout to be used')
         parser.add_argument('--max-jobs', action='store', default=None, dest='max_jobs', type=int,
                             help='Maximum number of jobs to execute before terminating worker')
+        parser.add_argument('--fork-job-execution', action='store', default=True, dest='fork_job_execution', type=bool,
+                            help='Fork job execution to another process')
         parser.add_argument(
             'queues', nargs='*', type=str,
             help='The queues to work on, separated by space, all queues should be using the same redis')
 
     def handle(self, **options):
         queues = options.get('queues', [])
         if not queues:
@@ -63,19 +64,19 @@
         # Verbosity is defined by default in BaseCommand for all commands
         verbosity = options.get('verbosity', 1)
         log_level = VERBOSITY_TO_LOG_LEVEL.get(verbosity, logging.INFO)
         setup_loghandlers(log_level)
 
         try:
             # Instantiate a worker
-            w = create_worker(*queues, name=options['name'], default_worker_ttl=options['worker_ttl'], )
-
-            # Call use_connection to push the redis connection into LocalStack
-            # without this, jobs using RQ's get_current_job() will fail
-            use_connection(w.connection)
+            w = create_worker(
+                *queues,
+                name=options['name'],
+                default_worker_ttl=options['worker_ttl'],
+                fork_job_execution=options['fork_job_execution'], )
 
             # Close any opened DB connection before any fork
             reset_db_connections()
 
             w.work(burst=options.get('burst', False),
                    logging_level=log_level,
                    max_jobs=options['max_jobs'], )
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/management/commands/run_job.py` & `django_rq_scheduler-2023.6.0/scheduler/management/commands/run_job.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py` & `django_rq_scheduler-2023.6.0/scheduler/migrations/0001_initial_squashed_0005_added_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py` & `django_rq_scheduler-2023.6.0/scheduler/migrations/0002_alter_cronjob_id_alter_repeatablejob_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0003_auto_20220329_2107.py` & `django_rq_scheduler-2023.6.0/scheduler/migrations/0003_auto_20220329_2107.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py` & `django_rq_scheduler-2023.6.0/scheduler/migrations/0004_cronjob_at_front_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py` & `django_rq_scheduler-2023.6.0/scheduler/migrations/0005_alter_cronjob_at_front_alter_repeatablejob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0006_auto_20230118_1640.py` & `django_rq_scheduler-2023.6.0/scheduler/migrations/0006_auto_20230118_1640.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0007_add_result_ttl.py` & `django_rq_scheduler-2023.6.0/scheduler/migrations/0007_add_result_ttl.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py` & `django_rq_scheduler-2023.6.0/scheduler/migrations/0008_rename_str_val_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py` & `django_rq_scheduler-2023.6.0/scheduler/migrations/0009_alter_jobarg_arg_type_alter_jobarg_val_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0010_queue.py` & `django_rq_scheduler-2023.6.0/scheduler/migrations/0010_queue.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py` & `django_rq_scheduler-2023.6.0/scheduler/migrations/0011_worker_alter_queue_options_alter_cronjob_at_front_and_more.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py` & `django_rq_scheduler-2023.6.0/scheduler/migrations/0012_alter_cronjob_name_alter_repeatablejob_name_and_more.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.2 on 2023-04-18 19:08
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ('scheduler', '0011_worker_alter_queue_options_alter_cronjob_at_front_and_more'),
     ]
 
     operations = [
         migrations.AlterField(
             model_name='cronjob',
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/models/args.py` & `django_rq_scheduler-2023.6.0/scheduler/models/args.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/models/scheduled_job.py` & `django_rq_scheduler-2023.6.0/scheduler/models/scheduled_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import croniter
 from django.apps import apps
 from django.contrib import admin
 from django.contrib.contenttypes.fields import GenericRelation
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.templatetags.tz import utc
+from django.urls import reverse
 from django.utils import timezone
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy as _
 from model_utils import Choices
 from model_utils.models import TimeStampedModel
 
 from scheduler import settings
@@ -47,15 +48,15 @@
     callable_kwargs = GenericRelation(JobKwarg, related_query_name='kwargs')
     enabled = models.BooleanField(
         _('enabled'), default=True,
         help_text=_('Should job be scheduled? This field is useful to keep '
                     'past jobs that should no longer be scheduled'),
     )
     queue = models.CharField(
-        _('queue'), max_length=16, choices=QUEUES,
+        _('queue'), max_length=255, choices=QUEUES,
         help_text=_('Queue name'), )
     job_id = models.CharField(
         _('job id'), max_length=128, editable=False, blank=True, null=True,
         help_text=_('Current job_id on queue'))
     repeat = models.PositiveIntegerField(
         _('repeat'), blank=True, null=True,
         help_text=_('Number of times to run the job. Leaving this blank means it will run forever.'), )
@@ -227,14 +228,18 @@
             queue=self.queue,
             repeat=self.repeat,
             at_front=self.at_front,
             timeout=self.timeout,
             result_ttl=self.result_ttl,
         )
 
+    def get_absolute_url(self):
+        model = self._meta.model.__name__.lower()
+        return reverse(f'admin:scheduler_{model}_change', args=[self.id, ])
+
     def __str__(self):
         func = self.function_string()
         return f'{self.JOB_TYPE}[{self.name}={func}]'
 
     def save(self, **kwargs):
         schedule_job = kwargs.pop('schedule_job', True)
         super(BaseJob, self).save(**kwargs)
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/queues.py` & `django_rq_scheduler-2023.6.0/scheduler/queues.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,58 @@
 from typing import List, Dict
 
+import fakeredis
 import redis
 from redis.sentinel import Sentinel
 
 from .rq_classes import JobExecution, DjangoQueue, DjangoWorker
+from .settings import get_config
 from .settings import logger
 
+_CONNECTION_PARAMS = {
+    'URL',
+    'DB',
+    'USE_REDIS_CACHE',
+    'UNIX_SOCKET_PATH',
+    'HOST',
+    'PORT',
+    'PASSWORD',
+    'SENTINELS',
+    'MASTER_NAME',
+    'SOCKET_TIMEOUT',
+    'SSL',
+    'CONNECTION_KWARGS',
+}
+
+
+class QueueNotFoundError(Exception):
+    pass
+
 
-def _get_redis_connection(config, use_strict_redis=False, fake=False):
+def _get_redis_connection(config, use_strict_redis=False):
     """
     Returns a redis connection from a connection config
     """
-    redis_cls = redis.StrictRedis if use_strict_redis else redis.Redis
+    if get_config('FAKEREDIS'):
+        redis_cls = fakeredis.FakeRedis if use_strict_redis else fakeredis.FakeStrictRedis
+    else:
+        redis_cls = redis.StrictRedis if use_strict_redis else redis.Redis
     logger.debug(f'Getting connection for {config}')
     if 'URL' in config:
         if config.get('SSL') or config.get('URL').startswith('rediss://'):
             return redis_cls.from_url(
                 config['URL'],
                 db=config.get('DB'),
                 ssl_cert_reqs=config.get('SSL_CERT_REQS', 'required'),
             )
         else:
             return redis_cls.from_url(
                 config['URL'],
                 db=config.get('DB'),
             )
-
     if 'UNIX_SOCKET_PATH' in config:
         return redis_cls(unix_socket_path=config['UNIX_SOCKET_PATH'], db=config['DB'])
 
     if 'SENTINELS' in config:
         connection_kwargs = {
             'db': config.get('DB'),
             'password': config.get('PASSWORD'),
@@ -52,98 +75,74 @@
         password=config.get('PASSWORD'),
         ssl=config.get('SSL', False),
         ssl_cert_reqs=config.get('SSL_CERT_REQS', 'required'),
         **config.get('REDIS_CLIENT_KWARGS', {})
     )
 
 
-class QueueNotFoundError(Exception):
-    pass
-
-
-def get_connection(name='default', use_strict_redis=False):
+def get_connection(queue_settings, use_strict_redis=False):
     """Returns a Redis connection to use based on parameters in SCHEDULER_QUEUES
     """
-    from .settings import QUEUES
-
-    if name not in QUEUES:
-        raise QueueNotFoundError(f'Queue {name} not found, queues={QUEUES.keys()}')
-
-    return _get_redis_connection(QUEUES[name], use_strict_redis)
+    return _get_redis_connection(queue_settings, use_strict_redis)
 
 
 def get_queue(
         name='default',
         default_timeout=None, is_async=None,
         autocommit=None,
         connection=None,
         **kwargs
 ) -> DjangoQueue:
     """Returns an DjangoQueue using parameters defined in `SCHEDULER_QUEUES`
     """
     from .settings import QUEUES
-
+    if name not in QUEUES:
+        raise QueueNotFoundError(f'Queue {name} not found, queues={QUEUES.keys()}')
+    queue_settings = QUEUES[name]
     if is_async is None:
-        is_async = QUEUES[name].get('ASYNC', True)
+        is_async = queue_settings.get('ASYNC', True)
 
     if default_timeout is None:
-        default_timeout = QUEUES[name].get('DEFAULT_TIMEOUT')
+        default_timeout = queue_settings.get('DEFAULT_TIMEOUT')
     if connection is None:
-        connection = get_connection(name)
+        connection = get_connection(queue_settings)
     return DjangoQueue(
         name,
         default_timeout=default_timeout,
         connection=connection,
         is_async=is_async,
         autocommit=autocommit,
         **kwargs
     )
 
 
 def get_all_workers():
     from .settings import QUEUES
     workers = set()
     for queue_name in QUEUES:
-        connection = get_connection(queue_name)
+        connection = get_connection(QUEUES[queue_name])
         try:
             curr_workers = set(DjangoWorker.all(connection=connection))
             workers.update(curr_workers)
         except redis.ConnectionError as e:
             logger.error(f'Could not connect for queue {queue_name}: {e}')
     return workers
 
 
-_CONNECTION_PARAMS = {
-    'URL',
-    'DB',
-    'USE_REDIS_CACHE',
-    'UNIX_SOCKET_PATH',
-    'HOST',
-    'PORT',
-    'PASSWORD',
-    'SENTINELS',
-    'MASTER_NAME',
-    'SOCKET_TIMEOUT',
-    'SSL',
-    'CONNECTION_KWARGS',
-}
-
-
 def _queues_share_connection_params(q1_params: Dict, q2_params: Dict):
     """Check that both queues share the same connection parameters
     """
     return all(
         ((p not in q1_params and p not in q2_params)
          or (q1_params.get(p, None) == q2_params.get(p, None)))
         for p in _CONNECTION_PARAMS)
 
 
 def get_queues(*queue_names, **kwargs) -> List[DjangoQueue]:
-    """
-    Return queue instances from specified queue names.
+    """Return queue instances from specified queue names.
     All instances must use the same Redis connection.
     """
     from .settings import QUEUES
 
     kwargs['job_class'] = JobExecution
     queue_params = QUEUES[queue_names[0]]
     queues = [get_queue(queue_names[0], **kwargs)]
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/rq_classes.py` & `django_rq_scheduler-2023.6.0/scheduler/rq_classes.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,26 +2,34 @@
 
 import django
 from django.apps import apps
 from redis import Redis
 from redis.client import Pipeline
 from rq import Worker
 from rq.command import send_stop_job_command
+from rq.decorators import job
+from rq.exceptions import InvalidJobOperation
 from rq.job import Job, JobStatus
+from rq.job import get_current_job  # noqa
 from rq.queue import Queue, logger
 from rq.registry import (
     DeferredJobRegistry, FailedJobRegistry, FinishedJobRegistry,
-    ScheduledJobRegistry, StartedJobRegistry, CanceledJobRegistry,
+    ScheduledJobRegistry, StartedJobRegistry, CanceledJobRegistry, BaseRegistry,
 )
 from rq.scheduler import RQScheduler
+from rq.worker import WorkerStatus
 
 from scheduler import settings
 
 MODEL_NAMES = ['ScheduledJob', 'RepeatableJob', 'CronJob']
 
+rq_job_decorator = job
+ExecutionStatus = JobStatus
+InvalidJobOperation = InvalidJobOperation
+
 
 def as_text(v: Union[bytes, str]) -> Optional[str]:
     """Converts a bytes value to a string using `utf-8`.
 
     :param v: The value (bytes or string)
     :raises: ValueError: If the value is not bytes or string
     :returns: Either the decoded string or None
@@ -42,17 +50,14 @@
     :param lst: A list (or list-like) object
 
     :returns: The list without None values
     """
     return [item for item in lst if item is not None]
 
 
-ExecutionStatus = JobStatus
-
-
 class JobExecution(Job):
     def __eq__(self, other):
         return isinstance(other, Job) and self.id == other.id
 
     @property
     def is_scheduled_job(self):
         return self.meta.get('scheduled_job_id', None) is not None
@@ -63,14 +68,15 @@
 
     def stop_execution(self, connection: Redis):
         send_stop_job_command(connection, self.id)
 
 
 class DjangoWorker(Worker):
     def __init__(self, *args, **kwargs):
+        self.fork_job_execution = kwargs.pop('fork_job_execution', True)
         kwargs['job_class'] = JobExecution
         kwargs['queue_class'] = DjangoQueue
         super(DjangoWorker, self).__init__(*args, **kwargs)
 
     def __eq__(self, other):
         return (isinstance(other, Worker)
                 and self.key == other.key
@@ -115,14 +121,22 @@
             if burst:
                 self.scheduler.enqueue_scheduled_jobs()
                 self.scheduler.release_locks()
             else:
                 proc = self.scheduler.start()
                 self._set_property('scheduler_pid', proc.pid)
 
+    def execute_job(self, job: 'Job', queue: 'Queue'):
+        if self.fork_job_execution:
+            super(DjangoWorker, self).execute_job(job, queue)
+        else:
+            self.set_state(WorkerStatus.BUSY)
+            self.perform_job(job, queue)
+            self.set_state(WorkerStatus.IDLE)
+
     def work(self, **kwargs) -> bool:
         kwargs.setdefault('with_scheduler', True)
         return super(DjangoWorker, self).work(**kwargs)
 
     def _set_property(self, prop_name: str, val, pipeline: Optional[Pipeline] = None):
         connection = pipeline if pipeline is not None else self.connection
         if val is None:
@@ -145,14 +159,32 @@
     enqueued later at the end of Django's request/response cycle.
     """
 
     def __init__(self, *args, **kwargs):
         kwargs['job_class'] = JobExecution
         super(DjangoQueue, self).__init__(*args, **kwargs)
 
+    def get_registry(self, name: str) -> Union[None, BaseRegistry, 'DjangoQueue']:
+        name = name.lower()
+        if name == 'queued':
+            return self
+        elif name == 'finished':
+            return self.finished_job_registry
+        elif name == 'failed':
+            return self.failed_job_registry
+        elif name == 'scheduled':
+            return self.scheduled_job_registry
+        elif name == 'started':
+            return self.started_job_registry
+        elif name == 'deferred':
+            return self.deferred_job_registry
+        elif name == 'canceled':
+            return self.canceled_job_registry
+        return None
+
     @property
     def finished_job_registry(self):
         return FinishedJobRegistry(self.name, self.connection)
 
     @property
     def started_job_registry(self):
         return StartedJobRegistry(self.name, self.connection, job_class=JobExecution, )
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/settings.py` & `django_rq_scheduler-2023.6.0/scheduler/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 
 logger = logging.getLogger("scheduler")
 
-QUEUES = None
-SCHEDULER_CONFIG = None
+QUEUES = dict()
+SCHEDULER_CONFIG = dict()
 
 
 def conf_settings():
     global QUEUES
     global SCHEDULER_CONFIG
 
     QUEUES = getattr(settings, 'SCHEDULER_QUEUES', None)
@@ -21,13 +21,18 @@
         raise ImproperlyConfigured("You have to define SCHEDULER_QUEUES in settings.py")
 
     SCHEDULER_CONFIG = {
         'EXECUTIONS_IN_PAGE': 20,
         'DEFAULT_RESULT_TTL': 600,  # 10 minutes
         'DEFAULT_TIMEOUT': 300,  # 5 minutes
         'SCHEDULER_INTERVAL': 10,  # 10 seconds
+        'FAKEREDIS': False,  # For testing purposes
     }
     user_settings = getattr(settings, 'SCHEDULER_CONFIG', {})
     SCHEDULER_CONFIG.update(user_settings)
 
 
 conf_settings()
+
+
+def get_config(key: str, default=None):
+    return SCHEDULER_CONFIG.get(key, None)
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/confirm_action.html` & `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/confirm_action.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 {% extends "admin/scheduler/scheduler_base.html" %}
 {% load scheduler_tags %}
 
 {% block breadcrumbs %}
     <div class="breadcrumbs">
         <a href="{% url 'admin:index' %}">Home</a> &rsaquo;
         <a href="{% url 'queues_home' %}">Queues</a> &rsaquo;
-        <a href="{% url 'queue_jobs' queue.name %}">{{ queue.name }}</a> &rsaquo;
+        <a href="{% url 'queue_registry_jobs' queue.name 'queued' %}">{{ queue.name }}</a> &rsaquo;
         {{ action|capfirst }}
     </div>
 {% endblock %}
 
 {% block content_title %}<h1>Are you sure?</h1>{% endblock %}
 
 {% block content %}
     <div id="content-main">
         <p>
             Are you sure you want to <b>{{ action|capfirst }}</b> the {{ total_jobs }} selected jobs from
-            <a href="{% url 'queue_jobs' queue.name %}" target="_blank">{{ queue.name }}</a>
+            <a href="{% url 'queue_registry_jobs' queue.name 'queued' %}" target="_blank">{{ queue.name }}</a>
             ? These jobs are selected:
         </p>
         <ul>
             {% for job in jobs %}
                 <li>
                     <a href="{% url 'job_details' job.id %}" target="_blank">{{ job.id }}</a>
                     {{ job | show_func_name }}
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/job_detail.html` & `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/job_detail.html`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,39 @@
 
 {% block title %}Job {{ job.id }} {{ block.super }}{% endblock %}
 
 {% block breadcrumbs %}
     <div class="breadcrumbs">
         <a href="{% url 'admin:index' %}">Home</a> &rsaquo;
         <a href="{% url 'queues_home' %}">Queues</a> &rsaquo;
-        <a href="{% url 'queue_jobs' queue.name %}">{{ queue.name }}</a> &rsaquo;
+        <a href="{% url 'queue_registry_jobs' queue.name 'queued' %}">{{ queue.name }}</a> &rsaquo;
         <a href="{% url 'job_details' job.id %}">{{ job.id }}</a>
     </div>
 {% endblock %}
 
-{% block content_title %}<h2>Job {{ job.id }}</h2>{% endblock %}
+{% block content_title %}
+    <h2>Job {{ job.id }}
+        {% if job.is_scheduled_job %}
+            <small>
+                <a href="{{ job|scheduled_job }}">Link to scheduled job</a>
+            </small>
+        {% endif %}
+    </h2>
+
+{% endblock %}
 
 {% block content %}
     <div id="content-main">
         <fieldset class="module aligned ">
             <div class="form-row">
                 <label>Queue:</label>
                 <div class="readonly">{{ job.origin }}</div>
             </div>
 
+
             <div class="form-row">
                 <label>Timeout:</label>
                 <div class="readonly">{{ job.timeout }}</div>
             </div>
 
             <div class="form-row">
                 <label>Result TTL:</label>
@@ -124,70 +134,86 @@
                 <label>Result:</label>
                 <div>{{ job.result | default:'-' }}</div>
             </div>
         </fieldset>
 
 
         <div class="submit-row">
-            <p class="deletelink-box"><a href="delete/" class="deletelink">Delete</a></p>
+            <div class="deletelink-box">
+                <a href="{% url 'queue_job_action'  job.id 'delete' %}"
+                   class="deletelink">Delete</a>
+            </div>
+            {% if job.is_started %}
+                <div class="deletelink-box">
+                    <form method='POST' action="{% url 'queue_job_action'  job.id 'cancel' %}">
+                        {% csrf_token %}
+                        <input type="submit" value="cancel" class="default" name="cancel">
+                    </form>
+                </div>
+            {% endif %}
             {% if job.is_failed %}
-                <form method='POST' action="{% url 'queue_requeue_job' queue.name job.id %}">
-                    {% csrf_token %}
-                    <input type="submit" value="Requeue" class="default" name="requeue">
-                </form>
+                <div class="deletelink-box">
+                    <form method='POST' action="{% url 'queue_job_action'  job.id 'requeue' %}">
+                        {% csrf_token %}
+                        <input type="submit" value="Requeue" class="default" name="requeue">
+                    </form>
+                </div>
             {% endif %}
             {% if not job.is_queued and not job.is_failed %}
-                <form method='POST' action="{% url 'queue_enqueue_job' queue.name job.id %}">
-                    {% csrf_token %}
-                    <input type="submit" value="Enqueue" class="default" name="Enqueue">
-                </form>
+                <div class="deletelink-box">
+                    <form method='POST' action="{% url 'queue_job_action'  job.id 'enqueue' %}">
+                        {% csrf_token %}
+                        <input type="submit" value="Enqueue" class="default" name="Enqueue">
+                    </form>
+                </div>
             {% endif %}
         </div>
+    </div>
 
 
-        <div class="inline-group" id="choice_set-group">
-
-            {% for result in job.results %}
-                <h2>Result {{ result.id }}</h2>
-                <div class="inline-related">
+    <div class="inline-group" id="choice_set-group">
 
-                    <fieldset class="module aligned ">
-                        <div class="form-row field-choice_text">
-                            <div>
-                                <label>Type:</label>
-                                <div class="readonly">{{ result.type.name }}</div>
-                            </div>
+        {% for result in job.results %}
+            <h2>Result {{ result.id }}</h2>
+            <div class="inline-related">
+
+                <fieldset class="module aligned ">
+                    <div class="form-row field-choice_text">
+                        <div>
+                            <label>Type:</label>
+                            <div class="readonly">{{ result.type.name }}</div>
                         </div>
+                    </div>
 
+                    <div class="form-row field-votes">
+                        <div>
+                            <label>Created at: {{ result.Type }}</label>
+                            <div class="readonly">{{ result.created_at|date:"Y-m-d, H:i:s" }}</div>
+                        </div>
+                    </div>
+                    {% if result.type.value == 1 %}
                         <div class="form-row field-votes">
                             <div>
-                                <label>Created at: {{ result.Type }}</label>
-                                <div class="readonly">{{ result.created_at|date:"Y-m-d, H:i:s" }}</div>
-                            </div>
-                        </div>
-                        {% if result.type.value == 1 %}
-                            <div class="form-row field-votes">
+                                <label>Return value:</label>
                                 <div>
-                                    <label>Return value:</label>
-                                    <div>
-                                        <pre>{{ result.return_value }}</pre>
-                                    </div>
+                                    <pre>{{ result.return_value }}</pre>
                                 </div>
                             </div>
-                        {% elif result.type.value == 2 %}
-                            <div class="form-row field-votes">
+                        </div>
+                    {% elif result.type.value == 2 %}
+                        <div class="form-row field-votes">
+                            <div>
+                                <label>Exception:</label>
                                 <div>
-                                    <label>Exception:</label>
-                                    <div>
-                                        <pre>{{ result.exc_string }}</pre>
-                                    </div>
+                                    <pre>{{ result.exc_string }}</pre>
                                 </div>
                             </div>
-                        {% endif %}
-                    </fieldset>
-                </div>
-            {% endfor %}
-        </div>
+                        </div>
+                    {% endif %}
+                </fieldset>
+            </div>
+        {% endfor %}
+    </div>
 
     </div>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends "admin/scheduler/scheduler_base.html" %} {% load static
 scheduler_tags %} {% load static %} {% block title %}Job {{ job.id }} {
 { block.super }}{% endblock %} {% block breadcrumbs %}
 Home › Queues › {{_queue.name_}} › {{_job.id_}}
 {% endblock %} {% block content_title %}
-***** Job {{ job.id }} *****
+***** Job {{ job.id }} {% if job.is_scheduled_job %} Link_to_scheduled_job {%
+endif %} *****
 {% endblock %} {% block content %}
 Queue:
 {{ job.origin }}
 Timeout:
 {{ job.timeout }}
 Result TTL:
 {{ job.result_ttl }}
@@ -38,15 +39,17 @@
 {% if exc_info %}
 Exception:
 {% if job.exc_info %}{{ job.exc_info|linebreaks }}{% endif %}
 {% endif %}
 Result:
 {{ job.result | default:'-' }}
 Delete
-{% if job.is_failed %}
+{% if job.is_started %}
+{% csrf_token %} [cancel]
+{% endif %} {% if job.is_failed %}
 {% csrf_token %} [Requeue]
 {% endif %} {% if not job.is_queued and not job.is_failed %}
 {% csrf_token %} [Enqueue]
 {% endif %}
 {% for result in job.results %}
 ***** Result {{ result.id }} *****
 Type:
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/jobs-list.partial.html` & `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/jobs-list.partial.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/jobs.html` & `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/jobs.html`

 * *Files 1% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 {% endblock %}
 
 
 {% block breadcrumbs %}
     <div class="breadcrumbs">
         <a href="{% url 'admin:index' %}">Home</a> &rsaquo;
         <a href="{% url 'queues_home' %}">Queues</a> &rsaquo;
-        <a href="{% url 'queue_jobs' queue.name %}">{{ queue.name }}</a>
+        <a href="{% url 'queue_registry_jobs' queue.name 'queued' %}">{{ queue.name }}</a>
     </div>
 {% endblock %}
 
 {% block content_title %}<h1>{{ job_status }} jobs in {{ queue.name }}</h1>{% endblock %}
 
 {% block content %}
 
     <div id="content-main">
         <ul class="object-tools">
             {% if job_status == 'Failed' %}
-                <li><a href="{% url 'queue_requeue_all' queue.name %}" class="requeuelink">Requeue All</a></li>
+                <li><a href="{% url 'queue_requeue_all' queue.name registry_name %}" class="requeuelink">Requeue All</a>
+                </li>
             {% endif %}
-            <li><a href="{% url 'queue_clear' queue.name %}" class="deletelink">Empty Queue</a></li>
+            <li><a href="{% url 'queue_clear' queue.name registry_name %}" class="deletelink">Empty Queue</a></li>
         </ul>
         <div class="module" id="changelist">
             <form id="changelist-form" action="{% url 'queue_confirm_action' queue.name %}" method="post">
                 {% csrf_token %}
                 <div class="actions">
                     <label>Actions:
                         <select name="action">
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/queue_workers.html` & `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/queue_workers.html`

 * *Files 7% similar despite different names*

```diff
@@ -10,25 +10,22 @@
 {% endblock %}
 
 
 {% block breadcrumbs %}
     <div class="breadcrumbs">
         <a href="{% url 'admin:index' %}">Home</a> &rsaquo;
         <a href="{% url 'queues_home' %}">Queues</a> &rsaquo;
-        <a href="{% url 'queue_jobs' queue.name %}">{{ queue.name }} Workers</a>
+        <a href="{% url 'queue_registry_jobs' queue.name 'queued' %}">Workers for '{{ queue.name }}'</a>
     </div>
 {% endblock %}
 
 {% block content_title %}<h1>Workers in {{ queue.name }}</h1>{% endblock %}
 
 {% block content %}
 
     <div id="content-main">
         <div class="module" id="changelist">
-            <form id="changelist-form" action="{% url 'queue_confirm_action' queue.name %}" method="post">
-                {% csrf_token %}
-                {% include 'admin/scheduler/workers-list.partial.html' %}
-            </form>
+            {% include 'admin/scheduler/workers-list.partial.html' %}
         </div>
     </div>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends "admin/scheduler/scheduler_base.html" %} {% load static
 scheduler_tags l10n %} {% block title %}Workers in {{ queue.name }} {
 { block.super }}{% endblock %} {% block extrastyle %} {{ block.super }}
 ss/changelists.css" %}"> {% endblock %} {% block breadcrumbs %}
-Home › Queues › {{_queue.name_}}_Workers
+Home › Queues › Workers_for_'{{_queue.name_}}'
 {% endblock %} {% block content_title %}
 ****** Workers in {{ queue.name }} ******
 {% endblock %} {% block content %}
-{% csrf_token %} {% include 'admin/scheduler/workers-list.partial.html' %}
+{% include 'admin/scheduler/workers-list.partial.html' %}
 {% endblock %}
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/scheduler_base.html` & `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/scheduler_base.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/stats.html` & `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/stats.html`

 * *Files 6% similar despite different names*

```diff
@@ -44,51 +44,51 @@
                     {% endif %}
                 </tr>
                 </thead>
                 <tbody>
                 {% for queue in queues %}
                     <tr class="{% cycle 'row1' 'row2' %}">
                         <th>
-                            <a href="{% url 'queue_jobs' queue.name %}">
+                            <a href="{% url 'queue_registry_jobs' queue.name 'queued' %}">
                                 {{ queue.name }}
                             </a>
                         </th>
                         <td>
-                            <a href="{% url 'queue_jobs' queue.name %}">
+                            <a href="{% url 'queue_registry_jobs' queue.name 'queued' %}">
                                 {{ queue.jobs }}
                             </a>
                         </td>
                         <td>{{ queue.oldest_job_timestamp }}</td>
                         <th>
-                            <a href="{% url 'queue_started_jobs' queue.name %}">
+                            <a href="{% url 'queue_registry_jobs' queue.name 'started' %}">
                                 {{ queue.started_jobs }}
                             </a>
                         </th>
                         <th>
-                            <a href="{% url 'queue_deferred_jobs' queue.name %}">
+                            <a href="{% url 'queue_registry_jobs' queue.name 'deferred' %}">
                                 {{ queue.deferred_jobs }}
                             </a>
                         </th>
                         <th>
-                            <a href="{% url 'queue_finished_jobs' queue.name %}">
+                            <a href="{% url 'queue_registry_jobs' queue.name 'finished' %}">
                                 {{ queue.finished_jobs }}
                             </a>
                         </th>
                         <th>
-                            <a href="{% url 'queue_failed_jobs' queue.name %}">
+                            <a href="{% url 'queue_registry_jobs' queue.name 'failed' %}">
                                 {{ queue.failed_jobs }}
                             </a>
                         </th>
                         <th>
-                            <a href="{% url 'queue_scheduled_jobs' queue.name %}">
+                            <a href="{% url 'queue_registry_jobs' queue.name 'scheduled' %}">
                                 {{ queue.scheduled_jobs }}
                             </a>
                         </th>
                         <th>
-                            <a href="{% url 'queue_failed_jobs' queue.name %}">
+                            <a href="{% url 'queue_registry_jobs' queue.name 'canceled' %}">
                                 {{ queue.canceled_jobs }}
                             </a>
                         </th>
                         <th><a href="{% url 'queue_workers' queue.name %}">
                             {{ queue.workers }}
                         </a>
                         </th>
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/worker_details.html` & `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/worker_details.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/workers-list.partial.html` & `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/workers-list.partial.html`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                         {{ worker.name }}
                     </a>
                 </td>
                 <td>{{ worker.get_state }}</td>
                 <td>{{ worker.birth_date|date:"Y-m-d, H:i:s" }}</td>
                 <td>{{ worker.hostname }}</td>
                 <td>{{ worker.pid|unlocalize }}</td>
-                <td>{{ worker.total_working_time|default:0|floatformat }}</td>
+                <td>{{ worker.total_working_time|default:0|floatformat }}secs</td>
                 <td>{{ worker.successful_job_count|default:0 }}</td>
                 <td>{{ worker.failed_job_count|default:0 }}</td>
                 <td>{{ worker | worker_scheduler_pid }}</td>
             </tr>
         {% endfor %}
         </tbody>
     </table>
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 {% load scheduler_tags %} {% load l10n %}
 Name         State            Birth                   Hostname        PID                   Working time                       Successful jobs                      Failed jobs                      Scheduler
  worker.name {                {                       {               {                     {                                  {                                    {
 %}'> {       {                {                       {               {                     {                                  {                                    {                                {{ worker |
 {            worker.get_state worker.birth_date|date: worker.hostname worker.pid|unlocalize worker.total_working_time|default: worker.successful_job_count|default: worker.failed_job_count|default: worker_scheduler_pid
-worker.name  }}               "Y-m-d, H:i:s" }}       }}              }}                    0|floatformat }}                   0 }}                                 0 }}                             }}
+worker.name  }}               "Y-m-d, H:i:s" }}       }}              }}                    0|floatformat }}secs               0 }}                                 0 }}                             }}
 }}
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/templates/admin/scheduler/workers.html` & `django_rq_scheduler-2023.6.0/scheduler/templates/admin/scheduler/workers.html`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/templatetags/scheduler_tags.py` & `django_rq_scheduler-2023.6.0/scheduler/templatetags/scheduler_tags.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 
 @register.filter
 def get_item(dictionary, key):
     return dictionary.get(key)
 
 
 @register.filter
+def scheduled_job(job: JobExecution):
+    scheduled_job = get_scheduled_job(*job.args)
+    return scheduled_job.get_absolute_url()
+
+
+@register.filter
 def worker_scheduler_pid(worker):
     return worker.scheduler_pid()
 
 
 @register.filter
 def job_result(job: JobExecution):
     result = job.latest_result()
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_internals.py` & `django_rq_scheduler-2023.6.0/scheduler/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_job_arg_models.py` & `django_rq_scheduler-2023.6.0/scheduler/tests/test_job_arg_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_job_decorator.py` & `django_rq_scheduler-2023.6.0/scheduler/tests/test_job_decorator.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_mgmt_cmds.py` & `django_rq_scheduler-2023.6.0/scheduler/tests/test_mgmt_cmds.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         job_ids = []
         for _ in range(0, 3):
             job = queue.enqueue(failing_job)
             jobs.append(job)
             job_ids.append(job.id)
 
         # Create a worker to execute these jobs
-        call_command('rqworker', burst=True)
+        call_command('rqworker', fork_job_execution=False, burst=True)
 
         # check if all jobs are really failed
         for job in jobs:
             self.assertTrue(job.is_failed)
 
     def test_rqworker__run_jobs(self):
         queue = get_queue('default')
@@ -40,15 +40,15 @@
         job_ids = []
         for _ in range(0, 3):
             job = queue.enqueue(failing_job)
             jobs.append(job)
             job_ids.append(job.id)
 
         # Create a worker to execute these jobs
-        call_command('rqworker', 'default', burst=True)
+        call_command('rqworker', 'default', fork_job_execution=False, burst=True)
 
         # check if all jobs are really failed
         for job in jobs:
             self.assertTrue(job.is_failed)
 
     def test_rqworker__worker_with_two_queues(self):
         queue = get_queue('default')
@@ -62,29 +62,29 @@
             jobs.append(job)
             job_ids.append(job.id)
         job = queue2.enqueue(failing_job)
         jobs.append(job)
         job_ids.append(job.id)
 
         # Create a worker to execute these jobs
-        call_command('rqworker', 'default', 'django_rq_scheduler_test', burst=True)
+        call_command('rqworker', 'default', 'django_rq_scheduler_test', fork_job_execution=False, burst=True)
 
         # check if all jobs are really failed
         for job in jobs:
             self.assertTrue(job.is_failed)
 
     def test_rqworker__worker_with_one_queue__does_not_perform_other_queue_job(self):
         queue = get_queue('default')
         queue2 = get_queue('django_rq_scheduler_test')
 
         job = queue.enqueue(failing_job)
         other_job = queue2.enqueue(failing_job)
 
         # Create a worker to execute these jobs
-        call_command('rqworker', 'default', burst=True)
+        call_command('rqworker', 'default', fork_job_execution=False, burst=True)
         # assert
         self.assertTrue(job.is_failed)
         self.assertTrue(other_job.is_queued)
 
 
 class RqstatsTest(TestCase):
     def test_rqstats__does_not_fail(self):
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_models.py` & `django_rq_scheduler-2023.6.0/scheduler/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from django.urls import reverse
 from django.utils import timezone
 
 from scheduler import settings
 from scheduler.models import BaseJob, CronJob, JobArg, JobKwarg, RepeatableJob, ScheduledJob
 from scheduler.tools import run_job, create_worker
 from . import jobs
-from .testtools import job_factory, jobarg_factory, _get_job_from_queue, SchedulerBaseCase, _get_executions
+from .testtools import (
+    job_factory, jobarg_factory, _get_job_from_scheduled_registry,
+    SchedulerBaseCase, _get_executions)
 from ..queues import get_queue
 
 
 def assert_response_has_msg(response, message):
     messages = [m.message for m in get_messages(response.wsgi_request)]
     assert message in messages, f'expected "{message}" in {messages}'
 
@@ -157,39 +159,39 @@
         def test_str(self):
             name = "test"
             job = job_factory(self.JobModelClass, name=name)
             self.assertEqual(f'{self.JobModelClass.__name__}[{name}={job.callable}()]', str(job))
 
         def test_callable_passthrough(self):
             job = job_factory(self.JobModelClass)
-            entry = _get_job_from_queue(job)
+            entry = _get_job_from_scheduled_registry(job)
             self.assertEqual(entry.func, run_job)
             job_model, job_id = entry.args
             self.assertEqual(job_model, self.JobModelClass.__name__)
             self.assertEqual(job_id, job.id)
 
         def test_timeout_passthrough(self):
             job = job_factory(self.JobModelClass, timeout=500)
-            entry = _get_job_from_queue(job)
+            entry = _get_job_from_scheduled_registry(job)
             self.assertEqual(entry.timeout, 500)
 
         def test_at_front_passthrough(self):
             job = job_factory(self.JobModelClass, at_front=True)
             queue = job.rqueue
             jobs_to_schedule = queue.scheduled_job_registry.get_job_ids()
             self.assertIn(job.job_id, jobs_to_schedule)
 
         def test_callable_result(self):
             job = job_factory(self.JobModelClass, )
-            entry = _get_job_from_queue(job)
+            entry = _get_job_from_scheduled_registry(job)
             self.assertEqual(entry.perform(), 2)
 
         def test_callable_empty_args_and_kwargs(self):
             job = job_factory(self.JobModelClass, callable='scheduler.tests.jobs.test_args_kwargs')
-            entry = _get_job_from_queue(job)
+            entry = _get_job_from_scheduled_registry(job)
             self.assertEqual(entry.perform(), 'test_args_kwargs()')
 
         def test_delete_args(self):
             job = job_factory(self.JobModelClass, )
             arg = jobarg_factory(JobArg, val='one', content_object=job)
             self.assertEqual(1, job.callable_args.count())
             arg.delete()
@@ -226,15 +228,15 @@
             job = job_factory(self.JobModelClass, callable='scheduler.tests.jobs.test_args_kwargs')
             date = timezone.now()
             jobarg_factory(JobArg, arg_type='str', val='one', content_object=job)
             jobarg_factory(JobKwarg, key='key1', arg_type='int', val=2, content_object=job)
             jobarg_factory(JobKwarg, key='key2', arg_type='datetime', val=date, content_object=job)
             jobarg_factory(JobKwarg, key='key3', arg_type='bool', val=False, content_object=job)
             job.save()
-            entry = _get_job_from_queue(job)
+            entry = _get_job_from_scheduled_registry(job)
             self.assertEqual(entry.perform(),
                              "test_args_kwargs('one', key1=2, key2={}, key3=False)".format(date))
 
         def test_function_string(self):
             job = job_factory(self.JobModelClass, )
             date = timezone.now()
             jobarg_factory(JobArg, arg_type='str', val='one', content_object=job)
@@ -326,27 +328,27 @@
             }
             model = job._meta.model.__name__.lower()
             url = reverse(f'admin:scheduler_{model}_changelist')
             # act
             res = self.client.post(url, data=data, follow=True)
             # assert part 1
             self.assertEqual(200, res.status_code)
-            entry = _get_job_from_queue(job)
+            entry = _get_job_from_scheduled_registry(job)
             job_model, scheduled_job_id = entry.args
             self.assertEqual(job_model, job.JOB_TYPE)
             self.assertEqual(scheduled_job_id, job.id)
             self.assertEqual('scheduled', entry.get_status())
             self.assertTrue(has_execution_with_status(job, 'queued'))
 
             # act 2
-            worker = create_worker('default')
+            worker = create_worker('default', fork_job_execution=False, )
             worker.work(burst=True)
 
             # assert 2
-            entry = _get_job_from_queue(job)
+            entry = _get_job_from_scheduled_registry(job)
             self.assertEqual(job_model, job.JOB_TYPE)
             self.assertEqual(scheduled_job_id, job.id)
             self.assertTrue(has_execution_with_status(job, 'finished'))
 
         def test_admin_enable_job(self):
             # arrange
             self.client.login(username='admin', password='admin')
@@ -445,15 +447,15 @@
             job.scheduled_time = scheduled_time
             utc = zoneinfo.ZoneInfo('UTC')
             expected = scheduled_time.astimezone(utc).isoformat()
             self.assertEqual(expected, job._schedule_time().isoformat())
 
         def test_result_ttl_passthrough(self):
             job = job_factory(self.JobModelClass, result_ttl=500)
-            entry = _get_job_from_queue(job)
+            entry = _get_job_from_scheduled_registry(job)
             self.assertEqual(entry.result_ttl, 500)
 
 
 class TestScheduledJob(BaseTestCases.TestSchedulableJob):
     JobModelClass = ScheduledJob
 
     def test_clean(self):
@@ -569,20 +571,20 @@
 
     def test_interval_display(self):
         job = job_factory(self.JobModelClass, interval=15, interval_unit='minutes')
         self.assertEqual(job.interval_display(), '15 minutes')
 
     def test_result_interval(self):
         job = job_factory(self.JobModelClass, )
-        entry = _get_job_from_queue(job)
+        entry = _get_job_from_scheduled_registry(job)
         self.assertEqual(entry.meta['interval'], 3600)
 
     def test_repeat(self):
         job = job_factory(self.JobModelClass, repeat=10)
-        entry = _get_job_from_queue(job)
+        entry = _get_job_from_scheduled_registry(job)
         self.assertEqual(entry.meta['repeat'], 10)
 
     def test_repeat_old_job_exhausted(self):
         base_time = timezone.now()
         job = job_factory(self.JobModelClass, scheduled_time=base_time - timedelta(hours=10), repeat=10)
         self.assertEqual(job.is_scheduled(), False)
 
@@ -635,15 +637,15 @@
         job.queue = list(settings.QUEUES)[0]
         job.callable = 'scheduler.tests.jobs.test_job'
         with self.assertRaises(ValidationError):
             job.clean_cron_string()
 
     def test_repeat(self):
         job = job_factory(self.JobModelClass, repeat=10)
-        entry = _get_job_from_queue(job)
+        entry = _get_job_from_scheduled_registry(job)
         self.assertEqual(entry.meta['repeat'], 10)
 
     def test_check_rescheduled_after_execution(self):
         job = job_factory(self.JobModelClass, )
         queue = job.rqueue
         first_run_id = job.job_id
         entry = queue.fetch_job(first_run_id)
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_redis_models.py` & `django_rq_scheduler-2023.6.0/scheduler/tests/test_redis_models.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_settings.py` & `django_rq_scheduler-2023.6.0/scheduler/tests/test_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 from django.conf import settings
 
 from scheduler.settings import conf_settings
 
 settings.SCHEDULER_QUEUES = {
     'default': {'HOST': 'localhost', 'PORT': 6379, 'DB': 0, 'DEFAULT_TIMEOUT': 500},
     'test': {
@@ -88,8 +90,11 @@
     'test_scheduler': {
         'HOST': 'localhost',
         'PORT': 6379,
         'DB': 0,
         'DEFAULT_TIMEOUT': 400,
     },
 }
+settings.SCHEDULER_CONFIG = dict(
+    FAKEREDIS=(os.getenv('FAKEREDIS', 'False') == 'True'),
+)
 conf_settings()
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/tests/test_worker.py` & `django_rq_scheduler-2023.6.0/scheduler/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/tests/testtools.py` & `django_rq_scheduler-2023.6.0/scheduler/tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,82 @@
-from datetime import timedelta
+import importlib
+import os
 
-from scheduler import settings
-from django.contrib.auth.models import User
-from django.contrib.contenttypes.models import ContentType
-from django.test import Client, TestCase
+import croniter
+from django.apps import apps
 from django.utils import timezone
 
-from scheduler.models import CronJob, JobKwarg, RepeatableJob, ScheduledJob
-from scheduler.queues import get_queue
-
-
-def sequence_gen():
-    n = 1
-    while True:
-        yield n
-        n += 1
-
-
-seq = sequence_gen()
-
-
-def job_factory(cls, instance_only=False, **kwargs):
-    values = dict(
-        name='Scheduled Job %d' % next(seq),
-        job_id=None,
-        queue=list(settings.QUEUES.keys())[0],
-        callable='scheduler.tests.jobs.test_job',
-        enabled=True,
-        timeout=None)
-    if cls == ScheduledJob:
-        values.update(dict(
-            result_ttl=None,
-            scheduled_time=timezone.now() + timedelta(days=1), ))
-    elif cls == RepeatableJob:
-        values.update(dict(
-            result_ttl=None,
-            interval=1,
-            interval_unit='hours',
-            repeat=None,
-            scheduled_time=timezone.now() + timedelta(days=1), ))
-    elif cls == CronJob:
-        values.update(dict(cron_string="0 0 * * *", repeat=None, ))
-    values.update(kwargs)
-    if instance_only:
-        instance = cls(**values)
-    else:
-        instance = cls.objects.create(**values)
-    return instance
-
-
-def jobarg_factory(cls, **kwargs):
-    content_object = kwargs.pop('content_object', None)
-    if content_object is None:
-        content_object = job_factory(ScheduledJob)
-    values = dict(
-        arg_type='str',
-        val='',
-        object_id=content_object.id,
-        content_type=ContentType.objects.get_for_model(content_object),
-        content_object=content_object,
-    )
-    if cls == JobKwarg:
-        values['key'] = 'key%d' % next(seq),
-    values.update(kwargs)
-    instance = cls.objects.create(**values)
-    return instance
-
-
-def _get_job_from_queue(django_job):
-    queue = django_job.rqueue
-    jobs_to_schedule = queue.scheduled_job_registry.get_job_ids()
-    entry = next(i for i in jobs_to_schedule if i == django_job.job_id)
-    return queue.fetch_job(entry)
-
-
-def _get_executions(django_job):
-    queue = get_queue(django_job.queue)
-    job_ids = (queue.get_job_ids()
-               + queue.finished_job_registry.get_job_ids()
-               + queue.scheduled_job_registry.get_job_ids()
-               + queue.failed_job_registry.get_job_ids())
-    return list(filter(
-        lambda j: j.is_execution_of(django_job),
-        map(lambda jid: queue.fetch_job(jid), job_ids)))
-
-
-class SchedulerBaseCase(TestCase):
-    @classmethod
-    def setUpTestData(cls) -> None:
-        super().setUpTestData()
-        try:
-            User.objects.create_superuser('admin', 'admin@a.com', 'admin')
-        except Exception:
-            pass
-        cls.client = Client()
-
-    def setUp(self) -> None:
-        super(SchedulerBaseCase, self).setUp()
-        queue = get_queue('default')
-        queue.empty()
-
-    def tearDown(self) -> None:
-        super(SchedulerBaseCase, self).setUp()
-        queue = get_queue('default')
-        queue.empty()
-
-    @classmethod
-    def setUpClass(cls):
-        super(SchedulerBaseCase, cls).setUpClass()
-        queue = get_queue('default')
-        queue.connection.flushall()
+from scheduler.queues import get_queues, logger, get_queue
+from scheduler.rq_classes import DjangoWorker, MODEL_NAMES
+from scheduler.settings import get_config
+
+
+def callable_func(callable_str: str):
+    path = callable_str.split('.')
+    module = importlib.import_module('.'.join(path[:-1]))
+    func = getattr(module, path[-1])
+    if callable(func) is False:
+        raise TypeError("'{}' is not callable".format(callable_str))
+    return func
+
+
+def get_next_cron_time(cron_string):
+    """Calculate the next scheduled time by creating a crontab object
+    with a cron string"""
+    now = timezone.now()
+    itr = croniter.croniter(cron_string, now)
+    return itr.get_next(timezone.datetime)
+
+
+def get_scheduled_job(task_model: str, task_id: int):
+    if task_model not in MODEL_NAMES:
+        raise ValueError(f'Job Model {task_model} does not exist, choices are {MODEL_NAMES}')
+    model = apps.get_model(app_label='scheduler', model_name=task_model)
+    task = model.objects.filter(id=task_id).first()
+    if task is None:
+        raise ValueError(f'Job {task_model}:{task_id} does not exit')
+    return task
+
+
+def run_job(task_model: str, task_id: int):
+    """Run a scheduled job
+    """
+    scheduled_job = get_scheduled_job(task_model, task_id)
+    logger.debug(f'Running task {str(scheduled_job)}')
+    args = scheduled_job.parse_args()
+    kwargs = scheduled_job.parse_kwargs()
+    res = scheduled_job.callable_func()(*args, **kwargs)
+    return res
+
+
+def _calc_worker_name(existing_worker_names):
+    hostname = os.uname()[1]
+    c = 1
+    worker_name = f'{hostname}-worker.{c}'
+    while worker_name in existing_worker_names:
+        c += 1
+        worker_name = f'{hostname}-worker.{c}'
+    return worker_name
+
+
+def create_worker(*queue_names, **kwargs):
+    """
+    Returns a Django worker for all queues or specified ones.
+    """
+
+    queues = get_queues(*queue_names)
+    existing_workers = DjangoWorker.all(connection=queues[0].connection)
+    existing_worker_names = set(map(lambda w: w.name, existing_workers))
+    kwargs['fork_job_execution'] = not get_config('FAKEREDIS')
+    if kwargs.get('name', None) is None:
+        kwargs['name'] = _calc_worker_name(existing_worker_names)
+
+    kwargs['name'] = kwargs['name'].replace('/', '.')
+    worker = DjangoWorker(queues, connection=queues[0].connection, **kwargs)
+    return worker
+
+
+def get_job_executions(queue_name, scheduled_job):
+    queue = get_queue(queue_name)
+    job_list = queue.get_all_jobs()
+    res = list(filter(lambda j: j.is_execution_of(scheduled_job), job_list))
+    return res
```

### Comparing `django_rq_scheduler-2023.5.0b5/scheduler/views.py` & `django_rq_scheduler-2023.6.0/scheduler/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 from math import ceil
+from typing import Tuple, Optional
 
 import redis
 from django.contrib import admin, messages
 from django.contrib.admin.views.decorators import staff_member_required
 from django.core.paginator import Paginator
 from django.http import JsonResponse
-from django.http.response import HttpResponseNotFound, Http404
+from django.http.response import HttpResponseNotFound, Http404, HttpResponseBadRequest
 from django.shortcuts import redirect
 from django.shortcuts import render
 from django.urls import reverse
 from django.views.decorators.cache import never_cache
 from redis.exceptions import ResponseError
 
-from .queues import get_all_workers, get_connection, logger, get_queue
-from .rq_classes import JobExecution, ExecutionStatus, DjangoWorker
+from .queues import get_all_workers, get_connection, logger, QueueNotFoundError
+from .queues import get_queue as get_queue_base
+from .rq_classes import JobExecution, DjangoWorker, DjangoQueue, InvalidJobOperation
 from .settings import SCHEDULER_CONFIG
 
 
+def get_queue(queue_name: str) -> DjangoQueue:
+    try:
+        return get_queue_base(queue_name)
+    except QueueNotFoundError as e:
+        logger.error(e)
+        raise Http404(e)
+
+
 def get_worker_executions(worker):
     res = list()
     for queue in worker.queues:
         curr_jobs = queue.get_all_jobs()
         curr_jobs = [j for j in curr_jobs if j.worker_name == worker.name]
         res.extend(curr_jobs)
     return res
@@ -48,15 +58,15 @@
     if run_maintenance_tasks:
         workers = get_all_workers()
         for worker in workers:
             worker.clean_registries()
     for queue_name in QUEUES:
         try:
             queue = get_queue(queue_name)
-            connection = get_connection(queue.name)
+            connection = get_connection(QUEUES[queue_name])
             connection_kwargs = connection.connection_pool.connection_kwargs
 
             if run_maintenance_tasks:
                 queue.clean_registries()
 
             # Raw access to the first item from left of the redis list.
             # This might not be accurate since new job can be added from the left
@@ -114,74 +124,41 @@
     if registry is not queue:
         for job_id in remove_job_ids:
             registry.remove(job_id)
 
     return valid_jobs, num_jobs, page_range
 
 
-def jobs_view(request, queue, registry, status_title):
+@never_cache
+@staff_member_required
+def jobs_view(request, queue_name: str, registry_name: str):
+    queue = get_queue(queue_name)
+    registry = queue.get_registry(registry_name)
+    if registry is None:
+        return HttpResponseNotFound()
+    title = registry_name.capitalize()
     page = int(request.GET.get('page', 1))
     job_list, num_jobs, page_range = _get_registry_job_list(queue, registry, page)
 
     context_data = {
         **admin.site.each_context(request),
         'queue': queue,
+        'registry_name': registry_name,
+        'registry': registry,
         'jobs': job_list,
         'num_jobs': num_jobs,
         'page': page,
         'page_range': page_range,
-        'job_status': status_title,
+        'job_status': title,
     }
     return render(request, 'admin/scheduler/jobs.html', context_data)
 
 
 @never_cache
 @staff_member_required
-def jobs(request, queue_name):
-    queue = get_queue(queue_name)
-    return jobs_view(request, queue, queue, 'Queued')
-
-
-@never_cache
-@staff_member_required
-def finished_jobs(request, queue_name):
-    queue = get_queue(queue_name)
-    return jobs_view(request, queue, queue.finished_job_registry, 'Finished')
-
-
-@never_cache
-@staff_member_required
-def failed_jobs(request, queue_name):
-    queue = get_queue(queue_name)
-    return jobs_view(request, queue, queue.failed_job_registry, 'Failed')
-
-
-@never_cache
-@staff_member_required
-def scheduled_jobs(request, queue_name):
-    queue = get_queue(queue_name)
-    return jobs_view(request, queue, queue.scheduled_job_registry, 'Scheduled')
-
-
-@never_cache
-@staff_member_required
-def started_jobs(request, queue_name):
-    queue = get_queue(queue_name)
-    return jobs_view(request, queue, queue.started_job_registry, 'Started')
-
-
-@never_cache
-@staff_member_required
-def deferred_jobs(request, queue_name):
-    queue = get_queue(queue_name)
-    return jobs_view(request, queue, queue.deferred_job_registry, 'Deferred')
-
-
-@never_cache
-@staff_member_required
 def queue_workers(request, queue_name):
     queue = get_queue(queue_name)
     all_workers = DjangoWorker.all(queue.connection)
     for w in all_workers:
         w.clean_registries()
     worker_list = [worker for worker in all_workers if queue.name in worker.queue_names()]
 
@@ -233,156 +210,133 @@
         'executions': page_obj,
         'page_range': page_range,
         'page_var': 'p',
     }
     return render(request, 'admin/scheduler/worker_details.html', context_data)
 
 
-@never_cache
-@staff_member_required
-def job_detail(request, job_id):
+def _find_job(job_id: str) -> Tuple[Optional[DjangoQueue], Optional[JobExecution]]:
     from scheduler.settings import QUEUES
-    queue_index, queue, job = None, None, None
 
     for queue_name in QUEUES:
         try:
             queue = get_queue(queue_name)
             job = JobExecution.fetch(job_id, connection=queue.connection)
-            break
+            if job.origin == queue_name:
+                return queue, job
         except Exception:
             pass
+    return None, None
+
+
+@never_cache
+@staff_member_required
+def job_detail(request, job_id: str):
+    queue, job = _find_job(job_id)
     if job is None:
-        raise Http404(f"Couldn't find job with this ID: {job_id}")
+        return HttpResponseBadRequest(f'Job {job_id} does not exist, maybe its TTL has passed')
     try:
         job.func_name
         data_is_valid = True
     except Exception:
         data_is_valid = False
 
     try:
         exc_info = job._exc_info
     except AttributeError:
         exc_info = None
 
     context_data = {
         **admin.site.each_context(request),
-        'queue_index': queue_index,
         'job': job,
         'dependency_id': job._dependency_id,
         'queue': queue,
         'data_is_valid': data_is_valid,
         'exc_info': exc_info,
     }
     return render(request, 'admin/scheduler/job_detail.html', context_data)
 
 
 @never_cache
 @staff_member_required
-def delete_job(request, queue_name, job_id):
-    queue = get_queue(queue_name)
-    job = JobExecution.fetch(job_id, connection=queue.connection)
-
-    if request.method == 'POST':
-        # Remove job id from queue and delete the actual job
-        queue.connection.lrem(queue.key, 0, job.id)
-        job.delete()
-        messages.info(request, 'You have successfully deleted %s' % job.id)
-        return redirect('queue_jobs', queue_name)
-
-    context_data = {
-        **admin.site.each_context(request),
-        'job': job,
-        'queue': queue,
-    }
-    return render(request, 'admin/scheduler/delete_job.html', context_data)
-
-
-@never_cache
-@staff_member_required
-def requeue_job_view(request, queue_name, job_id):
+def clear_queue_registry(request, queue_name, registry_name):
     queue = get_queue(queue_name)
-    job = JobExecution.fetch(job_id, connection=queue.connection)
+    registry = queue.get_registry(registry_name)
+    if registry is None:
+        return HttpResponseNotFound()
 
-    if request.method == 'POST':
-        job.requeue()
-        messages.info(request, f'You have successfully re-queued {job.id}')
-        return redirect('job_details', job_id)
-
-    context_data = {
-        **admin.site.each_context(request),
-        'job': job,
-        'queue': queue,
-    }
-    return render(request, 'admin/scheduler/delete_job.html', context_data)
-
-
-@never_cache
-@staff_member_required
-def clear_queue(request, queue_name):
-    queue = get_queue(queue_name)
-    next_url = request.META.get('HTTP_REFERER') or reverse('queue_jobs', args=[queue_name])
+    next_url = request.META.get('HTTP_REFERER') or reverse('queue_registry_jobs', args=[queue_name, registry_name])
     if request.method == 'POST':
         try:
-            queue.empty()
-            messages.info(request, f'You have successfully cleared the queue {queue.name}')
+            if registry is queue:
+                queue.empty()
+            else:
+                job_ids = registry.get_job_ids()
+                for job_id in job_ids:
+                    registry.remove(job_id, delete_job=True)
+            messages.info(request, f'You have successfully cleared the {registry_name} jobs in queue {queue.name}')
         except ResponseError as e:
             messages.error(request, f'error: {e}', )
             raise e
-        return redirect('queue_jobs', queue_name)
-
+        return redirect('queue_registry_jobs', queue_name, registry_name)
+    job_ids = registry.get_job_ids()
+    job_list = JobExecution.fetch_many(job_ids, connection=queue.connection)
     context_data = {
         **admin.site.each_context(request),
         'queue': queue,
-        'total_jobs': len(queue),
+        'total_jobs': len(registry),
         'action': 'empty',
-        'jobs': queue.get_jobs(),
+        'jobs': job_list,
         'next_url': next_url,
-        'action_url': reverse('queue_clear', args=[queue_name, ])
+        'action_url': reverse('queue_clear', args=[queue_name, registry_name, ])
     }
     return render(request, 'admin/scheduler/confirm_action.html', context_data)
 
 
 @never_cache
 @staff_member_required
-def requeue_all(request, queue_name):
+def requeue_all(request, queue_name, registry_name):
     queue = get_queue(queue_name)
-    next_url = request.META.get('HTTP_REFERER') or reverse('queue_jobs', args=[queue_name])
-    job_ids = queue.failed_job_registry.get_job_ids()
+    registry = queue.get_registry(registry_name)
+    if registry is None:
+        return HttpResponseNotFound()
+    next_url = request.META.get('HTTP_REFERER') or reverse('queue_registry_jobs', args=[queue_name, registry_name])
+    job_ids = registry.get_job_ids()
     if request.method == 'POST':
         count = 0
         # Confirmation received
         for job_id in job_ids:
             try:
                 job = JobExecution.fetch(job_id, connection=queue.connection)
                 job.requeue()
                 count += 1
             except Exception:
                 pass
 
         messages.info(request, f'You have successfully re-queued {count} jobs!')
-        return redirect('queue_jobs', queue_name)
+        return redirect('queue_registry_jobs', queue_name, registry_name)
 
     context_data = {
         **admin.site.each_context(request),
         'queue': queue,
         'total_jobs': len(queue.failed_job_registry),
         'action': 'requeue',
         'jobs': [queue.fetch_job(job_id) for job_id in job_ids],
         'next_url': next_url,
-        'action_url': reverse('queue_requeue_all', args=[queue_name, ])
+        'action_url': reverse('queue_requeue_all', args=[queue_name, registry_name])
     }
 
     return render(request, 'admin/scheduler/confirm_action.html', context_data)
 
 
 @never_cache
 @staff_member_required
 def confirm_action(request, queue_name):
     queue = get_queue(queue_name)
-    next_url = request.META.get('HTTP_REFERER') or reverse('queue_jobs', args=[queue_name])
+    next_url = request.META.get('HTTP_REFERER') or reverse('queue_registry_jobs', args=[queue_name, 'queued'])
 
     if request.method == 'POST' and request.POST.get('action', False):
         # confirm action
         if request.POST.get('_selected_action', False):
             job_id_list = request.POST.getlist('_selected_action')
             context_data = {
                 **admin.site.each_context(request),
@@ -398,69 +352,86 @@
     return redirect(next_url)
 
 
 @never_cache
 @staff_member_required
 def actions(request, queue_name):
     queue = get_queue(queue_name)
-    next_url = request.POST.get('next_url') or reverse('queue_jobs', args=[queue_name])
+    next_url = request.POST.get('next_url') or reverse('queue_registry_jobs', args=[queue_name, 'queued'])
 
-    if request.method == 'POST' and request.POST.get('action', False):
-        # do confirmed action
-        if request.POST.get('job_ids', False):
-            job_ids = request.POST.getlist('job_ids')
+    action = request.POST.get('action', False)
+    job_ids = request.POST.get('job_ids', False)
+    if request.method != 'POST' or not action or not job_ids:
+        return redirect(next_url)
+    job_ids = request.POST.getlist('job_ids')
+    if action == 'delete':
+        for job_id in job_ids:
+            job = JobExecution.fetch(job_id, connection=queue.connection)
+            # Remove job id from queue and delete the actual job
+            queue.connection.lrem(queue.key, 0, job.id)
+            job.delete()
+        messages.info(request, f'You have successfully deleted {len(job_ids)} jobs!')
+    elif action == 'requeue':
+        for job_id in job_ids:
+            job = JobExecution.fetch(job_id, connection=queue.connection)
+            job.requeue()
+        messages.info(request, f'You have successfully re-queued {len(job_ids)}  jobs!')
+    elif action == 'stop':
+        cancelled_jobs = 0
+        for job_id in job_ids:
+            try:
+                job = JobExecution.fetch(job_id, connection=queue.connection)
+                job.stop_execution(queue.connection)
+                job.cancel()
+                cancelled_jobs += 1
+            except Exception as e:
+                logger.warning(f'Could not stop job: {e}')
+                pass
+        messages.info(request, f'You have successfully stopped {cancelled_jobs}  jobs!')
+    return redirect(next_url)
 
-            if request.POST['action'] == 'delete':
-                for job_id in job_ids:
-                    job = JobExecution.fetch(job_id, connection=queue.connection)
-                    # Remove job id from queue and delete the actual job
-                    queue.connection.lrem(queue.key, 0, job.id)
-                    job.delete()
-                messages.info(request, f'You have successfully deleted {len(job_ids)} jobs!')
-            elif request.POST['action'] == 'requeue':
-                for job_id in job_ids:
-                    job = JobExecution.fetch(job_id, connection=queue.connection)
-                    job.requeue()
-                messages.info(request, f'You have successfully re-queued {len(job_ids)}  jobs!')
-            elif request.POST['action'] == 'stop':
-                cancelled_jobs = 0
-                for job_id in job_ids:
-                    try:
-                        job = JobExecution.fetch(job_id, connection=queue.connection)
-                        job.stop_execution(queue.connection)
-                        job.cancel()
-                        cancelled_jobs += 1
-                    except Exception as e:
-                        logger.warning(f'Could not stop job: {e}')
-                        pass
-                messages.info(request, f'You have successfully stopped {cancelled_jobs}  jobs!')
 
-    return redirect(next_url)
+SUPPORTED_JOB_ACTIONS = {'requeue', 'delete', 'enqueue', 'cancel'}
 
 
 @never_cache
 @staff_member_required
-def enqueue_job(request, queue_name, job_id):
-    """Enqueue deferred jobs"""
-    queue = get_queue(queue_name)
-    job = JobExecution.fetch(job_id, connection=queue.connection)
-
-    if request.method == 'POST':
-        queue.enqueue_job(job)
-
-        # Remove job from correct registry if needed
-        if job.get_status() == ExecutionStatus.DEFERRED:
-            queue.deferred_job_registry.remove(job)
-        elif job.get_status() == ExecutionStatus.FINISHED:
-            queue.finished_job_registry.remove(job)
-        elif job.get_status() == ExecutionStatus.SCHEDULED:
-            queue.scheduled_job_registry.remove(job)
-
-        messages.info(request, 'You have successfully enqueued %s' % job.id)
-        return redirect('job_details', job_id)
+def job_action(request, job_id: str, action: str):
+    queue, job = _find_job(job_id)
+    if job is None:
+        return HttpResponseBadRequest(f'Job {job_id} does not exist, maybe its TTL has passed')
+    if action not in SUPPORTED_JOB_ACTIONS:
+        return HttpResponseNotFound()
+
+    if request.method != 'POST':
+        context_data = {
+            **admin.site.each_context(request),
+            'job': job,
+            'queue': queue,
+            'action': action,
+        }
+        return render(request, 'admin/scheduler/single_job_action.html', context_data)
 
-    context_data = {
-        **admin.site.each_context(request),
-        'job': job,
-        'queue': queue,
-    }
-    return render(request, 'admin/scheduler/delete_job.html', context_data)
+    try:
+        if action == 'requeue':
+            job.requeue()
+            messages.info(request, f'You have successfully re-queued {job.id}')
+            return redirect('job_details', job_id)
+        elif action == 'delete':
+            # Remove job id from queue and delete the actual job
+            queue.connection.lrem(queue.key, 0, job.id)
+            job.delete()
+            messages.info(request, 'You have successfully deleted %s' % job.id)
+            return redirect('queue_registry_jobs', queue.name, 'queued')
+        elif action == 'enqueue':
+            job.delete(remove_from_queue=False)
+            queue._enqueue_job(job)
+            messages.info(request, 'You have successfully enqueued %s' % job.id)
+            return redirect('job_details', job_id)
+        elif action == 'cancel':
+            job.cancel()
+            messages.info(request, 'You have successfully enqueued %s' % job.id)
+            return redirect('job_details', job_id)
+    except InvalidJobOperation as e:
+        logger.warning(f'Could not perform action: {e}')
+        messages.warning(request, f'Could not perform action: {e}')
+    return redirect('job_details', job_id)
```

### Comparing `django_rq_scheduler-2023.5.0b5/PKG-INFO` & `django_rq_scheduler-2023.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rq-scheduler
-Version: 2023.5.0b5
+Version: 2023.6.0
 Summary: An async job scheduler for django using redis
 Home-page: https://github.com/dsoftwareinc/django-rq-scheduler
 License: MIT
 Keywords: redis,django,background-jobs,job-queue,task-queue,redis-queue,scheduled-jobs
 Author: Daniel Moran
 Author-email: daniel.maruani@gmail.com
 Maintainer: Daniel Moran
@@ -29,15 +29,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: croniter (>=1.3,<2.0)
 Requires-Dist: django (>=3.2)
 Requires-Dist: django-model-utils (>=4.3,<5.0)
-Requires-Dist: rq (>=1.13,<2.0)
+Requires-Dist: rq (>=1.14,<2.0)
 Project-URL: Bug Tracker, https://github.com/dsoftwareinc/django-rq-scheduler/issues
 Project-URL: Documentation, https://django-rq-scheduler.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/cunla
 Description-Content-Type: text/markdown
 
 Django RQ Scheduler
 ===================
```

