# Comparing `tmp/folioclient-0.8.tar.gz` & `tmp/folioclient-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/folioclient-0.8.tar", last modified: Wed Nov 20 09:06:45 2019, max compression
+gzip compressed data, was "dist/folioclient-0.9.tar", last modified: Mon Nov 25 11:53:17 2019, max compression
```

## Comparing `folioclient-0.8.tar` & `folioclient-0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0 theodor   (1000) theodor   (1000)        0 2019-11-20 09:06:45.000000 folioclient-0.8/
-drwxrwxrwx   0 theodor   (1000) theodor   (1000)        0 2019-11-20 09:06:45.000000 folioclient-0.8/folioclient/
--rwxrwxrwx   0 theodor   (1000) theodor   (1000)     1514 2019-07-06 10:17:31.000000 folioclient-0.8/folioclient/cached_property.py
--rwxrwxrwx   0 theodor   (1000) theodor   (1000)     6081 2019-11-20 09:02:58.000000 folioclient-0.8/folioclient/FolioClient.py
--rwxrwxrwx   0 theodor   (1000) theodor   (1000)       48 2019-07-06 09:21:33.000000 folioclient-0.8/folioclient/__init__.py
--rwxrwxrwx   0 theodor   (1000) theodor   (1000)      791 2019-11-20 09:06:45.000000 folioclient-0.8/PKG-INFO
--rwxrwxrwx   0 theodor   (1000) theodor   (1000)       13 2019-07-06 10:05:28.000000 folioclient-0.8/README
--rwxrwxrwx   0 theodor   (1000) theodor   (1000)       65 2019-11-05 07:40:16.000000 folioclient-0.8/setup.cfg
--rwxrwxrwx   0 theodor   (1000) theodor   (1000)     1002 2019-11-20 09:04:18.000000 folioclient-0.8/setup.py
+drwxrwxrwx   0 theodor   (1000) theodor   (1000)        0 2019-11-25 11:53:17.000000 folioclient-0.9/
+drwxrwxrwx   0 theodor   (1000) theodor   (1000)        0 2019-11-25 11:53:17.000000 folioclient-0.9/folioclient/
+-rwxrwxrwx   0 theodor   (1000) theodor   (1000)     1514 2019-07-06 10:17:31.000000 folioclient-0.9/folioclient/cached_property.py
+-rwxrwxrwx   0 theodor   (1000) theodor   (1000)     6824 2019-11-25 11:50:31.000000 folioclient-0.9/folioclient/FolioClient.py
+-rwxrwxrwx   0 theodor   (1000) theodor   (1000)       48 2019-07-06 09:21:33.000000 folioclient-0.9/folioclient/__init__.py
+-rwxrwxrwx   0 theodor   (1000) theodor   (1000)      791 2019-11-25 11:53:17.000000 folioclient-0.9/PKG-INFO
+-rwxrwxrwx   0 theodor   (1000) theodor   (1000)       13 2019-07-06 10:05:28.000000 folioclient-0.9/README
+-rwxrwxrwx   0 theodor   (1000) theodor   (1000)       65 2019-11-05 07:40:16.000000 folioclient-0.9/setup.cfg
+-rwxrwxrwx   0 theodor   (1000) theodor   (1000)     1002 2019-11-25 11:50:52.000000 folioclient-0.9/setup.py
```

### Comparing `folioclient-0.8/folioclient/cached_property.py` & `folioclient-0.9/folioclient/cached_property.py`

 * *Files identical despite different names*

### Comparing `folioclient-0.8/folioclient/FolioClient.py` & `folioclient-0.9/folioclient/FolioClient.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,93 +4,93 @@
 
 
 class FolioClient:
     '''handles communication and getting values from FOLIO'''
 
     def __init__(self, okapi_url, tenant_id, username, password):
         self.missing_location_codes = set()
-        self.cql_all = '?limit=100&query=cql.allRecords=1 sortby name'
+        self.cql_all = '?query=cql.allRecords=1 sortby name'
         self.okapi_url = okapi_url
         self.tenant_id = tenant_id
         self.username = username
         self.password = password
         self.login()
         self.okapi_headers = {'x-okapi-token': self.okapi_token,
                               'x-okapi-tenant': self.tenant_id,
                               'content-type': 'application/json'}
 
     @cached_property
     def identifier_types(self):
-        return self.folio_get("/identifier-types",
-                              "identifierTypes",
-                              self.cql_all)
+        return self.folio_get_all("/identifier-types",
+                                  "identifierTypes",
+                                  self.cql_all)
 
     @cached_property
     def contributor_types(self):
-        return self.folio_get("/contributor-types",
-                              "contributorTypes",
-                              self.cql_all)
+        return self.folio_get_all("/contributor-types",
+                                  "contributorTypes",
+                                  self.cql_all)
 
     @cached_property
     def contrib_name_types(self):
-        return self.folio_get("/contributor-name-types",
-                              "contributorNameTypes",
-                              self.cql_all)
+        return self.folio_get_all("/contributor-name-types",
+                                  "contributorNameTypes",
+                                  self.cql_all)
 
     @cached_property
     def instance_types(self):
-        return self.folio_get("/instance-types",
-                              "instanceTypes",
-                              self.cql_all)
+        return self.folio_get_all("/instance-types",
+                                  "instanceTypes",
+                                  self.cql_all)
 
     @cached_property
     def instance_formats(self):
-        return self.folio_get("/instance-formats",
-                              "instanceFormats",
-                              self.cql_all)
+        return self.folio_get_all("/instance-formats",
+                                  "instanceFormats",
+                                  self.cql_all)
 
     def get_single_instance(self, instance_id):
-        return self.folio_get("inventory/instances/{}"
-                              .format(instance_id))
+        return self.folio_get_all("inventory/instances/{}"
+                                  .format(instance_id))
 
     @cached_property
     def alt_title_types(self):
-        return self.folio_get("/alternative-title-types",
-                              "alternativeTitleTypes",
-                              self.cql_all)
+        return self.folio_get_all("/alternative-title-types",
+                                  "alternativeTitleTypes",
+                                  self.cql_all)
 
     @cached_property
     def locations(self):
-        return self.folio_get("/locations",
-                              "locations",
-                              self.cql_all)
+        return self.folio_get_all("/locations",
+                                  "locations",
+                                  self.cql_all)
 
     @cached_property
     def class_types(self):
-        return self.folio_get("/classification-types",
-                              "classificationTypes",
-                              self.cql_all)
+        return self.folio_get_all("/classification-types",
+                                  "classificationTypes",
+                                  self.cql_all)
 
     @cached_property
     def organizations(self):
-        return self.folio_get("/organizations-storage/organizations",
-                              "organizations",
-                              self.cql_all)
+        return self.folio_get_all("/organizations-storage/organizations",
+                                  "organizations",
+                                  self.cql_all)
 
     @cached_property
     def modes_of_issuance(self):
-        return self.folio_get("/modes-of-issuance",
-                              "issuanceModes",
-                              self.cql_all)
+        return self.folio_get_all("/modes-of-issuance",
+                                  "issuanceModes",
+                                  self.cql_all)
 
     @cached_property
     def instance_types(self):
-        return self.folio_get("/instance-types",
-                              "instanceTypes",
-                              self.cql_all)
+        return self.folio_get_all("/instance-types",
+                                  "instanceTypes",
+                                  self.cql_all)
 
     def login(self):
         '''Logs into FOLIO in order to get the okapi token'''
         headers = {
             'x-okapi-tenant': self.tenant_id,
             'content-type': 'application/json'}
         payload = {"username": self.username,
@@ -99,28 +99,42 @@
         url = self.okapi_url + path
         req = requests.post(url, data=json.dumps(payload), headers=headers)
         if req.status_code != 201:
             raise ValueError("Request failed {}".format(req.status_code))
         self.okapi_token = req.headers.get('x-okapi-token')
         self.refresh_token = req.headers.get('refreshtoken')
 
+    def folio_get_all(self, path, key=None, query=''):
+        '''Fetches ALL data objects from FOLIO and turns it into a json object'''
+        results = list()
+        limit = 100
+        offset = 0
+        q_template = "?limit={}&offset={}" if query == '' else "&limit={}&offset={}"
+        temp_res = self.folio_get(path, key, q_template.format(limit, offset))
+        results.append(temp_res)
+        while len(temp_res) == limit:
+            temp_res = self.folio_get(
+                path, key, q_template.format(limit, offset))
+            results.append(temp_res)
+        return results
+
     def folio_get(self, path, key=None, query=''):
         '''Fetches data from FOLIO and turns it into a json object'''
         url = self.okapi_url + path + query
         req = requests.get(url,
                            headers=self.okapi_headers)
         req.raise_for_status()
         result = (json.loads(req.text)[key] if key else json.loads(req.text))
         if not any(result):
             raise ValueError("No {} setup in tenant".format(key))
         return result
 
     def folio_get_single_object(self, path):
         '''Fetches data from FOLIO and turns it into a json object'''
-        url = self.okapi_url+path
+        url = self.okapi_url + path
         req = requests.get(url,
                            headers=self.okapi_headers)
         req.raise_for_status()
         result = json.loads(req.text)
         return result
 
     def get_instance_json_schema(self):
```

### Comparing `folioclient-0.8/PKG-INFO` & `folioclient-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: folioclient
-Version: 0.8
+Version: 0.9
 Summary: A simple wrapper over the FOLIO LMS system API:s
 Home-page: https://github.com/fontanka16/FolioClient
 Author: Theodor Tolstoy
 Author-email: pypi.teddes@tolstoy.se
 License: MIT
-Download-URL: https://github.com/fontanka16/FolioClient/archive/v_08.tar.gz
+Download-URL: https://github.com/fontanka16/FolioClient/archive/v_09.tar.gz
 Description: UNKNOWN
 Keywords: FOLIO,FOLIO_LSP,OKAPI,API Wrapper
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `folioclient-0.8/setup.py` & `folioclient-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
     name='folioclient',
     packages=['folioclient'],
-    version='0.8',
+    version='0.9',
     license='MIT',
     description='A simple wrapper over the FOLIO LMS system API:s',
     author='Theodor Tolstoy',
     author_email='pypi.teddes@tolstoy.se',
     url='https://github.com/fontanka16/FolioClient',
-    download_url='https://github.com/fontanka16/FolioClient/archive/v_08.tar.gz',
+    download_url='https://github.com/fontanka16/FolioClient/archive/v_09.tar.gz',
     keywords=['FOLIO', 'FOLIO_LSP', 'OKAPI', 'API Wrapper'],
     install_requires=[            # I get to this in a second
         'requests'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
```

