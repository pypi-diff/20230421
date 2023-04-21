# Comparing `tmp/vicops_api-1.0.2.tar.gz` & `tmp/vicops_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vicops_api-1.0.2.tar", last modified: Tue Apr 18 15:20:40 2023, max compression
+gzip compressed data, was "vicops_api-1.0.3.tar", last modified: Fri Apr 21 18:19:45 2023, max compression
```

## Comparing `vicops_api-1.0.2.tar` & `vicops_api-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 15:20:40.897432 vicops_api-1.0.2/
--rw-rw-rw-   0        0        0     1083 2023-03-04 14:34:18.000000 vicops_api-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      527 2023-04-18 15:20:40.896430 vicops_api-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-03-04 15:36:21.000000 vicops_api-1.0.2/README.md
--rw-rw-rw-   0        0        0       99 2023-03-04 15:18:20.000000 vicops_api-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 15:20:40.897432 vicops_api-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      647 2023-04-18 15:16:27.000000 vicops_api-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:20:40.885431 vicops_api-1.0.2/vicops_api/
--rw-rw-rw-   0        0        0      126 2023-04-18 15:19:30.000000 vicops_api-1.0.2/vicops_api/__init__.py
--rw-rw-rw-   0        0        0     4623 2023-04-18 15:16:35.000000 vicops_api-1.0.2/vicops_api/main.py
-drwxrwxrwx   0        0        0        0 2023-04-18 15:20:40.896430 vicops_api-1.0.2/vicops_api.egg-info/
--rw-rw-rw-   0        0        0      527 2023-04-18 15:20:40.000000 vicops_api-1.0.2/vicops_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-04-18 15:20:40.000000 vicops_api-1.0.2/vicops_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 15:20:40.000000 vicops_api-1.0.2/vicops_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 15:20:40.000000 vicops_api-1.0.2/vicops_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-18 15:20:40.000000 vicops_api-1.0.2/vicops_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 18:19:45.589810 vicops_api-1.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-03-04 14:34:18.000000 vicops_api-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      527 2023-04-21 18:19:45.589810 vicops_api-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-03-04 15:36:21.000000 vicops_api-1.0.3/README.md
+-rw-rw-rw-   0        0        0       99 2023-03-04 15:18:20.000000 vicops_api-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 18:19:45.589810 vicops_api-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      647 2023-04-21 18:17:15.000000 vicops_api-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:19:45.581811 vicops_api-1.0.3/vicops_api/
+-rw-rw-rw-   0        0        0      126 2023-04-21 18:12:38.000000 vicops_api-1.0.3/vicops_api/__init__.py
+-rw-rw-rw-   0        0        0     4769 2023-04-21 18:13:41.000000 vicops_api-1.0.3/vicops_api/main.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:19:45.588814 vicops_api-1.0.3/vicops_api.egg-info/
+-rw-rw-rw-   0        0        0      527 2023-04-21 18:19:45.000000 vicops_api-1.0.3/vicops_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-04-21 18:19:45.000000 vicops_api-1.0.3/vicops_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 18:19:45.000000 vicops_api-1.0.3/vicops_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 18:19:45.000000 vicops_api-1.0.3/vicops_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-21 18:19:45.000000 vicops_api-1.0.3/vicops_api.egg-info/top_level.txt
```

### Comparing `vicops_api-1.0.2/LICENSE` & `vicops_api-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vicops_api-1.0.2/PKG-INFO` & `vicops_api-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vicops_api
-Version: 1.0.2
+Version: 1.0.3
 Summary: python api wrapper for vicops2
 Home-page: https://github.com/ERTH2/vicops-api-py
 Author: artegoser
 License: MIT
 Project-URL: Source Code, https://github.com/ERTH2/vicops-api-py
 Keywords: api,wrapper,vicops
 Requires-Python: >=3.10
```

### Comparing `vicops_api-1.0.2/setup.py` & `vicops_api-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,12 +11,12 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/ERTH2/vicops-api-py",
     project_urls={
         "Source Code": "https://github.com/ERTH2/vicops-api-py",
     },
-    version="1.0.2",
+    version="1.0.3",
     packages=["vicops_api"],
     python_requires=">=3.10",
     install_requires=["requests"],
 )
```

### Comparing `vicops_api-1.0.2/vicops_api/main.py` & `vicops_api-1.0.3/vicops_api/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,27 @@
     def _getPost(self, url: str, body: object = {}) -> object:
         body["jwt"] = self.jwt
 
         res = requests.post(f"{self.host}{url}", data=body)
 
         if res.status_code != 200:
             return {
-                "msg": res.text,
+                "msg": res.json(),
                 "status": res.status_code,
                 "code": "denied",
             }
 
         return res.json()
 
     def _getGet(self, url: str) -> object:
         res = requests.get(f"{self.host}{url}")
 
         if res.status_code != 200:
             return {
-                "msg": res.text,
+                "msg": res.json(),
                 "status": res.status_code,
                 "code": "denied",
             }
 
         return res.json()
 
     def _checkRespAndAddJWT(self, resp: object) -> object:
@@ -37,35 +37,40 @@
         return resp
 
     def connectJwt(self, jwt: str) -> object:
         self.jwt = jwt
 
     def register(
         self,
+        id: str,
         name: str,
         second_name: str,
         password: str,
         country: str,
         type: str,
         contact: str,
     ) -> object:
         return self._checkRespAndAddJWT(
             self._getPost(
                 "/api/register",
                 {
+                    "id": id,
                     "name": name,
                     "second_name": second_name,
                     "password": password,
                     "country": country,
                     "type": type,
                     "contact": contact,
                 },
             )
         )
 
+    def get_error_codes(self) -> object:
+        return self._getGet("/api/error_codes")
+
     def transaction(
         self,
         recipient_id: str,
         amount: float,
         currency_id: str,
         description: str = "",
         type: str = "transfer",
```

### Comparing `vicops_api-1.0.2/vicops_api.egg-info/PKG-INFO` & `vicops_api-1.0.3/vicops_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vicops-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: python api wrapper for vicops2
 Home-page: https://github.com/ERTH2/vicops-api-py
 Author: artegoser
 License: MIT
 Project-URL: Source Code, https://github.com/ERTH2/vicops-api-py
 Keywords: api,wrapper,vicops
 Requires-Python: >=3.10
```

