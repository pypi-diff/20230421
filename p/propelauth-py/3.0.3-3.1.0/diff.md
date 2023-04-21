# Comparing `tmp/propelauth-py-3.0.3.tar.gz` & `tmp/propelauth-py-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-py-3.0.3.tar", last modified: Thu Mar 23 19:37:45 2023, max compression
+gzip compressed data, was "propelauth-py-3.1.0.tar", last modified: Fri Apr 21 18:23:38 2023, max compression
```

## Comparing `propelauth-py-3.0.3.tar` & `propelauth-py-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 19:37:45.949231 propelauth-py-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (116)     1067 2023-03-23 19:37:30.000000 propelauth-py-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1296 2023-03-23 19:37:45.949231 propelauth-py-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      991 2023-03-23 19:37:30.000000 propelauth-py-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 19:37:45.949231 propelauth-py-3.0.3/propelauth_py/
--rw-r--r--   0 runner    (1001) docker     (116)    11617 2023-03-23 19:37:30.000000 propelauth-py-3.0.3/propelauth_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    19469 2023-03-23 19:37:30.000000 propelauth-py-3.0.3/propelauth_py/api.py
--rw-r--r--   0 runner    (1001) docker     (116)     6481 2023-03-23 19:37:30.000000 propelauth-py-3.0.3/propelauth_py/auth_fns.py
--rw-r--r--   0 runner    (1001) docker     (116)     1956 2023-03-23 19:37:30.000000 propelauth-py-3.0.3/propelauth_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)      845 2023-03-23 19:37:30.000000 propelauth-py-3.0.3/propelauth_py/jwt.py
--rw-r--r--   0 runner    (1001) docker     (116)     3322 2023-03-23 19:37:30.000000 propelauth-py-3.0.3/propelauth_py/user.py
--rw-r--r--   0 runner    (1001) docker     (116)      325 2023-03-23 19:37:30.000000 propelauth-py-3.0.3/propelauth_py/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-23 19:37:45.949231 propelauth-py-3.0.3/propelauth_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1296 2023-03-23 19:37:45.000000 propelauth-py-3.0.3/propelauth_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      378 2023-03-23 19:37:45.000000 propelauth-py-3.0.3/propelauth_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-23 19:37:45.000000 propelauth-py-3.0.3/propelauth_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       29 2023-03-23 19:37:45.000000 propelauth-py-3.0.3/propelauth_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2023-03-23 19:37:45.000000 propelauth-py-3.0.3/propelauth_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-23 19:37:45.949231 propelauth-py-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      889 2023-03-23 19:37:30.000000 propelauth-py-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:23:38.440192 propelauth-py-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-21 18:23:38.440192 propelauth-py-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:23:38.436191 propelauth-py-3.1.0/propelauth_py/
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/propelauth_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20409 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/propelauth_py/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/propelauth_py/auth_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/propelauth_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/propelauth_py/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/propelauth_py/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/propelauth_py/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:23:38.440192 propelauth-py-3.1.0/propelauth_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-21 18:23:38.000000 propelauth-py-3.1.0/propelauth_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-21 18:23:38.000000 propelauth-py-3.1.0/propelauth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:23:38.000000 propelauth-py-3.1.0/propelauth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 18:23:38.000000 propelauth-py-3.1.0/propelauth_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 18:23:38.000000 propelauth-py-3.1.0/propelauth_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 18:23:38.440192 propelauth-py-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/setup.py
```

### Comparing `propelauth-py-3.0.3/LICENSE` & `propelauth-py-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.0.3/PKG-INFO` & `propelauth-py-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-py
-Version: 3.0.3
+Version: 3.1.0
 Summary: A python authentication library
 Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-py Version: 3.0.3 Summary: A python
+Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.0 Summary: A python
 authentication library Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth Author-email: support@propelauth.com License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE #
 PropelAuth Python SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A python library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-python). [PropelAuth](https://
```

### Comparing `propelauth-py-3.0.3/README.md` & `propelauth-py-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.0.3/propelauth_py/__init__.py` & `propelauth-py-3.1.0/propelauth_py/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import namedtuple
 
 from propelauth_py.api import _fetch_token_verification_metadata, TokenVerificationMetadata, \
     _fetch_user_metadata_by_user_id, \
     _fetch_user_metadata_by_email, _fetch_user_metadata_by_username, _fetch_batch_user_metadata_by_user_ids, \
     _fetch_batch_user_metadata_by_emails, _fetch_batch_user_metadata_by_usernames, OrgQueryOrderBy, UserQueryOrderBy, \
     _fetch_org, _fetch_org_by_query, _fetch_users_by_query, _fetch_users_in_org, _create_user, _update_user_email, \
-    _update_user_metadata, _create_magic_link, _migrate_user_from_external_source, _create_org, _add_user_to_org, \
-    _delete_user, _disable_user, _enable_user, _allow_org_to_setup_saml_connection, \
+    _update_user_metadata, _create_magic_link, _migrate_user_from_external_source, _create_org, _update_org_metadata, \
+    _add_user_to_org, _delete_user, _disable_user, _enable_user, _allow_org_to_setup_saml_connection, \
     _disallow_org_to_setup_saml_connection, _update_user_password, _create_access_token
 from propelauth_py.auth_fns import wrap_validate_access_token_and_get_user, \
     wrap_validate_access_token_and_get_user_with_org, \
     wrap_validate_access_token_and_get_user_with_org_by_minimum_role, \
     wrap_validate_access_token_and_get_user_with_org_by_exact_role, \
     wrap_validate_access_token_and_get_user_with_org_by_permission, \
     wrap_validate_access_token_and_get_user_with_org_by_all_permissions, \
@@ -48,14 +48,15 @@
     "update_user_email",
     "update_user_metadata",
     "update_user_password",
     "create_magic_link",
     "create_access_token",
     "migrate_user_from_external_source",
     "create_org",
+    "update_org_metadata",
     "add_user_to_org",
     "delete_user",
     "disable_user",
     "enable_user",
     "allow_org_to_setup_saml_connection",
     "disallow_org_to_setup_saml_connection"
 ])
@@ -104,16 +105,16 @@
         return _create_user(auth_url, api_key, email, email_confirmed, send_email_to_confirm_email_address,
                             ask_user_to_update_password_on_login,
                             password, username, first_name, last_name)
 
     def update_user_email(user_id, new_email, require_email_confirmation):
         return _update_user_email(auth_url, api_key, user_id, new_email, require_email_confirmation)
 
-    def update_user_metadata(user_id, username=None, first_name=None, last_name=None):
-        return _update_user_metadata(auth_url, api_key, user_id, username, first_name, last_name)
+    def update_user_metadata(user_id, username=None, first_name=None, last_name=None, metadata=None):
+        return _update_user_metadata(auth_url, api_key, user_id, username, first_name, last_name, metadata)
 
     def update_user_password(user_id, password, ask_user_to_update_password_on_login=False):
         return _update_user_password(auth_url, api_key, user_id, password, ask_user_to_update_password_on_login)
 
     def create_magic_link(email, redirect_to_url=None, expires_in_hours=None, create_new_user_if_one_doesnt_exist=None):
         return _create_magic_link(auth_url, api_key, email, redirect_to_url, expires_in_hours,
                                   create_new_user_if_one_doesnt_exist)
@@ -131,14 +132,17 @@
                                                   existing_mfa_base32_encoded_secret,
                                                   ask_user_to_update_password_on_login,
                                                   enabled, first_name, last_name, username)
 
     def create_org(name):
         return _create_org(auth_url, api_key, name)
 
+    def update_org_metadata(org_id, name=None, can_setup_saml=None, metadata=None):
+        return _update_org_metadata(auth_url, api_key, org_id, name, can_setup_saml, metadata)
+
     def add_user_to_org(user_id, org_id, role):
         return _add_user_to_org(auth_url, api_key, user_id, org_id, role)
 
     def delete_user(user_id):
         return _delete_user(auth_url, api_key, user_id)
 
     def disable_user(user_id):
@@ -203,14 +207,15 @@
         update_user_email=update_user_email,
         update_user_metadata=update_user_metadata,
         update_user_password=update_user_password,
         create_magic_link=create_magic_link,
         create_access_token=create_access_token,
         migrate_user_from_external_source=migrate_user_from_external_source,
         create_org=create_org,
+        update_org_metadata=update_org_metadata,
         add_user_to_org=add_user_to_org,
         enable_user=enable_user,
         disable_user=disable_user,
         delete_user=delete_user,
         allow_org_to_setup_saml_connection=allow_org_to_setup_saml_connection,
         disallow_org_to_setup_saml_connection=disallow_org_to_setup_saml_connection,
     )
```

### Comparing `propelauth-py-3.0.3/propelauth_py/api.py` & `propelauth-py-3.1.0/propelauth_py/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -224,26 +224,28 @@
         raise CreateUserException(response.json())
     elif not response.ok:
         raise RuntimeError("Unknown error when creating user")
 
     return response.json()
 
 
-def _update_user_metadata(auth_url, api_key, user_id, username=None, first_name=None, last_name=None):
+def _update_user_metadata(auth_url, api_key, user_id, username=None, first_name=None, last_name=None, metadata=None):
     if not _is_valid_id(user_id):
         return False
 
     url = auth_url + "/api/backend/v1/user/{}".format(user_id)
     json = {}
     if username is not None:
         json["username"] = username
     if first_name is not None:
         json["first_name"] = first_name
     if last_name is not None:
         json["last_name"] = last_name
+    if metadata is not None:
+        json["metadata"] = metadata
 
     response = requests.put(url, json=json, auth=_ApiKeyAuth(api_key))
     if response.status_code == 401:
         raise ValueError("api_key is incorrect")
     elif response.status_code == 400:
         raise UpdateUserMetadataException(response.json())
     elif response.status_code == 404:
@@ -379,14 +381,40 @@
         raise BadRequestException(response.json())
     elif not response.ok:
         raise RuntimeError("Unknown error when creating an org")
 
     return response.json()
 
 
+def _update_org_metadata(auth_url, api_key, org_id, name=None, can_setup_saml=None, metadata=None):
+    if not _is_valid_id(org_id):
+        return False
+
+    url = auth_url + "/api/backend/v1/org/{}".format(org_id)
+    json = {}
+    if name is not None:
+        json["name"] = name
+    if can_setup_saml is not None:
+        json["can_setup_saml"] = can_setup_saml
+    if metadata is not None:
+        json["metadata"] = metadata
+
+    response = requests.put(url, json=json, auth=_ApiKeyAuth(api_key))
+    if response.status_code == 401:
+        raise ValueError("api_key is incorrect")
+    elif response.status_code == 400:
+        raise UpdateUserMetadataException(response.json())
+    elif response.status_code == 404:
+        return False
+    elif not response.ok:
+        raise RuntimeError("Unknown error when updating org metadata")
+
+    return True
+
+
 def _add_user_to_org(auth_url, api_key, user_id, org_id, role):
     url = auth_url + "/api/backend/v1/org/add_user"
     json = {"user_id": user_id, "org_id": org_id, "role": role}
 
     response = requests.post(url, json=json, auth=_ApiKeyAuth(api_key))
     if response.status_code == 401:
         raise ValueError("api_key is incorrect")
```

### Comparing `propelauth-py-3.0.3/propelauth_py/auth_fns.py` & `propelauth-py-3.1.0/propelauth_py/auth_fns.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.0.3/propelauth_py/errors.py` & `propelauth-py-3.1.0/propelauth_py/errors.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.0.3/propelauth_py/jwt.py` & `propelauth-py-3.1.0/propelauth_py/jwt.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.0.3/propelauth_py.egg-info/PKG-INFO` & `propelauth-py-3.1.0/propelauth_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-py
-Version: 3.0.3
+Version: 3.1.0
 Summary: A python authentication library
 Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-py Version: 3.0.3 Summary: A python
+Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.0 Summary: A python
 authentication library Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth Author-email: support@propelauth.com License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE #
 PropelAuth Python SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A python library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-python). [PropelAuth](https://
```

### Comparing `propelauth-py-3.0.3/setup.py` & `propelauth-py-3.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="propelauth-py",
-    version="3.0.3",
+    version="3.1.0",
     description="A python authentication library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-py",
     packages=find_packages(include=["propelauth_py"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
```

