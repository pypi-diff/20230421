# Comparing `tmp/django-jwt-oidc-1.0.tar.gz` & `tmp/django-jwt-oidc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-jwt-oidc-1.0.tar", last modified: Fri Apr 21 15:53:21 2023, max compression
+gzip compressed data, was "django-jwt-oidc-1.0.1.tar", last modified: Fri Apr 21 16:05:58 2023, max compression
```

## Comparing `django-jwt-oidc-1.0.tar` & `django-jwt-oidc-1.0.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.673263 django-jwt-oidc-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-04-21 15:53:21.673263 django-jwt-oidc-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.669263 django-jwt-oidc-1.0/django_jwt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.669263 django-jwt-oidc-1.0/django_jwt/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/openid.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/rest_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.669263 django-jwt-oidc-1.0/django_jwt/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.669263 django-jwt-oidc-1.0/django_jwt/server/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/migrations/0002_webpage_logout_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/migrations/0003_nonceused_privateclaimswebpage_restrictuserstoweb_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.665263 django-jwt-oidc-1.0/django_jwt/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.669263 django-jwt-oidc-1.0/django_jwt/server/templates/django_jwt/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/templates/django_jwt/oidc_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/views_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/settings_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.665263 django-jwt-oidc-1.0/django_jwt/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.673263 django-jwt-oidc-1.0/django_jwt/templates/django_jwt/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/templates/django_jwt/fake_login.html
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/view_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.673263 django-jwt-oidc-1.0/django_jwt_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-04-21 15:53:21.000000 django-jwt-oidc-1.0/django_jwt_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-21 15:53:21.000000 django-jwt-oidc-1.0/django_jwt_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:53:21.000000 django-jwt-oidc-1.0/django_jwt_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 15:53:21.000000 django-jwt-oidc-1.0/django_jwt_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 15:53:21.000000 django-jwt-oidc-1.0/django_jwt_oidc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 15:53:21.673263 django-jwt-oidc-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:58.089480 django-jwt-oidc-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-21 16:05:58.089480 django-jwt-oidc-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:58.089480 django-jwt-oidc-1.0.1/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:58.089480 django-jwt-oidc-1.0.1/django_jwt/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/openid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/rest_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:58.089480 django-jwt-oidc-1.0.1/django_jwt/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:58.089480 django-jwt-oidc-1.0.1/django_jwt/server/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/migrations/0002_webpage_logout_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/migrations/0003_nonceused_privateclaimswebpage_restrictuserstoweb_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:58.085481 django-jwt-oidc-1.0.1/django_jwt/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:58.089480 django-jwt-oidc-1.0.1/django_jwt/server/templates/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/templates/django_jwt/oidc_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/server/views_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/settings_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:58.085481 django-jwt-oidc-1.0.1/django_jwt/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:58.089480 django-jwt-oidc-1.0.1/django_jwt/templates/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/templates/django_jwt/fake_login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/view_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/django_jwt/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:05:58.089480 django-jwt-oidc-1.0.1/django_jwt_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-21 16:05:58.000000 django-jwt-oidc-1.0.1/django_jwt_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-21 16:05:58.000000 django-jwt-oidc-1.0.1/django_jwt_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:05:58.000000 django-jwt-oidc-1.0.1/django_jwt_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 16:05:58.000000 django-jwt-oidc-1.0.1/django_jwt_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 16:05:58.000000 django-jwt-oidc-1.0.1/django_jwt_oidc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 16:05:58.089480 django-jwt-oidc-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-21 16:05:43.000000 django-jwt-oidc-1.0.1/setup.py
```

### Comparing `django-jwt-oidc-1.0/LICENSE.md` & `django-jwt-oidc-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/PKG-INFO` & `django-jwt-oidc-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jwt-oidc
-Version: 1.0
+Version: 1.0.1
 Summary: Django library that implements the authentification for OpenId SSO with JWT from oauth2.
 Home-page: https://github.com/Casassarnau/django-jwt
 Author: Arnau Casas Saez
 Author-email: casassarnau@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Casassarnau/django-jwt/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-jwt-oidc-1.0/README.md` & `django-jwt-oidc-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/apps.py` & `django-jwt-oidc-1.0.1/django_jwt/apps.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/auth.py` & `django-jwt-oidc-1.0.1/django_jwt/auth.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/middleware.py` & `django-jwt-oidc-1.0.1/django_jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/openid.py` & `django-jwt-oidc-1.0.1/django_jwt/openid.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/rest_framework.py` & `django-jwt-oidc-1.0.1/django_jwt/rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/server/admin.py` & `django-jwt-oidc-1.0.1/django_jwt/server/admin.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/server/apps.py` & `django-jwt-oidc-1.0.1/django_jwt/server/apps.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/server/forms.py` & `django-jwt-oidc-1.0.1/django_jwt/server/forms.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/server/migrations/0001_initial.py` & `django-jwt-oidc-1.0.1/django_jwt/server/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/server/migrations/0002_webpage_logout_all.py` & `django-jwt-oidc-1.0.1/django_jwt/server/migrations/0002_webpage_logout_all.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('server', '0001_initial'),
+        ('django_jwt_server', '0001_initial'),
     ]
 
     operations = [
         migrations.AddField(
             model_name='webpage',
             name='logout_all',
             field=models.BooleanField(default=True),
```

### Comparing `django-jwt-oidc-1.0/django_jwt/server/migrations/0003_nonceused_privateclaimswebpage_restrictuserstoweb_and_more.py` & `django-jwt-oidc-1.0.1/django_jwt/server/migrations/0003_nonceused_privateclaimswebpage_restrictuserstoweb_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/server/models.py` & `django-jwt-oidc-1.0.1/django_jwt/server/models.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/server/templates/django_jwt/oidc_confirmation.html` & `django-jwt-oidc-1.0.1/django_jwt/server/templates/django_jwt/oidc_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/server/urls.py` & `django-jwt-oidc-1.0.1/django_jwt/server/urls.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/server/views.py` & `django-jwt-oidc-1.0.1/django_jwt/server/views.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/server/views_utils.py` & `django-jwt-oidc-1.0.1/django_jwt/server/views_utils.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/settings_utils.py` & `django-jwt-oidc-1.0.1/django_jwt/settings_utils.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/templates/django_jwt/fake_login.html` & `django-jwt-oidc-1.0.1/django_jwt/templates/django_jwt/fake_login.html`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/urls.py` & `django-jwt-oidc-1.0.1/django_jwt/urls.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/view_utils.py` & `django-jwt-oidc-1.0.1/django_jwt/view_utils.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt/views.py` & `django-jwt-oidc-1.0.1/django_jwt/views.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/django_jwt_oidc.egg-info/PKG-INFO` & `django-jwt-oidc-1.0.1/django_jwt_oidc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jwt-oidc
-Version: 1.0
+Version: 1.0.1
 Summary: Django library that implements the authentification for OpenId SSO with JWT from oauth2.
 Home-page: https://github.com/Casassarnau/django-jwt
 Author: Arnau Casas Saez
 Author-email: casassarnau@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Casassarnau/django-jwt/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-jwt-oidc-1.0/django_jwt_oidc.egg-info/SOURCES.txt` & `django-jwt-oidc-1.0.1/django_jwt_oidc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0/setup.py` & `django-jwt-oidc-1.0.1/setup.py`

 * *Files identical despite different names*

