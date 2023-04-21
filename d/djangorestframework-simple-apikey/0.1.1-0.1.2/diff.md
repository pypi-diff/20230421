# Comparing `tmp/djangorestframework-simple-apikey-0.1.1.tar.gz` & `tmp/djangorestframework-simple-apikey-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-simple-apikey-0.1.1.tar", last modified: Sun Feb 26 07:44:10 2023, max compression
+gzip compressed data, was "djangorestframework-simple-apikey-0.1.2.tar", last modified: Fri Apr 21 18:55:40 2023, max compression
```

## Comparing `djangorestframework-simple-apikey-0.1.1.tar` & `djangorestframework-simple-apikey-0.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 07:44:10.918189 djangorestframework-simple-apikey-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-02-26 07:44:10.918189 djangorestframework-simple-apikey-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 07:44:10.914189 djangorestframework-simple-apikey-0.1.1/djangorestframework_simple_apikey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-02-26 07:44:10.000000 djangorestframework-simple-apikey-0.1.1/djangorestframework_simple_apikey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-02-26 07:44:10.000000 djangorestframework-simple-apikey-0.1.1/djangorestframework_simple_apikey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 07:44:10.000000 djangorestframework-simple-apikey-0.1.1/djangorestframework_simple_apikey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 07:44:10.000000 djangorestframework-simple-apikey-0.1.1/djangorestframework_simple_apikey.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-26 07:44:10.000000 djangorestframework-simple-apikey-0.1.1/djangorestframework_simple_apikey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-26 07:44:10.000000 djangorestframework-simple-apikey-0.1.1/djangorestframework_simple_apikey.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 07:44:10.918189 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 07:44:10.918189 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 07:44:10.918189 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/management/commands/generate_fernet_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 07:44:10.918189 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-02-26 07:44:10.918189 djangorestframework-simple-apikey-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 07:44:10.918189 djangorestframework-simple-apikey-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/tests/test_api_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/tests/test_api_key_ crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/tests/test_custom_django_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-02-26 07:43:56.000000 djangorestframework-simple-apikey-0.1.1/tests/test_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:55:40.809266 djangorestframework-simple-apikey-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-04-21 18:55:40.809266 djangorestframework-simple-apikey-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:55:40.805266 djangorestframework-simple-apikey-0.1.2/djangorestframework_simple_apikey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-04-21 18:55:40.000000 djangorestframework-simple-apikey-0.1.2/djangorestframework_simple_apikey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-21 18:55:40.000000 djangorestframework-simple-apikey-0.1.2/djangorestframework_simple_apikey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:55:40.000000 djangorestframework-simple-apikey-0.1.2/djangorestframework_simple_apikey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:55:40.000000 djangorestframework-simple-apikey-0.1.2/djangorestframework_simple_apikey.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-21 18:55:40.000000 djangorestframework-simple-apikey-0.1.2/djangorestframework_simple_apikey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-21 18:55:40.000000 djangorestframework-simple-apikey-0.1.2/djangorestframework_simple_apikey.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:55:40.809266 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:55:40.809266 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:55:40.809266 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/management/commands/generate_fernet_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:55:40.809266 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-21 18:55:40.809266 djangorestframework-simple-apikey-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:55:40.809266 djangorestframework-simple-apikey-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/tests/test_api_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/tests/test_api_key_ crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/tests/test_custom_django_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-21 18:55:31.000000 djangorestframework-simple-apikey-0.1.2/tests/test_permissions.py
```

### Comparing `djangorestframework-simple-apikey-0.1.1/LICENSE` & `djangorestframework-simple-apikey-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-0.1.1/PKG-INFO` & `djangorestframework-simple-apikey-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-simple-apikey
-Version: 0.1.1
+Version: 0.1.2
 Summary: API Key authentication and permissions for Django REST.
 Home-page: https://github.com/koladev32/djangorestframework-simple-apikey
 Author: Kolawole Mangabo
 Author-email: onaelmangabo@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -108,19 +108,14 @@
 **Important ⛔️** : You should treat the `FERNET_KEY` security at the same level as the Django `SECRET_KEY`. 🫡
 
 To generate the fernet key use the following command:
 
 ```python
 python manage.py generate_fernet_key
 ```
-or 
-
-```python
-django-admin generate_fernet_key
-```
 
 ## Changelog
 
 See [CHANGELOG.md](https://github.com/koladev32/djangorestframework-simple-apikey/blob/main/CHANGELOG.md).
 
 ## Contributing
```

### Comparing `djangorestframework-simple-apikey-0.1.1/README.md` & `djangorestframework-simple-apikey-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -86,19 +86,14 @@
 **Important ⛔️** : You should treat the `FERNET_KEY` security at the same level as the Django `SECRET_KEY`. 🫡
 
 To generate the fernet key use the following command:
 
 ```python
 python manage.py generate_fernet_key
 ```
-or 
-
-```python
-django-admin generate_fernet_key
-```
 
 ## Changelog
 
 See [CHANGELOG.md](https://github.com/koladev32/djangorestframework-simple-apikey/blob/main/CHANGELOG.md).
 
 ## Contributing
```

### Comparing `djangorestframework-simple-apikey-0.1.1/djangorestframework_simple_apikey.egg-info/PKG-INFO` & `djangorestframework-simple-apikey-0.1.2/djangorestframework_simple_apikey.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-simple-apikey
-Version: 0.1.1
+Version: 0.1.2
 Summary: API Key authentication and permissions for Django REST.
 Home-page: https://github.com/koladev32/djangorestframework-simple-apikey
 Author: Kolawole Mangabo
 Author-email: onaelmangabo@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -108,19 +108,14 @@
 **Important ⛔️** : You should treat the `FERNET_KEY` security at the same level as the Django `SECRET_KEY`. 🫡
 
 To generate the fernet key use the following command:
 
 ```python
 python manage.py generate_fernet_key
 ```
-or 
-
-```python
-django-admin generate_fernet_key
-```
 
 ## Changelog
 
 See [CHANGELOG.md](https://github.com/koladev32/djangorestframework-simple-apikey/blob/main/CHANGELOG.md).
 
 ## Contributing
```

### Comparing `djangorestframework-simple-apikey-0.1.1/djangorestframework_simple_apikey.egg-info/SOURCES.txt` & `djangorestframework-simple-apikey-0.1.2/djangorestframework_simple_apikey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/admin.py` & `djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/admin.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/backends.py` & `djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/backends.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import typing
 
 from django.contrib.auth.backends import BaseBackend
 from django.http import HttpRequest
 from django.utils.timezone import now
+from django.core.exceptions import ObjectDoesNotExist
 
 from rest_framework import exceptions
 
+
 from rest_framework_simple_api_key.crypto import ApiKeyCrypto
 from rest_framework_simple_api_key.models import APIKey
 from rest_framework_simple_api_key.parser import APIKeyParser
 
 
 class APIKeyAuthentication(BaseBackend):
     model = APIKey
@@ -54,15 +56,15 @@
         if "_pk" not in payload or "_exp" not in payload:
             raise exceptions.AuthenticationFailed("Invalid API Key.")
 
         if payload["_exp"] < now().timestamp():
             raise exceptions.AuthenticationFailed("API Key has already expired.")
         try:
             api_key = self.model.objects.get(id=payload["_pk"])
-        except APIKey.DoesNotExist:  # pylint: disable=maybe-no-member
+        except ObjectDoesNotExist:  # pylint: disable=maybe-no-member
             raise exceptions.AuthenticationFailed("No entity matching this api key.")
 
         if api_key.revoked:
             raise exceptions.AuthenticationFailed("This API Key has been revoked.")
 
         return api_key.entity, key
```

### Comparing `djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/crypto.py` & `djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/crypto.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/migrations/0001_initial.py` & `djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/models.py` & `djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/models.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/parser.py` & `djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/parser.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/permissions.py` & `djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/permissions.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-0.1.1/rest_framework_simple_api_key/settings.py` & `djangorestframework-simple-apikey-0.1.2/rest_framework_simple_api_key/settings.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-0.1.1/setup.cfg` & `djangorestframework-simple-apikey-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.1
+current_version = 0.1.2
 commit = True
 tag = True
 
 [bumpversion:file:pyproject.toml]
 search = version = "{current_version}"
 replace = version = "{new_version}"
```

### Comparing `djangorestframework-simple-apikey-0.1.1/tests/test_admin.py` & `djangorestframework-simple-apikey-0.1.2/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-0.1.1/tests/test_api_authentication.py` & `djangorestframework-simple-apikey-0.1.2/tests/test_api_authentication.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-0.1.1/tests/test_api_key_ crypto.py` & `djangorestframework-simple-apikey-0.1.2/tests/test_api_key_ crypto.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-0.1.1/tests/test_models.py` & `djangorestframework-simple-apikey-0.1.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-simple-apikey-0.1.1/tests/test_permissions.py` & `djangorestframework-simple-apikey-0.1.2/tests/test_permissions.py`

 * *Files identical despite different names*

