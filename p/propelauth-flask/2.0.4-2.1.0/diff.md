# Comparing `tmp/propelauth-flask-2.0.4.tar.gz` & `tmp/propelauth-flask-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-flask-2.0.4.tar", last modified: Thu Mar 23 21:57:49 2023, max compression
+gzip compressed data, was "propelauth-flask-2.1.0.tar", last modified: Fri Apr 21 19:59:23 2023, max compression
```

## Comparing `propelauth-flask-2.0.4.tar` & `propelauth-flask-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 21:57:49.130547 propelauth-flask-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (116)     1067 2023-03-23 21:57:32.000000 propelauth-flask-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1311 2023-03-23 21:57:49.130547 propelauth-flask-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      985 2023-03-23 21:57:32.000000 propelauth-flask-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 21:57:49.130547 propelauth-flask-2.0.4/propelauth_flask/
--rw-r--r--   0 runner    (1001) docker     (116)     4685 2023-03-23 21:57:32.000000 propelauth-flask-2.0.4/propelauth_flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7602 2023-03-23 21:57:32.000000 propelauth-flask-2.0.4/propelauth_flask/auth_decorator.py
--rw-r--r--   0 runner    (1001) docker     (116)     1047 2023-03-23 21:57:32.000000 propelauth-flask-2.0.4/propelauth_flask/user.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 21:57:49.130547 propelauth-flask-2.0.4/propelauth_flask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1311 2023-03-23 21:57:49.000000 propelauth-flask-2.0.4/propelauth_flask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      314 2023-03-23 21:57:49.000000 propelauth-flask-2.0.4/propelauth_flask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-23 21:57:49.000000 propelauth-flask-2.0.4/propelauth_flask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       41 2023-03-23 21:57:49.000000 propelauth-flask-2.0.4/propelauth_flask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2023-03-23 21:57:49.000000 propelauth-flask-2.0.4/propelauth_flask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-23 21:57:49.130547 propelauth-flask-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      928 2023-03-23 21:57:32.000000 propelauth-flask-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:59:23.065268 propelauth-flask-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-21 19:59:05.000000 propelauth-flask-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-21 19:59:23.065268 propelauth-flask-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-21 19:59:05.000000 propelauth-flask-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:59:23.065268 propelauth-flask-2.1.0/propelauth_flask/
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-21 19:59:05.000000 propelauth-flask-2.1.0/propelauth_flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-21 19:59:05.000000 propelauth-flask-2.1.0/propelauth_flask/auth_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-21 19:59:05.000000 propelauth-flask-2.1.0/propelauth_flask/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:59:23.065268 propelauth-flask-2.1.0/propelauth_flask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-21 19:59:23.000000 propelauth-flask-2.1.0/propelauth_flask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-21 19:59:23.000000 propelauth-flask-2.1.0/propelauth_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:59:23.000000 propelauth-flask-2.1.0/propelauth_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 19:59:23.000000 propelauth-flask-2.1.0/propelauth_flask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 19:59:23.000000 propelauth-flask-2.1.0/propelauth_flask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 19:59:23.065268 propelauth-flask-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-21 19:59:05.000000 propelauth-flask-2.1.0/setup.py
```

### Comparing `propelauth-flask-2.0.4/LICENSE` & `propelauth-flask-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.0.4/PKG-INFO` & `propelauth-flask-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-flask
-Version: 2.0.4
+Version: 2.1.0
 Summary: A library for managing authentication in Flask
 Home-page: https://github.com/propelauth/propelauth-flask
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-flask Version: 2.0.4 Summary: A library
+Metadata-Version: 2.1 Name: propelauth-flask Version: 2.1.0 Summary: A library
 for managing authentication in Flask Home-page: https://github.com/propelauth/
 propelauth-flask Author: PropelAuth Author-email: support@propelauth.com
 License: MIT Platform: UNKNOWN Description-Content-Type: text/markdown License-
 File: LICENSE # PropelAuth Flask SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A Flask library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-flask). [PropelAuth](https://
```

### Comparing `propelauth-flask-2.0.4/README.md` & `propelauth-flask-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.0.4/propelauth_flask/__init__.py` & `propelauth-flask-2.1.0/propelauth_flask/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
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
@@ -71,13 +72,14 @@
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

### Comparing `propelauth-flask-2.0.4/propelauth_flask/auth_decorator.py` & `propelauth-flask-2.1.0/propelauth_flask/auth_decorator.py`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.0.4/propelauth_flask/user.py` & `propelauth-flask-2.1.0/propelauth_flask/user.py`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.0.4/propelauth_flask.egg-info/PKG-INFO` & `propelauth-flask-2.1.0/propelauth_flask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-flask
-Version: 2.0.4
+Version: 2.1.0
 Summary: A library for managing authentication in Flask
 Home-page: https://github.com/propelauth/propelauth-flask
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-flask Version: 2.0.4 Summary: A library
+Metadata-Version: 2.1 Name: propelauth-flask Version: 2.1.0 Summary: A library
 for managing authentication in Flask Home-page: https://github.com/propelauth/
 propelauth-flask Author: PropelAuth Author-email: support@propelauth.com
 License: MIT Platform: UNKNOWN Description-Content-Type: text/markdown License-
 File: LICENSE # PropelAuth Flask SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A Flask library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-flask). [PropelAuth](https://
```

### Comparing `propelauth-flask-2.0.4/setup.py` & `propelauth-flask-2.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="propelauth-flask",
-    version="2.0.4",
+    version="2.1.0",
     description="A library for managing authentication in Flask",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-flask",
     packages=find_packages(include=["propelauth_flask"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
     license="MIT",
-    install_requires=["flask>=0.9", "propelauth-py==3.0.3", "requests"],
+    install_requires=["flask>=0.9", "propelauth-py==3.1.0", "requests"],
     setup_requires=pytest_runner,
     tests_require=["pytest==4.4.1"],
     test_suite="tests",
 )
```

