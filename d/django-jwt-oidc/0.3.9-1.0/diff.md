# Comparing `tmp/django-jwt-oidc-0.3.9.tar.gz` & `tmp/django-jwt-oidc-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-jwt-oidc-0.3.9.tar", last modified: Sat Sep  3 13:52:39 2022, max compression
+gzip compressed data, was "django-jwt-oidc-1.0.tar", last modified: Fri Apr 21 15:53:21 2023, max compression
```

## Comparing `django-jwt-oidc-0.3.9.tar` & `django-jwt-oidc-1.0.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 13:52:39.634022 django-jwt-oidc-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7609 2022-09-03 13:52:39.634022 django-jwt-oidc-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7015 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 13:52:39.630022 django-jwt-oidc-0.3.9/django_jwt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     3120 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 13:52:39.630022 django-jwt-oidc-0.3.9/django_jwt/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2195 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/openid.py
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/patterns.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/rest_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 13:52:39.634022 django-jwt-oidc-0.3.9/django_jwt/server/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/server/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/server/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 13:52:39.634022 django-jwt-oidc-0.3.9/django_jwt/server/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2843 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/server/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/server/migrations/0002_webpage_logout_all.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/server/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3301 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/server/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/server/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 13:52:39.634022 django-jwt-oidc-0.3.9/django_jwt/server/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/server/templates/oidc_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/server/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     7085 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/server/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1723 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/server/views_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/settings_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 13:52:39.634022 django-jwt-oidc-0.3.9/django_jwt/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/templates/fake_login.html
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     3604 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/view_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3763 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/django_jwt/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 13:52:39.634022 django-jwt-oidc-0.3.9/django_jwt_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7609 2022-09-03 13:52:39.000000 django-jwt-oidc-0.3.9/django_jwt_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-09-03 13:52:39.000000 django-jwt-oidc-0.3.9/django_jwt_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-03 13:52:39.000000 django-jwt-oidc-0.3.9/django_jwt_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-09-03 13:52:39.000000 django-jwt-oidc-0.3.9/django_jwt_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-03 13:52:39.000000 django-jwt-oidc-0.3.9/django_jwt_oidc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-03 13:52:39.634022 django-jwt-oidc-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-09-03 13:52:30.000000 django-jwt-oidc-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.673263 django-jwt-oidc-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-04-21 15:53:21.673263 django-jwt-oidc-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.669263 django-jwt-oidc-1.0/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.669263 django-jwt-oidc-1.0/django_jwt/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/openid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/rest_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.669263 django-jwt-oidc-1.0/django_jwt/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.669263 django-jwt-oidc-1.0/django_jwt/server/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/migrations/0002_webpage_logout_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/migrations/0003_nonceused_privateclaimswebpage_restrictuserstoweb_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.665263 django-jwt-oidc-1.0/django_jwt/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.669263 django-jwt-oidc-1.0/django_jwt/server/templates/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/templates/django_jwt/oidc_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/server/views_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/settings_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.665263 django-jwt-oidc-1.0/django_jwt/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.673263 django-jwt-oidc-1.0/django_jwt/templates/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/templates/django_jwt/fake_login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/view_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/django_jwt/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:53:21.673263 django-jwt-oidc-1.0/django_jwt_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11182 2023-04-21 15:53:21.000000 django-jwt-oidc-1.0/django_jwt_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-21 15:53:21.000000 django-jwt-oidc-1.0/django_jwt_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:53:21.000000 django-jwt-oidc-1.0/django_jwt_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 15:53:21.000000 django-jwt-oidc-1.0/django_jwt_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 15:53:21.000000 django-jwt-oidc-1.0/django_jwt_oidc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 15:53:21.673263 django-jwt-oidc-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-21 15:53:08.000000 django-jwt-oidc-1.0/setup.py
```

### Comparing `django-jwt-oidc-0.3.9/LICENSE.md` & `django-jwt-oidc-1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-0.3.9/django_jwt/apps.py` & `django-jwt-oidc-1.0/django_jwt/server/apps.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from django.apps import AppConfig
 
 from django_jwt.settings_utils import get_setting
 
 
-class DjangoJwtConfig(AppConfig):
+class DjangoJwtServerConfig(AppConfig):
     default_auto_field = 'django.db.models.BigAutoField'
-    name = 'django_jwt'
+    name = 'django_jwt.server'
+    label = 'django_jwt_server'
 
     def ready(self):
-        client_type = get_setting('JWT_CLIENT.TYPE')
-        if client_type == 'local':
-            apps = get_setting('INSTALLED_APPS')
-            if 'django_jwt.server' not in apps:
-                raise Exception('You need to add django_jwt.server into your INSTALLED_APPS in order to deploy the '
-                                'OpenId server')
+        apps = get_setting('INSTALLED_APPS')
+        if 'corsheaders' in apps:
+            from django_jwt.server import signals
+            signals
+        else:
+            raise Exception('corsheaders is required in order to protect your app from CORS')
+        if 'rest_framework' not in apps:
+            raise Exception('rest_framework is required in order to set your OIDC provider')
```

### Comparing `django-jwt-oidc-0.3.9/django_jwt/auth.py` & `django-jwt-oidc-1.0/django_jwt/auth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,119 @@
 import json
 import logging
 
 from django.contrib.auth import get_user_model
-from jwcrypto.jwt import JWT, JWTMissingKey
+from jwcrypto.jwt import JWT, JWTMissingKey, JWTExpired
 
 from django_jwt.openid import OpenId2Info
 from django_jwt.settings_utils import get_setting, get_domain_from_url
 
 
+logger = logging.getLogger(__name__)
+
+
 class JWTAuthentication:
     class JWTException(Exception):
         pass
 
     @classmethod
-    def authenticate_credentials(cls, key, nonce=None):
-        jwt = cls.validate_jwt(key)
+    def authenticate_credentials(cls, key, nonce=None, client_id=None):
+        try:
+            jwt = cls.validate_jwt(key)
+        except Exception as e:
+            if isinstance(e, JWTExpired):
+                raise e
+            logger.warning(e)
+            raise cls.JWTException('Token is not valid')
         claims = json.loads(jwt.claims)
-        if not cls.verify_claims(claims, nonce):
+        if not cls.verify_claims(claims, nonce, client_id):
             raise cls.JWTException('Token is not valid')
         user, created = cls.get_or_create_user(profile=claims)
-        return user
+        return user, jwt
+
+    @classmethod
+    def validate_authorization_jwt(cls, key, nonce=None, sub_attr='pk'):
+        try:
+            jwt = cls.validate_jwt(key)
+        except Exception as e:
+            if isinstance(e, JWTExpired):
+                raise e
+            logger.warning(e)
+            raise cls.JWTException('Token is not valid')
+        claims = json.loads(jwt.claims)
+        if not cls.verify_claims(claims, nonce):
+            raise cls.JWTException('Token is not valid')
+        model = get_user_model()
+        user = None
+        try:
+            user = model.objects.get(**{sub_attr: claims['sub']})
+        except model.DoesNotExist:
+            pass
+        return user, claims
 
     @classmethod
     def validate_jwt(cls, token, second=False):
         try:
             jwt = JWT(jwt=token, key=OpenId2Info().jwks)
         except JWTMissingKey:
             if second:
                 raise cls.JWTException('JWK not found')
             OpenId2Info().fetch_jwks()
             jwt = cls.validate_jwt(token=token, second=True)
-        except Exception as e:
+        except ValueError as e:
             logger = logging.getLogger(__name__)
             logger.info(e)
-            raise cls.JWTException('Token format is not valid or expired')
+            raise e
         return jwt
 
     @classmethod
-    def get_or_create_user(cls, profile):
+    def get_defaults_from_claims(cls, claims):
         model = get_user_model()
-        translation = get_setting('JWT_CLIENT.RENAME_ATTRIBUTES')
-        model_fields = [field.name for field in model._meta.get_fields()]
-        defaults = get_setting('JWT_CLIENT.DEFAULT_ATTRIBUTES')
-        defaults.update({translation.get(key, key): value for key, value in profile.items()
+        translation = {'sub': 'pk'}
+        translation.update(get_setting('JWT_OIDC.ID_TOKEN_RENAME_ATTRIBUTES'))
+        model_fields = [field.name for field in model._meta.get_fields()] + ['pk']
+        defaults = get_setting('JWT_OIDC.USER_DEFAULT_ATTRIBUTES')
+        defaults.update({translation.get(key, key): value for key, value in claims.items()
                          if translation.get(key, key) in model_fields})
         for key, value in defaults.items():
             change_field = getattr(model, 'change_%s' % key, None)
             if change_field is not None:
                 defaults[key] = change_field(model, value)
-        sub_field = translation.get('sub', None) or model.USERNAME_FIELD
-        kwargs = {sub_field: defaults[model.USERNAME_FIELD]}
-        if get_setting('JWT_CLIENT.CREATE_USER'):
+        claim_id = get_setting('JWT_OIDC.IDENTIFICATION_CLAIM')
+        user_id = translation.get(claim_id, claim_id)
+        if user_id not in defaults:
+            return None, False
+        kwargs = {user_id: defaults[user_id]}
+        del defaults[user_id]
+        return defaults, kwargs
+
+    @classmethod
+    def get_or_create_user(cls, profile):
+        model = get_user_model()
+        defaults, kwargs = cls.get_defaults_from_claims(profile)
+        if get_setting('JWT_OIDC.CREATE_USER'):
             return model.objects.get_or_create(defaults=defaults, **kwargs)
         try:
             return model.objects.get(**kwargs), False
         except model.DoesNotExist:
             return None, False
 
     @classmethod
     def verify_claims(cls, claims, nonce=None, client_id=None):
-        logger = logging.getLogger(__name__)
-        if client_id is None:
-            client_id = get_setting('JWT_CLIENT.CLIENT_ID')
-        if client_id not in claims.get('aud', []):
-            logger.info('Client id not in aud')
-            return False
-        openid_domain = get_domain_from_url(get_setting('JWT_CLIENT.OPENID2_URL'))
+        openid_domain = get_domain_from_url(get_setting('JWT_OIDC.DISCOVERY_ENDPOINT'))
+        if client_id is None and 'django_jwt.server' in get_setting('INSTALLED_APPS'):
+            if not any([aud.startswith(openid_domain) for aud in claims.get('aud', [])]):
+                return False
+        else:
+            if client_id is None:
+                client_id = get_setting('JWT_CLIENT.CLIENT_ID')
+            if client_id not in claims.get('aud', []):
+                logger.info('Client id not in aud')
+                return False
+        openid_domain = get_domain_from_url(get_setting('JWT_OIDC.DISCOVERY_ENDPOINT'))
         iss_domain = get_domain_from_url(claims.get('iss', ''))
         # openid_domain can't be '' because of apps.py
         if openid_domain != iss_domain:
             logger.info('Issuer %s is not from OPENID2_URL %s' % (claims.get('iss', ''), openid_domain))
             return False
         if nonce is not None and claims.get('nonce') != nonce:
             logger.info('Nonce changed')
```

### Comparing `django-jwt-oidc-0.3.9/django_jwt/openid.py` & `django-jwt-oidc-1.0/django_jwt/openid.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,43 +7,60 @@
 from django_jwt.exceptions import JWTClientException
 from django_jwt.patterns import Singleton
 from django_jwt.settings_utils import get_setting
 
 
 # singleton class that saves all information from the OpenId server
 class OpenId2Info(metaclass=Singleton):
-    def __init__(self):
-        url = get_setting('JWT_CLIENT.OPENID2_URL')
-        client_type = get_setting('JWT_CLIENT.TYPE')
-        if client_type == 'local':
-            apps = get_setting('INSTALLED_APPS')
-            if 'django_jwt.server' not in apps:
-                raise JWTClientException('django_jwt.server not installed for type local')
-        url += '/.well-known/openid-configuration'
+    def __init_local__(self):
+        apps = get_setting('INSTALLED_APPS')
+        if 'django_jwt.server' not in apps:
+            raise JWTClientException('django_jwt.server not installed for type local')
 
+    def __init_remote__(self):
+        url = get_setting('JWT_OIDC.DISCOVERY_ENDPOINT')
         # Getting urls info from OpenId server
         http = urllib3.PoolManager()
         r = http.request('GET', url)
         if r.status != 200:
             error_message = 'OpenID returned error code %s on openid-configuration: %s' % (r.status, url)
             logger = logging.getLogger(__name__)
             logger.critical(error_message)
             raise JWTClientException(error_message)
         data = json.loads(r.data.decode('UTF-8'))
         self.jwks_uri = data.get('jwks_uri', None)
+        self.token_endpoint = data.get('token_endpoint', None)
         self.authorization_endpoint = data.get('authorization_endpoint', None)
         self.end_session_endpoint = data.get('end_session_endpoint', None)
+        self.userinfo_endpoint = data.get('userinfo_endpoint', None)
         if self.jwks_uri is None or self.authorization_endpoint is None:
             raise JWTClientException('jkws_uri or authorization_endpoint not found in OpenId openid-configuration url')
+
+    def __init__(self):
+        self.jwks_uri = None
+        self.authorization_endpoint = None
+        self.end_session_endpoint = None
+        self.jwks = None
+        self.userinfo_endpoint = None
+        self.client_type = get_setting('JWT_OIDC.TYPE')
+        if self.client_type == 'client':
+            self.__init_local__()
+        elif self.client_type == 'provider':
+            self.__init_remote__()
         self.fetch_jwks()
 
     # Updates all the actual JWKS from the OPenId server
     def fetch_jwks(self):
         logger = logging.getLogger(__name__)
         logger.info('Fetching JWKs')
-        http = urllib3.PoolManager()
-        r = http.request('GET', self.jwks_uri)
-        if r.status != 200:
-            error_message = 'OpenID returned error code %s on jwks_uri: %s' % (r.status, self.jwks_uri)
-            logger.critical(error_message)
-            raise JWTClientException(error_message)
-        self.jwks = JWKSet.from_json(r.data.decode('UTF-8'))
+        if self.client_type == 'remote':
+            http = urllib3.PoolManager()
+            r = http.request('GET', self.jwks_uri)
+            if r.status != 200:
+                error_message = 'OpenID returned error code %s on jwks_uri: %s' % (r.status, self.jwks_uri)
+                logger.critical(error_message)
+                raise JWTClientException(error_message)
+            jwk_set_json = r.data.decode('UTF-8')
+        else:
+            from django_jwt.server.models import Key
+            jwk_set_json = json.dumps({'keys': Key.get_jwk_set()})
+        self.jwks = JWKSet.from_json(jwk_set_json)
```

### Comparing `django-jwt-oidc-0.3.9/django_jwt/rest_framework.py` & `django-jwt-oidc-1.0/django_jwt/rest_framework.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import logging
 
+from jwcrypto.jwt import JWTExpired
 from rest_framework import exceptions
 from rest_framework.authentication import TokenAuthentication
 from django.utils.translation import gettext_lazy as _
 
 from django_jwt.auth import JWTAuthentication
 
 
 class JWTTokenAuthentication(TokenAuthentication):
     keyword = 'Bearer'
 
     def authenticate_credentials(self, key):
         try:
-            user = JWTAuthentication.authenticate_credentials(key)
-        except JWTAuthentication.JWTException as e:
+            user, jwt = JWTAuthentication.authenticate_credentials(key)
+        except (JWTAuthentication.JWTException, JWTExpired) as e:
             logger = logging.getLogger(__name__)
             logger.warning(e)
             raise exceptions.AuthenticationFailed(_('Token is invalid or expired.'))
         if not user:
             raise exceptions.AuthenticationFailed(_('User does not exist.'))
-        return user, key
+        return user, jwt
```

### Comparing `django-jwt-oidc-0.3.9/django_jwt/server/migrations/0001_initial.py` & `django-jwt-oidc-1.0/django_jwt/server/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-0.3.9/django_jwt/server/migrations/0002_webpage_logout_all.py` & `django-jwt-oidc-1.0/django_jwt/server/migrations/0002_webpage_logout_all.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-0.3.9/django_jwt/templates/fake_login.html` & `django-jwt-oidc-1.0/django_jwt/templates/django_jwt/fake_login.html`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-0.3.9/django_jwt/view_utils.py` & `django-jwt-oidc-1.0/django_jwt/view_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,29 +66,29 @@
     hash_digest = hash_alg(access_token.encode('ascii')).digest()
     cut_at = int(len(hash_digest) / 2)
     truncated = hash_digest[:cut_at]
     at_hash = base64url_encode(truncated)
     return at_hash.decode('ascii')
 
 
-def base64url_encode(input):
+def base64url_encode(input_text):
     """Helper method to base64url_encode a string.
     Args:
-        input (str): A base64url_encoded string to encode.
+        input_text (str): A base64url_encoded string to encode.
     """
-    return base64.urlsafe_b64encode(input).replace(b'=', b'')
+    return base64.urlsafe_b64encode(input_text).rstrip(b"=")
 
 
 def crear_url_amb_jwt(request):
     fake_jwt = FakeJWT()
     now = datetime.now()
     expiration = timedelta(days=1)
     claim = {'sub': request.POST['username'], 'nonce': request.GET.get('nonce'), 'iat': int(now.timestamp()),
              'exp': int((now + expiration).timestamp()), 'iss': request.build_absolute_uri('/'),
              'aud': [request.GET.get('client_id')]}
     access_token = fake_jwt.generate_jwt(claim=claim)
     claim['at_hash'] = calculate_at_hash(access_token, hashlib.sha256)
     id_token = fake_jwt.generate_jwt(claim=claim)
     url = "%s%saccess_token=%s&id_token=%s&state=%s" % (request.GET.get('redirect_uri'),
-                                                        get_setting('JWT_CLIENT.REQUEST_RESPONSE_TYPE'), access_token,
+                                                        get_setting('JWT_OIDC.REQUEST_RESPONSE_TYPE'), access_token,
                                                         str(id_token), request.GET.get('state'))
     return url
```

### Comparing `django-jwt-oidc-0.3.9/django_jwt_oidc.egg-info/SOURCES.txt` & `django-jwt-oidc-1.0/django_jwt_oidc.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 django_jwt/views.py
 django_jwt/migrations/__init__.py
 django_jwt/server/__init__.py
 django_jwt/server/admin.py
 django_jwt/server/apps.py
 django_jwt/server/forms.py
 django_jwt/server/models.py
+django_jwt/server/serializers.py
 django_jwt/server/signals.py
 django_jwt/server/urls.py
 django_jwt/server/views.py
 django_jwt/server/views_utils.py
 django_jwt/server/migrations/0001_initial.py
 django_jwt/server/migrations/0002_webpage_logout_all.py
+django_jwt/server/migrations/0003_nonceused_privateclaimswebpage_restrictuserstoweb_and_more.py
 django_jwt/server/migrations/__init__.py
-django_jwt/server/templates/oidc_confirmation.html
-django_jwt/templates/fake_login.html
+django_jwt/server/templates/django_jwt/oidc_confirmation.html
+django_jwt/templates/django_jwt/fake_login.html
 django_jwt_oidc.egg-info/PKG-INFO
 django_jwt_oidc.egg-info/SOURCES.txt
 django_jwt_oidc.egg-info/dependency_links.txt
 django_jwt_oidc.egg-info/requires.txt
 django_jwt_oidc.egg-info/top_level.txt
```

### Comparing `django-jwt-oidc-0.3.9/setup.py` & `django-jwt-oidc-1.0/setup.py`

 * *Files identical despite different names*

