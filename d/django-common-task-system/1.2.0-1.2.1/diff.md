# Comparing `tmp/django-common-task-system-1.2.0.tar.gz` & `tmp/django-common-task-system-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-common-task-system-1.2.0.tar", last modified: Thu Apr 20 08:34:02 2023, max compression
+gzip compressed data, was "django-common-task-system-1.2.1.tar", last modified: Fri Apr 21 08:48:02 2023, max compression
```

## Comparing `django-common-task-system-1.2.0.tar` & `django-common-task-system-1.2.1.tar`

### file list

```diff
@@ -1,96 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.131681 django-common-task-system-1.2.0/
--rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      303 2023-04-20 08:34:02.130681 django-common-task-system-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.830295 django-common-task-system-1.2.0/django_common_task_system/
--rw-rw-rw-   0        0        0     3014 2023-04-17 02:45:20.000000 django-common-task-system-1.2.0/django_common_task_system/__init__.py
--rw-rw-rw-   0        0        0    10500 2023-04-19 07:34:32.000000 django-common-task-system-1.2.0/django_common_task_system/admin.py
--rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.2.0/django_common_task_system/apps.py
--rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.2.0/django_common_task_system/choices.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.2.0/django_common_task_system/fields.py
--rw-rw-rw-   0        0        0    15733 2023-04-17 08:15:48.000000 django-common-task-system-1.2.0/django_common_task_system/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.912514 django-common-task-system-1.2.0/django_common_task_system/migrations/
--rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.2.0/django_common_task_system/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.2.0/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
--rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.2.0/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
--rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.2.0/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.2.0/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.2.0/django_common_task_system/migrations/0006_consumerpermission.py
--rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.2.0/django_common_task_system/migrations/__init__.py
--rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.2.0/django_common_task_system/mixin.py
--rw-rw-rw-   0        0        0    35781 2023-04-20 05:47:24.000000 django-common-task-system-1.2.0/django_common_task_system/models.py
--rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.2.0/django_common_task_system/permissions.py
--rw-rw-rw-   0        0        0     2086 2023-04-13 06:35:40.000000 django-common-task-system-1.2.0/django_common_task_system/serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.737713 django-common-task-system-1.2.0/django_common_task_system/static/
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.737713 django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.926520 django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/css/
--rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/css/calendar.css
--rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.954514 django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/js/
--rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/js/calendar.js
--rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.008760 django-common-task-system-1.2.0/django_common_task_system/system_task/
--rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/__init__.py
--rw-rw-rw-   0        0        0     5005 2023-04-20 07:45:49.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/admin.py
--rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/apps.py
--rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/choices.py
--rw-rw-rw-   0        0        0     4130 2023-04-19 09:42:02.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.057761 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/
--rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
--rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
--rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
--rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
--rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
--rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/__init__.py
--rw-rw-rw-   0        0        0    14677 2023-04-20 05:44:40.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/models.py
--rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/process.py
--rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/queue.py
--rw-rw-rw-   0        0        0     1511 2023-04-17 03:57:06.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/serializers.py
--rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/tests.py
--rw-rw-rw-   0        0        0      771 2023-04-14 03:45:06.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/urls.py
--rw-rw-rw-   0        0        0     5308 2023-04-18 02:48:30.000000 django-common-task-system-1.2.0/django_common_task_system/system_task/views.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.059760 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     1674 2023-04-19 09:54:46.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/main.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.069174 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/
--rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/__init__.py
--rw-rw-rw-   0        0        0     2749 2023-04-19 09:51:15.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executor.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.093682 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/
--rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
--rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
--rw-rw-rw-   0        0        0     3500 2023-04-17 05:43:02.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
--rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
--rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
--rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.740710 django-common-task-system-1.2.0/django_common_task_system/templates/
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.740710 django-common-task-system-1.2.0/django_common_task_system/templates/admin/
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.094682 django-common-task-system-1.2.0/django_common_task_system/templates/admin/system_schedule/
--rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.2.0/django_common_task_system/templates/admin/system_schedule/change_list.html
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.108685 django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/
--rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/datetime_range.html
--rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/multi_day_select.html
--rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/multi_month_day_select.html
--rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/nlp_input.html
--rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/period.html
--rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/period_schedule.html
--rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.2.0/django_common_task_system/tests.py
--rw-rw-rw-   0        0        0      991 2023-04-14 03:33:36.000000 django-common-task-system-1.2.0/django_common_task_system/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.128684 django-common-task-system-1.2.0/django_common_task_system/utils/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.2.0/django_common_task_system/utils/__init__.py
--rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.2.0/django_common_task_system/utils/algorithm.py
--rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.2.0/django_common_task_system/utils/cron_utils.py
--rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.2.0/django_common_task_system/utils/foreign_key.py
--rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.2.0/django_common_task_system/utils/schedule_time.py
--rw-rw-rw-   0        0        0    11074 2023-04-20 08:31:56.000000 django-common-task-system-1.2.0/django_common_task_system/views.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:01.856425 django-common-task-system-1.2.0/django_common_task_system.egg-info/
--rw-rw-rw-   0        0        0      303 2023-04-20 08:34:01.000000 django-common-task-system-1.2.0/django_common_task_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4253 2023-04-20 08:34:01.000000 django-common-task-system-1.2.0/django_common_task_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 08:34:01.000000 django-common-task-system-1.2.0/django_common_task_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-04-20 08:34:01.000000 django-common-task-system-1.2.0/django_common_task_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-04-20 08:34:01.000000 django-common-task-system-1.2.0/django_common_task_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 08:34:02.131681 django-common-task-system-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-04-20 08:31:56.000000 django-common-task-system-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:34:02.129687 django-common-task-system-1.2.0/tests/
--rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.2.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:02.454622 django-common-task-system-1.2.1/
+-rw-rw-rw-   0        0        0     1085 2023-02-28 03:51:16.000000 django-common-task-system-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0      249 2023-03-07 02:40:16.000000 django-common-task-system-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      303 2023-04-21 08:48:02.454622 django-common-task-system-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-28 03:51:16.000000 django-common-task-system-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:01.999349 django-common-task-system-1.2.1/django_common_task_system/
+-rw-rw-rw-   0        0        0     3014 2023-04-17 02:45:20.000000 django-common-task-system-1.2.1/django_common_task_system/__init__.py
+-rw-rw-rw-   0        0        0    11044 2023-04-21 08:04:58.000000 django-common-task-system-1.2.1/django_common_task_system/admin.py
+-rw-rw-rw-   0        0        0      162 2023-03-30 02:09:33.000000 django-common-task-system-1.2.1/django_common_task_system/apps.py
+-rw-rw-rw-   0        0        0     1596 2023-04-17 06:43:49.000000 django-common-task-system-1.2.1/django_common_task_system/choices.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 02:19:10.000000 django-common-task-system-1.2.1/django_common_task_system/fields.py
+-rw-rw-rw-   0        0        0    15733 2023-04-17 08:15:48.000000 django-common-task-system-1.2.1/django_common_task_system/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:02.089636 django-common-task-system-1.2.1/django_common_task_system/migrations/
+-rw-rw-rw-   0        0        0     7826 2023-03-30 03:30:00.000000 django-common-task-system-1.2.1/django_common_task_system/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      493 2023-03-30 06:20:55.000000 django-common-task-system-1.2.1/django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
+-rw-rw-rw-   0        0        0      652 2023-03-31 03:28:46.000000 django-common-task-system-1.2.1/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
+-rw-rw-rw-   0        0        0     3283 2023-04-13 08:54:07.000000 django-common-task-system-1.2.1/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      495 2023-04-17 01:38:40.000000 django-common-task-system-1.2.1/django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1560 2023-04-17 08:33:41.000000 django-common-task-system-1.2.1/django_common_task_system/migrations/0006_consumerpermission.py
+-rw-rw-rw-   0        0        0     1275 2023-04-21 07:23:00.000000 django-common-task-system-1.2.1/django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 07:14:44.000000 django-common-task-system-1.2.1/django_common_task_system/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2679 2023-04-18 06:27:17.000000 django-common-task-system-1.2.1/django_common_task_system/mixin.py
+-rw-rw-rw-   0        0        0    36588 2023-04-21 07:09:25.000000 django-common-task-system-1.2.1/django_common_task_system/models.py
+-rw-rw-rw-   0        0        0     1010 2023-04-17 08:01:11.000000 django-common-task-system-1.2.1/django_common_task_system/permissions.py
+-rw-rw-rw-   0        0        0     2272 2023-04-21 08:20:32.000000 django-common-task-system-1.2.1/django_common_task_system/serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:01.903262 django-common-task-system-1.2.1/django_common_task_system/static/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:01.903262 django-common-task-system-1.2.1/django_common_task_system/static/common_task_system/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:02.104558 django-common-task-system-1.2.1/django_common_task_system/static/common_task_system/css/
+-rw-rw-rw-   0        0        0     2184 2023-03-06 01:34:11.000000 django-common-task-system-1.2.1/django_common_task_system/static/common_task_system/css/calendar.css
+-rw-rw-rw-   0        0        0      278 2023-03-06 01:34:11.000000 django-common-task-system-1.2.1/django_common_task_system/static/common_task_system/css/task_schedule_admin.css
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:02.146309 django-common-task-system-1.2.1/django_common_task_system/static/common_task_system/js/
+-rw-rw-rw-   0        0        0    22263 2023-03-06 02:25:03.000000 django-common-task-system-1.2.1/django_common_task_system/static/common_task_system/js/calendar.js
+-rw-rw-rw-   0        0        0     2879 2023-03-07 02:20:56.000000 django-common-task-system-1.2.1/django_common_task_system/static/common_task_system/js/task_schedule_admin.js
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:02.195922 django-common-task-system-1.2.1/django_common_task_system/system_task/
+-rw-rw-rw-   0        0        0        0 2023-04-13 02:42:52.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/__init__.py
+-rw-rw-rw-   0        0        0     5166 2023-04-21 07:14:23.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/admin.py
+-rw-rw-rw-   0        0        0      251 2023-03-31 02:24:57.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/apps.py
+-rw-rw-rw-   0        0        0      629 2023-04-14 01:40:24.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/choices.py
+-rw-rw-rw-   0        0        0     4130 2023-04-19 09:42:02.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:02.258815 django-common-task-system-1.2.1/django_common_task_system/system_task/migrations/
+-rw-rw-rw-   0        0        0    10614 2023-04-14 01:58:50.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      676 2023-04-11 02:25:48.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
+-rw-rw-rw-   0        0        0     2209 2023-04-13 05:28:04.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
+-rw-rw-rw-   0        0        0     1007 2023-04-13 08:54:07.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
+-rw-rw-rw-   0        0        0      467 2023-04-17 01:38:40.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
+-rw-rw-rw-   0        0        0     1540 2023-04-17 08:33:41.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
+-rw-rw-rw-   0        0        0     1062 2023-04-21 07:23:00.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/migrations/0007_systemexceptionreport.py
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:54:55.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/migrations/__init__.py
+-rw-rw-rw-   0        0        0    14945 2023-04-21 07:09:25.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/models.py
+-rw-rw-rw-   0        0        0     1132 2023-04-17 01:38:40.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/process.py
+-rw-rw-rw-   0        0        0     2237 2023-04-13 07:08:11.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/queue.py
+-rw-rw-rw-   0        0        0     1679 2023-04-21 07:11:39.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-03-31 01:54:55.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/tests.py
+-rw-rw-rw-   0        0        0      846 2023-04-21 07:22:44.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/urls.py
+-rw-rw-rw-   0        0        0     5505 2023-04-21 07:22:44.000000 django-common-task-system-1.2.1/django_common_task_system/system_task/views.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:02.267882 django-common-task-system-1.2.1/django_common_task_system/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 01:55:27.000000 django-common-task-system-1.2.1/django_common_task_system/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     1674 2023-04-19 09:54:46.000000 django-common-task-system-1.2.1/django_common_task_system/system_task_execution/main.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:02.279614 django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/
+-rw-rw-rw-   0        0        0        0 2023-04-04 05:08:30.000000 django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/__init__.py
+-rw-rw-rw-   0        0        0     3100 2023-04-21 07:40:43.000000 django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/executor.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:02.326488 django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/executors/
+-rw-rw-rw-   0        0        0      433 2023-04-06 08:14:13.000000 django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-04-17 01:38:40.000000 django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/executors/base.py
+-rw-rw-rw-   0        0        0     3500 2023-04-17 05:43:02.000000 django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py
+-rw-rw-rw-   0        0        0      832 2023-04-17 01:38:40.000000 django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py
+-rw-rw-rw-   0        0        0     1110 2023-04-12 09:22:44.000000 django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py
+-rw-rw-rw-   0        0        0      375 2023-04-12 09:08:53.000000 django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:01.907422 django-common-task-system-1.2.1/django_common_task_system/templates/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:01.906404 django-common-task-system-1.2.1/django_common_task_system/templates/admin/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:02.350377 django-common-task-system-1.2.1/django_common_task_system/templates/admin/system_schedule/
+-rw-rw-rw-   0        0        0     8242 2023-04-19 07:36:00.000000 django-common-task-system-1.2.1/django_common_task_system/templates/admin/system_schedule/change_list.html
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:02.421412 django-common-task-system-1.2.1/django_common_task_system/templates/task_schedule/
+-rw-rw-rw-   0        0        0      369 2023-03-02 02:43:40.000000 django-common-task-system-1.2.1/django_common_task_system/templates/task_schedule/datetime_range.html
+-rw-rw-rw-   0        0        0      594 2023-03-06 02:16:15.000000 django-common-task-system-1.2.1/django_common_task_system/templates/task_schedule/multi_day_select.html
+-rw-rw-rw-   0        0        0     3229 2023-03-06 03:09:42.000000 django-common-task-system-1.2.1/django_common_task_system/templates/task_schedule/multi_month_day_select.html
+-rw-rw-rw-   0        0        0     1391 2023-03-06 01:34:11.000000 django-common-task-system-1.2.1/django_common_task_system/templates/task_schedule/nlp_input.html
+-rw-rw-rw-   0        0        0      255 2023-03-02 09:35:44.000000 django-common-task-system-1.2.1/django_common_task_system/templates/task_schedule/period.html
+-rw-rw-rw-   0        0        0      538 2023-03-03 07:27:10.000000 django-common-task-system-1.2.1/django_common_task_system/templates/task_schedule/period_schedule.html
+-rw-rw-rw-   0        0        0       63 2023-02-28 03:52:03.000000 django-common-task-system-1.2.1/django_common_task_system/tests.py
+-rw-rw-rw-   0        0        0     1060 2023-04-21 07:22:44.000000 django-common-task-system-1.2.1/django_common_task_system/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:02.452629 django-common-task-system-1.2.1/django_common_task_system/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:07:47.000000 django-common-task-system-1.2.1/django_common_task_system/utils/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-02-17 06:35:48.000000 django-common-task-system-1.2.1/django_common_task_system/utils/algorithm.py
+-rw-rw-rw-   0        0        0      240 2023-02-16 06:57:32.000000 django-common-task-system-1.2.1/django_common_task_system/utils/cron_utils.py
+-rw-rw-rw-   0        0        0      522 2023-02-27 08:52:47.000000 django-common-task-system-1.2.1/django_common_task_system/utils/foreign_key.py
+-rw-rw-rw-   0        0        0     2015 2023-03-06 06:01:14.000000 django-common-task-system-1.2.1/django_common_task_system/utils/schedule_time.py
+-rw-rw-rw-   0        0        0    11510 2023-04-21 08:19:22.000000 django-common-task-system-1.2.1/django_common_task_system/views.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:02.029357 django-common-task-system-1.2.1/django_common_task_system.egg-info/
+-rw-rw-rw-   0        0        0      303 2023-04-21 08:48:01.000000 django-common-task-system-1.2.1/django_common_task_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4423 2023-04-21 08:48:01.000000 django-common-task-system-1.2.1/django_common_task_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:48:01.000000 django-common-task-system-1.2.1/django_common_task_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-04-21 08:48:01.000000 django-common-task-system-1.2.1/django_common_task_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-21 08:48:01.000000 django-common-task-system-1.2.1/django_common_task_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 08:48:02.455621 django-common-task-system-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-04-21 08:46:19.000000 django-common-task-system-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:48:02.453627 django-common-task-system-1.2.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-30 01:27:13.000000 django-common-task-system-1.2.1/tests/__init__.py
```

### Comparing `django-common-task-system-1.2.0/LICENSE` & `django-common-task-system-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/__init__.py` & `django-common-task-system-1.2.1/django_common_task_system/__init__.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/admin.py` & `django-common-task-system-1.2.1/django_common_task_system/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from django.contrib import admin
 from django.urls import reverse
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django_common_objects.admin import UserAdmin
 from django.db.models import Count
 from datetime import datetime
-from .choices import TaskScheduleType, ScheduleTimingType, ScheduleQueueModule
+from .choices import TaskScheduleType, ScheduleTimingType, ScheduleQueueModule, ConsumerPermissionType
 from . import models, forms, get_task_model, get_schedule_log_model
+
 TaskModel = get_task_model()
 TaskScheduleLogModel = get_schedule_log_model()
 
 
 class TaskAdmin(UserAdmin):
     schedule_model = models.TaskSchedule
 
@@ -263,25 +264,39 @@
     def task_num(self, obj):
         return self.builtins.queues.get(obj.queue.code).queue.qsize()
     task_num.short_description = '任务数量'
 
 
 class ConsumerPermissionAdmin(admin.ModelAdmin):
     form = forms.ConsumerPermissionForm
-    list_display = ('id', 'producer', 'type', 'status', 'update_time')
+    list_display = ('id', 'producer', 'type', 'summary', 'status', 'update_time')
 
     fields = (
         ('producer', 'status'),
         'type',
         'ip_whitelist',
         'config'
     )
 
+    def summary(self, obj):
+        if obj.type == ConsumerPermissionType.IP_WHITE_LIST:
+            return obj.config['ip_whitelist'][0:5]
+        return '-'
+    summary.short_description = '摘要'
+
+
+class ExceptionReportAdmin(admin.ModelAdmin):
+    list_display = ('id', 'ip', 'content', 'create_time')
+
+    def get_readonly_fields(self, request, obj=None):
+        return [field.name for field in self.model._meta.fields]
+
 
 admin.site.register(TaskModel, TaskAdmin)
 admin.site.register(models.TaskSchedule, TaskScheduleAdmin)
 admin.site.register(models.TaskScheduleCallback, TaskScheduleCallbackAdmin)
 admin.site.register(TaskScheduleLogModel, TaskScheduleLogAdmin)
 admin.site.register(models.TaskScheduleQueue, TaskScheduleQueueAdmin)
 admin.site.register(models.TaskScheduleProducer, TaskScheduleProducerAdmin)
 admin.site.register(models.ConsumerPermission, ConsumerPermissionAdmin)
+admin.site.register(models.ExceptionReport, ExceptionReportAdmin)
```

### Comparing `django-common-task-system-1.2.0/django_common_task_system/choices.py` & `django-common-task-system-1.2.1/django_common_task_system/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/fields.py` & `django-common-task-system-1.2.1/django_common_task_system/fields.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/forms.py` & `django-common-task-system-1.2.1/django_common_task_system/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/migrations/0001_initial.py` & `django-common-task-system-1.2.1/django_common_task_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py` & `django-common-task-system-1.2.1/django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py` & `django-common-task-system-1.2.1/django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/migrations/0006_consumerpermission.py` & `django-common-task-system-1.2.1/django_common_task_system/migrations/0006_consumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/mixin.py` & `django-common-task-system-1.2.1/django_common_task_system/mixin.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/models.py` & `django-common-task-system-1.2.1/django_common_task_system/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -586,14 +586,37 @@
 
 class ConsumerPermission(AbstractConsumerPermission):
     class Meta(AbstractConsumerPermission.Meta):
         db_table = 'schedule_consumer_permission'
         abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
 
 
+class AbstractExceptionReport(models.Model):
+    id = models.AutoField(primary_key=True, verbose_name='ID')
+    ip = models.CharField(max_length=100, verbose_name='IP')
+    content = models.TextField(verbose_name='内容')
+    create_time = models.DateTimeField(default=timezone.now, verbose_name='创建时间')
+
+    class Meta:
+        db_table = 'task_exception_report'
+        verbose_name = verbose_name_plural = '异常报告'
+        ordering = ('-create_time',)
+        abstract = True
+
+    def __str__(self):
+        return "Exception(%s, %s)" % (self.ip, self.content[:50])
+
+    __repr__ = __str__
+
+
+class ExceptionReport(AbstractExceptionReport):
+    class Meta(AbstractExceptionReport.Meta):
+        abstract = 'django_common_task_system' not in settings.INSTALLED_APPS
+
+
 class BuiltinModels(OrderedDict):
     model: models.Model = None
     model_unique_kwargs = []
 
     def init_object(self, obj: models.Model):
         kwargs = {
             key: getattr(obj, key) for key in self.model_unique_kwargs
```

### Comparing `django-common-task-system-1.2.0/django_common_task_system/permissions.py` & `django-common-task-system-1.2.1/django_common_task_system/permissions.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/serializers.py` & `django-common-task-system-1.2.1/django_common_task_system/serializers.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,7 +61,15 @@
 
 class TaskScheduleLogSerializer(serializers.ModelSerializer):
     schedule = serializers.PrimaryKeyRelatedField(queryset=models.TaskSchedule.objects.all())
 
     class Meta:
         model = TaskScheduleLogModel
         fields = '__all__'
+
+
+class ExceptionSerializer(serializers.ModelSerializer):
+    ip = serializers.ReadOnlyField()
+
+    class Meta:
+        model = models.ExceptionReport
+        fields = '__all__'
```

### Comparing `django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/css/calendar.css` & `django-common-task-system-1.2.1/django_common_task_system/static/common_task_system/css/calendar.css`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/js/calendar.js` & `django-common-task-system-1.2.1/django_common_task_system/static/common_task_system/js/calendar.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/static/common_task_system/js/task_schedule_admin.js` & `django-common-task-system-1.2.1/django_common_task_system/static/common_task_system/js/task_schedule_admin.js`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task/admin.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,20 +129,25 @@
 
 class SystemScheduleProducerAdmin(base_admin.TaskScheduleProducerAdmin):
     form = forms.SystemScheduleProducerForm
     schedule_get_name = 'system_schedule_get'
     builtins = models.builtins
 
 
-class ConsumerPermissionAdmin(base_admin.ConsumerPermissionAdmin):
+class SystemConsumerPermissionAdmin(base_admin.ConsumerPermissionAdmin):
+    pass
+
+
+class SystemExceptionAdmin(base_admin.ExceptionReportAdmin):
     pass
 
 
 admin.site.register(models.SystemTask, SystemTaskAdmin)
 admin.site.register(models.SystemScheduleCallback, SystemScheduleCallbackAdmin)
 admin.site.register(models.SystemSchedule, SystemScheduleAdmin)
 admin.site.register(models.SystemScheduleLog, SystemScheduleLogAdmin)
 admin.site.register(models.SystemScheduleQueue, SystemScheduleQueueAdmin)
 admin.site.register(models.SystemScheduleProducer, SystemScheduleProducerAdmin)
 admin.site.register(models.SystemProcess, SystemProcessAdmin)
-admin.site.register(models.SystemConsumerPermission, ConsumerPermissionAdmin)
+admin.site.register(models.SystemConsumerPermission, SystemConsumerPermissionAdmin)
+admin.site.register(models.SystemExceptionReport, SystemExceptionAdmin)
```

#### html2text {}

```diff
@@ -45,16 +45,19 @@
 ( 'æ¥çæ¥å¿' % url ) show_log.short_description = 'æ¥å¿' def
 has_delete_permission(self, request, obj=None): return False class
 SystemScheduleQueueAdmin(base_admin.TaskScheduleQueueAdmin): form =
 forms.SystemScheduleQueueForm builtins = models.builtins schedule_get_name =
 'system_schedule_get' class SystemScheduleProducerAdmin
 (base_admin.TaskScheduleProducerAdmin): form = forms.SystemScheduleProducerForm
 schedule_get_name = 'system_schedule_get' builtins = models.builtins class
-ConsumerPermissionAdmin(base_admin.ConsumerPermissionAdmin): pass
-admin.site.register(models.SystemTask, SystemTaskAdmin) admin.site.register
+SystemConsumerPermissionAdmin(base_admin.ConsumerPermissionAdmin): pass class
+SystemExceptionAdmin(base_admin.ExceptionReportAdmin): pass admin.site.register
+(models.SystemTask, SystemTaskAdmin) admin.site.register
 (models.SystemScheduleCallback, SystemScheduleCallbackAdmin)
 admin.site.register(models.SystemSchedule, SystemScheduleAdmin)
 admin.site.register(models.SystemScheduleLog, SystemScheduleLogAdmin)
 admin.site.register(models.SystemScheduleQueue, SystemScheduleQueueAdmin)
 admin.site.register(models.SystemScheduleProducer, SystemScheduleProducerAdmin)
 admin.site.register(models.SystemProcess, SystemProcessAdmin)
-admin.site.register(models.SystemConsumerPermission, ConsumerPermissionAdmin)
+admin.site.register(models.SystemConsumerPermission,
+SystemConsumerPermissionAdmin) admin.site.register
+(models.SystemExceptionReport, SystemExceptionAdmin)
```

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task/choices.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task/choices.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task/forms.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task/forms.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0001_initial.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task/models.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.db import models
 from django.conf import settings
 from django_common_task_system.choices import ScheduleQueueModule, TaskScheduleStatus, ConsumerPermissionType
 from django_common_task_system.models import (
     AbstractTask, AbstractTaskSchedule, AbstractTaskScheduleLog, TaskScheduleLog, AbstractScheduleCallback, 
-    AbstractTaskScheduleProducer, AbstractTaskScheduleQueue, AbstractConsumerPermission, 
-    BaseBuiltinQueues, BaseBuiltinProducers, BaseConsumerPermissions, BaseBuiltins, 
+    AbstractTaskScheduleProducer, AbstractTaskScheduleQueue, AbstractConsumerPermission, AbstractExceptionReport,
+    BaseBuiltinQueues, BaseBuiltinProducers, BaseConsumerPermissions, BaseBuiltins,
     BuiltinModels
 )
 from django_common_objects.models import CommonCategory
 from django.contrib.auth import get_user_model
 
 User = get_user_model()
 
@@ -85,14 +85,21 @@
                                  on_delete=models.CASCADE, verbose_name='生产者')
 
     class Meta(AbstractConsumerPermission.Meta):
         db_table = 'system_consumer_permission'
         abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
 
 
+class SystemExceptionReport(AbstractExceptionReport):
+
+    class Meta(AbstractExceptionReport.Meta):
+        db_table = 'system_exception_report'
+        abstract = 'django_common_task_system.system_task' not in settings.INSTALLED_APPS
+
+
 class SystemProcess(models.Model):
     id = models.AutoField(primary_key=True, verbose_name='ID')
     process_id = models.PositiveIntegerField(verbose_name='进程ID', unique=True)
     process_name = models.CharField(max_length=100, verbose_name='进程名称')
     env = models.CharField(max_length=500, verbose_name='环境变量', blank=True, null=True)
     status = models.BooleanField(default=True, verbose_name='状态')
     log_file = models.CharField(max_length=200, verbose_name='日志文件')
```

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task/process.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task/process.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task/queue.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task/queue.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task/serializers.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,7 +40,13 @@
 
 
 class TaskScheduleLogSerializer(serializers.TaskScheduleLogSerializer):
     schedule = PrimaryKeyRelatedField(queryset=models.SystemSchedule.objects.all())
 
     class Meta(serializers.TaskScheduleLogSerializer.Meta):
         model = models.SystemScheduleLog
+
+
+class ExceptionSerializer(serializers.ExceptionSerializer):
+
+    class Meta(serializers.ExceptionSerializer.Meta):
+        model = models.SystemExceptionReport
```

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task/urls.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task/urls.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,8 +6,9 @@
     path('schedule/produce/<int:pk>/', views.ScheduleProduceView.as_view(), name='system_schedule_produce'),
     path('schedule/queue/<slug:code>/get/', views.SystemScheduleQueueAPI.get, name='system_schedule_get'),
     path('schedule/put/', views.SystemScheduleQueueAPI.put, name='system_schedule_put'),
     path('schedule/retry/', views.SystemScheduleQueueAPI.retry, name='system_schedule_retry'),
     path('schedule/queue/status/', views.SystemScheduleQueueAPI.status),
     path('process/logs/<int:process_id>/', views.SystemProcessView.show_logs, name='system_process_log'),
     path('process/stop/<int:process_id>/', views.SystemProcessView.stop_process, name='system_process_stop'),
+    path('exception/report/', views.SystemExceptionReportView.as_view()),
 ]
```

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task/views.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from rest_framework.response import Response
 from rest_framework.views import APIView
 from rest_framework.request import Request
 from rest_framework import status
 from django.db.models.signals import post_save, post_delete
 from django.db import connection
 from django.http.response import HttpResponse
-from django_common_task_system.models import system_initialize_signal, system_schedule_event
+from django_common_task_system.models import system_initialize_signal
 from .models import SystemScheduleQueue, SystemSchedule, \
-    SystemProcess, SystemScheduleProducer, SystemScheduleLog, SystemConsumerPermission
-from django_common_task_system.views import TaskScheduleQueueAPI, TaskScheduleThread
+    SystemProcess, SystemScheduleProducer, SystemScheduleLog, SystemConsumerPermission, SystemExceptionReport
+from django_common_task_system.views import TaskScheduleQueueAPI, TaskScheduleThread, ExceptionReportView
 from .models import builtins
-from .serializers import QueueScheduleSerializer
+from .serializers import QueueScheduleSerializer, ExceptionSerializer
 import os
 
 
 builtins.initialize()
 
 
 class SystemScheduleThread(TaskScheduleThread):
@@ -125,7 +125,12 @@
         try:
             process = SystemProcess.objects.get(process_id=process_id)
         except SystemProcess.DoesNotExist:
             return HttpResponse('SystemProcess(%s)不存在' % process_id)
         process.delete()
         return HttpResponse('SystemProcess(%s)已停止' % process_id)
 
+
+class SystemExceptionReportView(ExceptionReportView):
+
+    queryset = SystemExceptionReport.objects.all()
+    serializer_class = ExceptionSerializer
```

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task_execution/main.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task_execution/main.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executor.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import os
 import time
+import traceback
+import socket
 import requests
 from queue import Queue
 from datetime import datetime
 from django.urls import reverse
 from .executors import Executors
 from . import settings
 from urllib.parse import urljoin
-from django_common_task_system.system_task.models import SystemSchedule, SystemTask, builtins
+from django_common_task_system.system_task.models import SystemSchedule, SystemTask, builtins, SystemExceptionReport
 from django_common_task_system.models import TaskScheduleCallback
 
 
+IP = socket.gethostbyname(socket.gethostname())
 system_task_queue = Queue()
 logger = settings.logger
 
 
 def request_system_schedule(url):
     response = requests.get(url)
     if response.status_code == 200:
@@ -79,7 +82,14 @@
     while True:
         try:
             schedule = get_system_schedule(consumer_url)
             logger.info('get system schedule: %s', schedule)
             run(schedule)
         except Exception as e:
             logger.exception(e)
+            try:
+                SystemExceptionReport.objects.create(
+                    ip=IP,
+                    content=traceback.format_exc(),
+                )
+            except Exception as e:
+                logger.exception(e)
```

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/base.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/executors/base.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/executors/exception.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/executors/shell.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py` & `django-common-task-system-1.2.1/django_common_task_system/system_task_execution/system_task_execution/executors/sql.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/templates/admin/system_schedule/change_list.html` & `django-common-task-system-1.2.1/django_common_task_system/templates/admin/system_schedule/change_list.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/multi_day_select.html` & `django-common-task-system-1.2.1/django_common_task_system/templates/task_schedule/multi_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/multi_month_day_select.html` & `django-common-task-system-1.2.1/django_common_task_system/templates/task_schedule/multi_month_day_select.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/nlp_input.html` & `django-common-task-system-1.2.1/django_common_task_system/templates/task_schedule/nlp_input.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/templates/task_schedule/period_schedule.html` & `django-common-task-system-1.2.1/django_common_task_system/templates/task_schedule/period_schedule.html`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/urls.py` & `django-common-task-system-1.2.1/django_common_task_system/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,9 @@
     path('schedule/retry/', views.TaskScheduleQueueAPI.retry, name='task_schedule_retry'),
     path('schedule/put/', views.TaskScheduleQueueAPI.put, name='task_schedule_put'),
     path('schedule/detail/<int:pk>/', views.TaskScheduleDetailView.as_view()),
     path('schedule/queue/<slug:code>/get/', views.TaskScheduleQueueAPI.get, name='task_schedule_get'),
     path('schedule/queue/detail/<int:pk>/', views.TaskScheduleQueueAPI.get_by_id),
     path('schedule/queue/status/', views.TaskScheduleQueueAPI.status),
     path('schedule/time-parse/', views.ScheduleTimeParseView.as_view()),
+    path('exception/report/', views.ExceptionReportView.as_view()),
 ] + router.urls
```

### Comparing `django-common-task-system-1.2.0/django_common_task_system/utils/algorithm.py` & `django-common-task-system-1.2.1/django_common_task_system/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/utils/foreign_key.py` & `django-common-task-system-1.2.1/django_common_task_system/utils/foreign_key.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/utils/schedule_time.py` & `django-common-task-system-1.2.1/django_common_task_system/utils/schedule_time.py`

 * *Files identical despite different names*

### Comparing `django-common-task-system-1.2.0/django_common_task_system/views.py` & `django-common-task-system-1.2.1/django_common_task_system/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from django.db.models.signals import post_delete, post_save
 from django.dispatch import receiver
 from rest_framework import status
 from rest_framework.decorators import api_view
+from rest_framework.generics import CreateAPIView
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.views import APIView
 from rest_framework.viewsets import ModelViewSet
 from django.http.response import JsonResponse
 from . import serializers, get_task_model, get_schedule_log_model, get_task_schedule_model, get_task_schedule_serializer
 from .choices import TaskScheduleStatus
-from .models import TaskSchedule, TaskScheduleProducer, TaskScheduleQueue, ConsumerPermission, builtins, ScheduleConfig
+from .models import TaskSchedule, TaskScheduleProducer, TaskScheduleQueue, \
+    ConsumerPermission, ExceptionReport, builtins, ScheduleConfig
 from django_common_objects.rest_view import UserListAPIView, UserRetrieveAPIView
 from queue import Empty
 from datetime import datetime
 from jionlp_time import parse_time
 from .utils.schedule_time import nlp_config_to_schedule_config
 from .models import system_initialize_signal, system_schedule_event
 from threading import Thread
@@ -43,15 +45,15 @@
         for producer in self.producers.values():
             queue = self.queues[producer.queue.code]
             # 队列长度大于1000时不再生产, 防止内存溢出
             if queue.queue.qsize() > 1000:
                 continue
             queryset = self.schedule_model.objects.filter(**producer.filters)
             if producer.lte_now:
-                queryset = queryset.filter(next_schedule_time__lte=datetime.now())
+                queryset = queryset.filter(next_schedule_time__lte=now)
             for schedule in queryset:
                 try:
                     while schedule.next_schedule_time <= now:
                         data = self.serializer(schedule).data
                         data['queue'] = queue.code
                         queue.queue.put(data)
                         schedule.next_schedule_time = ScheduleConfig(config=schedule.config
@@ -253,7 +255,17 @@
             schedule = nlp_config_to_schedule_config(result, sentence=sentence)
             return Response({
                 "jio_result": result,
                 "schedule": schedule
             })
         except Exception as e:
             return Response({'error': str(e)}, status=status.HTTP_500_INTERNAL_SERVER_ERROR)
+
+
+class ExceptionReportView(CreateAPIView):
+    queryset = ExceptionReport.objects.all()
+    serializer_class = serializers.ExceptionSerializer
+
+    def perform_create(self, serializer):
+        meta = self.request.META
+        ip = meta.get('HTTP_X_FORWARDED_FOR') if meta.get('HTTP_X_FORWARDED_FOR') else meta.get('REMOTE_ADDR')
+        serializer.save(ip=ip)
```

### Comparing `django-common-task-system-1.2.0/django_common_task_system.egg-info/SOURCES.txt` & `django-common-task-system-1.2.1/django_common_task_system.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 django_common_task_system.egg-info/top_level.txt
 django_common_task_system/migrations/0001_initial.py
 django_common_task_system/migrations/0002_alter_taskschedule_unique_together.py
 django_common_task_system/migrations/0003_alter_taskschedulelog_schedule.py
 django_common_task_system/migrations/0004_taskschedulequeue_taskschedulelog_queue_and_more.py
 django_common_task_system/migrations/0005_alter_taskscheduleproducer_name.py
 django_common_task_system/migrations/0006_consumerpermission.py
+django_common_task_system/migrations/0007_exceptionreport_alter_taskschedulelog_options.py
 django_common_task_system/migrations/__init__.py
 django_common_task_system/static/common_task_system/css/calendar.css
 django_common_task_system/static/common_task_system/css/task_schedule_admin.css
 django_common_task_system/static/common_task_system/js/calendar.js
 django_common_task_system/static/common_task_system/js/task_schedule_admin.js
 django_common_task_system/system_task/__init__.py
 django_common_task_system/system_task/admin.py
@@ -45,14 +46,15 @@
 django_common_task_system/system_task/views.py
 django_common_task_system/system_task/migrations/0001_initial.py
 django_common_task_system/system_task/migrations/0002_remove_systemtask_task_type_systemtask_tags.py
 django_common_task_system/system_task/migrations/0003_systemschedulequeue_config_and_more.py
 django_common_task_system/system_task/migrations/0004_systemschedulelog_queue_and_more.py
 django_common_task_system/system_task/migrations/0005_alter_systemscheduleproducer_name.py
 django_common_task_system/system_task/migrations/0006_systemconsumerpermission.py
+django_common_task_system/system_task/migrations/0007_systemexceptionreport.py
 django_common_task_system/system_task/migrations/__init__.py
 django_common_task_system/system_task_execution/__init__.py
 django_common_task_system/system_task_execution/main.py
 django_common_task_system/system_task_execution/system_task_execution/__init__.py
 django_common_task_system/system_task_execution/system_task_execution/executor.py
 django_common_task_system/system_task_execution/system_task_execution/settings.py
 django_common_task_system/system_task_execution/system_task_execution/executors/__init__.py
```

### Comparing `django-common-task-system-1.2.0/setup.py` & `django-common-task-system-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-common-task-system',
     packages=find_packages(exclude=['local_tests']),
-    version='1.2.0',
+    version='1.2.1',
     install_requires=[
         "django-common-objects>=1.0.5",
         "django>=3.2.18",
         "croniter>=1.3.8",
         "djangorestframework>=3.14.0",
         "PyMySQL>=1.0.2",
         "jionlp-time>=1.0.0",
```

