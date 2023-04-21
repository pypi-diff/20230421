# Comparing `tmp/ngits-users-1.0.5.tar.gz` & `tmp/ngits-users-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngits-users-1.0.5.tar", last modified: Wed Dec  7 07:30:03 2022, max compression
+gzip compressed data, was "ngits-users-1.0.6.tar", last modified: Fri Apr 21 08:18:49 2023, max compression
```

## Comparing `ngits-users-1.0.5.tar` & `ngits-users-1.0.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-07 07:30:03.273066 ngits-users-1.0.5/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      136 2022-10-13 07:47:53.000000 ngits-users-1.0.5/MANIFEST.in
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     7949 2022-12-07 07:30:03.273066 ngits-users-1.0.5/PKG-INFO
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     5361 2022-12-06 15:06:58.000000 ngits-users-1.0.5/README.rst
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      736 2022-10-12 11:53:58.000000 ngits-users-1.0.5/pyproject.toml
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      823 2022-12-07 07:30:03.277066 ngits-users-1.0.5/setup.cfg
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       38 2022-10-12 06:57:54.000000 ngits-users-1.0.5/setup.py
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-07 07:30:03.269066 ngits-users-1.0.5/src/
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-07 07:30:03.269066 ngits-users-1.0.5/src/ngits_users.egg-info/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     7949 2022-12-07 07:30:03.000000 ngits-users-1.0.5/src/ngits_users.egg-info/PKG-INFO
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1078 2022-12-07 07:30:03.000000 ngits-users-1.0.5/src/ngits_users.egg-info/SOURCES.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        1 2022-12-07 07:30:03.000000 ngits-users-1.0.5/src/ngits_users.egg-info/dependency_links.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      116 2022-12-07 07:30:03.000000 ngits-users-1.0.5/src/ngits_users.egg-info/requires.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        6 2022-12-07 07:30:03.000000 ngits-users-1.0.5/src/ngits_users.egg-info/top_level.txt
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-07 07:30:03.273066 ngits-users-1.0.5/src/users/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-10-12 11:53:58.000000 ngits-users-1.0.5/src/users/__init__.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      368 2022-10-12 11:53:58.000000 ngits-users-1.0.5/src/users/admin.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      193 2022-10-12 11:53:58.000000 ngits-users-1.0.5/src/users/apps.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1997 2022-12-06 15:09:10.000000 ngits-users-1.0.5/src/users/forms.py
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-07 07:30:03.273066 ngits-users-1.0.5/src/users/migrations/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3021 2022-10-12 11:53:58.000000 ngits-users-1.0.5/src/users/migrations/0001_initial.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-10-12 11:53:58.000000 ngits-users-1.0.5/src/users/migrations/__init__.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      344 2022-10-12 11:53:58.000000 ngits-users-1.0.5/src/users/models.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3581 2022-11-10 07:53:31.000000 ngits-users-1.0.5/src/users/schemas.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3122 2022-11-09 20:52:55.000000 ngits-users-1.0.5/src/users/serializers.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      357 2022-10-12 11:53:58.000000 ngits-users-1.0.5/src/users/signals.py
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-07 07:30:03.269066 ngits-users-1.0.5/src/users/static/
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-07 07:30:03.269066 ngits-users-1.0.5/src/users/static/users/
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-07 07:30:03.273066 ngits-users-1.0.5/src/users/static/users/css/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     2333 2022-10-12 11:53:58.000000 ngits-users-1.0.5/src/users/static/users/css/style.css
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-07 07:30:03.273066 ngits-users-1.0.5/src/users/static/users/img/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    11327 2022-10-12 11:53:58.000000 ngits-users-1.0.5/src/users/static/users/img/fail.svg
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    20062 2022-10-12 11:53:58.000000 ngits-users-1.0.5/src/users/static/users/img/success.svg
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      603 2022-10-17 08:13:38.000000 ngits-users-1.0.5/src/users/tasks.py
-drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2022-12-07 07:30:03.273066 ngits-users-1.0.5/src/users/templates/
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      538 2022-12-06 14:14:05.000000 ngits-users-1.0.5/src/users/templates/change_password.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      118 2022-10-12 11:53:58.000000 ngits-users-1.0.5/src/users/templates/change_password_email.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       71 2022-12-06 14:14:05.000000 ngits-users-1.0.5/src/users/templates/change_password_email.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      602 2022-12-06 14:14:05.000000 ngits-users-1.0.5/src/users/templates/form_site.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      575 2022-12-06 14:14:05.000000 ngits-users-1.0.5/src/users/templates/info_site.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      395 2022-12-06 14:14:05.000000 ngits-users-1.0.5/src/users/templates/password_changed.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      117 2022-10-12 11:53:58.000000 ngits-users-1.0.5/src/users/templates/registration_email.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       70 2022-12-06 14:14:05.000000 ngits-users-1.0.5/src/users/templates/registration_email.txt
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      384 2022-10-12 11:53:58.000000 ngits-users-1.0.5/src/users/templates/verify_error.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      389 2022-10-12 11:53:58.000000 ngits-users-1.0.5/src/users/templates/verify_ok.html
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1302 2022-11-09 20:52:55.000000 ngits-users-1.0.5/src/users/urls.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3047 2022-12-06 15:09:10.000000 ngits-users-1.0.5/src/users/utils.py
--rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    11075 2022-11-10 07:53:31.000000 ngits-users-1.0.5/src/users/views.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.673721 ngits-users-1.0.6/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      136 2023-04-21 06:52:22.000000 ngits-users-1.0.6/MANIFEST.in
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     8497 2023-04-21 08:18:49.673721 ngits-users-1.0.6/PKG-INFO
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     5773 2023-04-21 08:17:08.000000 ngits-users-1.0.6/README.rst
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      736 2023-04-21 06:52:22.000000 ngits-users-1.0.6/pyproject.toml
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      823 2023-04-21 08:18:49.673721 ngits-users-1.0.6/setup.cfg
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       38 2023-04-21 06:52:22.000000 ngits-users-1.0.6/setup.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.669721 ngits-users-1.0.6/src/
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.669721 ngits-users-1.0.6/src/ngits_users.egg-info/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     8497 2023-04-21 08:18:49.000000 ngits-users-1.0.6/src/ngits_users.egg-info/PKG-INFO
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1078 2023-04-21 08:18:49.000000 ngits-users-1.0.6/src/ngits_users.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        1 2023-04-21 08:18:49.000000 ngits-users-1.0.6/src/ngits_users.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      116 2023-04-21 08:18:49.000000 ngits-users-1.0.6/src/ngits_users.egg-info/requires.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        6 2023-04-21 08:18:49.000000 ngits-users-1.0.6/src/ngits_users.egg-info/top_level.txt
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.673721 ngits-users-1.0.6/src/users/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/__init__.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      368 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/admin.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      193 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/apps.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1997 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/forms.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.673721 ngits-users-1.0.6/src/users/migrations/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3021 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/migrations/0001_initial.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/migrations/__init__.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      344 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/models.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3657 2023-04-21 08:17:08.000000 ngits-users-1.0.6/src/users/schemas.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3122 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/serializers.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      357 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/signals.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.669721 ngits-users-1.0.6/src/users/static/
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.669721 ngits-users-1.0.6/src/users/static/users/
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.673721 ngits-users-1.0.6/src/users/static/users/css/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     2333 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/static/users/css/style.css
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.673721 ngits-users-1.0.6/src/users/static/users/img/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    11327 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/static/users/img/fail.svg
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    20062 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/static/users/img/success.svg
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      603 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/tasks.py
+drwxr-xr-x   0 gitlab-runner   (998) gitlab-runner   (998)        0 2023-04-21 08:18:49.673721 ngits-users-1.0.6/src/users/templates/
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      538 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/change_password.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      118 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/change_password_email.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       71 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/change_password_email.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      602 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/form_site.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      575 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/info_site.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      395 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/password_changed.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      117 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/registration_email.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)       70 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/registration_email.txt
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      384 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/verify_error.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)      389 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/templates/verify_ok.html
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     1302 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/urls.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)     3047 2023-04-21 06:52:22.000000 ngits-users-1.0.6/src/users/utils.py
+-rw-r--r--   0 gitlab-runner   (998) gitlab-runner   (998)    11600 2023-04-21 08:17:08.000000 ngits-users-1.0.6/src/users/views.py
```

### Comparing `ngits-users-1.0.5/PKG-INFO` & `ngits-users-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ngits-users
-Version: 1.0.5
+Version: 1.0.6
 Summary: Base users application for Django projects
 Home-page: https://ngits.dev
 Author: NGITs
 License: BSD-3-Clause
 Description: ngits-users
         ============
         
@@ -242,18 +242,35 @@
                 /templates
                     /change_password_email.html
                     /change_password_email.txt
                     /change_password.html
         
         *For fore details check out library default templates*
         
+        Login response codes
+        --------------------
+        
+        400 response:
+        
+        +---------------+--------------------+
+        | error_code    | error_msg          |
+        +===============+====================+
+        | 00            | Login failed       |
+        +---------------+--------------------+
+        | 01            | User not found     |
+        +---------------+--------------------+
+        | 02            | User not active    |
+        +---------------+--------------------+
+        
         Additional information
         ----------------------
         
         This package also support *django tranlations*.
+        
+        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ngits-users-1.0.5/README.rst` & `ngits-users-1.0.6/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -235,11 +235,27 @@
         /templates
             /change_password_email.html
             /change_password_email.txt
             /change_password.html
 
 *For fore details check out library default templates*
 
+Login response codes
+--------------------
+
+400 response:
+
++---------------+--------------------+
+| error_code    | error_msg          |
++===============+====================+
+| 00            | Login failed       |
++---------------+--------------------+
+| 01            | User not found     |
++---------------+--------------------+
+| 02            | User not active    |
++---------------+--------------------+
+
 Additional information
 ----------------------
 
-This package also support *django tranlations*.
+This package also support *django tranlations*.
+
```

#### html2text {}

```diff
@@ -44,9 +44,14 @@
 you have to create new files in your configured templates directory named: -
 Email templates: **these should contain {{ url|safe }}** -
 ``change_password_email.html`` - ``change_password_email.txt`` -
 ``registration_email.html`` - ``registration_email.txt`` - View templates: -
 ``change_password.html`` - **this have to contain {{ form }} !** -
 ``verify_ok.html`` - ``verify_error.html`` e.g.: :: /repo /manage.py /templates
 /change_password_email.html /change_password_email.txt /change_password.html
-*For fore details check out library default templates* Additional information -
---------------------- This package also support *django tranlations*.
+*For fore details check out library default templates* Login response codes ---
+----------------- 400 response: +---------------+--------------------+ |
+error_code | error_msg | +===============+====================+ | 00 | Login
+failed | +---------------+--------------------+ | 01 | User not found | +------
+---------+--------------------+ | 02 | User not active | +---------------+-----
+---------------+ Additional information ---------------------- This package
+also support *django tranlations*.
```

### Comparing `ngits-users-1.0.5/pyproject.toml` & `ngits-users-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.5/setup.cfg` & `ngits-users-1.0.6/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ngits-users
-version = 1.0.5
+version = 1.0.6
 description = Base users application for Django projects
 long_description = file: README.rst
 url = https://ngits.dev
 author = NGITs
 license = BSD-3-Clause
 classifiers = 
 	Environment :: Web Environment
```

### Comparing `ngits-users-1.0.5/src/ngits_users.egg-info/PKG-INFO` & `ngits-users-1.0.6/src/ngits_users.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ngits-users
-Version: 1.0.5
+Version: 1.0.6
 Summary: Base users application for Django projects
 Home-page: https://ngits.dev
 Author: NGITs
 License: BSD-3-Clause
 Description: ngits-users
         ============
         
@@ -242,18 +242,35 @@
                 /templates
                     /change_password_email.html
                     /change_password_email.txt
                     /change_password.html
         
         *For fore details check out library default templates*
         
+        Login response codes
+        --------------------
+        
+        400 response:
+        
+        +---------------+--------------------+
+        | error_code    | error_msg          |
+        +===============+====================+
+        | 00            | Login failed       |
+        +---------------+--------------------+
+        | 01            | User not found     |
+        +---------------+--------------------+
+        | 02            | User not active    |
+        +---------------+--------------------+
+        
         Additional information
         ----------------------
         
         This package also support *django tranlations*.
+        
+        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ngits-users-1.0.5/src/ngits_users.egg-info/SOURCES.txt` & `ngits-users-1.0.6/src/ngits_users.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.5/src/users/forms.py` & `ngits-users-1.0.6/src/users/forms.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.5/src/users/migrations/0001_initial.py` & `ngits-users-1.0.6/src/users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.5/src/users/schemas.py` & `ngits-users-1.0.6/src/users/schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,15 +102,19 @@
     },
     response_only=True,
     status_codes=["400"],
 )
 
 ACCOUNT_LOGIN_FAILED_RESPONSE = OpenApiExample(
     "login_failed",
-    value={"detail": "Login failed!"},
+    value={
+        "00": "Login failed!",
+        "01": "User not found",
+        "02": "User not active",
+    },
     response_only=True,
     status_codes=["400"],
 )
 
 ACCOUNT_DELETED_RESPONSE = OpenApiExample(
     "account_deleted",
     value={"detail": "Account deleted!"},
```

### Comparing `ngits-users-1.0.5/src/users/serializers.py` & `ngits-users-1.0.6/src/users/serializers.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.5/src/users/static/users/css/style.css` & `ngits-users-1.0.6/src/users/static/users/css/style.css`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.5/src/users/static/users/img/fail.svg` & `ngits-users-1.0.6/src/users/static/users/img/fail.svg`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.5/src/users/static/users/img/success.svg` & `ngits-users-1.0.6/src/users/static/users/img/success.svg`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.5/src/users/tasks.py` & `ngits-users-1.0.6/src/users/tasks.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.5/src/users/templates/change_password.html` & `ngits-users-1.0.6/src/users/templates/change_password.html`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.5/src/users/templates/form_site.html` & `ngits-users-1.0.6/src/users/templates/form_site.html`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.5/src/users/templates/info_site.html` & `ngits-users-1.0.6/src/users/templates/info_site.html`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.5/src/users/urls.py` & `ngits-users-1.0.6/src/users/urls.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.5/src/users/utils.py` & `ngits-users-1.0.6/src/users/utils.py`

 * *Files identical despite different names*

### Comparing `ngits-users-1.0.5/src/users/views.py` & `ngits-users-1.0.6/src/users/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,25 +93,38 @@
     )
 )
 class StandardLoginView(APIView):
     def post(self, request):
         serializer = StandardLoginSerializer(data=request.data)
         serializer.is_valid(raise_exception=True)
 
+        try:
+            user = User.objects.get(email=serializer.data["email"])
+            if not user.is_active:
+                return Response(
+                    {"error_code": "02", "error_msg": _("User not active")},
+                    status=status.HTTP_400_BAD_REQUEST,
+                )
+        except User.DoesNotExist:
+            return Response(
+                {"error_code": "01", "error_msg": _("User not found")},
+                status=status.HTTP_400_BAD_REQUEST,
+            )
+
         user = authenticate(
             username=serializer.data["email"],
             password=serializer.data["password"],
         )
 
         if user is not None:
             token_serializer = TokenSerializer(user.auth_token)
             return Response(token_serializer.data, status=status.HTTP_200_OK)
         else:
             return Response(
-                {"detail": _("Login failed!")},
+                {"error_code": "00", "error_msg": _("Login failed!")},
                 status=status.HTTP_400_BAD_REQUEST,
             )
 
 
 @extend_schema_view(
     post=extend_schema(
         request=None,
```

