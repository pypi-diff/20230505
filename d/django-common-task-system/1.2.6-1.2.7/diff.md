# Comparing `tmp/django-common-task-system-1.2.6.tar.gz` & `tmp/django-common-task-system-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-task-system-1.2.6.tar", last modified: Thu May  4 07:18:00 2023, max compression
+gzip compressed data, was "django-common-task-system-1.2.7.tar", last modified: Fri May  5 06:06:02 2023, max compression
```

## Comparing `django-common-task-system-1.2.6.tar` & `django-common-task-system-1.2.7.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.129160 django-common-task-system-1.2.6/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.2.6/LICENSE
--rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0      303 2023-05-04 07:18:00.129160 django-common-task-system-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.077477 django-common-task-system-1.2.6/django_common_task_system/
--rw-rw-rw-   0        0        0     3015 2023-05-04 05:28:57.000000 django-common-task-system-1.2.6/django_common_task_system/__init__.py
--rw-rw-rw-   0        0        0    11370 2023-04-21 09:44:38.000000 django-common-task-system-1.2.6/django_common_task_system/admin.py
--rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.2.6/django_common_task_system/apps.py
--rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.2.6/django_common_task_system/choices.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.2.6/django_common_task_system/fields.py
--rw-rw-rw-   0        0        0    15985 2023-04-26 08:54:39.000000 django-common-task-system-1.2.6/django_common_task_system/forms.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.095472 django-common-task-system-1.2.6/django_common_task_system/migrations/
--rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
--rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
--rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/0006_consumerpermission.py
--rw-rw-rw-   0        0        0     1275 2023-04-21 07:23:00.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.2.6/django_common_task_system/migrations/__init__.py
--rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.2.6/django_common_task_system/mixin.py
--rw-rw-rw-   0        0        0    36866 2023-04-26 08:13:50.000000 django-common-task-system-1.2.6/django_common_task_system/models.py
--rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.2.6/django_common_task_system/permissions.py
--rw-rw-rw-   0        0        0     2425 2023-05-04 05:26:09.000000 django-common-task-system-1.2.6/django_common_task_system/serializers.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.063059 django-common-task-system-1.2.6/django_common_task_system/static/
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.064067 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.096473 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/css/
--rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/css/calendar.css
--rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.098482 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/js/
--rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/js/calendar.js
--rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
--rw-rw-rw-   0        0        0     1145 2023-05-04 07:00:46.000000 django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/js/task_type_admin.js
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.106482 django-common-task-system-1.2.6/django_common_task_system/system_task/
--rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/__init__.py
--rw-rw-rw-   0        0        0     5503 2023-05-04 07:00:46.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/admin.py
--rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/apps.py
--rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/choices.py
--rw-rw-rw-   0        0        0     4728 2023-05-04 07:00:46.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/forms.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.113473 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/
--rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
--rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
--rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
--rw-rw-rw-   0        0        0     1062 2023-04-21 07:23:00.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/__init__.py
--rw-rw-rw-   0        0        0    14945 2023-04-21 07:09:25.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/models.py
--rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/process.py
--rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/queue.py
--rw-rw-rw-   0        0        0     1679 2023-04-21 07:11:39.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/serializers.py
--rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/tests.py
--rw-rw-rw-   0        0        0      846 2023-04-21 07:22:44.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/urls.py
--rw-rw-rw-   0        0        0     5505 2023-04-21 07:22:44.000000 django-common-task-system-1.2.6/django_common_task_system/system_task/views.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.115148 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     1674 2023-04-19 09:54:46.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/main.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.117155 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     3100 2023-04-21 07:40:43.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executor.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.121157 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/
--rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
--rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
--rw-rw-rw-   0        0        0     3708 2023-04-27 05:37:12.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
--rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
--rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
--rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.066058 django-common-task-system-1.2.6/django_common_task_system/templates/
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.065060 django-common-task-system-1.2.6/django_common_task_system/templates/admin/
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.121157 django-common-task-system-1.2.6/django_common_task_system/templates/admin/system_schedule/
--rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.2.6/django_common_task_system/templates/admin/system_schedule/change_list.html
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.125164 django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/
--rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/datetime_range.html
--rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/multi_day_select.html
--rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/multi_month_day_select.html
--rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/nlp_input.html
--rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/period.html
--rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/period_schedule.html
--rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.2.6/django_common_task_system/tests.py
--rw-rw-rw-   0        0        0     1060 2023-04-21 07:22:44.000000 django-common-task-system-1.2.6/django_common_task_system/urls.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.128157 django-common-task-system-1.2.6/django_common_task_system/utils/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.2.6/django_common_task_system/utils/__init__.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.2.6/django_common_task_system/utils/algorithm.py
--rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.2.6/django_common_task_system/utils/cron_utils.py
--rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.2.6/django_common_task_system/utils/foreign_key.py
--rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.2.6/django_common_task_system/utils/schedule_time.py
--rw-rw-rw-   0        0        0    12089 2023-05-04 07:11:55.000000 django-common-task-system-1.2.6/django_common_task_system/views.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.089480 django-common-task-system-1.2.6/django_common_task_system.egg-info/
--rw-rw-rw-   0        0        0      303 2023-05-04 07:18:00.000000 django-common-task-system-1.2.6/django_common_task_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4497 2023-05-04 07:18:00.000000 django-common-task-system-1.2.6/django_common_task_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 07:18:00.000000 django-common-task-system-1.2.6/django_common_task_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-05-04 07:18:00.000000 django-common-task-system-1.2.6/django_common_task_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-05-04 07:18:00.000000 django-common-task-system-1.2.6/django_common_task_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 07:18:00.130159 django-common-task-system-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-05-04 07:17:46.000000 django-common-task-system-1.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:18:00.128157 django-common-task-system-1.2.6/tests/
--rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.2.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:02.076983 django-common-task-system-1.2.7/
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      303 2023-05-05 06:06:02.075984 django-common-task-system-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.739192 django-common-task-system-1.2.7/django_common_task_system/
+-rw-rw-rw-   0        0        0     3015 2023-05-04 05:28:57.000000 django-common-task-system-1.2.7/django_common_task_system/__init__.py
+-rw-rw-rw-   0        0        0    11370 2023-04-21 09:44:38.000000 django-common-task-system-1.2.7/django_common_task_system/admin.py
+-rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.2.7/django_common_task_system/apps.py
+-rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.2.7/django_common_task_system/choices.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.2.7/django_common_task_system/fields.py
+-rw-rw-rw-   0        0        0    15985 2023-04-26 08:54:39.000000 django-common-task-system-1.2.7/django_common_task_system/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.811245 django-common-task-system-1.2.7/django_common_task_system/migrations/
+-rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.2.7/django_common_task_system/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.2.7/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+-rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.2.7/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+-rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.2.7/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.2.7/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.2.7/django_common_task_system/migrations/0006_consumerpermission.py
+-rw-rw-rw-   0        0        0     1275 2023-04-21 07:23:00.000000 django-common-task-system-1.2.7/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.2.7/django_common_task_system/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.2.7/django_common_task_system/mixin.py
+-rw-rw-rw-   0        0        0    36866 2023-04-26 08:13:50.000000 django-common-task-system-1.2.7/django_common_task_system/models.py
+-rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.2.7/django_common_task_system/permissions.py
+-rw-rw-rw-   0        0        0     2425 2023-05-04 05:26:09.000000 django-common-task-system-1.2.7/django_common_task_system/serializers.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.649462 django-common-task-system-1.2.7/django_common_task_system/static/
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.649462 django-common-task-system-1.2.7/django_common_task_system/static/common_task_system/
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.821811 django-common-task-system-1.2.7/django_common_task_system/static/common_task_system/css/
+-rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.2.7/django_common_task_system/static/common_task_system/css/calendar.css
+-rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.2.7/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.850000 django-common-task-system-1.2.7/django_common_task_system/static/common_task_system/js/
+-rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.2.7/django_common_task_system/static/common_task_system/js/calendar.js
+-rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.2.7/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+-rw-rw-rw-   0        0        0     1145 2023-05-04 07:00:46.000000 django-common-task-system-1.2.7/django_common_task_system/static/common_task_system/js/task_type_admin.js
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.895341 django-common-task-system-1.2.7/django_common_task_system/system_task/
+-rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/__init__.py
+-rw-rw-rw-   0        0        0     5571 2023-05-05 05:35:03.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/admin.py
+-rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/apps.py
+-rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/choices.py
+-rw-rw-rw-   0        0        0     4486 2023-05-05 05:36:52.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.949795 django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/
+-rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+-rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
+-rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
+-rw-rw-rw-   0        0        0     1062 2023-04-21 07:23:00.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/__init__.py
+-rw-rw-rw-   0        0        0    14965 2023-05-05 05:22:55.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/models.py
+-rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/process.py
+-rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/queue.py
+-rw-rw-rw-   0        0        0     1679 2023-04-21 07:11:39.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/tests.py
+-rw-rw-rw-   0        0        0      846 2023-04-21 07:22:44.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/urls.py
+-rw-rw-rw-   0        0        0     5508 2023-05-05 05:22:55.000000 django-common-task-system-1.2.7/django_common_task_system/system_task/views.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.957555 django-common-task-system-1.2.7/django_common_task_system/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.2.7/django_common_task_system/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     1674 2023-04-19 09:54:46.000000 django-common-task-system-1.2.7/django_common_task_system/system_task_execution/main.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.965650 django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     3100 2023-04-21 07:40:43.000000 django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/executor.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.994426 django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/executors/
+-rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+-rw-rw-rw-   0        0        0     3708 2023-04-27 05:37:12.000000 django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+-rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+-rw-rw-rw-   0        0        0     1116 2023-05-05 05:22:55.000000 django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+-rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.652463 django-common-task-system-1.2.7/django_common_task_system/templates/
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.652463 django-common-task-system-1.2.7/django_common_task_system/templates/admin/
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.995427 django-common-task-system-1.2.7/django_common_task_system/templates/admin/system_schedule/
+-rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.2.7/django_common_task_system/templates/admin/system_schedule/change_list.html
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:02.045351 django-common-task-system-1.2.7/django_common_task_system/templates/task_schedule/
+-rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.2.7/django_common_task_system/templates/task_schedule/datetime_range.html
+-rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.2.7/django_common_task_system/templates/task_schedule/multi_day_select.html
+-rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.2.7/django_common_task_system/templates/task_schedule/multi_month_day_select.html
+-rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.2.7/django_common_task_system/templates/task_schedule/nlp_input.html
+-rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.2.7/django_common_task_system/templates/task_schedule/period.html
+-rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.2.7/django_common_task_system/templates/task_schedule/period_schedule.html
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.2.7/django_common_task_system/tests.py
+-rw-rw-rw-   0        0        0     1060 2023-04-21 07:22:44.000000 django-common-task-system-1.2.7/django_common_task_system/urls.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:02.073973 django-common-task-system-1.2.7/django_common_task_system/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.2.7/django_common_task_system/utils/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.2.7/django_common_task_system/utils/algorithm.py
+-rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.2.7/django_common_task_system/utils/cron_utils.py
+-rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.2.7/django_common_task_system/utils/foreign_key.py
+-rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.2.7/django_common_task_system/utils/schedule_time.py
+-rw-rw-rw-   0        0        0    12089 2023-05-04 07:11:55.000000 django-common-task-system-1.2.7/django_common_task_system/views.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:01.756591 django-common-task-system-1.2.7/django_common_task_system.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-05-05 06:06:01.000000 django-common-task-system-1.2.7/django_common_task_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4497 2023-05-05 06:06:01.000000 django-common-task-system-1.2.7/django_common_task_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 06:06:01.000000 django-common-task-system-1.2.7/django_common_task_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-05-05 06:06:01.000000 django-common-task-system-1.2.7/django_common_task_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-05-05 06:06:01.000000 django-common-task-system-1.2.7/django_common_task_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 06:06:02.076983 django-common-task-system-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-05-05 05:41:46.000000 django-common-task-system-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:06:02.074983 django-common-task-system-1.2.7/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.2.7/tests/__init__.py
```

### Comparing `django-common-task-system-1.2.6/LICENSE` & `django-common-task-system-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/__init__.py` & `django-common-task-system-1.2.7/django_common_task_system/__init__.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/admin.py` & `django-common-task-system-1.2.7/django_common_task_system/admin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/choices.py` & `django-common-task-system-1.2.7/django_common_task_system/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/fields.py` & `django-common-task-system-1.2.7/django_common_task_system/fields.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/forms.py` & `django-common-task-system-1.2.7/django_common_task_system/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/migrations/0001_initial.py` & `django-common-task-system-1.2.7/django_common_task_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py` & `django-common-task-system-1.2.7/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py` & `django-common-task-system-1.2.7/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/migrations/0006_consumerpermission.py` & `django-common-task-system-1.2.7/django_common_task_system/migrations/0006_consumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py` & `django-common-task-system-1.2.7/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/mixin.py` & `django-common-task-system-1.2.7/django_common_task_system/mixin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/models.py` & `django-common-task-system-1.2.7/django_common_task_system/models.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/permissions.py` & `django-common-task-system-1.2.7/django_common_task_system/permissions.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/serializers.py` & `django-common-task-system-1.2.7/django_common_task_system/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/css/calendar.css` & `django-common-task-system-1.2.7/django_common_task_system/static/common_task_system/css/calendar.css`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/js/calendar.js` & `django-common-task-system-1.2.7/django_common_task_system/static/common_task_system/js/calendar.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/js/task_schedule_admin.js` & `django-common-task-system-1.2.7/django_common_task_system/static/common_task_system/js/task_schedule_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/static/common_task_system/js/task_type_admin.js` & `django-common-task-system-1.2.7/django_common_task_system/static/common_task_system/js/task_type_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/admin.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         "config",
         'description',
     )
     filter_horizontal = []
     list_filter = ('category', 'parent')
 
     def has_delete_permission(self, request, obj=None):
-        if obj:
+        if obj and not request.user.is_superuser:
             return obj.category != models.builtins.categories.system_default_category
         return True
 
     class Media:
         js = (
             'https://cdn.bootcss.com/jquery/3.3.1/jquery.min.js',
             'https://cdn.bootcss.com/popper.js/1.14.3/umd/popper.min.js',
@@ -85,15 +85,15 @@
     queues = models.builtins.queues
     schedule_put_name = 'system_schedule_put'
     list_display = ('id', 'admin_task', 'schedule_type', 'schedule_sub_type', 'next_schedule_time',
                     'status', 'put', 'logs', 'update_time')
     list_filter = ('task__category', )
 
     def has_delete_permission(self, request, obj=None):
-        if obj:
+        if obj and not request.user.is_superuser:
             return obj.task.category != models.builtins.categories.system_default_category
         return True
 
 
 class SystemScheduleLogAdmin(base_admin.TaskScheduleLogAdmin):
     schedule_retry_name = 'system_schedule_retry'
```

#### html2text {}

```diff
@@ -17,38 +17,40 @@
 os.path.isfile(instance.log_file) and not instance.log_file.endswith('system-
 process-default.log'): os.remove(instance.log_file) class SystemTaskAdmin
 (base_admin.TaskAdmin): form = forms.SystemTaskForm schedule_model =
 models.SystemSchedule list_display = ('id', 'admin_parent', 'name', 'category',
 'admin_status', 'schedules', 'update_time') fields = ( 'category', ("name",
 "status",), ("parent", 'queue'), "script", "config", 'description', )
 filter_horizontal = [] list_filter = ('category', 'parent') def
-has_delete_permission(self, request, obj=None): if obj: return obj.category !=
+has_delete_permission(self, request, obj=None): if obj and not
+request.user.is_superuser: return obj.category !=
 models.builtins.categories.system_default_category return True class Media: js
 = ( 'https://cdn.bootcss.com/jquery/3.3.1/jquery.min.js', 'https://
 cdn.bootcss.com/popper.js/1.14.3/umd/popper.min.js', 'https://cdn.bootcss.com/
 bootstrap/4.1.3/js/bootstrap.min.js', 'common_task_system/js/
 task_type_admin.js', ) class SystemScheduleCallbackAdmin
 (base_admin.TaskScheduleCallbackAdmin): pass class SystemScheduleAdmin
 (base_admin.TaskScheduleAdmin): task_model = models.SystemTask
 schedule_log_model = models.SystemScheduleLog queues = models.builtins.queues
 schedule_put_name = 'system_schedule_put' list_display = ('id', 'admin_task',
 'schedule_type', 'schedule_sub_type', 'next_schedule_time', 'status', 'put',
 'logs', 'update_time') list_filter = ('task__category', ) def
-has_delete_permission(self, request, obj=None): if obj: return
-obj.task.category != models.builtins.categories.system_default_category return
-True class SystemScheduleLogAdmin(base_admin.TaskScheduleLogAdmin):
-schedule_retry_name = 'system_schedule_retry' class SystemProcessAdmin
-(admin.ModelAdmin): list_display = ('process_id', 'process_name', 'log_file',
-'status', 'stop_process', 'show_log', 'update_time') form =
-forms.SystemProcessForm fields = ( 'system_path', 'process_name', 'env',
-'log_file', 'process_id', 'create_time', ) readonly_fields = ('create_time',
-'update_time') def stop_process(self, obj): url = reverse
-('system_process_stop', args=(obj.process_id,)) return format_html( 'åæ­¢' %
-url ) stop_process.short_description = 'åæ­¢è¿è¡' def show_log(self, obj):
-url = reverse('system_process_log', args=(obj.process_id,)) return format_html
+has_delete_permission(self, request, obj=None): if obj and not
+request.user.is_superuser: return obj.task.category !=
+models.builtins.categories.system_default_category return True class
+SystemScheduleLogAdmin(base_admin.TaskScheduleLogAdmin): schedule_retry_name =
+'system_schedule_retry' class SystemProcessAdmin(admin.ModelAdmin):
+list_display = ('process_id', 'process_name', 'log_file', 'status',
+'stop_process', 'show_log', 'update_time') form = forms.SystemProcessForm
+fields = ( 'system_path', 'process_name', 'env', 'log_file', 'process_id',
+'create_time', ) readonly_fields = ('create_time', 'update_time') def
+stop_process(self, obj): url = reverse('system_process_stop', args=
+(obj.process_id,)) return format_html( 'åæ­¢' % url )
+stop_process.short_description = 'åæ­¢è¿è¡' def show_log(self, obj): url =
+reverse('system_process_log', args=(obj.process_id,)) return format_html
 ( 'æ¥çæ¥å¿' % url ) show_log.short_description = 'æ¥å¿' def
 has_delete_permission(self, request, obj=None): return False class
 SystemScheduleQueueAdmin(base_admin.TaskScheduleQueueAdmin): form =
 forms.SystemScheduleQueueForm builtins = models.builtins schedule_get_name =
 'system_schedule_get' class SystemScheduleProducerAdmin
 (base_admin.TaskScheduleProducerAdmin): form = forms.SystemScheduleProducerForm
 schedule_get_name = 'system_schedule_get' builtins = models.builtins class
```

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/choices.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/forms.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/forms.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,56 +4,55 @@
 import time
 from .process import ProcessManager
 from ..system_task_execution.main import start_system_client
 from django_common_task_system.forms import TaskScheduleProducerForm, TaskScheduleQueueForm
 
 
 class SystemTaskForm(forms.ModelForm):
-    config = forms.CharField(
+    config = forms.JSONField(
         label='配置',
         widget=forms.Textarea(attrs={'style': 'width: 70%;'}),
         required=False,
     )
     queue = forms.ModelChoiceField(
         queryset=models.SystemScheduleQueue.objects.all(),
         required=False,
         label='队列',
         widget=forms.Select(attrs={'class': 'form-control'})
     )
 
     script = forms.CharField(
         label='脚本',
         widget=forms.Textarea(attrs={'style': 'width: 70%;'}),
+        required=False
     )
 
     def __init__(self, *args, **kwargs):
         super(SystemTaskForm, self).__init__(*args, **kwargs)
         if self.instance.id:
             parent = self.instance.parent
             if parent == models.builtins.tasks.sql_produce_parent_task:
-                self.fields['queue'].initial = models.SystemScheduleQueue.objects.get(
+                self.initial['queue'] = models.SystemScheduleQueue.objects.get(
                     code=self.instance.config.get('queue')
                 )
-                self.fields['script'].initial = self.instance.config.get('sql')
-            elif parent == models.builtins.tasks.sql_execution_parent_task:
-                self.fields['script'].initial = self.instance.config.get('sql')
-            elif parent == models.builtins.tasks.shell_execution_parent_task:
-                self.fields['script'].initial = self.instance.config.get('shell')
+            self.initial['script'] = self.instance.config.get('script')
 
     def clean(self):
         cleaned_data = super(SystemTaskForm, self).clean()
         parent = cleaned_data.get('parent')
         required_fields = parent.config.get('required_fields', []) if parent else []
         config = cleaned_data.get('config', {})
-        queue = cleaned_data.pop('queue')
-        if queue:
-            config['queue'] = queue.code
         for field in required_fields:
-            if not config.get(field):
-                self.add_error('config', '%s不能为空' % field)
+            value = cleaned_data.pop(field, None)
+            if not value:
+                self.add_error('name', '%s不能为空' % field)
+            if field == 'queue':
+                config[field] = value.code
+            else:
+                config[field] = value
         return cleaned_data
 
     class Meta:
         model = models.SystemTask
         fields = '__all__'
```

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0001_initial.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/models.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,44 +193,44 @@
         user = categories.system_default_category.user
 
         self.shell_execution_parent_task = self.model(
             name='Shell执行',
             user=user,
             category=categories.system_base_category,
             config={
-                'required_fields': ['shell'],
+                'required_fields': ['script'],
             }
         )
         self.sql_execution_parent_task = self.model(
             name='SQL执行',
             user=user,
             category=categories.system_base_category,
             config={
-                'required_fields': ['sql'],
+                'required_fields': ['script'],
             }
         )
 
         self.sql_produce_parent_task = self.model(
             name='SQL生产',
             user=user,
             category=categories.system_base_category,
             config={
-                'required_fields': ['sql', 'queue'],
+                'required_fields': ['script', 'queue'],
             }
         )
 
         interval = 1
         unit = 'month'
         self.system_log_cleaning = self.model(
             name='系统日志清理',
             parent=self.sql_execution_parent_task,
             category=categories.system_default_category,
             user=user,
             config={
-                'sql': 'delete from %s where create_time < date_sub(now(), interval %s %s);' %
+                'script': 'delete from %s where create_time < date_sub(now(), interval %s %s);' %
                        (SystemScheduleLog._meta.db_table, interval, unit)
             },
         )
 
         max_retry_times = 5
         self.system_exception_handling = self.model(
             name='系统异常处理',
@@ -245,15 +245,15 @@
         unit = 'month'
         self.task_log_cleaning = self.model(
             name='任务日志清理',
             user=user,
             category=categories.system_default_category,
             parent=self.sql_execution_parent_task,
             config={
-                'sql': 'delete from %s where create_time < date_sub(now(), interval %s %s);' %
+                'script': 'delete from %s where create_time < date_sub(now(), interval %s %s);' %
                        (TaskScheduleLog._meta.db_table, interval, unit)
             },
         )
 
         max_retry_times = 5
         self.task_exception_handling = self.model(
             name='任务异常处理',
@@ -265,35 +265,35 @@
         )
 
         self.test_sql_execution = self.model(
             name='测试SQL执行任务',
             parent=self.sql_execution_parent_task,
             category=categories.system_test_category,
             config={
-                'sql': 'select * from %s limit 10;' % SystemScheduleLog._meta.db_table
+                'script': 'select * from %s limit 10;' % SystemScheduleLog._meta.db_table
             },
             user=user
         )
 
         self.test_sql_produce = self.model(
             name='测试SQL生产任务',
             parent=self.sql_produce_parent_task,
             category=categories.system_test_category,
             config={
-                'sql': 'select * from %s limit 10;' % SystemScheduleLog._meta.db_table,
+                'script': 'select * from %s limit 10;' % SystemScheduleLog._meta.db_table,
                 'queue': queues.test.code
             },
             user=user
         )
         self.test_shell_execution = self.model(
             name='测试Shell执行任务',
             parent=self.shell_execution_parent_task,
             category=categories.system_test_category,
             config={
-                'shell': 'echo "hello world"'
+                'script': 'echo "hello world"'
             },
             user=user
         )
         super(BuiltinTasks, self).__init__()
 
 
 class BuiltinSchedules(BuiltinModels):
```

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/process.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/process.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/queue.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/queue.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/serializers.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/serializers.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/urls.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task/views.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 class ScheduleProduceView(APIView):
 
     def post(self, request: Request, pk: int):
         try:
             schedule = SystemSchedule.objects.get(id=pk)
         except SystemSchedule.DoesNotExist:
             return Response({'message': 'schedule_id(%s)不存在' % pk}, status=status.HTTP_404_NOT_FOUND)
-        sql: str = schedule.task.config.get('sql', '').strip()
+        sql: str = schedule.task.config.get('script', '').strip()
         if not sql:
             return Response({'message': 'sql语句不能为空'}, status=status.HTTP_400_BAD_REQUEST)
         if not sql.startswith('select'):
             return Response({'message': 'sql语句必须以select开头'}, status=status.HTTP_400_BAD_REQUEST)
         try:
             queue = builtins.queues[schedule.task.config['queue']].queue
             max_size = schedule.task.config.get('max_size', 10000)
```

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task_execution/main.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task_execution/main.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executor.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/executor.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/base.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/executors/base.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py` & `django-common-task-system-1.2.7/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 
 class SqlExecutor(BaseExecutor):
     name = builtins.tasks.sql_execution_parent_task.name
 
     def execute(self):
         result = []
-        commands = self.schedule.task.config.get('sql', '').split(';')
+        commands = self.schedule.task.config.get('script', '').split(';')
         with connection.cursor() as cursor:
             for sql in commands:
                 sql = sql.strip()
                 if sql:
                     cmd_result = {
-                        'sql': sql,
+                        'script': sql,
                         'result': cursor.execute(sql)
                     }
                     result.append(cmd_result)
         return result
 
 
 class SqlProduceExecutor(BaseExecutor):
```

### Comparing `django-common-task-system-1.2.6/django_common_task_system/templates/admin/system_schedule/change_list.html` & `django-common-task-system-1.2.7/django_common_task_system/templates/admin/system_schedule/change_list.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/multi_day_select.html` & `django-common-task-system-1.2.7/django_common_task_system/templates/task_schedule/multi_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/multi_month_day_select.html` & `django-common-task-system-1.2.7/django_common_task_system/templates/task_schedule/multi_month_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/nlp_input.html` & `django-common-task-system-1.2.7/django_common_task_system/templates/task_schedule/nlp_input.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/templates/task_schedule/period_schedule.html` & `django-common-task-system-1.2.7/django_common_task_system/templates/task_schedule/period_schedule.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/urls.py` & `django-common-task-system-1.2.7/django_common_task_system/urls.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/utils/algorithm.py` & `django-common-task-system-1.2.7/django_common_task_system/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/utils/foreign_key.py` & `django-common-task-system-1.2.7/django_common_task_system/utils/foreign_key.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/utils/schedule_time.py` & `django-common-task-system-1.2.7/django_common_task_system/utils/schedule_time.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system/views.py` & `django-common-task-system-1.2.7/django_common_task_system/views.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/django_common_task_system.egg-info/SOURCES.txt` & `django-common-task-system-1.2.7/django_common_task_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.6/setup.py` & `django-common-task-system-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-common-task-system',
     packages=find_packages(exclude=['local_tests']),
-    version='1.2.6',
+    version='1.2.7',
     install_requires=[
         "django-common-objects>=1.0.5",
         "django>=3.2.18",
         "croniter>=1.3.8",
         "djangorestframework>=3.14.0",
         "PyMySQL>=1.0.2",
         "jionlp-time>=1.0.0",
```

