# Comparing `tmp/idds-common-1.2.2.tar.gz` & `tmp/idds-common-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-common-1.2.2.tar", last modified: Wed Apr 19 10:35:56 2023, max compression
+gzip compressed data, was "idds-common-1.2.3.tar", last modified: Fri Apr 21 12:33:17 2023, max compression
```

## Comparing `idds-common-1.2.2.tar` & `idds-common-1.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:35:56.558234 idds-common-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-19 10:35:37.000000 idds-common-1.2.2/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-19 10:35:56.558234 idds-common-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-19 10:35:37.000000 idds-common-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:35:56.554234 idds-common-1.2.2/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:35:56.554234 idds-common-1.2.2/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 10:35:37.000000 idds-common-1.2.2/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:35:56.554234 idds-common-1.2.2/lib/idds/common/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 10:35:37.000000 idds-common-1.2.2/lib/idds/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20398 2023-04-19 10:35:37.000000 idds-common-1.2.2/lib/idds/common/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-19 10:35:37.000000 idds-common-1.2.2/lib/idds/common/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-19 10:35:37.000000 idds-common-1.2.2/lib/idds/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-04-19 10:35:37.000000 idds-common-1.2.2/lib/idds/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-19 10:35:37.000000 idds-common-1.2.2/lib/idds/common/dict_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-04-19 10:35:37.000000 idds-common-1.2.2/lib/idds/common/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-19 10:35:37.000000 idds-common-1.2.2/lib/idds/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:35:56.558234 idds-common-1.2.2/lib/idds/common/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 10:35:37.000000 idds-common-1.2.2/lib/idds/common/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-19 10:35:37.000000 idds-common-1.2.2/lib/idds/common/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-19 10:35:37.000000 idds-common-1.2.2/lib/idds/common/plugin/plugin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-19 10:35:37.000000 idds-common-1.2.2/lib/idds/common/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-04-19 10:35:37.000000 idds-common-1.2.2/lib/idds/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-19 10:35:53.000000 idds-common-1.2.2/lib/idds/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:35:56.558234 idds-common-1.2.2/lib/idds_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-19 10:35:56.000000 idds-common-1.2.2/lib/idds_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-19 10:35:56.000000 idds-common-1.2.2/lib/idds_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:35:56.000000 idds-common-1.2.2/lib/idds_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-19 10:35:56.000000 idds-common-1.2.2/lib/idds_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 10:35:56.000000 idds-common-1.2.2/lib/idds_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 10:35:56.558234 idds-common-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-19 10:35:37.000000 idds-common-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:35:56.554234 idds-common-1.2.2/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:35:56.558234 idds-common-1.2.2/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-19 10:35:53.000000 idds-common-1.2.2/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:17.442612 idds-common-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-21 12:33:07.000000 idds-common-1.2.3/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-21 12:33:17.442612 idds-common-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-21 12:33:07.000000 idds-common-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:17.438612 idds-common-1.2.3/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:17.438612 idds-common-1.2.3/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 12:33:07.000000 idds-common-1.2.3/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:17.442612 idds-common-1.2.3/lib/idds/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 12:33:07.000000 idds-common-1.2.3/lib/idds/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20671 2023-04-21 12:33:07.000000 idds-common-1.2.3/lib/idds/common/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-21 12:33:07.000000 idds-common-1.2.3/lib/idds/common/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-21 12:33:07.000000 idds-common-1.2.3/lib/idds/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-04-21 12:33:07.000000 idds-common-1.2.3/lib/idds/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-21 12:33:07.000000 idds-common-1.2.3/lib/idds/common/dict_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-04-21 12:33:07.000000 idds-common-1.2.3/lib/idds/common/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-21 12:33:07.000000 idds-common-1.2.3/lib/idds/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:17.442612 idds-common-1.2.3/lib/idds/common/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 12:33:07.000000 idds-common-1.2.3/lib/idds/common/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-21 12:33:07.000000 idds-common-1.2.3/lib/idds/common/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-21 12:33:07.000000 idds-common-1.2.3/lib/idds/common/plugin/plugin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-21 12:33:07.000000 idds-common-1.2.3/lib/idds/common/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-04-21 12:33:07.000000 idds-common-1.2.3/lib/idds/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-21 12:33:15.000000 idds-common-1.2.3/lib/idds/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:17.442612 idds-common-1.2.3/lib/idds_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-21 12:33:17.000000 idds-common-1.2.3/lib/idds_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-21 12:33:17.000000 idds-common-1.2.3/lib/idds_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:33:17.000000 idds-common-1.2.3/lib/idds_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 12:33:17.000000 idds-common-1.2.3/lib/idds_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 12:33:17.000000 idds-common-1.2.3/lib/idds_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-21 12:33:17.442612 idds-common-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-21 12:33:07.000000 idds-common-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:17.438612 idds-common-1.2.3/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:17.442612 idds-common-1.2.3/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-21 12:33:15.000000 idds-common-1.2.3/tools/env/environment.yml
```

### Comparing `idds-common-1.2.2/LICENSE.rst` & `idds-common-1.2.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.2/PKG-INFO` & `idds-common-1.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-common
-Version: 1.2.2
+Version: 1.2.3
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-common-1.2.2/lib/idds/common/authentication.py` & `idds-common-1.2.3/lib/idds/common/authentication.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,17 @@
 def decode_value(val):
     if isinstance(val, str):
         val = val.encode()
     decoded = base64.urlsafe_b64decode(val + b'==')
     return int.from_bytes(decoded, 'big')
 
 
-def should_verify():
+def should_verify(no_verify=False):
+    if no_verify:
+        return False
     if os.environ.get('IDDS_AUTH_NO_VERIFY', None):
         return False
     return True
 
 
 class BaseAuthentication(object):
     def __init__(self, timeout=None):
@@ -90,31 +92,31 @@
 
 class OIDCAuthentication(BaseAuthentication):
     def __init__(self, timeout=None):
         super(OIDCAuthentication, self).__init__(timeout=timeout)
 
     def get_auth_config(self, vo):
         ret = {'vo': vo, 'oidc_config_url': None, 'client_id': None,
-               'client_secret': None, 'audience': None}
+               'client_secret': None, 'audience': None, 'no_verify': True}
 
         if self.config and self.config.has_section(vo):
-            for name in ['oidc_config_url', 'client_id', 'client_secret', 'vo', 'audience']:
+            for name in ['oidc_config_url', 'client_id', 'client_secret', 'vo', 'audience', 'no_verify']:
                 if self.config.has_option(vo, name):
                     ret[name] = self.config.get(vo, name)
         return ret
 
-    def get_http_content(self, url):
+    def get_http_content(self, url, no_verify=False):
         try:
-            r = requests.get(url, allow_redirects=True, verify=should_verify())
+            r = requests.get(url, allow_redirects=True, verify=should_verify(no_verify))
             return r.content
         except Exception as error:
             return False, 'Failed to get http content for %s: %s' (str(url), str(error))
 
     def get_endpoint_config(self, auth_config):
-        content = self.get_http_content(auth_config['oidc_config_url'])
+        content = self.get_http_content(auth_config['oidc_config_url'], no_verify=auth_config['no_verify'])
         endpoint_config = json.loads(content)
         # ret = {'token_endpoint': , 'device_authorization_endpoint': None}
         return endpoint_config
 
     def get_oidc_sign_url(self, vo):
         try:
             allow_vos = self.get_allow_vos()
@@ -130,15 +132,15 @@
 
             headers = {'content-type': 'application/x-www-form-urlencoded'}
 
             result = requests.session().post(endpoint_config['device_authorization_endpoint'],
                                              # data=json.dumps(data),
                                              urlencode(data).encode(),
                                              timeout=self.timeout,
-                                             verify=should_verify(),
+                                             verify=should_verify(auth_config['no_verify']),
                                              headers=headers)
 
             if result is not None:
                 if result.status_code == HTTP_STATUS_CODE.OK and result.text:
                     return True, json.loads(result.text)
                 else:
                     return False, "Failed to get oidc sign in URL (status: %s, text: %s)" % (result.status_code, result.text)
@@ -175,15 +177,15 @@
             if expires_in > self.max_expires_in:
                 expires_in = self.max_expires_in
 
             result = requests.session().post(endpoint_config['token_endpoint'],
                                              # data=json.dumps(data),
                                              urlencode(data).encode(),
                                              timeout=self.timeout,
-                                             verify=should_verify(),
+                                             verify=should_verify(auth_config['no_verify']),
                                              headers=headers)
             if result is not None:
                 if result.status_code == HTTP_STATUS_CODE.OK and result.text:
                     return True, json.loads(result.text)
                 else:
                     return False, json.loads(result.text)
             else:
@@ -207,30 +209,30 @@
 
             headers = {'content-type': 'application/x-www-form-urlencoded'}
 
             result = requests.session().post(endpoint_config['token_endpoint'],
                                              # data=json.dumps(data),
                                              urlencode(data).encode(),
                                              timeout=self.timeout,
-                                             verify=should_verify(),
+                                             verify=should_verify(auth_config['no_verify']),
                                              headers=headers)
 
             if result is not None:
                 if result.status_code == HTTP_STATUS_CODE.OK and result.text:
                     return True, json.loads(result.text)
                 else:
                     return False, "Failed to refresh oidc token (status: %s, text: %s)" % (result.status_code, result.text)
             else:
                 return False, "Failed to refresh oidc token. Response is None."
         except requests.exceptions.ConnectionError as error:
             return False, 'Failed to refresh oidc token. ConnectionError: ' + str(error)
         except Exception as error:
             return False, 'Failed to refresh oidc token: ' + str(error)
 
-    def get_public_key(self, token, jwks_uri):
+    def get_public_key(self, token, jwks_uri, no_verify=False):
         headers = jwt.get_unverified_header(token)
         if headers is None or 'kid' not in headers:
             raise jwt.exceptions.InvalidTokenError('cannot extract kid from headers')
         kid = headers['kid']
 
         jwks_content = self.get_http_content(jwks_uri)
         jwks = json.loads(jwks_content)
@@ -258,15 +260,15 @@
             # check audience
             decoded_token = jwt.decode(token, verify=False, options={"verify_signature": False})
             audience = decoded_token['aud']
             if audience not in [auth_config['audience'], auth_config['client_id']]:
                 # discovery_endpoint = auth_config['oidc_config_url']
                 return False, "The audience %s of the token doesn't match vo configuration(client_id: %s)." % (audience, auth_config['client_id']), None
 
-            public_key = self.get_public_key(token, endpoint_config['jwks_uri'])
+            public_key = self.get_public_key(token, endpoint_config['jwks_uri'], no_verify=auth_config['no_verify'])
             # decode token only with RS256
             if 'iss' in decoded_token and decoded_token['iss'] and decoded_token['iss'] != endpoint_config['issuer'] and endpoint_config['issuer'].startswith(decoded_token['iss']):
                 # iss is missing the last '/' in access tokens
                 issuer = decoded_token['iss']
             else:
                 issuer = endpoint_config['issuer']
```

### Comparing `idds-common-1.2.2/lib/idds/common/cache.py` & `idds-common-1.2.3/lib/idds/common/cache.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.2/lib/idds/common/config.py` & `idds-common-1.2.3/lib/idds/common/config.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.2/lib/idds/common/constants.py` & `idds-common-1.2.3/lib/idds/common/constants.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.2/lib/idds/common/dict_class.py` & `idds-common-1.2.3/lib/idds/common/dict_class.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.2/lib/idds/common/event.py` & `idds-common-1.2.3/lib/idds/common/event.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.2/lib/idds/common/exceptions.py` & `idds-common-1.2.3/lib/idds/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.2/lib/idds/common/plugin/plugin_base.py` & `idds-common-1.2.3/lib/idds/common/plugin/plugin_base.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.2/lib/idds/common/plugin/plugin_utils.py` & `idds-common-1.2.3/lib/idds/common/plugin/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.2/lib/idds/common/status_utils.py` & `idds-common-1.2.3/lib/idds/common/status_utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.2/lib/idds/common/utils.py` & `idds-common-1.2.3/lib/idds/common/utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.2/lib/idds_common.egg-info/PKG-INFO` & `idds-common-1.2.3/lib/idds_common.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-common
-Version: 1.2.2
+Version: 1.2.3
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-common-1.2.2/lib/idds_common.egg-info/SOURCES.txt` & `idds-common-1.2.3/lib/idds_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.2/setup.py` & `idds-common-1.2.3/setup.py`

 * *Files identical despite different names*

