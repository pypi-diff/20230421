# Comparing `tmp/ngits-tickets-1.0.2.tar.gz` & `tmp/ngits-tickets-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngits-tickets-1.0.2.tar", last modified: Mon Dec 12 09:01:00 2022, max compression
+gzip compressed data, was "ngits-tickets-1.0.3.tar", last modified: Fri Apr 21 10:50:05 2023, max compression
```

## Comparing `ngits-tickets-1.0.2.tar` & `ngits-tickets-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-12 09:01:00.319015 ngits-tickets-1.0.2/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       62 2022-10-27 09:23:05.000000 ngits-tickets-1.0.2/MANIFEST.in
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     4313 2022-12-12 09:01:00.319015 ngits-tickets-1.0.2/PKG-INFO
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     2666 2022-12-08 09:16:24.000000 ngits-tickets-1.0.2/README.rst
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      737 2022-10-27 09:23:05.000000 ngits-tickets-1.0.2/pyproject.toml
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      740 2022-12-12 09:01:00.323015 ngits-tickets-1.0.2/setup.cfg
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       38 2022-10-27 09:23:05.000000 ngits-tickets-1.0.2/setup.py
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-12 09:01:00.319015 ngits-tickets-1.0.2/src/
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-12 09:01:00.319015 ngits-tickets-1.0.2/src/ngits_tickets.egg-info/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     4313 2022-12-12 09:01:00.000000 ngits-tickets-1.0.2/src/ngits_tickets.egg-info/PKG-INFO
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      603 2022-12-12 09:01:00.000000 ngits-tickets-1.0.2/src/ngits_tickets.egg-info/SOURCES.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        1 2022-12-12 09:01:00.000000 ngits-tickets-1.0.2/src/ngits_tickets.egg-info/dependency_links.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       48 2022-12-12 09:01:00.000000 ngits-tickets-1.0.2/src/ngits_tickets.egg-info/requires.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        8 2022-12-12 09:01:00.000000 ngits-tickets-1.0.2/src/ngits_tickets.egg-info/top_level.txt
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-12 09:01:00.319015 ngits-tickets-1.0.2/src/tickets/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-10-27 09:23:05.000000 ngits-tickets-1.0.2/src/tickets/__init__.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      301 2022-10-27 09:23:05.000000 ngits-tickets-1.0.2/src/tickets/admin.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      146 2022-10-27 09:23:05.000000 ngits-tickets-1.0.2/src/tickets/apps.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      281 2022-12-06 08:54:22.000000 ngits-tickets-1.0.2/src/tickets/consts.py
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-12 09:01:00.319015 ngits-tickets-1.0.2/src/tickets/migrations/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1052 2022-10-27 09:23:05.000000 ngits-tickets-1.0.2/src/tickets/migrations/0001_initial.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      495 2022-12-06 08:54:22.000000 ngits-tickets-1.0.2/src/tickets/migrations/0002_ticket_type.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      377 2022-12-08 09:16:24.000000 ngits-tickets-1.0.2/src/tickets/migrations/0003_alter_ticket_type.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-10-27 09:23:05.000000 ngits-tickets-1.0.2/src/tickets/migrations/__init__.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      700 2022-12-08 09:16:24.000000 ngits-tickets-1.0.2/src/tickets/models.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      974 2022-12-08 09:16:24.000000 ngits-tickets-1.0.2/src/tickets/serializers.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      264 2022-10-27 09:23:05.000000 ngits-tickets-1.0.2/src/tickets/urls.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      428 2022-10-27 09:23:05.000000 ngits-tickets-1.0.2/src/tickets/views.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:05.298473 ngits-tickets-1.0.3/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       62 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/MANIFEST.in
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     4313 2023-04-21 10:50:05.298473 ngits-tickets-1.0.3/PKG-INFO
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     2666 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/README.rst
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      737 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/pyproject.toml
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      727 2023-04-21 10:50:05.298473 ngits-tickets-1.0.3/setup.cfg
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       38 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/setup.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:05.294473 ngits-tickets-1.0.3/src/
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:05.298473 ngits-tickets-1.0.3/src/ngits_tickets.egg-info/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     4313 2023-04-21 10:50:05.000000 ngits-tickets-1.0.3/src/ngits_tickets.egg-info/PKG-INFO
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      603 2023-04-21 10:50:05.000000 ngits-tickets-1.0.3/src/ngits_tickets.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        1 2023-04-21 10:50:05.000000 ngits-tickets-1.0.3/src/ngits_tickets.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       37 2023-04-21 10:50:05.000000 ngits-tickets-1.0.3/src/ngits_tickets.egg-info/requires.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        8 2023-04-21 10:50:05.000000 ngits-tickets-1.0.3/src/ngits_tickets.egg-info/top_level.txt
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:05.298473 ngits-tickets-1.0.3/src/tickets/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/src/tickets/__init__.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      301 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/src/tickets/admin.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      146 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/src/tickets/apps.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      281 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/src/tickets/consts.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:50:05.298473 ngits-tickets-1.0.3/src/tickets/migrations/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1052 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/src/tickets/migrations/0001_initial.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      495 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/src/tickets/migrations/0002_ticket_type.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      377 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/src/tickets/migrations/0003_alter_ticket_type.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/src/tickets/migrations/__init__.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      700 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/src/tickets/models.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      974 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/src/tickets/serializers.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      264 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/src/tickets/urls.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      428 2023-04-21 10:15:23.000000 ngits-tickets-1.0.3/src/tickets/views.py
```

### Comparing `ngits-tickets-1.0.2/PKG-INFO` & `ngits-tickets-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ngits-tickets
-Version: 1.0.2
+Version: 1.0.3
 Summary: Base ticket app for Django projects
 Home-page: https://ngits.dev
 Author: NGITs
 License: BSD-3-Clause
 Description: ngits-tickets
         =============
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 1.2 Name: ngits-tickets Version: 1.0.2 Summary: Base ticket
+Metadata-Version: 1.2 Name: ngits-tickets Version: 1.0.3 Summary: Base ticket
 app for Django projects Home-page: https://ngits.dev Author: NGITs License:
 BSD-3-Clause Description: ngits-tickets ============= Base `tickets`
 application for Django projects Setup ----- 1. Install using pip:
 ~~~~~~~~~~~~~~~~~~~~~ :: pip install ngits-tickets 2. Change your ``settings``
 file: ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ :: INSTALLED_APPS = [ ...
 "rest_framework", "rest_framework.authtoken", "tickets" ] ... REST_FRAMEWORK =
 { "DEFAULT_AUTHENTICATION_CLASSES":
```

### Comparing `ngits-tickets-1.0.2/README.rst` & `ngits-tickets-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `ngits-tickets-1.0.2/pyproject.toml` & `ngits-tickets-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ngits-tickets-1.0.2/setup.cfg` & `ngits-tickets-1.0.3/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ngits-tickets
-version = 1.0.2
+version = 1.0.3
 description = Base ticket app for Django projects
 long_description = file: README.rst
 url = https://ngits.dev
 author = NGITs
 license = BSD-3-Clause
 classifiers = 
 	Environment :: Web Environment
@@ -20,14 +20,14 @@
 [options]
 include_package_data = true
 packages = tickets
 package_dir = 
 	= src
 python_requires = >=3.9
 install_requires = 
-	Django >= 4.0.*
-	djangorestframework == 3.13.*, < 3.14
+	Django == 4.*
+	djangorestframework == 3.*
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ngits-tickets-1.0.2/src/ngits_tickets.egg-info/PKG-INFO` & `ngits-tickets-1.0.3/src/ngits_tickets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ngits-tickets
-Version: 1.0.2
+Version: 1.0.3
 Summary: Base ticket app for Django projects
 Home-page: https://ngits.dev
 Author: NGITs
 License: BSD-3-Clause
 Description: ngits-tickets
         =============
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 1.2 Name: ngits-tickets Version: 1.0.2 Summary: Base ticket
+Metadata-Version: 1.2 Name: ngits-tickets Version: 1.0.3 Summary: Base ticket
 app for Django projects Home-page: https://ngits.dev Author: NGITs License:
 BSD-3-Clause Description: ngits-tickets ============= Base `tickets`
 application for Django projects Setup ----- 1. Install using pip:
 ~~~~~~~~~~~~~~~~~~~~~ :: pip install ngits-tickets 2. Change your ``settings``
 file: ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ :: INSTALLED_APPS = [ ...
 "rest_framework", "rest_framework.authtoken", "tickets" ] ... REST_FRAMEWORK =
 { "DEFAULT_AUTHENTICATION_CLASSES":
```

### Comparing `ngits-tickets-1.0.2/src/ngits_tickets.egg-info/SOURCES.txt` & `ngits-tickets-1.0.3/src/ngits_tickets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ngits-tickets-1.0.2/src/tickets/migrations/0001_initial.py` & `ngits-tickets-1.0.3/src/tickets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ngits-tickets-1.0.2/src/tickets/models.py` & `ngits-tickets-1.0.3/src/tickets/models.py`

 * *Files identical despite different names*

### Comparing `ngits-tickets-1.0.2/src/tickets/serializers.py` & `ngits-tickets-1.0.3/src/tickets/serializers.py`

 * *Files identical despite different names*

