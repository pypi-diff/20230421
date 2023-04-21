# Comparing `tmp/django-seeker-7.3.0.tar.gz` & `tmp/django-seeker-7.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-seeker-7.3.0.tar", last modified: Wed Feb  8 16:11:04 2023, max compression
+gzip compressed data, was "django-seeker-7.3.1.tar", last modified: Fri Apr 21 13:48:16 2023, max compression
```

## Comparing `django-seeker-7.3.0.tar` & `django-seeker-7.3.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-08 16:11:04.546478 django-seeker-7.3.0/
--rw-rw----   0 ruttenb   (1328) ims        (100)     1316 2018-10-01 19:52:22.000000 django-seeker-7.3.0/LICENSE
--rw-rw----   0 ruttenb   (1328) ims        (100)       38 2018-10-01 19:52:22.000000 django-seeker-7.3.0/MANIFEST.in
--rw-r--r--   0 ruttenb   (1328) ims        (100)      589 2023-02-08 16:11:04.548472 django-seeker-7.3.0/PKG-INFO
--rw-rw----   0 ruttenb   (1328) ims        (100)      249 2018-10-01 19:52:22.000000 django-seeker-7.3.0/README.md
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-08 16:11:04.248461 django-seeker-7.3.0/django_seeker.egg-info/
--rw-rw----   0 ruttenb   (1328) ims        (100)      589 2023-02-08 16:11:02.000000 django-seeker-7.3.0/django_seeker.egg-info/PKG-INFO
--rw-rw----   0 ruttenb   (1328) ims        (100)     2086 2023-02-08 16:11:03.000000 django-seeker-7.3.0/django_seeker.egg-info/SOURCES.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)        1 2023-02-08 16:11:02.000000 django-seeker-7.3.0/django_seeker.egg-info/dependency_links.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)       70 2023-02-08 16:11:03.000000 django-seeker-7.3.0/django_seeker.egg-info/requires.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)        7 2023-02-08 16:11:03.000000 django-seeker-7.3.0/django_seeker.egg-info/top_level.txt
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-08 16:11:04.320462 django-seeker-7.3.0/seeker/
--rw-r--r--   0 ruttenb   (1328) ims        (100)      599 2023-02-08 16:10:52.000000 django-seeker-7.3.0/seeker/__init__.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      564 2019-04-26 17:33:41.000000 django-seeker-7.3.0/seeker/admin.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     2945 2019-06-18 15:37:07.000000 django-seeker-7.3.0/seeker/apps.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     1024 2023-02-08 16:06:40.000000 django-seeker-7.3.0/seeker/dsl.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)    25148 2023-02-08 16:06:40.000000 django-seeker-7.3.0/seeker/facets.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     1630 2019-02-08 19:43:15.000000 django-seeker-7.3.0/seeker/forms.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     2078 2019-10-10 15:12:29.000000 django-seeker-7.3.0/seeker/indexer.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-08 16:11:04.343474 django-seeker-7.3.0/seeker/management/
--rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.3.0/seeker/management/__init__.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-08 16:11:04.364466 django-seeker-7.3.0/seeker/management/commands/
--rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.3.0/seeker/management/commands/__init__.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     2295 2023-02-08 16:06:40.000000 django-seeker-7.3.0/seeker/management/commands/dropindex.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     1188 2023-02-08 16:06:40.000000 django-seeker-7.3.0/seeker/management/commands/dumpindex.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     1275 2023-02-08 16:06:40.000000 django-seeker-7.3.0/seeker/management/commands/loadindex.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     4026 2023-02-08 16:06:40.000000 django-seeker-7.3.0/seeker/management/commands/reindex.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)    11740 2023-02-08 16:06:40.000000 django-seeker-7.3.0/seeker/mapping.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     1016 2019-06-18 15:37:07.000000 django-seeker-7.3.0/seeker/middleware.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-08 16:11:04.397463 django-seeker-7.3.0/seeker/migrations/
--rw-rw----   0 ruttenb   (1328) ims        (100)     1193 2019-06-18 15:37:07.000000 django-seeker-7.3.0/seeker/migrations/0001_initial.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      499 2018-10-01 19:52:22.000000 django-seeker-7.3.0/seeker/migrations/0002_auto_20150507_0134.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      838 2018-10-01 19:52:32.000000 django-seeker-7.3.0/seeker/migrations/0003_auto_20180214_1501.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      971 2018-10-01 19:52:32.000000 django-seeker-7.3.0/seeker/migrations/0004_auto_20180322_1412.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      457 2018-10-01 19:52:32.000000 django-seeker-7.3.0/seeker/migrations/0005_auto_20180330_1708.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      714 2019-06-25 20:26:14.000000 django-seeker-7.3.0/seeker/migrations/0006_auto_20190625_1139.py
--rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.3.0/seeker/migrations/__init__.py
--rw-rw----   0 ruttenb   (1328) ims        (100)     1602 2020-10-14 20:36:41.000000 django-seeker-7.3.0/seeker/models.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      877 2021-09-01 20:33:51.000000 django-seeker-7.3.0/seeker/registry.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)      823 2022-12-15 21:11:12.000000 django-seeker-7.3.0/seeker/signals.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-08 16:11:04.172462 django-seeker-7.3.0/seeker/templates/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-08 16:11:04.439464 django-seeker-7.3.0/seeker/templates/advanced_seeker/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-08 16:11:04.461469 django-seeker-7.3.0/seeker/templates/advanced_seeker/facets/
--rw-rw----   0 ruttenb   (1328) ims        (100)      628 2018-10-01 19:52:32.000000 django-seeker-7.3.0/seeker/templates/advanced_seeker/facets/date_range.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      444 2018-10-01 19:52:32.000000 django-seeker-7.3.0/seeker/templates/advanced_seeker/facets/range.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      218 2018-10-01 19:52:32.000000 django-seeker-7.3.0/seeker/templates/advanced_seeker/facets/terms.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      306 2019-03-14 18:04:52.000000 django-seeker-7.3.0/seeker/templates/advanced_seeker/facets/text.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      218 2018-10-01 19:52:32.000000 django-seeker-7.3.0/seeker/templates/advanced_seeker/facets/year_histogram.html
--rw-r--r--   0 ruttenb   (1328) ims        (100)     2561 2022-12-15 21:11:12.000000 django-seeker-7.3.0/seeker/templates/advanced_seeker/footer.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      243 2018-10-01 19:52:32.000000 django-seeker-7.3.0/seeker/templates/advanced_seeker/header.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      854 2019-10-17 18:45:08.000000 django-seeker-7.3.0/seeker/templates/advanced_seeker/pager.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     2428 2019-09-23 17:53:11.000000 django-seeker-7.3.0/seeker/templates/advanced_seeker/results.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      465 2018-10-01 19:52:32.000000 django-seeker-7.3.0/seeker/templates/advanced_seeker/save_form.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     1341 2018-10-01 19:52:32.000000 django-seeker-7.3.0/seeker/templates/advanced_seeker/seeker.html
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-08 16:11:04.500463 django-seeker-7.3.0/seeker/templates/seeker/
--rw-rw----   0 ruttenb   (1328) ims        (100)      267 2019-09-23 17:53:11.000000 django-seeker-7.3.0/seeker/templates/seeker/column.html
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-08 16:11:04.517468 django-seeker-7.3.0/seeker/templates/seeker/facets/
--rw-rw----   0 ruttenb   (1328) ims        (100)      476 2018-10-01 19:52:22.000000 django-seeker-7.3.0/seeker/templates/seeker/facets/range.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      477 2018-10-01 19:52:22.000000 django-seeker-7.3.0/seeker/templates/seeker/facets/terms.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      184 2019-03-14 18:04:52.000000 django-seeker-7.3.0/seeker/templates/seeker/facets/text.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      508 2018-10-01 19:52:22.000000 django-seeker-7.3.0/seeker/templates/seeker/facets/year_histogram.html
--rw-r--r--   0 ruttenb   (1328) ims        (100)      832 2022-12-15 21:11:12.000000 django-seeker-7.3.0/seeker/templates/seeker/footer.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     2059 2019-08-29 20:00:08.000000 django-seeker-7.3.0/seeker/templates/seeker/form.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     1185 2018-10-01 19:52:32.000000 django-seeker-7.3.0/seeker/templates/seeker/header.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      768 2018-10-01 19:52:22.000000 django-seeker-7.3.0/seeker/templates/seeker/pager.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     1867 2018-10-01 19:52:22.000000 django-seeker-7.3.0/seeker/templates/seeker/results.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     1556 2018-10-01 19:52:22.000000 django-seeker-7.3.0/seeker/templates/seeker/save.html
--rw-rw----   0 ruttenb   (1328) ims        (100)      228 2018-10-01 19:52:22.000000 django-seeker-7.3.0/seeker/templates/seeker/score.html
--rw-rw----   0 ruttenb   (1328) ims        (100)     1299 2019-08-29 20:00:08.000000 django-seeker-7.3.0/seeker/templates/seeker/seeker.html
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-02-08 16:11:04.542470 django-seeker-7.3.0/seeker/templatetags/
--rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.3.0/seeker/templatetags/__init__.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     4044 2022-12-15 21:11:12.000000 django-seeker-7.3.0/seeker/templatetags/seeker.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)     7165 2023-02-08 16:06:40.000000 django-seeker-7.3.0/seeker/utils.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)    86043 2023-02-08 16:06:40.000000 django-seeker-7.3.0/seeker/views.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      418 2023-02-08 16:11:04.551465 django-seeker-7.3.0/setup.cfg
--rw-r--r--   0 ruttenb   (1328) ims        (100)     1048 2023-02-08 16:06:40.000000 django-seeker-7.3.0/setup.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:16.218403 django-seeker-7.3.1/
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1316 2018-10-01 19:52:22.000000 django-seeker-7.3.1/LICENSE
+-rw-rw----   0 ruttenb   (1328) ims        (100)       38 2018-10-01 19:52:22.000000 django-seeker-7.3.1/MANIFEST.in
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      589 2023-04-21 13:48:16.219405 django-seeker-7.3.1/PKG-INFO
+-rw-rw----   0 ruttenb   (1328) ims        (100)      249 2018-10-01 19:52:22.000000 django-seeker-7.3.1/README.md
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:15.756385 django-seeker-7.3.1/django_seeker.egg-info/
+-rw-rw----   0 ruttenb   (1328) ims        (100)      589 2023-04-21 13:48:10.000000 django-seeker-7.3.1/django_seeker.egg-info/PKG-INFO
+-rw-rw----   0 ruttenb   (1328) ims        (100)     2086 2023-04-21 13:48:10.000000 django-seeker-7.3.1/django_seeker.egg-info/SOURCES.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)        1 2023-04-21 13:48:10.000000 django-seeker-7.3.1/django_seeker.egg-info/dependency_links.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)       70 2023-04-21 13:48:10.000000 django-seeker-7.3.1/django_seeker.egg-info/requires.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)        7 2023-04-21 13:48:10.000000 django-seeker-7.3.1/django_seeker.egg-info/top_level.txt
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:15.917385 django-seeker-7.3.1/seeker/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      599 2023-04-21 13:46:11.000000 django-seeker-7.3.1/seeker/__init__.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      564 2019-04-26 17:33:41.000000 django-seeker-7.3.1/seeker/admin.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)     2945 2019-06-18 15:37:07.000000 django-seeker-7.3.1/seeker/apps.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     1024 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/dsl.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    25148 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/facets.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1630 2019-02-08 19:43:15.000000 django-seeker-7.3.1/seeker/forms.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)     2078 2019-10-10 15:12:29.000000 django-seeker-7.3.1/seeker/indexer.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:15.975391 django-seeker-7.3.1/seeker/management/
+-rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/management/__init__.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:15.998383 django-seeker-7.3.1/seeker/management/commands/
+-rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/management/commands/__init__.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     2295 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/management/commands/dropindex.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     1188 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/management/commands/dumpindex.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     1275 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/management/commands/loadindex.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     4026 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/management/commands/reindex.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    11740 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/mapping.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1016 2019-06-18 15:37:07.000000 django-seeker-7.3.1/seeker/middleware.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:16.063384 django-seeker-7.3.1/seeker/migrations/
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1193 2019-06-18 15:37:07.000000 django-seeker-7.3.1/seeker/migrations/0001_initial.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      499 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/migrations/0002_auto_20150507_0134.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      838 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/migrations/0003_auto_20180214_1501.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      971 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/migrations/0004_auto_20180322_1412.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      457 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/migrations/0005_auto_20180330_1708.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      714 2019-06-25 20:26:14.000000 django-seeker-7.3.1/seeker/migrations/0006_auto_20190625_1139.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/migrations/__init__.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1602 2020-10-14 20:36:41.000000 django-seeker-7.3.1/seeker/models.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      877 2021-09-01 20:33:51.000000 django-seeker-7.3.1/seeker/registry.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      823 2022-12-15 21:11:12.000000 django-seeker-7.3.1/seeker/signals.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:15.680394 django-seeker-7.3.1/seeker/templates/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:16.092401 django-seeker-7.3.1/seeker/templates/advanced_seeker/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:16.119386 django-seeker-7.3.1/seeker/templates/advanced_seeker/facets/
+-rw-rw----   0 ruttenb   (1328) ims        (100)      628 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/facets/date_range.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      444 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/facets/range.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      218 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/facets/terms.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      306 2019-03-14 18:04:52.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/facets/text.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      218 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/facets/year_histogram.html
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     2561 2022-12-15 21:11:12.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/footer.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      243 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/header.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      854 2019-10-17 18:45:08.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/pager.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     2428 2019-09-23 17:53:11.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/results.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      465 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/save_form.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1341 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/advanced_seeker/seeker.html
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:16.183393 django-seeker-7.3.1/seeker/templates/seeker/
+-rw-rw----   0 ruttenb   (1328) ims        (100)      267 2019-09-23 17:53:11.000000 django-seeker-7.3.1/seeker/templates/seeker/column.html
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:16.204383 django-seeker-7.3.1/seeker/templates/seeker/facets/
+-rw-rw----   0 ruttenb   (1328) ims        (100)      476 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templates/seeker/facets/range.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      477 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templates/seeker/facets/terms.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      184 2019-03-14 18:04:52.000000 django-seeker-7.3.1/seeker/templates/seeker/facets/text.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      508 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templates/seeker/facets/year_histogram.html
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      832 2022-12-15 21:11:12.000000 django-seeker-7.3.1/seeker/templates/seeker/footer.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     2059 2019-08-29 20:00:08.000000 django-seeker-7.3.1/seeker/templates/seeker/form.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1185 2018-10-01 19:52:32.000000 django-seeker-7.3.1/seeker/templates/seeker/header.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      768 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templates/seeker/pager.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1867 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templates/seeker/results.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1556 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templates/seeker/save.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)      228 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templates/seeker/score.html
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1299 2019-08-29 20:00:08.000000 django-seeker-7.3.1/seeker/templates/seeker/seeker.html
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2023-04-21 13:48:16.213406 django-seeker-7.3.1/seeker/templatetags/
+-rw-rw----   0 ruttenb   (1328) ims        (100)        0 2018-10-01 19:52:22.000000 django-seeker-7.3.1/seeker/templatetags/__init__.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     4044 2022-12-15 21:11:12.000000 django-seeker-7.3.1/seeker/templatetags/seeker.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     7197 2023-04-21 13:46:11.000000 django-seeker-7.3.1/seeker/utils.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    86043 2023-02-08 16:06:40.000000 django-seeker-7.3.1/seeker/views.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      418 2023-04-21 13:48:16.227386 django-seeker-7.3.1/setup.cfg
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     1048 2023-02-08 16:06:40.000000 django-seeker-7.3.1/setup.py
```

### Comparing `django-seeker-7.3.0/LICENSE` & `django-seeker-7.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/PKG-INFO` & `django-seeker-7.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-seeker
-Version: 7.3.0
+Version: 7.3.1
 Summary: A python package for mapping and querying Django models in Elasticsearch/OpenSearch.
 Home-page: https://github.com/imsweb/django-seeker
 Author: Dan Watson
 Author-email: watsond@imsweb.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-seeker-7.3.0/django_seeker.egg-info/PKG-INFO` & `django-seeker-7.3.1/django_seeker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-seeker
-Version: 7.3.0
+Version: 7.3.1
 Summary: A python package for mapping and querying Django models in Elasticsearch/OpenSearch.
 Home-page: https://github.com/imsweb/django-seeker
 Author: Dan Watson
 Author-email: watsond@imsweb.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-seeker-7.3.0/django_seeker.egg-info/SOURCES.txt` & `django-seeker-7.3.1/django_seeker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/__init__.py` & `django-seeker-7.3.1/seeker/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '7.3.0'
+__version__ = '7.3.1'
 
 from .facets import DateRangeFacet, DateTermsFacet, Facet, GlobalTermsFacet, RangeFilter, TermsFacet, YearHistogram, TextFacet
 from .mapping import (
     build_mapping, deep_field_factory, DEFAULT_ANALYZER, document_field, document_from_model, Indexable, index_factory, ModelIndex,
     RawMultiString, RawString)
 from .registry import app_documents, documents, model_documents, register
 from .utils import delete, index, search
```

### Comparing `django-seeker-7.3.0/seeker/admin.py` & `django-seeker-7.3.1/seeker/admin.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/apps.py` & `django-seeker-7.3.1/seeker/apps.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/dsl.py` & `django-seeker-7.3.1/seeker/dsl.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/facets.py` & `django-seeker-7.3.1/seeker/facets.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/forms.py` & `django-seeker-7.3.1/seeker/forms.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/indexer.py` & `django-seeker-7.3.1/seeker/indexer.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/management/commands/dropindex.py` & `django-seeker-7.3.1/seeker/management/commands/dropindex.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/management/commands/dumpindex.py` & `django-seeker-7.3.1/seeker/management/commands/dumpindex.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/management/commands/loadindex.py` & `django-seeker-7.3.1/seeker/management/commands/loadindex.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/management/commands/reindex.py` & `django-seeker-7.3.1/seeker/management/commands/reindex.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/mapping.py` & `django-seeker-7.3.1/seeker/mapping.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/middleware.py` & `django-seeker-7.3.1/seeker/middleware.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/migrations/0001_initial.py` & `django-seeker-7.3.1/seeker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/migrations/0003_auto_20180214_1501.py` & `django-seeker-7.3.1/seeker/migrations/0003_auto_20180214_1501.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/migrations/0004_auto_20180322_1412.py` & `django-seeker-7.3.1/seeker/migrations/0004_auto_20180322_1412.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/migrations/0006_auto_20190625_1139.py` & `django-seeker-7.3.1/seeker/migrations/0006_auto_20190625_1139.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/models.py` & `django-seeker-7.3.1/seeker/models.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/registry.py` & `django-seeker-7.3.1/seeker/registry.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/signals.py` & `django-seeker-7.3.1/seeker/signals.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/templates/advanced_seeker/facets/date_range.html` & `django-seeker-7.3.1/seeker/templates/advanced_seeker/facets/date_range.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/templates/advanced_seeker/footer.html` & `django-seeker-7.3.1/seeker/templates/advanced_seeker/footer.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/templates/advanced_seeker/pager.html` & `django-seeker-7.3.1/seeker/templates/advanced_seeker/pager.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/templates/advanced_seeker/results.html` & `django-seeker-7.3.1/seeker/templates/advanced_seeker/results.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/templates/advanced_seeker/seeker.html` & `django-seeker-7.3.1/seeker/templates/advanced_seeker/seeker.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/templates/seeker/footer.html` & `django-seeker-7.3.1/seeker/templates/seeker/footer.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/templates/seeker/form.html` & `django-seeker-7.3.1/seeker/templates/seeker/form.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/templates/seeker/header.html` & `django-seeker-7.3.1/seeker/templates/seeker/header.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/templates/seeker/pager.html` & `django-seeker-7.3.1/seeker/templates/seeker/pager.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/templates/seeker/results.html` & `django-seeker-7.3.1/seeker/templates/seeker/results.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/templates/seeker/save.html` & `django-seeker-7.3.1/seeker/templates/seeker/save.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/templates/seeker/seeker.html` & `django-seeker-7.3.1/seeker/templates/seeker/seeker.html`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/templatetags/seeker.py` & `django-seeker-7.3.1/seeker/templatetags/seeker.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/seeker/utils.py` & `django-seeker-7.3.1/seeker/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,20 +50,21 @@
 def index(obj, index=None, using=None):
     """
     Shortcut to index a Django object based on it's model class.
     """
     from django.contrib.contenttypes.models import ContentType
     model_class = ContentType.objects.get_for_model(obj).model_class()
     for doc_class in model_documents.get(model_class, []):
-        if not doc_class.queryset().filter(pk=obj.pk).exists():
+        instance = doc_class.queryset().filter(pk=obj.pk).first()
+        if not instance:
             continue
         doc_using = using or doc_class._index._using or 'default'
         doc_index = index or doc_class._index._name
         connection = connections.get_connection(doc_using)
-        body = doc_class.serialize(obj)
+        body = doc_class.serialize(instance)
         doc_id = body.pop('_id', None)
         connection.index(
             index=doc_index,
             body=body,
             id=doc_id,
             refresh=True
         )
```

### Comparing `django-seeker-7.3.0/seeker/views.py` & `django-seeker-7.3.1/seeker/views.py`

 * *Files identical despite different names*

### Comparing `django-seeker-7.3.0/setup.py` & `django-seeker-7.3.1/setup.py`

 * *Files identical despite different names*

