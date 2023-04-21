# Comparing `tmp/oidc_client-0.1.3.tar.gz` & `tmp/oidc_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_client-0.1.3.tar", max compression
+gzip compressed data, was "oidc_client-0.2.0.tar", max compression
```

## Comparing `oidc_client-0.1.3.tar` & `oidc_client-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1085 2023-04-20 11:14:26.451110 oidc_client-0.1.3/LICENSE.md
--rw-r--r--   0        0        0     1069 2023-04-20 11:14:26.451110 oidc_client-0.1.3/README.md
--rw-r--r--   0        0        0      541 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/__init__.py
--rw-r--r--   0        0        0       30 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/__main__.py
--rw-r--r--   0        0        0     4815 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/cli.py
--rw-r--r--   0        0        0     3540 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/config.py
--rw-r--r--   0        0        0      925 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/discovery.py
--rw-r--r--   0        0        0      488 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/error.py
--rw-r--r--   0        0        0      215 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/index.html
--rw-r--r--   0        0        0     1791 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/lib.py
--rw-r--r--   0        0        0     1123 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/localhost.crt
--rw-r--r--   0        0        0     1704 2023-04-20 11:14:26.451110 oidc_client-0.1.3/oidc_client/localhost.key
--rw-r--r--   0        0        0     7603 2023-04-20 11:14:26.452111 oidc_client-0.1.3/oidc_client/oauth.py
--rw-r--r--   0        0        0      807 2023-04-20 11:14:26.452111 oidc_client-0.1.3/oidc_client/pkce.py
--rw-r--r--   0        0        0      556 2023-04-20 11:14:26.452111 oidc_client-0.1.3/oidc_client/tls.py
--rw-r--r--   0        0        0     1320 2023-04-20 11:14:26.452111 oidc_client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 oidc_client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-21 15:13:40.948593 oidc_client-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1069 2023-04-21 15:13:40.948593 oidc_client-0.2.0/README.md
+-rw-r--r--   0        0        0      541 2023-04-21 15:13:40.948593 oidc_client-0.2.0/oidc_client/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-21 15:13:40.948593 oidc_client-0.2.0/oidc_client/__main__.py
+-rw-r--r--   0        0        0     4925 2023-04-21 15:13:40.948593 oidc_client-0.2.0/oidc_client/cli.py
+-rw-r--r--   0        0        0     3697 2023-04-21 15:13:40.948593 oidc_client-0.2.0/oidc_client/config.py
+-rw-r--r--   0        0        0      925 2023-04-21 15:13:40.948593 oidc_client-0.2.0/oidc_client/discovery.py
+-rw-r--r--   0        0        0      488 2023-04-21 15:13:40.948593 oidc_client-0.2.0/oidc_client/error.py
+-rw-r--r--   0        0        0      215 2023-04-21 15:13:40.949594 oidc_client-0.2.0/oidc_client/index.html
+-rw-r--r--   0        0        0     1882 2023-04-21 15:13:40.949594 oidc_client-0.2.0/oidc_client/lib.py
+-rw-r--r--   0        0        0     1123 2023-04-21 15:13:40.949594 oidc_client-0.2.0/oidc_client/localhost.crt
+-rw-r--r--   0        0        0     1704 2023-04-21 15:13:40.949594 oidc_client-0.2.0/oidc_client/localhost.key
+-rw-r--r--   0        0        0     7656 2023-04-21 15:13:40.949594 oidc_client-0.2.0/oidc_client/oauth.py
+-rw-r--r--   0        0        0      807 2023-04-21 15:13:40.949594 oidc_client-0.2.0/oidc_client/pkce.py
+-rw-r--r--   0        0        0      556 2023-04-21 15:13:40.949594 oidc_client-0.2.0/oidc_client/tls.py
+-rw-r--r--   0        0        0     1320 2023-04-21 15:13:40.949594 oidc_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 oidc_client-0.2.0/PKG-INFO
```

### Comparing `oidc_client-0.1.3/LICENSE.md` & `oidc_client-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oidc_client-0.1.3/README.md` & `oidc_client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `oidc_client-0.1.3/oidc_client/__init__.py` & `oidc_client-0.2.0/oidc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.1.3/oidc_client/cli.py` & `oidc_client-0.2.0/oidc_client/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     try:
         auth = login(
             provider_config,
             client_id=profile.client_id,
             client_secret=profile.client_secret,
             redirect_uri=profile.redirect_uri,
             scope=profile.scope,
+            audience=profile.audience,
             interactive=args.interactive,
         )
     except (ProviderConfigError, TokenRequestParamError) as error:
         if args.debug:
             traceback.print_exception(error)
         exit(f"Login configuration error: {error}")
     except AuthorizationError as error:
@@ -120,14 +121,15 @@
     )
     overrides.add_argument(
         "--scope",
         help=f"scope (can be given multiple times, default: '{DEFAULT_OIDC_SCOPE}')",
         default=[],
         action="append",
     )
+    overrides.add_argument("--audience", help="audience of the token")
     outputs = parser_login.add_mutually_exclusive_group()
     outputs.add_argument(
         "--only-id-token", help="only output the ID token", action="store_true"
     )
     outputs.add_argument(
         "--only-access-token", help="only output the access token", action="store_true"
     )
```

### Comparing `oidc_client-0.1.3/oidc_client/config.py` & `oidc_client-0.2.0/oidc_client/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     """OIDC client profile."""
 
     issuer: str
     client_id: str
     client_secret: str | None = None
     redirect_uri: str = DEFAULT_REDIRECT_URI
     scope: str = DEFAULT_OIDC_SCOPE
+    audience: str | None = None
 
     def __post_init__(self) -> None:
         if not self.issuer.startswith("https://"):
             raise ProviderConfigError("OIDC issuer must be HTTPS.")
 
         validate_redirect_uri(self.redirect_uri)
 
@@ -112,8 +113,11 @@
         or os.getenv("OIDC_REDIRECT_URI")
         or data.get("redirect_uri")
         or DEFAULT_REDIRECT_URI,
         scope=" ".join(getattr(overrides, "scope", []))
         or os.getenv("OIDC_SCOPE")
         or data.get("scope")
         or DEFAULT_OIDC_SCOPE,
+        audience=getattr(overrides, "audience", None)
+        or os.getenv("OIDC_AUDIENCE")
+        or data.get("audience"),
     )
```

### Comparing `oidc_client-0.1.3/oidc_client/discovery.py` & `oidc_client-0.2.0/oidc_client/discovery.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.1.3/oidc_client/lib.py` & `oidc_client-0.2.0/oidc_client/lib.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 def login(
     provider_config: ProviderConfig,
     client_id: str,
     client_secret: str | None = None,
     redirect_uri: str | None = None,
     scope: str = DEFAULT_OIDC_SCOPE,
+    audience: str | None = None,
     interactive: bool = False,
 ) -> TokenResponse:
     """Perform OIDC login.
 
     The interactive mode requires the user to log in using a web browser.
     """
     if interactive:
@@ -41,20 +42,22 @@
         return fetch_token(
             provider_config.token_endpoint,
             grant_type=GrantType.AUTHORIZATION_CODE,
             client_id=client_id,
             redirect_uri=redirect_uri,
             code=code,
             pkce_secret=pkce_secret,
+            audience=audience,
         )
 
     if not client_secret:
         raise TokenRequestParamError(
             "client_secret must be provided for non-interactive login."
         )
 
     return fetch_token(
         provider_config.token_endpoint,
         grant_type=GrantType.CLIENT_CREDENTIALS,
         client_id=client_id,
         client_secret=client_secret,
+        audience=audience,
     )
```

### Comparing `oidc_client-0.1.3/oidc_client/localhost.crt` & `oidc_client-0.2.0/oidc_client/localhost.crt`

 * *Files identical despite different names*

### Comparing `oidc_client-0.1.3/oidc_client/localhost.key` & `oidc_client-0.2.0/oidc_client/localhost.key`

 * *Files identical despite different names*

### Comparing `oidc_client-0.1.3/oidc_client/oauth.py` & `oidc_client-0.2.0/oidc_client/oauth.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,21 +188,25 @@
     endpoint: str,
     client_id: str,
     grant_type: GrantType,
     redirect_uri: str | None = None,
     code: str | None = None,
     pkce_secret: PKCESecret | None = None,
     client_secret: str | None = None,
+    audience: str | None = None,
 ) -> TokenResponse:
     """Fetch a token from the provider's token endpoint."""
     data = {
         "grant_type": format(grant_type),
         "client_id": client_id,
     }
 
+    if audience:
+        data["audience"] = audience
+
     match grant_type:
         case GrantType.AUTHORIZATION_CODE:
             if not (pkce_secret and code and redirect_uri):
                 raise TypeError(
                     "the authorization code flow is only allowed with PKCE "
                     "and requires both code and redirect URI."
                 )
@@ -212,17 +216,15 @@
                 "code_verifier": str(pkce_secret),
             }
         case GrantType.CLIENT_CREDENTIALS:
             if not client_secret:
                 raise TypeError(
                     "the client credentials grant requires a client secret."
                 )
-            data |= {
-                "client_secret": client_secret,
-            }
+            data["client_secret"] = client_secret
         case _:
             raise ValueError("unsupported grant type.")
 
     request = Request(endpoint, data=urlencode(sorted(data.items())).encode())
     try:
         with urlopen(request) as response:
             token_data = json.load(response)
```

### Comparing `oidc_client-0.1.3/oidc_client/pkce.py` & `oidc_client-0.2.0/oidc_client/pkce.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.1.3/oidc_client/tls.py` & `oidc_client-0.2.0/oidc_client/tls.py`

 * *Files identical despite different names*

### Comparing `oidc_client-0.1.3/pyproject.toml` & `oidc_client-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oidc-client"
-version = "0.1.3"
+version = "0.2.0"
 description = "A pure-Python OpenID Connect client"
 readme = "README.md"
 keywords = ["openid", "oidc", "oauth", "oauth2"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Topic :: Internet :: WWW/HTTP",
```

### Comparing `oidc_client-0.1.3/PKG-INFO` & `oidc_client-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc-client
-Version: 0.1.3
+Version: 0.2.0
 Summary: A pure-Python OpenID Connect client
 Home-page: https://gitlab.com/lzinsou/oidc-client
 Keywords: openid,oidc,oauth,oauth2
 Author: Loris Zinsou
 Author-email: lzinsou@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

