# Comparing `tmp/propelauth-django-rest-framework-2.0.2.tar.gz` & `tmp/propelauth-django-rest-framework-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-django-rest-framework-2.0.2.tar", last modified: Thu Mar 23 21:58:34 2023, max compression
+gzip compressed data, was "propelauth-django-rest-framework-2.1.0.tar", last modified: Fri Apr 21 20:00:10 2023, max compression
```

## Comparing `propelauth-django-rest-framework-2.0.2.tar` & `propelauth-django-rest-framework-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 21:58:34.447033 propelauth-django-rest-framework-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1067 2023-03-23 21:58:10.000000 propelauth-django-rest-framework-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1392 2023-03-23 21:58:34.443032 propelauth-django-rest-framework-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1018 2023-03-23 21:58:10.000000 propelauth-django-rest-framework-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 21:58:34.443032 propelauth-django-rest-framework-2.0.2/propelauth_django_rest_framework/
--rw-r--r--   0 runner    (1001) docker     (116)     4666 2023-03-23 21:58:10.000000 propelauth-django-rest-framework-2.0.2/propelauth_django_rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8426 2023-03-23 21:58:10.000000 propelauth-django-rest-framework-2.0.2/propelauth_django_rest_framework/auth_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 21:58:34.443032 propelauth-django-rest-framework-2.0.2/propelauth_django_rest_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1392 2023-03-23 21:58:34.000000 propelauth-django-rest-framework-2.0.2/propelauth_django_rest_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      399 2023-03-23 21:58:34.000000 propelauth-django-rest-framework-2.0.2/propelauth_django_rest_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-23 21:58:34.000000 propelauth-django-rest-framework-2.0.2/propelauth_django_rest_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       57 2023-03-23 21:58:34.000000 propelauth-django-rest-framework-2.0.2/propelauth_django_rest_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       33 2023-03-23 21:58:34.000000 propelauth-django-rest-framework-2.0.2/propelauth_django_rest_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-23 21:58:34.447033 propelauth-django-rest-framework-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1011 2023-03-23 21:58:10.000000 propelauth-django-rest-framework-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:00:10.183692 propelauth-django-rest-framework-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-21 19:59:56.000000 propelauth-django-rest-framework-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-21 20:00:10.183692 propelauth-django-rest-framework-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-21 19:59:56.000000 propelauth-django-rest-framework-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:00:10.183692 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-21 19:59:56.000000 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-04-21 19:59:56.000000 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework/auth_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:00:10.183692 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-21 20:00:10.000000 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-21 20:00:10.000000 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:00:10.000000 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-21 20:00:10.000000 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 20:00:10.000000 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 20:00:10.183692 propelauth-django-rest-framework-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-21 19:59:56.000000 propelauth-django-rest-framework-2.1.0/setup.py
```

### Comparing `propelauth-django-rest-framework-2.0.2/LICENSE` & `propelauth-django-rest-framework-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.0.2/PKG-INFO` & `propelauth-django-rest-framework-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-django-rest-framework
-Version: 2.0.2
+Version: 2.1.0
 Summary: A library for managing authentication in Django Rest Framework
 Home-page: https://github.com/propelauth/propelauth-django-rest-framework
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.0.2
+Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.1.0
 Summary: A library for managing authentication in Django Rest Framework Home-
 page: https://github.com/propelauth/propelauth-django-rest-framework Author:
 PropelAuth Author-email: support@propelauth.com License: MIT Platform: UNKNOWN
 Description-Content-Type: text/markdown License-File: LICENSE # PropelAuth
 Django Rest Framework Library
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A Django Rest Framework library for managing authentication, backed by
```

### Comparing `propelauth-django-rest-framework-2.0.2/README.md` & `propelauth-django-rest-framework-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.0.2/propelauth_django_rest_framework/__init__.py` & `propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "fetch_org", "fetch_org_by_query", "fetch_users_by_query", "fetch_users_in_org",
     "create_user",
     "update_user_email",
     "update_user_metadata",
     "update_user_password",
     "create_magic_link", "create_access_token",
     "migrate_user_from_external_source", "create_org", "add_user_to_org",
+    "update_org_metadata",
     "delete_user", "disable_user", "enable_user",
     "allow_org_to_setup_saml_connection", "disallow_org_to_setup_saml_connection"
 ])
 
 
 def init_auth(auth_url: str, api_key: str, token_verification_metadata: TokenVerificationMetadata = None,
               debug_mode=False):
@@ -69,13 +70,14 @@
         update_user_metadata=auth.update_user_metadata,
         update_user_password=auth.update_user_password,
         create_magic_link=auth.create_magic_link,
         create_access_token=auth.create_access_token,
         migrate_user_from_external_source=auth.migrate_user_from_external_source,
         create_org=auth.create_org,
         add_user_to_org=auth.add_user_to_org,
+        update_org_metadata=auth.update_org_metadata,
         enable_user=auth.enable_user,
         disable_user=auth.disable_user,
         delete_user=auth.delete_user,
         allow_org_to_setup_saml_connection=auth.allow_org_to_setup_saml_connection,
         disallow_org_to_setup_saml_connection=auth.disallow_org_to_setup_saml_connection,
     )
```

### Comparing `propelauth-django-rest-framework-2.0.2/propelauth_django_rest_framework/auth_helpers.py` & `propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework/auth_helpers.py`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.0.2/propelauth_django_rest_framework.egg-info/PKG-INFO` & `propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-django-rest-framework
-Version: 2.0.2
+Version: 2.1.0
 Summary: A library for managing authentication in Django Rest Framework
 Home-page: https://github.com/propelauth/propelauth-django-rest-framework
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.0.2
+Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.1.0
 Summary: A library for managing authentication in Django Rest Framework Home-
 page: https://github.com/propelauth/propelauth-django-rest-framework Author:
 PropelAuth Author-email: support@propelauth.com License: MIT Platform: UNKNOWN
 Description-Content-Type: text/markdown License-File: LICENSE # PropelAuth
 Django Rest Framework Library
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A Django Rest Framework library for managing authentication, backed by
```

### Comparing `propelauth-django-rest-framework-2.0.2/setup.py` & `propelauth-django-rest-framework-2.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="propelauth-django-rest-framework",
-    version="2.0.2",
+    version="2.1.0",
     description="A library for managing authentication in Django Rest Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-django-rest-framework",
     packages=find_packages(include=["propelauth_django_rest_framework"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
     license="MIT",
-    install_requires=["django", "djangorestframework", "propelauth-py==3.0.3", "requests"],
+    install_requires=["django", "djangorestframework", "propelauth-py==3.1.0", "requests"],
     setup_requires=pytest_runner,
     tests_require=["pytest==4.4.1"],
     test_suite="tests",
 )
```

