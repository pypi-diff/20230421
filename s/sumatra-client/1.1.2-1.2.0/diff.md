# Comparing `tmp/sumatra-client-1.1.2.tar.gz` & `tmp/sumatra-client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumatra-client-1.1.2.tar", last modified: Wed Mar  8 23:33:22 2023, max compression
+gzip compressed data, was "sumatra-client-1.2.0.tar", last modified: Fri Apr 21 20:39:45 2023, max compression
```

## Comparing `sumatra-client-1.1.2.tar` & `sumatra-client-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-03-08 23:33:22.828618 sumatra-client-1.1.2/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      167 2021-12-08 03:47:40.000000 sumatra-client-1.1.2/LICENSE
--rw-r--r--   0 kuhlmann   (501) staff       (20)      542 2023-03-08 23:33:22.828754 sumatra-client-1.1.2/PKG-INFO
--rw-r--r--   0 kuhlmann   (501) staff       (20)       93 2022-02-04 23:04:56.000000 sumatra-client-1.1.2/README.md
--rw-r--r--   0 kuhlmann   (501) staff       (20)       90 2021-12-03 22:49:56.000000 sumatra-client-1.1.2/pyproject.toml
--rw-r--r--   0 kuhlmann   (501) staff       (20)      767 2023-03-08 23:33:22.829364 sumatra-client-1.1.2/setup.cfg
--rw-r--r--   0 kuhlmann   (501) staff       (20)       85 2022-09-23 13:58:44.000000 sumatra-client-1.1.2/setup.py
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-03-08 23:33:22.825332 sumatra-client-1.1.2/sumatra_client/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      178 2023-03-08 23:30:11.000000 sumatra-client-1.1.2/sumatra_client/__init__.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     7453 2023-03-08 23:30:11.000000 sumatra-client-1.1.2/sumatra_client/auth.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)    21413 2023-03-08 23:30:11.000000 sumatra-client-1.1.2/sumatra_client/cli.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)    97533 2023-03-08 23:30:11.000000 sumatra-client-1.1.2/sumatra_client/client.py
--rw-r--r--   0 kuhlmann   (501) staff       (20)     8211 2023-03-08 23:30:11.000000 sumatra-client-1.1.2/sumatra_client/config.py
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-03-08 23:33:22.828022 sumatra-client-1.1.2/sumatra_client.egg-info/
--rw-r--r--   0 kuhlmann   (501) staff       (20)      542 2023-03-08 23:33:22.000000 sumatra-client-1.1.2/sumatra_client.egg-info/PKG-INFO
--rw-r--r--   0 kuhlmann   (501) staff       (20)      461 2023-03-08 23:33:22.000000 sumatra-client-1.1.2/sumatra_client.egg-info/SOURCES.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2023-03-08 23:33:22.000000 sumatra-client-1.1.2/sumatra_client.egg-info/dependency_links.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)       52 2023-03-08 23:33:22.000000 sumatra-client-1.1.2/sumatra_client.egg-info/entry_points.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2021-12-03 22:57:42.000000 sumatra-client-1.1.2/sumatra_client.egg-info/not-zip-safe
--rw-r--r--   0 kuhlmann   (501) staff       (20)       97 2023-03-08 23:33:22.000000 sumatra-client-1.1.2/sumatra_client.egg-info/requires.txt
--rw-r--r--   0 kuhlmann   (501) staff       (20)       15 2023-03-08 23:33:22.000000 sumatra-client-1.1.2/sumatra_client.egg-info/top_level.txt
-drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-03-08 23:33:22.828317 sumatra-client-1.1.2/tests/
--rw-r--r--   0 kuhlmann   (501) staff       (20)     2309 2022-09-23 13:58:44.000000 sumatra-client-1.1.2/tests/test_config.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-04-21 20:39:45.732391 sumatra-client-1.2.0/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      167 2021-12-08 03:47:40.000000 sumatra-client-1.2.0/LICENSE
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      542 2023-04-21 20:39:45.732576 sumatra-client-1.2.0/PKG-INFO
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       93 2022-02-04 23:04:56.000000 sumatra-client-1.2.0/README.md
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       90 2021-12-03 22:49:56.000000 sumatra-client-1.2.0/pyproject.toml
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      767 2023-04-21 20:39:45.733482 sumatra-client-1.2.0/setup.cfg
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       85 2022-09-23 13:58:44.000000 sumatra-client-1.2.0/setup.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-04-21 20:39:45.728530 sumatra-client-1.2.0/sumatra_client/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      178 2023-04-05 19:51:09.000000 sumatra-client-1.2.0/sumatra_client/__init__.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     6859 2023-04-21 20:08:04.000000 sumatra-client-1.2.0/sumatra_client/auth.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)    21519 2023-04-21 20:08:04.000000 sumatra-client-1.2.0/sumatra_client/cli.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)    98466 2023-04-21 20:08:04.000000 sumatra-client-1.2.0/sumatra_client/client.py
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     8211 2023-04-05 19:51:09.000000 sumatra-client-1.2.0/sumatra_client/config.py
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-04-21 20:39:45.731471 sumatra-client-1.2.0/sumatra_client.egg-info/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      542 2023-04-21 20:39:45.000000 sumatra-client-1.2.0/sumatra_client.egg-info/PKG-INFO
+-rw-r--r--   0 kuhlmann   (501) staff       (20)      461 2023-04-21 20:39:45.000000 sumatra-client-1.2.0/sumatra_client.egg-info/SOURCES.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2023-04-21 20:39:45.000000 sumatra-client-1.2.0/sumatra_client.egg-info/dependency_links.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       52 2023-04-21 20:39:45.000000 sumatra-client-1.2.0/sumatra_client.egg-info/entry_points.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)        1 2021-12-03 22:57:42.000000 sumatra-client-1.2.0/sumatra_client.egg-info/not-zip-safe
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       97 2023-04-21 20:39:45.000000 sumatra-client-1.2.0/sumatra_client.egg-info/requires.txt
+-rw-r--r--   0 kuhlmann   (501) staff       (20)       15 2023-04-21 20:39:45.000000 sumatra-client-1.2.0/sumatra_client.egg-info/top_level.txt
+drwxr-xr-x   0 kuhlmann   (501) staff       (20)        0 2023-04-21 20:39:45.731951 sumatra-client-1.2.0/tests/
+-rw-r--r--   0 kuhlmann   (501) staff       (20)     2309 2022-09-23 13:58:44.000000 sumatra-client-1.2.0/tests/test_config.py
```

### Comparing `sumatra-client-1.1.2/PKG-INFO` & `sumatra-client-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumatra-client
-Version: 1.1.2
+Version: 1.2.0
 Summary: Sumatra Python Client and CLI
 Home-page: https://sumatra.ai
 Author: Sumatra
 Author-email: support@sumatra.ai
 License: Sumatra Proprietary
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sumatra-client-1.1.2/setup.cfg` & `sumatra-client-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sumatra-client
-version = 1.1.2
+version = 1.2.0
 author = Sumatra
 author_email = support@sumatra.ai
 url = https://sumatra.ai
 description = Sumatra Python Client and CLI
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Sumatra Proprietary
```

### Comparing `sumatra-client-1.1.2/sumatra_client/auth.py` & `sumatra-client-1.2.0/sumatra_client/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
 import click
 import requests
-import secrets
-import base64
-import hashlib
+import json
 import time
 from logging import getLogger
 
 from configparser import ConfigParser
 from requests.auth import AuthBase
 from urllib.parse import urlencode, urlparse, parse_qs
 from http.server import BaseHTTPRequestHandler, HTTPServer
@@ -28,28 +26,30 @@
     def __str__(self) -> str:
         return "Your auth token has expired. Run `sumatra login` to refresh."
 
 
 class CognitoJwtAuth(AuthBase):
     """Authorization: JWT_TOKEN"""
 
-    def __init__(self):
+    def __init__(self, tenant):
         self._jwt_token = CONFIG.jwt_token
+        self._tenant = tenant
 
     def __eq__(self, other):
         return self._jwt_token == other._jwt_token
 
     def __ne__(self, other):
         return not self == other
 
     def __call__(self, r):
         if not self._jwt_token:
             auth = CognitoAuth()
             self._jwt_token = auth.get_or_refresh_token()
         r.headers["Authorization"] = self._jwt_token
+        r.headers["x-sumatra-tenant"] = self._tenant
         return r
 
 
 class SDKKeyAuth(AuthBase):
     """x-api-key: SDK_KEY"""
 
     def __init__(self):
@@ -66,53 +66,49 @@
         return r
 
 
 class CallbackServerHandler(BaseHTTPRequestHandler):
     def log_message(self, format, *args):
         logger.debug(format % args)
 
-    def do_GET(self):
-        ret = parse_qs(urlparse(self.path).query)
-        logger.debug(f"Received local auth callback: {ret}")
+    def do_POST(self):
+        l = int(self.headers.get("Content-Length", 0))
+        response_json = json.loads(self.rfile.read(l))
+        if "error" in response_json:
+            raise RuntimeError(response_json.get("error"))
 
-        self.server.code = ret["code"][0]
-        self.server.state = ret["state"][0]
+        self.server.refresh_token = response_json.get("refreshToken")
+        self.server.id_token = response_json.get("idToken")
+        self.server.access_token = response_json.get("accessToken")
+        self.server.expires_at = response_json.get("expiration")
 
-        self.send_response(301)
-        self.send_header("Location", "https://sumatra.ai/login-success")
+        self.send_response(200)
         self.end_headers()
+        self.wfile.flush()
 
 
 class CallbackServer(HTTPServer):
     def __init__(self, *args, **kwargs):
         # Because HTTPServer is an old-style class, super() can't be used.
         HTTPServer.__init__(self, *args, **kwargs)
-        self.code = None
-        self.state = None
+        self.refresh_token = None
+        self.id_token = None
+        self.access_token = None
+        self.expires_at = None
 
 
 class CognitoAuth:
     def __init__(self):
         self._redirect_uri = None
-        self._code = None
         self._code_verifier = None
+        self._response = {}
 
     def fetch_new_tokens(self) -> None:
-        self._fetch_authorization_code()
-
-        params = {
-            "grant_type": "authorization_code",
-            "code": self._code,
-            "code_verifier": self._code_verifier,
-            "redirect_uri": self._redirect_uri,
-            "client_id": CONFIG.user_pool_client_id,
-        }
-        response = requests.post(CONFIG.cognito_token_url, data=params)
-        response.raise_for_status()
-        tokens = self._parse_token_response(response)
+        self._fetch_authorization_tokens()
+        tokens = self._parse_token_response(self._response)
         self._save_tokens(tokens)
 
     def get_or_refresh_token(self) -> str:
         tokens = self._load_tokens()
         if time.time() > tokens["expiration"]:
             try:
                 tokens = self._refresh_tokens(tokens["refresh"])
@@ -156,76 +152,60 @@
             "refresh_token": refresh_token,
             "client_id": CONFIG.user_pool_client_id,
             "scope": "email profile openid aws.cognito.signin.user.admin",
         }
         logger.debug(f"POSTing to {CONFIG.cognito_token_url}: {params}")
         response = requests.post(CONFIG.cognito_token_url, data=params)
         logger.debug(f"Received: {response}")
-        new_tokens = self._parse_token_response(response)
+        new_tokens = self._parse_token_response(response.json())
         new_tokens["refresh"] = refresh_token
         self._save_tokens(new_tokens)
         return new_tokens
 
     # open browser and allow user to authenticate using selected cognito flow
     # and store returned auth code
-    def _fetch_authorization_code(self):
+    def _fetch_authorization_tokens(self):
         logger.info("Launching browser-based authentication.")
-        auth_url, init_state = self._build_auth_url()
+        auth_url = self._build_auth_url()
         try:
             click.launch(auth_url)
             self._httpd.handle_request()
         finally:
-            assert init_state == self._httpd.state
-            self._code = self._httpd.code
+            self._response = {
+                "refresh_token": self._httpd.refresh_token,
+                "id_token": self._httpd.id_token,
+                "access_token": self._httpd.access_token,
+                "expires_at": self._httpd.expires_at,
+            }
             self._httpd.server_close()
 
     def _build_auth_url(self):
-        self._code_verifier = secrets.token_urlsafe(43)
-        code_challenge = base64.urlsafe_b64encode(
-            hashlib.sha256(self._code_verifier.encode("utf-8")).digest()
-        ).rstrip(b"=")
-        state = str(secrets.randbits(64))
-
         self._start_callback_listener()
 
-        params = {
-            "redirect_uri": self._redirect_uri,
-            "response_type": "code",
-            "client_id": CONFIG.user_pool_client_id,
-            "identity_provider": "COGNITO",
-            "scope": "email profile openid aws.cognito.signin.user.admin",
-            "state": state,
-            "code_challenge": code_challenge,
-            "code_challenge_method": "S256",
-        }
-
-        return f"{CONFIG.cognito_auth_url}?{urlencode(params)}", state
+        return f"{CONFIG.instance_url}/log-in-ext/{self._redirect_port}"
 
     def _start_callback_listener(self):
         for port in AUTH_REDIRECT_PORTS:
             try:
                 self._httpd = CallbackServer(("", int(port)), CallbackServerHandler)
                 self._redirect_uri = f"http://localhost:{port}"
+                self._redirect_port = port
                 break
             except OSError as e:
                 if e.errno == 48:
                     continue
                 else:
                     raise OSError(f"error during authentication: {e}")
         else:
-            raise e
+            raise
 
     def _parse_token_response(self, response):
-        response_json = response.json()
-        if "error" in response_json:
-            raise RuntimeError(response_json["error"])
-
         now = int(time.time())
-        expires_in = response_json.get("expires_in")
-        expiration = now if not expires_in else now + int(expires_in)
+        expires_at = response.get("expires_at")
+        expiration = now if not expires_at else int(expires_at)
 
         return {
-            "access": response_json.get("access_token"),
-            "id": response_json.get("id_token"),
-            "refresh": response_json.get("refresh_token"),
+            "access": response.get("access_token"),
+            "id": response.get("id_token"),
+            "refresh": response.get("refresh_token"),
             "expiration": expiration,
         }
```

### Comparing `sumatra-client-1.1.2/sumatra_client/cli.py` & `sumatra-client-1.2.0/sumatra_client/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 import uuid
 import argparse
 import logging
+import requests
 from colorama import Fore, Style
 from sumatra_client.config import CONFIG
 from sumatra_client.auth import CognitoAuth
 from sumatra_client.client import Client
 
 
 logger = logging.getLogger("sumatra.cli")
@@ -111,24 +112,26 @@
 
 
 def login(args) -> None:
     instance = args.instance
     try:
         curr_instance = CONFIG.instance
     except:
-        curr_instance = None
-    while not instance:
-        prompt = "Sumatra Instance URL [%s]: " % (
-            curr_instance or "e.g.: yourco.sumatra.ai"
-        )
-        instance = input(prompt).strip()
-        if not instance:
-            instance = curr_instance
+        curr_instance = "console.sumatra.ai"
+    prompt = f"Sumatra Instance URL [{curr_instance}]: "
+    instance = input(prompt).strip()
+    if not instance:
+        instance = curr_instance
     CONFIG.instance = instance
-    CONFIG.update_from_stack()
+    try:
+        CONFIG.update_from_stack()
+    except requests.exceptions.ConnectionError:
+        print(f"Unable to connect to {instance}. Please check the URL and try again.")
+        sys.exit(1)
+
     CONFIG.save(update_default_instance=True)
 
     auth = CognitoAuth()
     auth.fetch_new_tokens()
     print("Authentication successful.")
```

### Comparing `sumatra-client-1.1.2/sumatra_client/client.py` & `sumatra-client-1.2.0/sumatra_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,29 +107,33 @@
     __Bots:__ Set the `SUMATRA_INSTANCE` and `SUMATRA_SDK_KEY` environment variables
     """
 
     def __init__(
         self,
         instance: Optional[str] = None,
         branch: Optional[str] = None,
+        workspace: str = "_default",
     ):
         """
         Create connection object.
 
         Arguments:
             instance: Sumatra instance url, e.g. `yourco.sumatra.ai`. If unspecified, the your config default will be used.
             branch: Set default branch. If unspecified, your config default will be used.
+            workspace: Sumatra workspace name to connect to. Required if not using an SDK key
         """
         if instance:
             CONFIG.instance = instance
         if CONFIG.sdk_key:
             auth: AuthBase = SDKKeyAuth()
             endpoint = CONFIG.sdk_graphql_url
         else:
-            auth = CognitoJwtAuth()
+            if not workspace:
+                raise ValueError("workspace argument required when not using an SDK key")
+            auth = CognitoJwtAuth(workspace)
             endpoint = CONFIG.console_graphql_url
 
         self._branch = branch or CONFIG.default_branch
 
         self._gql_client = python_graphql_client.GraphqlClient(
             auth=auth, endpoint=endpoint
         )
@@ -954,14 +958,15 @@
 
         where = f"where {where}" if where else ""
         inputs = ""
         if include_inputs:
             inputs = ', event as "_inputs"'
             json_fields.append("_inputs")
 
+        features = [f'"{feature}"' for feature in features]
         returned = ", ".join(["_id", "_time"] + features)
 
         query = f"""with tmp as (
             select
             event_id "_id"
             ,event_ts "_time"
             {inputs}
@@ -2445,15 +2450,15 @@
         ret = self._gql_client.execute(query=query)
 
         if "errors" in ret:
             raise RuntimeError(ret["errors"][0]["message"])
 
         return [tenant["key"] for tenant in ret["data"]["tenants"]["nodes"]]
 
-    def set_tenant(self, username: Str, tenant: Str):
+    def set_tenant(self, username: str, tenant: str):
         """
         Set tenant for user
         """
         query = """
             mutation SetTenant($username: String!, $tenant: String!) {
                  setUserTenant(username: $username, tenant: $tenant) {
                     tenant
@@ -2469,15 +2474,15 @@
                 "tenant": tenant,
             },
         )
 
         if "errors" in ret:
             raise RuntimeError(ret["errors"][0]["message"])
 
-    def set_role(self, username: Str, role: Str):
+    def set_role(self, username: str, role: str):
         """
         Set role for user
         """
         query = """
             mutation SetRole($username: String!, $role: String!) {
                  setUserRole(username: $username, role: $role) {
                     role
@@ -2969,24 +2974,42 @@
         S3 bucket path where results are stored.
         """
         self.wait()
         return self._mtr["path"]
 
     def get_events(self, event_type: str, features: List[str] = []) -> pd.DataFrame:
         """
+        (DEPRECATED)
         Return enriched events of specified type. Waits if
         job is still processing.
 
         Arguments:
             event_type: Name of event type to fetch.
             features: Feature names to fetch. By default, fetch all.
 
         Returns:
             Enriched events
         """
+        logger.warn(
+            "get_events() is deprecated and will be removed in the next release. Use get_features() instead."
+        )
+        return self.get_features(event_type, features)
+
+    def get_features(self, event_type: str, features: List[str] = []) -> pd.DataFrame:
+        """
+        Return feature values for given event type. Waits if
+        job is still processing.
+
+        Arguments:
+            event_type: Name of event type to fetch.
+            features: Feature names to fetch. By default, fetch all.
+
+        Returns:
+            Feature dataframe
+        """
         # if event_type not in self.event_types:
         #    raise RuntimeError(f"Event type '{event_type}' not found.")
 
         self.wait()
         session = self._client._get_session()
 
         path = f"{self.path}/events/event_type={event_type}/"
```

### Comparing `sumatra-client-1.1.2/sumatra_client/config.py` & `sumatra-client-1.2.0/sumatra_client/config.py`

 * *Files identical despite different names*

### Comparing `sumatra-client-1.1.2/sumatra_client.egg-info/PKG-INFO` & `sumatra-client-1.2.0/sumatra_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumatra-client
-Version: 1.1.2
+Version: 1.2.0
 Summary: Sumatra Python Client and CLI
 Home-page: https://sumatra.ai
 Author: Sumatra
 Author-email: support@sumatra.ai
 License: Sumatra Proprietary
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sumatra-client-1.1.2/tests/test_config.py` & `sumatra-client-1.2.0/tests/test_config.py`

 * *Files identical despite different names*

