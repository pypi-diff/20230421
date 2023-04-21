# Comparing `tmp/djangorestfilemanager-2.0.tar.gz` & `tmp/djangorestfilemanager-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangorestfilemanager-2.0.tar", last modified: Tue Apr  4 07:26:00 2023, max compression
+gzip compressed data, was "dist/djangorestfilemanager-2.0.1.tar", last modified: Fri Apr 21 07:21:49 2023, max compression
```

## Comparing `djangorestfilemanager-2.0.tar` & `djangorestfilemanager-2.0.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4599 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/djangorestfilemanager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/djangorestfilemanager/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/djangorestfilemanager/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/djangorestfilemanager/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/djangorestfilemanager/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/djangorestfilemanager/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      878 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/djangorestfilemanager/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1537 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/migrations/0002_auto_20200302_0947.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/migrations/0003_auto_20200311_1022.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/migrations/0004_auto_20200318_1806.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/migrations/0005_auto_20200319_1235.py
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/migrations/0006_auto_20200429_1220.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/migrations/0007_alter_file_name.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/migrations/0008_alter_file_field.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/migrations/0009_auto_20210810_0945.py
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/migrations/0010_auto_alter_data.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2863 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/models.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/djangorestfilemanager/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4561 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/tests/test_download_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/tests/test_upload_files.py
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1663 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/djangorestfilemanager/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/djangorestfilemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4599 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/djangorestfilemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1625 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/djangorestfilemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/djangorestfilemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      151 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/djangorestfilemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/djangorestfilemanager.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      600 2023-04-04 07:26:00.000000 djangorestfilemanager-2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-04 07:25:50.000000 djangorestfilemanager-2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4601 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      878 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0002_auto_20200302_0947.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0003_auto_20200311_1022.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0004_auto_20200318_1806.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0005_auto_20200319_1235.py
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0006_auto_20200429_1220.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0007_alter_file_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0008_alter_file_field.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0009_auto_20210810_0945.py
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0010_auto_alter_data.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4561 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/tests/test_download_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/tests/test_upload_files.py
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/djangorestfilemanager/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/djangorestfilemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4601 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/djangorestfilemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/djangorestfilemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/djangorestfilemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/djangorestfilemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/djangorestfilemanager.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      602 2023-04-21 07:21:49.000000 djangorestfilemanager-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-21 07:21:39.000000 djangorestfilemanager-2.0.1/setup.py
```

### Comparing `djangorestfilemanager-2.0/LICENSE.txt` & `djangorestfilemanager-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/PKG-INFO` & `djangorestfilemanager-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestfilemanager
-Version: 2.0
+Version: 2.0.1
 Summary: Django REST File Manager.
 Home-page: https://gitlab.com/kas-factory/packages/django-rest-file-manager
 Author: Avelino @ KF
 Author-email: avelino@kasfactory.net
 License: COPYRIGHT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `djangorestfilemanager-2.0/README.md` & `djangorestfilemanager-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/admin.py` & `djangorestfilemanager-2.0.1/djangorestfilemanager/admin.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/app_settings.py` & `djangorestfilemanager-2.0.1/djangorestfilemanager/app_settings.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/locale/en/LC_MESSAGES/django.mo` & `djangorestfilemanager-2.0.1/djangorestfilemanager/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/locale/en/LC_MESSAGES/django.po` & `djangorestfilemanager-2.0.1/djangorestfilemanager/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/locale/es/LC_MESSAGES/django.mo` & `djangorestfilemanager-2.0.1/djangorestfilemanager/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/locale/es/LC_MESSAGES/django.po` & `djangorestfilemanager-2.0.1/djangorestfilemanager/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/migrations/0001_initial.py` & `djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/migrations/0002_auto_20200302_0947.py` & `djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0002_auto_20200302_0947.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/migrations/0003_auto_20200311_1022.py` & `djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0003_auto_20200311_1022.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/migrations/0004_auto_20200318_1806.py` & `djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0004_auto_20200318_1806.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/migrations/0009_auto_20210810_0945.py` & `djangorestfilemanager-2.0.1/djangorestfilemanager/migrations/0009_auto_20210810_0945.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/models.py` & `djangorestfilemanager-2.0.1/djangorestfilemanager/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         primary_key=True
     )
     file = models.FileField(
         verbose_name='File',
         storage=get_file_system_storage(),
         upload_to=set_storage_file_dir,
         blank=False,
-        max_length=255,
         null=True
     )
     name = models.CharField(
         verbose_name='Name',
         max_length=255
     )
     username = models.CharField(
```

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/serializers.py` & `djangorestfilemanager-2.0.1/djangorestfilemanager/serializers.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/tests/test_download_files.py` & `djangorestfilemanager-2.0.1/djangorestfilemanager/tests/test_download_files.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/tests/test_upload_files.py` & `djangorestfilemanager-2.0.1/djangorestfilemanager/tests/test_upload_files.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager/views.py` & `djangorestfilemanager-2.0.1/djangorestfilemanager/views.py`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager.egg-info/PKG-INFO` & `djangorestfilemanager-2.0.1/djangorestfilemanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestfilemanager
-Version: 2.0
+Version: 2.0.1
 Summary: Django REST File Manager.
 Home-page: https://gitlab.com/kas-factory/packages/django-rest-file-manager
 Author: Avelino @ KF
 Author-email: avelino@kasfactory.net
 License: COPYRIGHT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `djangorestfilemanager-2.0/djangorestfilemanager.egg-info/SOURCES.txt` & `djangorestfilemanager-2.0.1/djangorestfilemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangorestfilemanager-2.0/setup.cfg` & `djangorestfilemanager-2.0.1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangorestfilemanager
-version = 2.0
+version = 2.0.1
 description = Django REST File Manager.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/kas-factory/packages/django-rest-file-manager
 author = Avelino @ KF
 author_email = avelino@kasfactory.net
 license = COPYRIGHT
```

