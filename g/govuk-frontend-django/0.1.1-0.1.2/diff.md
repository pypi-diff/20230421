# Comparing `tmp/govuk_frontend_django-0.1.1.tar.gz` & `tmp/govuk_frontend_django-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govuk_frontend_django-0.1.1.tar", max compression
+gzip compressed data, was "govuk_frontend_django-0.1.2.tar", max compression
```

## Comparing `govuk_frontend_django-0.1.1.tar` & `govuk_frontend_django-0.1.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1091 2023-04-18 16:00:56.529873 govuk_frontend_django-0.1.1/LICENSE
--rw-r--r--   0        0        0     1017 2023-04-20 16:39:24.126485 govuk_frontend_django-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.556313 govuk_frontend_django-0.1.1/govuk_frontend_django/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.561863 govuk_frontend_django-0.1.1/govuk_frontend_django/components/__init__.py
--rw-r--r--   0        0        0     1296 2023-04-20 12:42:14.586043 govuk_frontend_django-0.1.1/govuk_frontend_django/components/accordion.py
--rw-r--r--   0        0        0      939 2023-04-20 12:42:14.581422 govuk_frontend_django-0.1.1/govuk_frontend_django/components/back_link.py
--rw-r--r--   0        0        0     3767 2023-04-18 16:00:56.573577 govuk_frontend_django-0.1.1/govuk_frontend_django/components/base.py
--rw-r--r--   0        0        0     1170 2023-04-20 12:42:14.592265 govuk_frontend_django-0.1.1/govuk_frontend_django/components/breadcrumbs.py
--rw-r--r--   0        0        0     1221 2023-04-20 12:42:14.589664 govuk_frontend_django-0.1.1/govuk_frontend_django/components/button.py
--rw-r--r--   0        0        0     1838 2023-04-20 12:42:14.598186 govuk_frontend_django-0.1.1/govuk_frontend_django/components/character_count.py
--rw-r--r--   0        0        0     1892 2023-04-20 12:42:14.600823 govuk_frontend_django-0.1.1/govuk_frontend_django/components/checkboxes.py
--rw-r--r--   0        0        0     1723 2023-04-20 12:42:14.599909 govuk_frontend_django-0.1.1/govuk_frontend_django/components/cookie_banner.py
--rw-r--r--   0        0        0     1598 2023-04-20 12:42:14.602359 govuk_frontend_django-0.1.1/govuk_frontend_django/components/date_input.py
--rw-r--r--   0        0        0     1053 2023-04-20 12:42:14.597544 govuk_frontend_django-0.1.1/govuk_frontend_django/components/details.py
--rw-r--r--   0        0        0     1023 2023-04-20 12:42:14.607348 govuk_frontend_django-0.1.1/govuk_frontend_django/components/error_message.py
--rw-r--r--   0        0        0     1349 2023-04-20 12:42:14.613252 govuk_frontend_django-0.1.1/govuk_frontend_django/components/error_summary.py
--rw-r--r--   0        0        0     1024 2023-04-20 12:42:14.605229 govuk_frontend_django-0.1.1/govuk_frontend_django/components/fieldset.py
--rw-r--r--   0        0        0     1251 2023-04-20 12:42:14.606408 govuk_frontend_django-0.1.1/govuk_frontend_django/components/file_upload.py
--rw-r--r--   0        0        0     2007 2023-04-20 12:42:14.627934 govuk_frontend_django-0.1.1/govuk_frontend_django/components/footer.py
--rw-r--r--   0        0        0     1552 2023-04-20 12:42:14.613758 govuk_frontend_django-0.1.1/govuk_frontend_django/components/header.py
--rw-r--r--   0        0        0      927 2023-04-20 12:42:14.610338 govuk_frontend_django-0.1.1/govuk_frontend_django/components/hint.py
--rw-r--r--   0        0        0     1890 2023-04-20 12:42:14.623920 govuk_frontend_django-0.1.1/govuk_frontend_django/components/input.py
--rw-r--r--   0        0        0      960 2023-04-20 12:42:14.615085 govuk_frontend_django-0.1.1/govuk_frontend_django/components/inset_text.py
--rw-r--r--   0        0        0     1024 2023-04-20 12:42:14.621898 govuk_frontend_django-0.1.1/govuk_frontend_django/components/label.py
--rw-r--r--   0        0        0     1241 2023-04-20 12:42:14.628819 govuk_frontend_django-0.1.1/govuk_frontend_django/components/notification_banner.py
--rw-r--r--   0        0        0     1729 2023-04-20 12:42:14.623896 govuk_frontend_django-0.1.1/govuk_frontend_django/components/pagination.py
--rw-r--r--   0        0        0     1015 2023-04-20 12:42:14.619587 govuk_frontend_django-0.1.1/govuk_frontend_django/components/panel.py
--rw-r--r--   0        0        0      980 2023-04-20 12:42:14.620287 govuk_frontend_django-0.1.1/govuk_frontend_django/components/phase_banner.py
--rw-r--r--   0        0        0     1753 2023-04-20 12:42:14.629631 govuk_frontend_django-0.1.1/govuk_frontend_django/components/radios.py
--rw-r--r--   0        0        0     1504 2023-04-20 12:42:14.633487 govuk_frontend_django-0.1.1/govuk_frontend_django/components/select.py
--rw-r--r--   0        0        0      956 2023-04-20 12:42:14.623517 govuk_frontend_django-0.1.1/govuk_frontend_django/components/skip_link.py
--rw-r--r--   0        0        0     1850 2023-04-20 12:42:14.630760 govuk_frontend_django-0.1.1/govuk_frontend_django/components/summary_list.py
--rw-r--r--   0        0        0     1653 2023-04-20 12:42:14.634408 govuk_frontend_django-0.1.1/govuk_frontend_django/components/table.py
--rw-r--r--   0        0        0     1171 2023-04-20 12:42:14.629681 govuk_frontend_django-0.1.1/govuk_frontend_django/components/tabs.py
--rw-r--r--   0        0        0      892 2023-04-20 12:42:14.627472 govuk_frontend_django-0.1.1/govuk_frontend_django/components/tag.py
--rw-r--r--   0        0        0     1344 2023-04-20 12:42:14.630308 govuk_frontend_django-0.1.1/govuk_frontend_django/components/textarea.py
--rw-r--r--   0        0        0      986 2023-04-20 12:42:14.633202 govuk_frontend_django-0.1.1/govuk_frontend_django/components/warning_text.py
--rw-r--r--   0        0        0     2584 2023-04-18 16:38:49.732120 govuk_frontend_django-0.1.1/govuk_frontend_django/templates/govuk_frontend_django/base.html
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.543579 govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/__init__.py
--rw-r--r--   0        0        0     6411 2023-04-18 16:20:36.488163 govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py
--rw-r--r--   0        0        0     1500 2023-04-18 16:43:36.564559 govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py
--rw-r--r--   0        0        0     1202 2023-04-18 16:39:43.479073 govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py
--rw-r--r--   0        0        0     2904 2023-04-18 16:39:52.639160 govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py
--rw-r--r--   0        0        0     2177 2023-04-18 16:39:58.841418 govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py
--rw-r--r--   0        0        0     1522 2023-04-18 16:40:02.398875 govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py
--rw-r--r--   0        0        0     5044 2023-04-18 16:40:08.273697 govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py
--rw-r--r--   0        0        0     1373 2023-04-18 16:40:12.508567 govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/header.py
--rw-r--r--   0        0        0     2129 2023-04-18 16:40:15.259567 govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py
--rw-r--r--   0        0        0     1340 2023-04-18 16:40:19.370940 govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py
--rw-r--r--   0        0        0     6872 2023-04-18 16:40:25.682436 govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py
--rw-r--r--   0        0        0     1357 2023-04-18 16:40:28.276062 govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/table.py
--rw-r--r--   0        0        0     1231 2023-04-18 16:40:33.574374 govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py
--rw-r--r--   0        0        0     1159 2023-04-20 16:45:57.317212 govuk_frontend_django-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 govuk_frontend_django-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-18 16:00:56.529873 govuk_frontend_django-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1017 2023-04-20 16:48:35.945315 govuk_frontend_django-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.556313 govuk_frontend_django-0.1.2/govuk_frontend_django/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.561863 govuk_frontend_django-0.1.2/govuk_frontend_django/components/__init__.py
+-rw-r--r--   0        0        0     1296 2023-04-20 12:42:14.586043 govuk_frontend_django-0.1.2/govuk_frontend_django/components/accordion.py
+-rw-r--r--   0        0        0      939 2023-04-20 12:42:14.581422 govuk_frontend_django-0.1.2/govuk_frontend_django/components/back_link.py
+-rw-r--r--   0        0        0     3767 2023-04-18 16:00:56.573577 govuk_frontend_django-0.1.2/govuk_frontend_django/components/base.py
+-rw-r--r--   0        0        0     1170 2023-04-20 12:42:14.592265 govuk_frontend_django-0.1.2/govuk_frontend_django/components/breadcrumbs.py
+-rw-r--r--   0        0        0     1221 2023-04-20 12:42:14.589664 govuk_frontend_django-0.1.2/govuk_frontend_django/components/button.py
+-rw-r--r--   0        0        0     1838 2023-04-20 12:42:14.598186 govuk_frontend_django-0.1.2/govuk_frontend_django/components/character_count.py
+-rw-r--r--   0        0        0     1892 2023-04-20 12:42:14.600823 govuk_frontend_django-0.1.2/govuk_frontend_django/components/checkboxes.py
+-rw-r--r--   0        0        0     1723 2023-04-20 12:42:14.599909 govuk_frontend_django-0.1.2/govuk_frontend_django/components/cookie_banner.py
+-rw-r--r--   0        0        0     1598 2023-04-20 12:42:14.602359 govuk_frontend_django-0.1.2/govuk_frontend_django/components/date_input.py
+-rw-r--r--   0        0        0     1053 2023-04-20 12:42:14.597544 govuk_frontend_django-0.1.2/govuk_frontend_django/components/details.py
+-rw-r--r--   0        0        0     1023 2023-04-20 12:42:14.607348 govuk_frontend_django-0.1.2/govuk_frontend_django/components/error_message.py
+-rw-r--r--   0        0        0     1349 2023-04-20 12:42:14.613252 govuk_frontend_django-0.1.2/govuk_frontend_django/components/error_summary.py
+-rw-r--r--   0        0        0     1024 2023-04-20 12:42:14.605229 govuk_frontend_django-0.1.2/govuk_frontend_django/components/fieldset.py
+-rw-r--r--   0        0        0     1251 2023-04-20 12:42:14.606408 govuk_frontend_django-0.1.2/govuk_frontend_django/components/file_upload.py
+-rw-r--r--   0        0        0     2007 2023-04-20 12:42:14.627934 govuk_frontend_django-0.1.2/govuk_frontend_django/components/footer.py
+-rw-r--r--   0        0        0     1552 2023-04-20 12:42:14.613758 govuk_frontend_django-0.1.2/govuk_frontend_django/components/header.py
+-rw-r--r--   0        0        0      927 2023-04-20 12:42:14.610338 govuk_frontend_django-0.1.2/govuk_frontend_django/components/hint.py
+-rw-r--r--   0        0        0     1890 2023-04-20 12:42:14.623920 govuk_frontend_django-0.1.2/govuk_frontend_django/components/input.py
+-rw-r--r--   0        0        0      960 2023-04-20 12:42:14.615085 govuk_frontend_django-0.1.2/govuk_frontend_django/components/inset_text.py
+-rw-r--r--   0        0        0     1024 2023-04-20 12:42:14.621898 govuk_frontend_django-0.1.2/govuk_frontend_django/components/label.py
+-rw-r--r--   0        0        0     1241 2023-04-20 12:42:14.628819 govuk_frontend_django-0.1.2/govuk_frontend_django/components/notification_banner.py
+-rw-r--r--   0        0        0     1729 2023-04-20 12:42:14.623896 govuk_frontend_django-0.1.2/govuk_frontend_django/components/pagination.py
+-rw-r--r--   0        0        0     1015 2023-04-20 12:42:14.619587 govuk_frontend_django-0.1.2/govuk_frontend_django/components/panel.py
+-rw-r--r--   0        0        0      980 2023-04-20 12:42:14.620287 govuk_frontend_django-0.1.2/govuk_frontend_django/components/phase_banner.py
+-rw-r--r--   0        0        0     1753 2023-04-20 12:42:14.629631 govuk_frontend_django-0.1.2/govuk_frontend_django/components/radios.py
+-rw-r--r--   0        0        0     1504 2023-04-20 12:42:14.633487 govuk_frontend_django-0.1.2/govuk_frontend_django/components/select.py
+-rw-r--r--   0        0        0      956 2023-04-20 12:42:14.623517 govuk_frontend_django-0.1.2/govuk_frontend_django/components/skip_link.py
+-rw-r--r--   0        0        0     1850 2023-04-20 12:42:14.630760 govuk_frontend_django-0.1.2/govuk_frontend_django/components/summary_list.py
+-rw-r--r--   0        0        0     1653 2023-04-20 12:42:14.634408 govuk_frontend_django-0.1.2/govuk_frontend_django/components/table.py
+-rw-r--r--   0        0        0     1171 2023-04-20 12:42:14.629681 govuk_frontend_django-0.1.2/govuk_frontend_django/components/tabs.py
+-rw-r--r--   0        0        0      892 2023-04-20 12:42:14.627472 govuk_frontend_django-0.1.2/govuk_frontend_django/components/tag.py
+-rw-r--r--   0        0        0     1344 2023-04-20 12:42:14.630308 govuk_frontend_django-0.1.2/govuk_frontend_django/components/textarea.py
+-rw-r--r--   0        0        0      986 2023-04-20 12:42:14.633202 govuk_frontend_django-0.1.2/govuk_frontend_django/components/warning_text.py
+-rw-r--r--   0        0        0     2584 2023-04-18 16:38:49.732120 govuk_frontend_django-0.1.2/govuk_frontend_django/templates/govuk_frontend_django/base.html
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.543579 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/__init__.py
+-rw-r--r--   0        0        0     6411 2023-04-18 16:20:36.488163 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py
+-rw-r--r--   0        0        0     1500 2023-04-18 16:43:36.564559 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py
+-rw-r--r--   0        0        0     1202 2023-04-18 16:39:43.479073 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py
+-rw-r--r--   0        0        0     2904 2023-04-18 16:39:52.639160 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py
+-rw-r--r--   0        0        0     2177 2023-04-18 16:39:58.841418 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py
+-rw-r--r--   0        0        0     1522 2023-04-18 16:40:02.398875 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py
+-rw-r--r--   0        0        0     5044 2023-04-18 16:40:08.273697 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py
+-rw-r--r--   0        0        0     1373 2023-04-18 16:40:12.508567 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/header.py
+-rw-r--r--   0        0        0     2129 2023-04-18 16:40:15.259567 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py
+-rw-r--r--   0        0        0     1340 2023-04-18 16:40:19.370940 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py
+-rw-r--r--   0        0        0     6872 2023-04-18 16:40:25.682436 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py
+-rw-r--r--   0        0        0     1357 2023-04-18 16:40:28.276062 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/table.py
+-rw-r--r--   0        0        0     1231 2023-04-18 16:40:33.574374 govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py
+-rw-r--r--   0        0        0     1219 2023-04-21 08:44:08.300797 govuk_frontend_django-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 govuk_frontend_django-0.1.2/PKG-INFO
```

### Comparing `govuk_frontend_django-0.1.1/LICENSE` & `govuk_frontend_django-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/README.md` & `govuk_frontend_django-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GOV.UK Frontend Django
 
 [Documentation Site](https://uktrade.github.io/govuk-frontend-django/) | [GitHub](https://github.com/uktrade/govuk-frontend-django/) | [PyPI](https://pypi.org/project/govuk-frontend-django/)
 
 
-The `govuk_frontend_django` package contains django functionality to help when building a GOV.UK website.
+The `govuk_frontend_django` package contains Django functionality to help when building a GOV.UK website.
 
 The main part of this package is the [template tags](./template-tags/index.md) that it offers for use in your templates. These template tags will reduce the amount of markup that you need to maintain in your project.
 
 This package also contains some helpful [templates](./templates.md) for your project, such as the `govuk_frontend_django/base.html` template which contains the basic structure of a GOV.UK website.
 Packages
 ## Getting started
```

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/accordion.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/accordion.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/back_link.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/back_link.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/base.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/base.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/breadcrumbs.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/button.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/button.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/character_count.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/character_count.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/checkboxes.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/checkboxes.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/cookie_banner.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/date_input.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/date_input.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/details.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/details.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/error_message.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/error_message.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/error_summary.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/error_summary.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/fieldset.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/fieldset.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/file_upload.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/file_upload.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/footer.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/footer.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/header.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/header.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/hint.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/hint.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/input.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/input.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/inset_text.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/inset_text.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/label.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/label.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/notification_banner.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/notification_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/pagination.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/pagination.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/panel.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/panel.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/phase_banner.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/phase_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/radios.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/radios.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/select.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/select.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/skip_link.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/skip_link.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/summary_list.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/summary_list.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/table.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/table.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/tabs.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/tabs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/tag.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/tag.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/textarea.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/textarea.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/components/warning_text.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/components/warning_text.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/templates/govuk_frontend_django/base.html` & `govuk_frontend_django-0.1.2/govuk_frontend_django/templates/govuk_frontend_django/base.html`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/header.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/header.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/table.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/table.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py` & `govuk_frontend_django-0.1.2/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.1.1/pyproject.toml` & `govuk_frontend_django-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "govuk-frontend-django"
-version = "0.1.1"
-description = ""
+version = "0.1.2"
+description = "Django functionality to help when building a GOV.UK website."
 authors = [
     "DBT Live Service Team <live.services@digital.trade.gov.uk>",
     "Cam Lamb <cameron.lamb@digital.trade.gov.uk>",
     "Sam Dudley <samuel.dudley@digital.trade.gov.uk>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `govuk_frontend_django-0.1.1/PKG-INFO` & `govuk_frontend_django-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-django
-Version: 0.1.1
-Summary: 
+Version: 0.1.2
+Summary: Django functionality to help when building a GOV.UK website.
 Home-page: https://uktrade.github.io/govuk-frontend-django/
 License: MIT
 Author: DBT Live Service Team
 Author-email: live.services@digital.trade.gov.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 Description-Content-Type: text/markdown
 
 # GOV.UK Frontend Django
 
 [Documentation Site](https://uktrade.github.io/govuk-frontend-django/) | [GitHub](https://github.com/uktrade/govuk-frontend-django/) | [PyPI](https://pypi.org/project/govuk-frontend-django/)
 
 
-The `govuk_frontend_django` package contains django functionality to help when building a GOV.UK website.
+The `govuk_frontend_django` package contains Django functionality to help when building a GOV.UK website.
 
 The main part of this package is the [template tags](./template-tags/index.md) that it offers for use in your templates. These template tags will reduce the amount of markup that you need to maintain in your project.
 
 This package also contains some helpful [templates](./templates.md) for your project, such as the `govuk_frontend_django/base.html` template which contains the basic structure of a GOV.UK website.
 Packages
 ## Getting started
```

