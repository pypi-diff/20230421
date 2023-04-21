# Comparing `tmp/aleksis_app_evalu-1.0b0.tar.gz` & `tmp/aleksis_app_evalu-1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_evalu-1.0b0.tar", max compression
+gzip compressed data, was "aleksis_app_evalu-1.0b1.tar", max compression
```

## Comparing `aleksis_app_evalu-1.0b0.tar` & `aleksis_app_evalu-1.0b1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0     3533 2023-03-03 19:02:25.997998 aleksis_app_evalu-1.0b0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2021-08-25 15:31:49.756358 aleksis_app_evalu-1.0b0/LICENCE.rst
--rw-r--r--   0        0        0     1020 2023-03-03 16:52:10.739363 aleksis_app_evalu-1.0b0/README.rst
--rw-r--r--   0        0        0      151 2021-08-25 15:31:49.756358 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/__init__.py
--rw-r--r--   0        0        0      537 2021-10-17 15:12:24.543181 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/admin.py
--rw-r--r--   0        0        0      423 2023-03-03 16:53:53.535478 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/apps.py
--rw-r--r--   0        0        0     3587 2022-12-26 14:10:50.903272 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/forms.py
--rw-r--r--   0        0        0     5187 2023-03-03 18:53:04.691779 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/frontend/index.js
--rw-r--r--   0        0        0      292 2023-03-03 19:14:08.486926 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/frontend/messages/de.json
--rw-r--r--   0        0        0      281 2023-03-03 18:53:04.707780 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/frontend/messages/en.json
--rw-r--r--   0        0        0      353 2023-03-03 19:14:08.486926 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/frontend/messages/ru.json
--rw-r--r--   0        0        0      339 2023-03-03 19:14:08.486926 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/frontend/messages/uk.json
--rw-r--r--   0        0        0        0 2021-08-25 15:31:49.756358 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/.keepdir
--rw-r--r--   0        0        0      463 2022-12-29 09:38:46.139135 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    27819 2022-12-29 09:30:32.227993 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      463 2022-12-29 09:38:46.135135 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      799 2022-12-29 09:30:34.476021 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/ar/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    22784 2022-12-29 09:38:46.143135 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    37507 2022-12-29 09:36:59.761475 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-12-29 09:38:46.143135 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/de_DE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      669 2022-12-29 09:30:34.468021 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/de_DE/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      379 2022-12-29 09:38:46.143135 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    27735 2022-12-29 09:30:32.199993 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2022-12-29 09:38:46.139135 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      715 2022-12-29 09:30:34.452021 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/fr/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      337 2022-12-29 09:38:46.135135 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    27689 2022-12-29 09:30:32.183993 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-12-29 09:38:46.135135 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/la/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      669 2022-12-29 09:30:34.448021 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/la/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      337 2022-12-29 09:38:46.135135 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    27689 2022-12-29 09:30:32.251994 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-12-29 09:38:46.131135 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/nb_NO/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      669 2022-12-29 09:30:34.488022 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/nb_NO/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    28933 2023-03-03 19:30:11.109170 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43749 2023-03-03 19:14:08.486926 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      518 2022-12-29 09:38:46.135135 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      859 2022-12-29 09:30:34.476021 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/ru/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      337 2022-12-29 09:38:46.147135 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    27689 2022-12-29 09:30:32.239993 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2022-12-29 09:38:46.143135 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      669 2022-12-29 09:30:34.484022 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/tr_TR/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    28014 2023-03-03 19:30:11.109170 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    42812 2023-03-03 19:14:08.490926 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      602 2022-12-29 09:38:46.139135 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      946 2022-12-29 09:30:34.476021 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/uk/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     2765 2022-01-04 11:04:16.842963 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/managers.py
--rw-r--r--   0        0        0    10430 2021-08-25 17:40:07.969708 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0001_initial.py
--rw-r--r--   0        0        0     2636 2021-09-15 15:08:53.491093 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0002_evaluation_item.py
--rw-r--r--   0        0        0      626 2021-09-15 16:09:19.830309 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0003_question_no_rich_text.py
--rw-r--r--   0        0        0     1037 2021-10-08 19:11:24.757640 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0004_privacy_form.py
--rw-r--r--   0        0        0     1293 2021-10-12 13:14:26.523745 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0005_key_model.py
--rw-r--r--   0        0        0      680 2021-10-17 15:18:54.384670 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0006_key_pair.py
--rw-r--r--   0        0        0     2372 2021-11-07 17:25:17.230920 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0007_drop_reference_registration.py
--rw-r--r--   0        0        0     4724 2022-01-04 11:03:49.131078 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0008_comparison_group.py
--rw-r--r--   0        0        0     1919 2022-01-04 11:03:49.131078 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0009_auto_20211206_1448.py
--rw-r--r--   0        0        0      466 2022-01-06 09:57:40.750329 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0010_evaluationresult_result_key.py
--rw-r--r--   0        0        0      650 2022-01-22 16:34:50.069630 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0011_evaluation_finished.py
--rw-r--r--   0        0        0      648 2022-12-26 13:47:53.265731 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0012_deletion.py
--rw-r--r--   0        0        0        0 2021-08-25 15:31:49.756358 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/__init__.py
--rw-r--r--   0        0        0    28237 2022-12-26 14:10:50.903272 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/models.py
--rw-r--r--   0        0        0     1480 2022-01-22 21:01:50.906256 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/preferences.py
--rw-r--r--   0        0        0     5190 2022-12-26 14:10:50.903272 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/rules.py
--rw-r--r--   0        0        0       42 2023-01-23 11:09:37.491124 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/settings.py
--rw-r--r--   0        0        0        0 2021-08-25 15:31:49.756358 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/static/.keepdir
--rw-r--r--   0        0        0     1173 2023-03-03 18:53:04.795783 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/static/css/evalu.css
--rw-r--r--   0        0        0     4539 2023-03-03 18:53:04.867786 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/static/js/evalu/results.js
--rw-r--r--   0        0        0     1635 2021-09-23 17:58:49.575840 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tables.py
--rw-r--r--   0        0        0      992 2022-01-04 11:03:49.135078 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tasks.py
--rw-r--r--   0        0        0     3597 2022-12-26 14:10:50.907271 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/list.html
--rw-r--r--   0        0        0      461 2021-09-15 15:48:01.898215 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/part/create.html
--rw-r--r--   0        0        0      824 2021-09-15 16:10:38.110787 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/part/edit.html
--rw-r--r--   0        0        0      547 2021-09-15 15:47:40.578719 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/part/list.html
--rw-r--r--   0        0        0     5014 2021-11-07 15:41:50.370642 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/participate/form.html
--rw-r--r--   0        0        0     1786 2021-11-02 10:11:44.551137 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/participate/list.html
--rw-r--r--   0        0        0     1766 2022-01-06 11:27:53.606283 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/password.html
--rw-r--r--   0        0        0      635 2021-09-23 17:50:48.301364 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/phase/create.html
--rw-r--r--   0        0        0     2486 2022-12-26 13:47:53.265731 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/phase/delete_data.html
--rw-r--r--   0        0        0     3459 2022-12-26 13:47:53.269731 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/phase/detail.html
--rw-r--r--   0        0        0      963 2022-01-04 11:03:49.135078 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/phase/edit.html
--rw-r--r--   0        0        0      551 2021-09-19 15:45:37.465953 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/phase/list.html
--rw-r--r--   0        0        0      757 2022-01-10 09:14:41.065946 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/phase/status.html
--rw-r--r--   0        0        0     4342 2022-12-26 13:47:53.269731 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/registration/detail.html
--rw-r--r--   0        0        0     1542 2022-01-22 20:44:08.069531 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/registration/finish.html
--rw-r--r--   0        0        0     2555 2022-12-26 14:10:50.907271 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/registration/manage.html
--rw-r--r--   0        0        0     1637 2022-01-04 11:03:49.135078 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/registration/print.html
--rw-r--r--   0        0        0     3158 2021-10-17 15:43:51.845970 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/registration/register.html
--rw-r--r--   0        0        0     4264 2023-01-23 11:11:23.371361 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/results.html
--rw-r--r--   0        0        0     3328 2023-01-23 11:11:29.375426 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/results_pdf.html
--rw-r--r--   0        0        0     2498 2021-11-07 12:18:55.383387 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/material/fields/aleksis_agreementwidget.html
--rw-r--r--   0        0        0     1361 2022-01-06 09:57:40.754329 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tests/models/test_evaluation_key_pair.py
--rw-r--r--   0        0        0      432 2022-01-04 11:10:24.578118 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tests/models/test_evaluation_part.py
--rw-r--r--   0        0        0     3331 2022-01-10 09:12:05.276778 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tests/models/test_evaluation_phase.py
--rw-r--r--   0        0        0     3371 2022-01-04 11:27:23.110701 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tests/models/test_evaluation_registration.py
--rw-r--r--   0        0        0     2371 2022-01-06 09:57:40.754329 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tests/models/test_evaluation_result.py
--rw-r--r--   0        0        0     2688 2022-01-04 11:27:23.618698 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tests/models/util.py
--rw-r--r--   0        0        0     2937 2022-12-26 14:10:50.907271 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/urls.py
--rw-r--r--   0        0        0     2062 2022-12-26 14:10:50.907271 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/util/predicates.py
--rw-r--r--   0        0        0    19819 2022-12-26 14:10:50.907271 aleksis_app_evalu-1.0b0/aleksis/apps/evalu/views.py
--rw-r--r--   0        0        0     1288 2023-03-03 16:52:37.345985 aleksis_app_evalu-1.0b0/pyproject.toml
--rw-r--r--   0        0        0     3091 1970-01-01 00:00:00.000000 aleksis_app_evalu-1.0b0/setup.py
--rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 aleksis_app_evalu-1.0b0/PKG-INFO
+-rw-r--r--   0        0        0     3716 2023-04-21 15:45:43.526650 aleksis_app_evalu-1.0b1/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2021-08-25 15:31:49.756358 aleksis_app_evalu-1.0b1/LICENCE.rst
+-rw-r--r--   0        0        0     1020 2023-03-03 16:52:10.739363 aleksis_app_evalu-1.0b1/README.rst
+-rw-r--r--   0        0        0      151 2021-08-25 15:31:49.756358 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/__init__.py
+-rw-r--r--   0        0        0      537 2021-10-17 15:12:24.543181 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/admin.py
+-rw-r--r--   0        0        0      423 2023-03-03 16:53:53.535478 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/apps.py
+-rw-r--r--   0        0        0     3587 2022-12-26 14:10:50.903272 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/forms.py
+-rw-r--r--   0        0        0     7227 2023-04-19 15:24:29.089482 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/frontend/index.js
+-rw-r--r--   0        0        0      292 2023-03-03 19:14:08.486926 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/frontend/messages/de.json
+-rw-r--r--   0        0        0      281 2023-03-03 18:53:04.707780 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/frontend/messages/en.json
+-rw-r--r--   0        0        0      353 2023-03-03 19:14:08.486926 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/frontend/messages/ru.json
+-rw-r--r--   0        0        0      339 2023-03-03 19:14:08.486926 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/frontend/messages/uk.json
+-rw-r--r--   0        0        0        0 2021-08-25 15:31:49.756358 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/.keepdir
+-rw-r--r--   0        0        0      463 2022-12-29 09:38:46.139135 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    27819 2022-12-29 09:30:32.227993 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      463 2022-12-29 09:38:46.135135 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      799 2022-12-29 09:30:34.476021 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/ar/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    22784 2022-12-29 09:38:46.143135 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    37507 2022-12-29 09:36:59.761475 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2022-12-29 09:38:46.143135 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/de_DE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      669 2022-12-29 09:30:34.468021 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/de_DE/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      379 2022-12-29 09:38:46.143135 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    27735 2022-12-29 09:30:32.199993 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2022-12-29 09:38:46.139135 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      715 2022-12-29 09:30:34.452021 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/fr/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      337 2022-12-29 09:38:46.135135 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    27689 2022-12-29 09:30:32.183993 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2022-12-29 09:38:46.135135 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/la/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      669 2022-12-29 09:30:34.448021 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/la/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      337 2022-12-29 09:38:46.135135 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    27689 2022-12-29 09:30:32.251994 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2022-12-29 09:38:46.131135 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/nb_NO/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      669 2022-12-29 09:30:34.488022 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/nb_NO/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    28933 2023-03-03 19:30:11.109170 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43749 2023-03-03 19:14:08.486926 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      518 2022-12-29 09:38:46.135135 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      859 2022-12-29 09:30:34.476021 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      337 2022-12-29 09:38:46.147135 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    27689 2022-12-29 09:30:32.239993 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2022-12-29 09:38:46.143135 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      669 2022-12-29 09:30:34.484022 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/tr_TR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    28014 2023-03-03 19:30:11.109170 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    42812 2023-03-03 19:14:08.490926 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      602 2022-12-29 09:38:46.139135 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      946 2022-12-29 09:30:34.476021 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/uk/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     2765 2022-01-04 11:04:16.842963 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/managers.py
+-rw-r--r--   0        0        0    10430 2021-08-25 17:40:07.969708 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2636 2021-09-15 15:08:53.491093 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0002_evaluation_item.py
+-rw-r--r--   0        0        0      626 2021-09-15 16:09:19.830309 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0003_question_no_rich_text.py
+-rw-r--r--   0        0        0     1037 2021-10-08 19:11:24.757640 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0004_privacy_form.py
+-rw-r--r--   0        0        0     1293 2021-10-12 13:14:26.523745 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0005_key_model.py
+-rw-r--r--   0        0        0      680 2021-10-17 15:18:54.384670 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0006_key_pair.py
+-rw-r--r--   0        0        0     2372 2021-11-07 17:25:17.230920 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0007_drop_reference_registration.py
+-rw-r--r--   0        0        0     4724 2022-01-04 11:03:49.131078 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0008_comparison_group.py
+-rw-r--r--   0        0        0     1919 2022-01-04 11:03:49.131078 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0009_auto_20211206_1448.py
+-rw-r--r--   0        0        0      466 2022-01-06 09:57:40.750329 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0010_evaluationresult_result_key.py
+-rw-r--r--   0        0        0      650 2022-01-22 16:34:50.069630 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0011_evaluation_finished.py
+-rw-r--r--   0        0        0      648 2022-12-26 13:47:53.265731 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0012_deletion.py
+-rw-r--r--   0        0        0        0 2021-08-25 15:31:49.756358 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/__init__.py
+-rw-r--r--   0        0        0    28237 2022-12-26 14:10:50.903272 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/models.py
+-rw-r--r--   0        0        0     1480 2022-01-22 21:01:50.906256 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/preferences.py
+-rw-r--r--   0        0        0     5190 2022-12-26 14:10:50.903272 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/rules.py
+-rw-r--r--   0        0        0       42 2023-01-23 11:09:37.491124 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/settings.py
+-rw-r--r--   0        0        0        0 2021-08-25 15:31:49.756358 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/static/.keepdir
+-rw-r--r--   0        0        0     1173 2023-03-03 18:53:04.795783 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/static/css/evalu.css
+-rw-r--r--   0        0        0     4539 2023-03-03 18:53:04.867786 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/static/js/evalu/results.js
+-rw-r--r--   0        0        0     1635 2021-09-23 17:58:49.575840 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tables.py
+-rw-r--r--   0        0        0      992 2022-01-04 11:03:49.135078 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tasks.py
+-rw-r--r--   0        0        0     3597 2022-12-26 14:10:50.907271 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/list.html
+-rw-r--r--   0        0        0      461 2021-09-15 15:48:01.898215 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/part/create.html
+-rw-r--r--   0        0        0      824 2021-09-15 16:10:38.110787 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/part/edit.html
+-rw-r--r--   0        0        0      547 2021-09-15 15:47:40.578719 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/part/list.html
+-rw-r--r--   0        0        0     5014 2021-11-07 15:41:50.370642 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/participate/form.html
+-rw-r--r--   0        0        0     1786 2021-11-02 10:11:44.551137 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/participate/list.html
+-rw-r--r--   0        0        0     1766 2022-01-06 11:27:53.606283 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/password.html
+-rw-r--r--   0        0        0      635 2021-09-23 17:50:48.301364 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/phase/create.html
+-rw-r--r--   0        0        0     2486 2022-12-26 13:47:53.265731 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/phase/delete_data.html
+-rw-r--r--   0        0        0     3459 2022-12-26 13:47:53.269731 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/phase/detail.html
+-rw-r--r--   0        0        0      963 2022-01-04 11:03:49.135078 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/phase/edit.html
+-rw-r--r--   0        0        0      551 2021-09-19 15:45:37.465953 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/phase/list.html
+-rw-r--r--   0        0        0      757 2022-01-10 09:14:41.065946 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/phase/status.html
+-rw-r--r--   0        0        0     4342 2022-12-26 13:47:53.269731 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/registration/detail.html
+-rw-r--r--   0        0        0     1542 2022-01-22 20:44:08.069531 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/registration/finish.html
+-rw-r--r--   0        0        0     2555 2022-12-26 14:10:50.907271 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/registration/manage.html
+-rw-r--r--   0        0        0     1637 2022-01-04 11:03:49.135078 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/registration/print.html
+-rw-r--r--   0        0        0     3158 2021-10-17 15:43:51.845970 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/registration/register.html
+-rw-r--r--   0        0        0     4264 2023-01-23 11:11:23.371361 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/results.html
+-rw-r--r--   0        0        0     3328 2023-01-23 11:11:29.375426 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/results_pdf.html
+-rw-r--r--   0        0        0     2498 2021-11-07 12:18:55.383387 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/material/fields/aleksis_agreementwidget.html
+-rw-r--r--   0        0        0     1361 2022-01-06 09:57:40.754329 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tests/models/test_evaluation_key_pair.py
+-rw-r--r--   0        0        0      432 2022-01-04 11:10:24.578118 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tests/models/test_evaluation_part.py
+-rw-r--r--   0        0        0     3331 2022-01-10 09:12:05.276778 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tests/models/test_evaluation_phase.py
+-rw-r--r--   0        0        0     3371 2022-01-04 11:27:23.110701 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tests/models/test_evaluation_registration.py
+-rw-r--r--   0        0        0     2371 2022-01-06 09:57:40.754329 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tests/models/test_evaluation_result.py
+-rw-r--r--   0        0        0     2688 2022-01-04 11:27:23.618698 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tests/models/util.py
+-rw-r--r--   0        0        0     2937 2022-12-26 14:10:50.907271 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/urls.py
+-rw-r--r--   0        0        0     2062 2022-12-26 14:10:50.907271 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/util/predicates.py
+-rw-r--r--   0        0        0    19819 2022-12-26 14:10:50.907271 aleksis_app_evalu-1.0b1/aleksis/apps/evalu/views.py
+-rw-r--r--   0        0        0     1288 2023-04-21 15:46:14.222586 aleksis_app_evalu-1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     3091 1970-01-01 00:00:00.000000 aleksis_app_evalu-1.0b1/setup.py
+-rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 aleksis_app_evalu-1.0b1/PKG-INFO
```

### Comparing `aleksis_app_evalu-1.0b0/CHANGELOG.rst` & `aleksis_app_evalu-1.0b1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,24 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-`1.0b0` – 2022-03-03
---------------------
+`1.0b1`_ - 2022-04-21
+---------------------
+
+Fixed
+~~~~~
+
+* Many views were not compatible with new SPA.
+
+`1.0b0`_ – 2022-03-03
+---------------------
 
 This version requires AlekSIS-Core 3.0. It is incompatible with any previous
 version.
 
 Removed
 ~~~~~~~
 
@@ -20,16 +28,16 @@
 Added
 ~~~~~
 
 * Add SPA support for AlekSIS-Core 3.0
 * Add Ukrainian and Russian locale (contributed by Sergiy Gorichenko from Fre(i)e Software GmbH).
 
 
-`0.5.1` - 2022-01-23
---------------------
+`0.5.1`_ - 2022-01-23
+---------------------
 
 Fixed
 ~~~~~
 
 * Charts in results page weren't loaded.
 
 `0.5`_ - 2022-12-29
@@ -176,7 +184,8 @@
 .. _0.3.2: https://edugit.org/katharineum/AlekSIS-App-EvaLU/-/tags/0.3.2
 .. _0.4: https://edugit.org/katharineum/AlekSIS-App-EvaLU/-/tags/0.4
 .. _0.4.1: https://edugit.org/katharineum/AlekSIS-App-EvaLU/-/tags/0.4.1
 .. _0.4.2: https://edugit.org/katharineum/AlekSIS-App-EvaLU/-/tags/0.4.2
 .. _0.5: https://edugit.org/katharineum/AlekSIS-App-EvaLU/-/tags/0.5
 .. _0.5.1: https://edugit.org/katharineum/AlekSIS-App-EvaLU/-/tags/0.5.1
 .. _1.0b0: https://edugit.org/katharineum/AlekSIS-App-EvaLU/-/tags/1.0b0
+.. _1.0b1: https://edugit.org/katharineum/AlekSIS-App-EvaLU/-/tags/1.0b1
```

### Comparing `aleksis_app_evalu-1.0b0/LICENCE.rst` & `aleksis_app_evalu-1.0b1/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/README.rst` & `aleksis_app_evalu-1.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/admin.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/admin.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/forms.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/frontend/index.js` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/frontend/index.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -21,22 +21,31 @@
         props: {
             byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
         },
     }, {
         path: "parts/create/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.createEvaluationPart",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "parts/:pk/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.editEvaluationPart",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "parts/:pk/delete/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.deleteEvaluationPart",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "phases/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.evaluationPhases",
         meta: {
             inMenu: true,
             titleKey: "evalu.phases.menu_title",
@@ -46,30 +55,45 @@
         props: {
             byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
         },
     }, {
         path: "phases/create/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.createEvaluationPhase",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "phases/:pk/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.evaluationPhase",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "phases/:pk/edit/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.editEvaluationPhase",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "phases/:pk/delete/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.deleteEvaluationPhase",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "phases/:pk/deletion/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.deleteDataFromPhase",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "evaluations/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.evaluationPhasesOverview",
         meta: {
             inMenu: true,
             titleKey: "evalu.evaluation.all_menu_title",
@@ -79,42 +103,66 @@
         props: {
             byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
         },
     }, {
         path: "evaluations/:pk/register/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.registerForEvaluation",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "evaluations/registrations/:pk/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.evaluationRegistration",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "evaluations/registrations/:pk/manage/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.manageEvaluationProcess",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "evaluations/groups/:pk/start/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.startEvaluationForGroup",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "evaluations/groups/:pk/stop/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.stopEvaluationForGroup",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "evaluations/registrations/:pk/finish/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.finishEvaluation",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "evaluations/registrations/:pk/results/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.evaluationResults",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "evaluations/registrations/:pk/results/pdf/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.evaluationResultsAsPdf",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, {
         path: "evaluations/evaluate/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.evaluationsAsParticipant",
         meta: {
             inMenu: true,
             titleKey: "evalu.evaluation.my_menu_title",
@@ -124,9 +172,12 @@
         props: {
             byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
         },
     }, {
         path: "evaluations/evaluate/:pk/",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "evalu.evaluatePerson",
+        props: {
+            byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
+        },
     }, ],
 };
```

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/ar/LC_MESSAGES/djangojs.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/de_DE/LC_MESSAGES/djangojs.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/de_DE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/fr/LC_MESSAGES/djangojs.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/la/LC_MESSAGES/django.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/la/LC_MESSAGES/djangojs.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/la/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/nb_NO/LC_MESSAGES/djangojs.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/nb_NO/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/ru/LC_MESSAGES/djangojs.mo` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/ru/LC_MESSAGES/djangojs.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/tr_TR/LC_MESSAGES/djangojs.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/uk/LC_MESSAGES/djangojs.mo` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/locale/uk/LC_MESSAGES/djangojs.po` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/managers.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/managers.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0001_initial.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0002_evaluation_item.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0002_evaluation_item.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0003_question_no_rich_text.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0003_question_no_rich_text.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0004_privacy_form.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0004_privacy_form.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0005_key_model.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0005_key_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0006_key_pair.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0006_key_pair.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0007_drop_reference_registration.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0007_drop_reference_registration.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0008_comparison_group.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0008_comparison_group.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0009_auto_20211206_1448.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0009_auto_20211206_1448.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0011_evaluation_finished.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0011_evaluation_finished.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/migrations/0012_deletion.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/migrations/0012_deletion.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/models.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/preferences.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/rules.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/static/css/evalu.css` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/static/css/evalu.css`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/static/js/evalu/results.js` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/static/js/evalu/results.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tables.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tasks.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tasks.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/list.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/part/edit.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/part/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/part/list.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/part/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/participate/form.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/participate/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/participate/list.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/participate/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/password.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/password.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/phase/create.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/phase/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/phase/delete_data.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/phase/delete_data.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/phase/detail.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/phase/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/phase/edit.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/phase/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/phase/list.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/phase/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/phase/status.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/phase/status.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/registration/detail.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/registration/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/registration/finish.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/registration/finish.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/registration/manage.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/registration/manage.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/registration/print.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/registration/print.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/registration/register.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/registration/register.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/results.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/results.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/evalu/results_pdf.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/evalu/results_pdf.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/templates/material/fields/aleksis_agreementwidget.html` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/templates/material/fields/aleksis_agreementwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tests/models/test_evaluation_key_pair.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tests/models/test_evaluation_key_pair.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tests/models/test_evaluation_phase.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tests/models/test_evaluation_phase.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tests/models/test_evaluation_registration.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tests/models/test_evaluation_registration.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tests/models/test_evaluation_result.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tests/models/test_evaluation_result.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/tests/models/util.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/tests/models/util.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/urls.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/util/predicates.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/util/predicates.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/aleksis/apps/evalu/views.py` & `aleksis_app_evalu-1.0b1/aleksis/apps/evalu/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_evalu-1.0b0/pyproject.toml` & `aleksis_app_evalu-1.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-EvaLU"
-version = "1.0b0"
+version = "1.0b1"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = ["CHANGELOG.rst", "LICENCE.rst", "aleksis/**/*.mo"]
 
 description = "Unofficial AlekSIS App EvaLU (Evaluation of teaching and lesson quality)"
```

### Comparing `aleksis_app_evalu-1.0b0/setup.py` & `aleksis_app_evalu-1.0b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
  'django-formtools>=2.3,<3.0']
 
 entry_points = \
 {'aleksis.app': ['evalu = aleksis.apps.evalu.apps:DefaultConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-evalu',
-    'version': '1.0b0',
+    'version': '1.0b1',
     'description': 'Unofficial AlekSIS App EvaLU (Evaluation of teaching and lesson quality)',
     'long_description': 'Unofficial AlekSIS App EvaLU (Evaluation of teaching and lesson quality)\n========================================================================\n\nAlekSIS\n-------\n\nThis is an unofficial application for use with the `AlekSIS`_ platform.\n\nFeatures\n--------\n\nThis app can be used to evaluate teaching and lesson quality of teachers.\n\nLicence\n-------\n\n::\n\n  Copyright © 2021, 2022, 2023 Jonathan Weth <dev@jonathanweth.de>\n\n  Licenced under the EUPL, version 1.2 or later\n\nCreate graph of models\n----------------------\n\n::\n\n  poetry run pip install pygraphviz\n  poetry run aleksis-admin graph_models evalu -X Site,ExtensibleModel -x site,extended_data -o\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\n.. _AlekSIS: https://edugit.org/AlekSIS/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n',
     'author': 'Jonathan Weth',
     'author_email': 'dev@jonathanweth.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://edugit.org/katharineum/AlekSIS-App-EvaLU',
```

### Comparing `aleksis_app_evalu-1.0b0/PKG-INFO` & `aleksis_app_evalu-1.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-evalu
-Version: 1.0b0
+Version: 1.0b1
 Summary: Unofficial AlekSIS App EvaLU (Evaluation of teaching and lesson quality)
 Home-page: https://edugit.org/katharineum/AlekSIS-App-EvaLU
 License: EUPL-1.2
 Author: Jonathan Weth
 Author-email: dev@jonathanweth.de
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
```

