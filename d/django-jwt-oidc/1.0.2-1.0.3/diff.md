# Comparing `tmp/django-jwt-oidc-1.0.2.tar.gz` & `tmp/django-jwt-oidc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-jwt-oidc-1.0.2.tar", last modified: Fri Apr 21 16:12:36 2023, max compression
+gzip compressed data, was "django-jwt-oidc-1.0.3.tar", last modified: Fri Apr 21 16:40:27 2023, max compression
```

## Comparing `django-jwt-oidc-1.0.2.tar` & `django-jwt-oidc-1.0.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:12:36.730783 django-jwt-oidc-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-21 16:12:36.726783 django-jwt-oidc-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:12:36.726783 django-jwt-oidc-1.0.2/django_jwt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:12:36.726783 django-jwt-oidc-1.0.2/django_jwt/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/openid.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/rest_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:12:36.726783 django-jwt-oidc-1.0.2/django_jwt/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:12:36.726783 django-jwt-oidc-1.0.2/django_jwt/server/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/migrations/0002_webpage_logout_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/migrations/0003_nonceused_privateclaimswebpage_restrictuserstoweb_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:12:36.722783 django-jwt-oidc-1.0.2/django_jwt/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:12:36.726783 django-jwt-oidc-1.0.2/django_jwt/server/templates/django_jwt/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/templates/django_jwt/oidc_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/server/views_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/settings_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:12:36.722783 django-jwt-oidc-1.0.2/django_jwt/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:12:36.726783 django-jwt-oidc-1.0.2/django_jwt/templates/django_jwt/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/templates/django_jwt/fake_login.html
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/view_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/django_jwt/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:12:36.726783 django-jwt-oidc-1.0.2/django_jwt_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-21 16:12:36.000000 django-jwt-oidc-1.0.2/django_jwt_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-21 16:12:36.000000 django-jwt-oidc-1.0.2/django_jwt_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:12:36.000000 django-jwt-oidc-1.0.2/django_jwt_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 16:12:36.000000 django-jwt-oidc-1.0.2/django_jwt_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 16:12:36.000000 django-jwt-oidc-1.0.2/django_jwt_oidc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 16:12:36.730783 django-jwt-oidc-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-21 16:12:25.000000 django-jwt-oidc-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:40:27.772463 django-jwt-oidc-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-21 16:40:27.772463 django-jwt-oidc-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:40:27.764463 django-jwt-oidc-1.0.3/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:40:27.764463 django-jwt-oidc-1.0.3/django_jwt/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/openid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/rest_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:40:27.768463 django-jwt-oidc-1.0.3/django_jwt/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:40:27.768463 django-jwt-oidc-1.0.3/django_jwt/server/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/migrations/0002_webpage_logout_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/migrations/0003_nonceused_privateclaimswebpage_restrictuserstoweb_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:40:27.760462 django-jwt-oidc-1.0.3/django_jwt/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:40:27.768463 django-jwt-oidc-1.0.3/django_jwt/server/templates/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/templates/django_jwt/oidc_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17307 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/server/views_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/settings_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:40:27.760462 django-jwt-oidc-1.0.3/django_jwt/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:40:27.768463 django-jwt-oidc-1.0.3/django_jwt/templates/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/templates/django_jwt/fake_login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/view_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/django_jwt/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:40:27.772463 django-jwt-oidc-1.0.3/django_jwt_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-21 16:40:27.000000 django-jwt-oidc-1.0.3/django_jwt_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-21 16:40:27.000000 django-jwt-oidc-1.0.3/django_jwt_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:40:27.000000 django-jwt-oidc-1.0.3/django_jwt_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 16:40:27.000000 django-jwt-oidc-1.0.3/django_jwt_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 16:40:27.000000 django-jwt-oidc-1.0.3/django_jwt_oidc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 16:40:27.772463 django-jwt-oidc-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-21 16:40:15.000000 django-jwt-oidc-1.0.3/setup.py
```

### Comparing `django-jwt-oidc-1.0.2/LICENSE.md` & `django-jwt-oidc-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/PKG-INFO` & `django-jwt-oidc-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jwt-oidc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django library that implements the authentification for OpenId SSO with JWT from oauth2.
 Home-page: https://github.com/Casassarnau/django-jwt
 Author: Arnau Casas Saez
 Author-email: casassarnau@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Casassarnau/django-jwt/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-jwt-oidc-1.0.2/README.md` & `django-jwt-oidc-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/apps.py` & `django-jwt-oidc-1.0.3/django_jwt/apps.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/auth.py` & `django-jwt-oidc-1.0.3/django_jwt/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     def verify_claims(cls, claims, nonce=None, client_id=None):
         openid_domain = get_domain_from_url(get_setting('JWT_OIDC.DISCOVERY_ENDPOINT'))
         if client_id is None and 'django_jwt.server' in get_setting('INSTALLED_APPS'):
             if not any([aud.startswith(openid_domain) for aud in claims.get('aud', [])]):
                 return False
         else:
             if client_id is None:
-                client_id = get_setting('JWT_CLIENT.CLIENT_ID')
+                client_id = get_setting('JWT_OIDC.CLIENT_ID')
             if client_id not in claims.get('aud', []):
                 logger.info('Client id not in aud')
                 return False
         openid_domain = get_domain_from_url(get_setting('JWT_OIDC.DISCOVERY_ENDPOINT'))
         iss_domain = get_domain_from_url(claims.get('iss', ''))
         # openid_domain can't be '' because of apps.py
         if openid_domain != iss_domain:
```

### Comparing `django-jwt-oidc-1.0.2/django_jwt/middleware.py` & `django-jwt-oidc-1.0.3/django_jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/openid.py` & `django-jwt-oidc-1.0.3/django_jwt/openid.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,25 +38,25 @@
     def __init__(self):
         self.jwks_uri = None
         self.authorization_endpoint = None
         self.end_session_endpoint = None
         self.jwks = None
         self.userinfo_endpoint = None
         self.client_type = get_setting('JWT_OIDC.TYPE')
-        if self.client_type == 'client':
+        if self.client_type == 'provider':
             self.__init_local__()
-        elif self.client_type == 'provider':
+        elif self.client_type == 'client':
             self.__init_remote__()
         self.fetch_jwks()
 
     # Updates all the actual JWKS from the OPenId server
     def fetch_jwks(self):
         logger = logging.getLogger(__name__)
         logger.info('Fetching JWKs')
-        if self.client_type == 'remote':
+        if self.client_type == 'client':
             http = urllib3.PoolManager()
             r = http.request('GET', self.jwks_uri)
             if r.status != 200:
                 error_message = 'OpenID returned error code %s on jwks_uri: %s' % (r.status, self.jwks_uri)
                 logger.critical(error_message)
                 raise JWTClientException(error_message)
             jwk_set_json = r.data.decode('UTF-8')
```

### Comparing `django-jwt-oidc-1.0.2/django_jwt/rest_framework.py` & `django-jwt-oidc-1.0.3/django_jwt/rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/server/admin.py` & `django-jwt-oidc-1.0.3/django_jwt/server/admin.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/server/apps.py` & `django-jwt-oidc-1.0.3/django_jwt/server/apps.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/server/forms.py` & `django-jwt-oidc-1.0.3/django_jwt/server/forms.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/server/migrations/0001_initial.py` & `django-jwt-oidc-1.0.3/django_jwt/server/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/server/migrations/0002_webpage_logout_all.py` & `django-jwt-oidc-1.0.3/django_jwt/server/migrations/0002_webpage_logout_all.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/server/migrations/0003_nonceused_privateclaimswebpage_restrictuserstoweb_and_more.py` & `django-jwt-oidc-1.0.3/django_jwt/server/migrations/0003_nonceused_privateclaimswebpage_restrictuserstoweb_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/server/models.py` & `django-jwt-oidc-1.0.3/django_jwt/server/models.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/server/templates/django_jwt/oidc_confirmation.html` & `django-jwt-oidc-1.0.3/django_jwt/server/templates/django_jwt/oidc_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/server/urls.py` & `django-jwt-oidc-1.0.3/django_jwt/server/urls.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/server/views.py` & `django-jwt-oidc-1.0.3/django_jwt/server/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,26 +69,33 @@
     def prepare_scopes_for_template(self, scopes):
         if 'openid' in scopes:
             scopes.remove('openid')
 
     def required_to_log_in(self):
         max_age = self.request.GET.get('max_age', None)
         login_date = self.request.session.get('login_date', None)
+        if max_age is None or login_date is None:
+            return False
         max_login_age = timezone.now() - timezone.timedelta(seconds=int(max_age))
         return login_date < max_login_age
 
     def check_prompt_and_max_age(self):
         prompt = self.request.GET.get('prompt', 'none')
         if (prompt == 'login' and self.request.session.get('oidc_loging_again', None) is None) or \
                 self.required_to_log_in():
             self.request.session['oidc_loging_again'] = True
-            return redirect(get_setting('LOGIN_URL'))
+            return redirect(get_setting('LOGIN_URL') + '?' + urlencode({'next': self.request.get_full_path()}))
         if prompt == 'select_account' and self.request.session.get('oidc_select_user', None) is None:
             self.request.session['oidc_select_user'] = True
-            return redirect(get_setting('SELECT_USER_URL'))
+            return redirect(get_setting('SELECT_USER_URL') + '?' +
+                            urlencode({'next': self.request.get_full_path()}))
+        if self.request.session.get('oidc_select_user', None) is not None:
+            del self.request.session['oidc_select_user']
+        if self.request.session.get('oidc_loging_again', None) is not None:
+            del self.request.session['oidc_loging_again']
         return None
 
     def get(self, request, *args, **kwargs):
         response = self.check_prompt_and_max_age()
         if response is not None:
             return response
         web = kwargs.get('web')
```

### Comparing `django-jwt-oidc-1.0.2/django_jwt/server/views_utils.py` & `django-jwt-oidc-1.0.3/django_jwt/server/views_utils.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/settings_utils.py` & `django-jwt-oidc-1.0.3/django_jwt/settings_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     'JWT_OIDC.MAX_REFRESH': 10,
     'JWT_OIDC.USERINFO_SERIALIZER': 'django_jwt.server.serializers.UserSerializer',
     'JWT_OIDC.USERINFO_SERIALIZER_EXCLUDE': ['password'],
     'JWT_OIDC.CLIENT_DISPLAY': None,
     'JWT_OIDC.CLIENT_PROMPT': None,
     'JWT_OIDC.CLIENT_MAX_AGE': None,
     'JWT_OIDC.CLIENT_UI_LOCALES': None,
-    'JWT_OIDC.CLIENT_CLAIM_LOCALES': None,
+    'JWT_OIDC.CLIENT_CLAIMS_LOCALES': None,
     'JWT_OIDC.CLIENT_ID_TOKEN_HINT': None,
     'JWT_OIDC.CLIENT_LOGIN_HINT': None,
     'JWT_OIDC.CLIENT_ACR_VALUES': None,
 }
 
 
 JWT_DEFAULT_CONVERTERS = {
```

### Comparing `django-jwt-oidc-1.0.2/django_jwt/templates/django_jwt/fake_login.html` & `django-jwt-oidc-1.0.3/django_jwt/templates/django_jwt/fake_login.html`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/urls.py` & `django-jwt-oidc-1.0.3/django_jwt/urls.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/view_utils.py` & `django-jwt-oidc-1.0.3/django_jwt/view_utils.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt/views.py` & `django-jwt-oidc-1.0.3/django_jwt/views.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/django_jwt_oidc.egg-info/PKG-INFO` & `django-jwt-oidc-1.0.3/django_jwt_oidc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jwt-oidc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django library that implements the authentification for OpenId SSO with JWT from oauth2.
 Home-page: https://github.com/Casassarnau/django-jwt
 Author: Arnau Casas Saez
 Author-email: casassarnau@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Casassarnau/django-jwt/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-jwt-oidc-1.0.2/django_jwt_oidc.egg-info/SOURCES.txt` & `django-jwt-oidc-1.0.3/django_jwt_oidc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.2/setup.py` & `django-jwt-oidc-1.0.3/setup.py`

 * *Files identical despite different names*

