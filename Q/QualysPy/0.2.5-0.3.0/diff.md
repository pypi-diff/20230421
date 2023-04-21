# Comparing `tmp/qualyspy-0.2.5.tar.gz` & `tmp/qualyspy-0.3.0.tar.gz`

## Comparing `qualyspy-0.2.5.tar` & `qualyspy-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.2.5/.vscode/launch.json
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.2.5/.vscode/settings.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.2.5/.vscode/tasks.json
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.2.5/debug/build.sh
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.2.5/debug/dtd.txt
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.2.5/debug/output.txt
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.2.5/debug/parse_dtd.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.2.5/debug/quickscan.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.2.5/debug/remove_cookies.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 qualyspy-0.2.5/debug/test.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/make.bat
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/conf.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/index.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/modules.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/qualyspy.assets.host_list.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/qualyspy.assets.host_list_detection.rst
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/qualyspy.qualysapi.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/qualyspy.qutils.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/qualyspy.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.2.5/docs/source/qualyspy.scan_configuration.knowledgebase.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/__init__.py
--rw-r--r--   0        0        0    17347 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/qualysapi.py
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/qutils.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/urls.json
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/asset_mgmt_tagging/__init__.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/asset_mgmt_tagging/asset.py
--rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/asset_mgmt_tagging/tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/assets/__init__.py
--rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/assets/host_list.py
--rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/assets/host_list_detection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/certview/__init__.py
--rw-r--r--   0        0        0    15310 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/certview/certificate.py
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/certview/sql/certview_init.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/scan_configuration/__init__.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.2.5/qualyspy/scan_configuration/knowledgebase.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.2.5/requirements/deploy.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.2.5/requirements/dev.txt
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.2.5/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.2.5/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.2.5/README.md
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.3.0/.vscode/launch.json
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.3.0/.vscode/tasks.json
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.3.0/debug/build.sh
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.3.0/debug/dtd.txt
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.3.0/debug/output.txt
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.3.0/debug/parse_dtd.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.3.0/debug/quickscan.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.3.0/debug/remove_cookies.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 qualyspy-0.3.0/debug/test.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/conf.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/index.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/modules.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/qualyspy.assets.host_list.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/qualyspy.assets.host_list_detection.rst
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/qualyspy.qualysapi.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/qualyspy.qutils.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/qualyspy.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.3.0/docs/source/qualyspy.scan_configuration.knowledgebase.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/__init__.py
+-rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/qualysapi.py
+-rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/qutils.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/urls.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/asset_mgmt_tagging/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/asset_mgmt_tagging/api_input.py
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/asset_mgmt_tagging/asset.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/asset_mgmt_tagging/tag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/assets/__init__.py
+-rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/assets/host_list.py
+-rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/assets/host_list_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/certview/__init__.py
+-rw-r--r--   0        0        0    15601 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/certview/certificate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/scan_configuration/__init__.py
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.3.0/qualyspy/scan_configuration/knowledgebase.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.3.0/requirements/deploy.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.3.0/requirements/dev.txt
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.3.0/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.3.0/README.md
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 qualyspy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.3.0/PKG-INFO
```

### Comparing `qualyspy-0.2.5/.vscode/launch.json` & `qualyspy-0.3.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/debug/dtd.txt` & `qualyspy-0.3.0/debug/dtd.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/debug/output.txt` & `qualyspy-0.3.0/debug/output.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/debug/parse_dtd.py` & `qualyspy-0.3.0/debug/parse_dtd.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/debug/quickscan.py` & `qualyspy-0.3.0/debug/quickscan.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/debug/remove_cookies.py` & `qualyspy-0.3.0/debug/remove_cookies.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/docs/Makefile` & `qualyspy-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/docs/make.bat` & `qualyspy-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/docs/source/conf.py` & `qualyspy-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/qualyspy/qualysapi.py` & `qualyspy-0.3.0/qualyspy/qualysapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,14 @@
     def _perform_request(
         self,
         method: str,
         path: str,
         params: Optional[MutableMapping[str, Any]] = None,
         data: Optional[Union[MutableMapping[str, Any], str]] = None,
         /,
-        use_auth: bool = False,
         add_headers: MutableMapping[str, str] = {},
     ) -> str:
         """Helper method for "request" methods.  Performs the API request and returns the text as
         a string, to be parsed by the calling function.
         """
 
         headers = self._headers
@@ -219,15 +218,15 @@
 
         root = API_ROOT
         if "/certview/" in path:
             root = API_GATEWAY_ROOT
             headers["Authorization"] = "Bearer " + self._bearer_token
 
         auth = None
-        if use_auth:
+        if "/qps/" in path:
             auth = (CREDENTIALS["username"], CREDENTIALS["password"])
 
         match method:
             case "get":
                 response = requests.get(
                     root + path,
                     headers=headers,
@@ -273,15 +272,14 @@
     def _request(
         self,
         method: str,
         path: str,
         /,
         params: Optional[MutableMapping[str, Any]] = None,
         data: Optional[Union[MutableMapping[str, Any], str]] = None,
-        use_auth: bool = False,
         add_headers: MutableMapping[str, str] = {},
     ) -> Any:
         """Performs an API request to the connection for a given API path and returns the result.
 
         Args:
             method:
                 The method of the request (ex. get, post)
@@ -300,26 +298,24 @@
             An lxml.objectify object of the XML output of the API request.
         """
         for api in self._in_out_headers:
             if path.startswith(api):
                 add_headers.update(self._in_out_headers[api])
 
         response = self._perform_request(
-            method, path, params, data, use_auth=use_auth, add_headers=add_headers
+            method, path, params, data, add_headers=add_headers
         )
 
         match add_headers["Content-Type"]:
             case "application/xml":
                 xml = lxml.objectify.fromstring(re.split("\n", response, 1)[1])
-                if "/qps/rest/2.0/" in path:
-                    response_code = str(xml.responseCode)
-                    if response_code != "SUCCESS":
-                        raise Qualys_API_Error(xml.responseErrorDetails.errorMessage)
                 return xml
             case "application/json":
+                if "qps" in path:
+                    return json.loads(response)["ServiceResponse"]
                 return json.loads(response)
             case _:
                 return response
 
     def get(
         self,
         path: str,
@@ -351,45 +347,40 @@
         return self._request("get", path, params=params, add_headers=add_headers)
 
     def post(
         self,
         path: str,
         data: Optional[Union[MutableMapping[str, Any], str]] = None,
         *,
-        use_auth: bool = False,
         add_headers: MutableMapping[str, str] = {},
     ) -> Any:
         """Performs an POST request to the connection for a given API path and returns the result.
 
         Normally, it is not intended that this function be called manually.  Instead, this would be
         run by functions in other modules of this package.  However, this method is
         considered part of the public interface to cover any API functions which are not currently
         implemented in this package.
 
         Args:
             path:
                 The path of the API request. ex. /api/2.0/fo/scan/?action=list
             data:
                 A dictionary of information to be sent in the body of a POST request.
-            use_auth:
-                Use auth for authentication, rather than cookies. Which to use depends on the API
-                being called.
             add_headers:
                 Include additional headers in the request. These headers will not persist to the
                 next request.
 
         Returns:
             An lxml.objectify object of the XML output of the API request.
         """
 
         return self._request(
             "post",
             path,
             data=json.dumps(data),
-            use_auth=use_auth,
             add_headers=add_headers,
         )
 
     def _request_file(
         self,
         method: str,
         path: str,
```

### Comparing `qualyspy-0.2.5/qualyspy/qutils.py` & `qualyspy-0.3.0/qualyspy/qutils.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/qualyspy/urls.json` & `qualyspy-0.3.0/qualyspy/urls.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8148148148148148%*

 * *Differences: {"'Count Assets'": "'/qps/rest/2.0/count/am/asset'",*

 * * "'Count Tags'": "'/qps/rest/2.0/count/am/tag'",*

 * * "'Delete Asset'": "'/qps/rest/2.0/delete/am/asset'",*

 * * "'Delete Tag'": "'/qps/rest/2.0/delete/am/tag'",*

 * * "'Get Asset Info'": "'/qps/rest/2.0/get/am/asset/'"}*

```diff
@@ -1,14 +1,19 @@
 {
     "Add IPs": "/api/2.0/fo/asset/ip/?action=add",
     "Cancel VM Scan": "/api/2.0/fo/scan/?action=cancel",
     "CertView Authentication": "/auth",
+    "Count Assets": "/qps/rest/2.0/count/am/asset",
+    "Count Tags": "/qps/rest/2.0/count/am/tag",
     "Create Tag": "/qps/rest/2.0/create/am/tag",
+    "Delete Asset": "/qps/rest/2.0/delete/am/asset",
+    "Delete Tag": "/qps/rest/2.0/delete/am/tag",
     "Delete VM Scan": "/api/2.0/fo/scan/?action=delete",
     "Fetch VM Scan": "/api/2.0/fo/scan/?action=fetch",
+    "Get Asset Info": "/qps/rest/2.0/get/am/asset/",
     "Host List": "/api/2.0/fo/asset/host/?action=list",
     "Host List Detection": "/api/2.0/fo/asset/host/vm/detection/?action=list",
     "IP List": "/api/2.0/fo/asset/ip/?action=list",
     "KnowledgeBase": "/api/2.0/fo/knowledge_base/vuln/?action=list",
     "Launch VM Scan": "/api/2.0/fo/scan/?action=launch",
     "List CertView Certificates": "/certview/v2/certificates",
     "Pause VM Scan": "/api/2.0/fo/scan/?action=pause",
```

### Comparing `qualyspy-0.2.5/qualyspy/assets/host_list.py` & `qualyspy-0.3.0/qualyspy/assets/host_list.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/qualyspy/assets/host_list_detection.py` & `qualyspy-0.3.0/qualyspy/assets/host_list_detection.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/qualyspy/certview/certificate.py` & `qualyspy-0.3.0/qualyspy/certview/certificate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 import datetime
-import importlib.resources
 import ipaddress
 from typing import Any, TypeVar
 
 import psycopg2.extensions
-import pydantic as pd
+import pydantic as pyd
 import pydantic.networks
 import pydantic.utils
 import sqlalchemy as sa
 import sqlalchemy.dialects.postgresql as sa_pg
 import sqlalchemy.orm as orm
 
 from .. import qualysapi, qutils
 
-SQL = importlib.resources.files("qualyspy").joinpath("certview").joinpath("sql")
-
 
 class Base(orm.DeclarativeBase):
     pass
 
 
 Base.metadata.schema = "certificate"
 
 
-def adapt_pydantic_ip_address(ip: pd.IPvAnyAddress) -> Any:
+def adapt_pydantic_ip_address(ip: pyd.IPvAnyAddress) -> Any:
     return psycopg2.extensions.AsIs(repr(ip.exploded))
 
 
 psycopg2.extensions.register_adapter(
     pydantic.networks.IPv4Address, adapt_pydantic_ip_address  # type: ignore
 )
 psycopg2.extensions.register_adapter(
@@ -35,15 +32,15 @@
 )
 
 
 ####################################################################################################
 # Subject_Alternative_Name
 
 
-class Subject_Alternative_Names(pd.BaseModel):
+class Subject_Alternative_Names(pyd.BaseModel):
     dns_names = list[str]
     ip_address = list[ipaddress.IPv4Address | ipaddress.IPv6Address]
 
     class Config:
         alias_generator = qutils.to_lower_camel
         orm_mode = True
         allow_population_by_field_name = True
@@ -68,15 +65,15 @@
 
 ####################################################################################################
 
 ####################################################################################################
 # Subject
 
 
-class Subject(pd.BaseModel):
+class Subject(pyd.BaseModel):
     organization: str
     locality: str
     name: str
     state: str
     country: str
     organization_unit: list[str] | None
 
@@ -108,15 +105,15 @@
 
 ####################################################################################################
 
 ####################################################################################################
 # Issuer
 
 
-class Issuer(pd.BaseModel):
+class Issuer(pyd.BaseModel):
     organization: str
     organization_unit: list[str]
     name: str
     country: str
     state: str
     certhash: str
     locality: str
@@ -161,15 +158,15 @@
     )
 
 
 ####################################################################################################
 # Host_Instance
 
 
-class Host_Instance(pd.BaseModel):
+class Host_Instance(pyd.BaseModel):
     id: int
     port: int
     fqdn: str
     protocol: str
     service: str | None
     grade: str
 
@@ -207,17 +204,17 @@
     )
 
 
 ####################################################################################################
 # Asset_Interface
 
 
-class Asset_Interface(pd.BaseModel):
+class Asset_Interface(pyd.BaseModel):
     hostname: str | None
-    address: pd.IPvAnyAddress
+    address: pyd.IPvAnyAddress
 
     class Config:
         orm_mode = True
         allow_population_by_field_name = True
 
 
 class Asset_Interface_ORM(Base):
@@ -237,22 +234,23 @@
 
 ####################################################################################################
 
 ####################################################################################################
 # Asset
 
 
-class Asset(pd.BaseModel):
+class Asset(pyd.BaseModel):
     id: int
     uuid: str
     netbios_name: str
     name: str
     operating_system: str | None
     host_instances: list[Host_Instance]
     asset_interfaces: list[Asset_Interface] | None
+    primary_ip: pyd.IPvAnyAddress
 
     class Config:
         alias_generator = qutils.to_lower_camel
         orm_mode = True
         allow_population_by_field_name = True
 
 
@@ -272,21 +270,24 @@
         back_populates="asset"
     )
 
     certificate_id: orm.Mapped[int] = orm.mapped_column(sa.ForeignKey("certificate.id"))
     certificate: orm.Mapped["Certificate_ORM"] = orm.relationship(
         back_populates="assets", uselist=False
     )
+    primary_ip: orm.Mapped[
+        ipaddress.IPv4Address | ipaddress.IPv6Address
+    ] = orm.mapped_column("address", sa_pg.INET, primary_key=True)
 
 
 ####################################################################################################
 # Certificate
 
 
-class Certificate(pd.BaseModel):
+class Certificate(pyd.BaseModel):
     id: int
     certhash: str
     key_size: int
     serial_number: str
     valid_to_date: datetime.datetime
     valid_to: int
     valid_from_date: datetime.datetime
@@ -301,14 +302,15 @@
     imported: bool
     self_signed: bool
     issuer: Issuer | None
     rootissuer: Issuer | None
     issuer_category: str
     instance_count: int
     asset_count: int
+    sources: list[str]
     assets: list[Asset]
     key_usage: list[str]
     raw_data: str
     enhanced_key_usage: list[str] | None
     subject_key_identifier: str | None
     auth_key_identifier: str | None
     subject_alternative_names: Subject_Alternative_Names | None
@@ -353,14 +355,15 @@
     )
     rootissuer: orm.Mapped[RootIssuer_ORM | None] = orm.relationship(
         back_populates="rootissuer_of", uselist=False
     )
     issuer_category: orm.Mapped[str]
     instance_count: orm.Mapped[int]
     asset_count: orm.Mapped[int]
+    sources: orm.Mapped[list[str]] = orm.mapped_column(sa.ARRAY(sa.String))
     assets: orm.Mapped[list[Asset_ORM]] = orm.relationship(back_populates="certificate")
     key_usage: orm.Mapped[list[str]] = orm.mapped_column(sa.ARRAY(sa.String))
     raw_data: orm.Mapped[str]
     enhanced_key_usage: orm.Mapped[list[str] | None] = orm.mapped_column(
         sa.ARRAY(sa.String)
     )
     subject_key_identifier: orm.Mapped[str | None]
@@ -372,26 +375,26 @@
 
 ####################################################################################################
 
 ####################################################################################################
 # Function input
 
 
-class Field_Value_Operator(pd.BaseModel):
+class Field_Value_Operator(pyd.BaseModel):
     field: str
     value: str
     operator: str
 
 
-class Filter(pd.BaseModel):
+class Filter(pyd.BaseModel):
     filters: list[Field_Value_Operator]
     operation: str = "AND"
 
 
-class List_CertView_Certificates_V2_Input(pd.BaseModel):
+class List_CertView_Certificates_V2_Input(pyd.BaseModel):
     filter: Filter | None = None
     page_number: int = 0
     page_size: int | None = None
     exclude_fields: str | None = None
 
     class Config:
         alias_generator = qutils.to_lower_camel
@@ -425,17 +428,19 @@
             for cert in raw:
                 c = Certificate.parse_obj(cert)
 
                 # subject.name somtimes includes null characters "\x00", even though the GUI doesn't
                 # show these.  I've opened a ticket with Qualys about it.  In the meanwhile, this
                 # will replace them with something PostgreSQL is happy with.
                 # Also other fields, apparently...
-                c.subject.name = c.subject.name.replace("\x00", "\uFFFD")
-                c.subject.locality = c.subject.locality.replace("\x00", "\uFFFD")
-                c.subject.state = c.subject.state.replace("\x00", "\uFFFD")
+                #
+                # Qualys claim to have fixed this, so commenting it out for now.
+                # c.subject.name = c.subject.name.replace("\x00", "\uFFFD")
+                # c.subject.locality = c.subject.locality.replace("\x00", "\uFFFD")
+                # c.subject.state = c.subject.state.replace("\x00", "\uFFFD")
 
                 certificates.append(c)
             return certificates
         else:
             return None
 
     def call(
```

### Comparing `qualyspy-0.2.5/qualyspy/scan_configuration/knowledgebase.py` & `qualyspy-0.3.0/qualyspy/scan_configuration/knowledgebase.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/.gitignore` & `qualyspy-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/LICENSE` & `qualyspy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.5/pyproject.toml` & `qualyspy-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "QualysPy"
-version = "0.2.5"
+version = "0.3.0"
 authors = [
   { name="Jordan Barnartt", email="jbarnart@uwaterloo.ca" },
 ]
 description = "A Python wrapper for the Qualys API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `qualyspy-0.2.5/PKG-INFO` & `qualyspy-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QualysPy
-Version: 0.2.5
+Version: 0.3.0
 Summary: A Python wrapper for the Qualys API.
 Project-URL: Homepage, https://github.com/JordanBarnartt/qualyspy
 Project-URL: Bug Tracker, https://github.com/JordanBarnartt/qualyspy/issues
 Author-email: Jordan Barnartt <jbarnart@uwaterloo.ca>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

