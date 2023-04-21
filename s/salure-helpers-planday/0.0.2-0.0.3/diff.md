# Comparing `tmp/salure_helpers_planday-0.0.2.tar.gz` & `tmp/salure_helpers_planday-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_planday-0.0.2.tar", last modified: Fri Apr 14 11:45:18 2023, max compression
+gzip compressed data, was "dist/salure_helpers_planday-0.0.3.tar", last modified: Fri Apr 21 13:52:42 2023, max compression
```

## Comparing `salure_helpers_planday-0.0.2.tar` & `salure_helpers_planday-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/
--rw-r--r--   0 root         (0) root         (0)      265 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers/planday/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-14 11:45:03.000000 salure_helpers_planday-0.0.2/salure_helpers/planday/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12872 2023-04-14 11:45:03.000000 salure_helpers_planday-0.0.2/salure_helpers/planday/planday.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers_planday.egg-info/
--rw-r--r--   0 root         (0) root         (0)      265 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers_planday.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers_planday.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers_planday.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers_planday.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers_planday.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers_planday.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-14 11:45:03.000000 salure_helpers_planday-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:52:42.000000 salure_helpers_planday-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)      265 2023-04-21 13:52:42.000000 salure_helpers_planday-0.0.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:52:42.000000 salure_helpers_planday-0.0.3/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:52:42.000000 salure_helpers_planday-0.0.3/salure_helpers/planday/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-21 13:52:27.000000 salure_helpers_planday-0.0.3/salure_helpers/planday/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15381 2023-04-21 13:52:27.000000 salure_helpers_planday-0.0.3/salure_helpers/planday/planday.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:52:42.000000 salure_helpers_planday-0.0.3/salure_helpers_planday.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      265 2023-04-21 13:52:42.000000 salure_helpers_planday-0.0.3/salure_helpers_planday.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-04-21 13:52:42.000000 salure_helpers_planday-0.0.3/salure_helpers_planday.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 13:52:42.000000 salure_helpers_planday-0.0.3/salure_helpers_planday.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 13:52:42.000000 salure_helpers_planday-0.0.3/salure_helpers_planday.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-21 13:52:42.000000 salure_helpers_planday-0.0.3/salure_helpers_planday.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-21 13:52:42.000000 salure_helpers_planday-0.0.3/salure_helpers_planday.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 13:52:42.000000 salure_helpers_planday-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-21 13:52:27.000000 salure_helpers_planday-0.0.3/setup.py
```

### Comparing `salure_helpers_planday-0.0.2/salure_helpers/planday/planday.py` & `salure_helpers_planday-0.0.3/salure_helpers/planday/planday.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 import requests
 import json
 import datetime
+import time
 
 
 class Planday:
 
     def __init__(self, refresh_token: str, client_id: str, planday_base_url: str = 'https://openapi.planday.com/'):
         self.base_url = planday_base_url
         self.refresh_token = refresh_token
@@ -67,15 +68,22 @@
         """
         This function returns all possible portals (environments) for the access token
         :return: dataframe with results
         """
         url = f'{self.base_url}portal/v1.0/info'
         access_token = self.__get_access_token()
         headers = self.__get_headers(access_token=access_token)
-        response = requests.get(url=url, headers=headers)
+
+        try:
+            response = requests.get(url=url, headers=headers)
+        except requests.exceptions.ConnectionError:
+            print("Connection error, retrying...")
+            time.sleep(5)
+            response = requests.get(url=url, headers=headers)
+
         if 200 <= response.status_code < 300:
             df = pd.DataFrame(response.json()['data']['portals'])
             return df
         else:
             raise ConnectionError(f"Planday returned an error while retrieving portals: {response.status_code, response.text}")
 
     def get_departments(self, portal_id: str) -> pd.DataFrame:
@@ -83,15 +91,22 @@
         This function returns all departments in the specified portal.
         :param portal_id: portal ID from planday. See get_portals
         :return: dataframe with results
         """
         url = f'{self.base_url}hr/v1/departments'
         access_token = self.__get_child_token(portal_id=portal_id)
         headers = self.__get_headers(access_token=access_token)
-        response = requests.get(url=url, headers=headers)
+
+        try:
+            response = requests.get(url=url, headers=headers)
+        except requests.exceptions.ConnectionError:
+            print("Connection error, retrying...")
+            time.sleep(5)
+            response = requests.get(url=url, headers=headers)
+
         if 200 <= response.status_code < 300:
             df = pd.DataFrame(response.json()['data'])
             return df
         else:
             raise ConnectionError(f"Planday returned an error while retrieving departments: {response.status_code, response.text}")
 
     def get_contract_rules(self, portal_id: str) -> pd.DataFrame:
@@ -99,15 +114,22 @@
         This function returns all contract rules in the specified portal.
         :param portal_id: portal ID from planday. See get_portals
         :return: dataframe with results
         """
         url = f'{self.base_url}contractrules/v1.0/contractrules'
         access_token = self.__get_child_token(portal_id=portal_id)
         headers = self.__get_headers(access_token=access_token)
-        response = requests.get(url=url, headers=headers)
+
+        try:
+            response = requests.get(url=url, headers=headers)
+        except requests.exceptions.ConnectionError:
+            print("Connection error, retrying...")
+            time.sleep(5)
+            response = requests.get(url=url, headers=headers)
+
         if 200 <= response.status_code < 300:
             df = pd.DataFrame(response.json()['data'])
             return df
         else:
             raise ConnectionError(f"Planday returned an error while retrieving contract rules: {response.status_code, response.text}")
 
     def get_custom_fields(self, portal_id: str) -> pd.DataFrame:
@@ -115,15 +137,22 @@
         This function returns all custom fields in the specified portal.
         :param portal_id: portal ID from planday. See get_portals
         :return: dataframe with results
         """
         url = f'{self.base_url}hr/v1.0/employees/fielddefinitions'
         access_token = self.__get_child_token(portal_id=portal_id)
         headers = self.__get_headers(access_token=access_token)
-        response = requests.get(url=url, headers=headers)
+
+        try:
+            response = requests.get(url=url, headers=headers)
+        except requests.exceptions.ConnectionError:
+            print("Connection error, retrying...")
+            time.sleep(5)
+            response = requests.get(url=url, headers=headers)
+
         if 200 <= response.status_code < 300:
             df = pd.DataFrame(response.json()['data'])
             return df
         else:
             raise ConnectionError(f"Planday returned an error while retrieving custom fields: {response.status_code, response.text}")
 
     def get_shifts(self, portal_id: str, from_date: datetime, to_date: datetime) -> pd.DataFrame:
@@ -136,24 +165,40 @@
         """
         url = f"{self.base_url}scheduling/v1.0/shifts"
         access_token = self.__get_child_token(portal_id=portal_id)
         headers = self.__get_headers(access_token=access_token)
         total_response = []
         got_all_results = False
         no_of_loops = 0
+        retry = 0
+
         while not got_all_results:
             params = {"limit": "50", "offset": f"{50 * no_of_loops}", "to": to_date, "from": from_date}
-            response = requests.get(url=url, headers=headers, params=params)
-            if response.status_code == 200:
+            error = False
+            response = ''
+
+            try:
+                response = requests.get(url=url, headers=headers, params=params)
+            except requests.exceptions.ConnectionError:
+                print("Connection error, retrying...")
+                time.sleep(5)
+                error = True
+
+            if error is False and response.status_code == 200:
                 response_json = response.json()
                 no_of_loops += 1
                 got_all_results = False if len(response_json['data']) == 50 else True
                 total_response += response_json['data']
+                retry = 0
             else:
-                raise ConnectionError(f"Planday returned an error while retrieving shifts: {response.status_code, response.text}")
+                if retry < 5:
+                    retry += 1
+                    time.sleep(5)
+                else:
+                    raise ConnectionError(f"Planday returned an error while retrieving shifts: {response.status_code, response.text}")
 
         print(f"Received {len(total_response)} shifts from Planday")
 
         df = pd.DataFrame(total_response)
 
         return df
 
@@ -165,24 +210,40 @@
         """
         url = f"{self.base_url}scheduling/v1.0/shifttypes"
         access_token = self.__get_child_token(portal_id=portal_id)
         headers = self.__get_headers(access_token=access_token)
         total_response = []
         got_all_results = False
         no_of_loops = 0
+        retry = 0
+
         while not got_all_results:
             params = {"limit": "50", "offset": f"{50 * no_of_loops}"}
-            response = requests.get(url=url, headers=headers, params=params)
-            if response.status_code == 200:
+            error = False
+            response = ''
+
+            try:
+                response = requests.get(url=url, headers=headers, params=params)
+            except requests.exceptions.ConnectionError:
+                print("Connection error, retrying...")
+                time.sleep(5)
+                error = True
+            
+            if error is False and response.status_code == 200:
                 response_json = response.json()
                 no_of_loops += 1
                 got_all_results = False if len(response_json['data']) == 50 else True
                 total_response += response_json['data']
+
             else:
-                raise ConnectionError(f"Planday returned an error while retrieving shifttypes: {response.status_code, response.text}")
+                if retry < 5:
+                    retry += 1
+                    time.sleep(5)
+                else:
+                    raise ConnectionError(f"Planday returned an error while retrieving shifttypes: {response.status_code, response.text}")
 
         print(f"Received {len(total_response)} shifttypes from Planday")
 
         df = pd.DataFrame(total_response)
 
         return df
 
@@ -213,24 +274,40 @@
         """
         url = f'{self.base_url}hr/v1.0/employees'
         access_token = self.__get_child_token(portal_id=portal_id)
         headers = self.__get_headers(access_token=access_token)
         total_response = []
         got_all_results = False
         no_of_loops = 0
+        retry = 0
+
         while not got_all_results:
             params = {"limit": "50", "offset": f"{50 * no_of_loops}"}
-            response = requests.get(url=url, headers=headers, params=params)
-            if response.status_code == 200:
+            error = False
+            response = ''
+
+            try:
+                response = requests.get(url=url, headers=headers, params=params)
+            except requests.exceptions.ConnectionError:
+                print("Connection error, retrying...")
+                time.sleep(5)
+                error = True
+
+            if error is False and response.status_code == 200:
                 response_json = response.json()
                 no_of_loops += 1
                 got_all_results = False if len(response_json['data']) == 50 else True
                 total_response += response_json['data']
+
             else:
-                raise ConnectionError(f"Planday returned an error while retrieving employees: {response.status_code, response.text}")
+                if retry < 5:
+                    retry += 1
+                    time.sleep(5)
+                else:
+                    raise ConnectionError(f"Planday returned an error while retrieving employees: {response.status_code, response.text}")
 
         print(f"Received {len(total_response)} employees from Planday")
 
         df = pd.DataFrame(total_response)
 
         return df
 
@@ -242,24 +319,40 @@
         """
         url = f'{self.base_url}hr/v1.0/employeetypes'
         access_token = self.__get_child_token(portal_id=portal_id)
         headers = self.__get_headers(access_token=access_token)
         total_response = []
         got_all_results = False
         no_of_loops = 0
+        retry = 0
+
         while not got_all_results:
             params = {"limit": "50", "offset": f"{50 * no_of_loops}"}
-            response = requests.get(url=url, headers=headers, params=params)
-            if response.status_code == 200:
+            error = False
+            response = ''
+
+            try:
+                response = requests.get(url=url, headers=headers, params=params)
+            except requests.exceptions.ConnectionError:
+                print("Connection error, retrying...")
+                time.sleep(5)
+                error = True
+
+            if error is False and response.status_code == 200:
                 response_json = response.json()
                 no_of_loops += 1
                 got_all_results = False if len(response_json['data']) == 50 else True
                 total_response += response_json['data']
+
             else:
-                raise ConnectionError(f"Planday returned an error while retrieving employee types: {response.status_code, response.text}")
+                if retry < 5:
+                    retry += 1
+                    time.sleep(5)
+                else:
+                    raise ConnectionError(f"Planday returned an error while retrieving employee types: {response.status_code, response.text}")
 
         print(f"Received {len(total_response)} employee types from Planday")
 
         df = pd.DataFrame(total_response)
 
         return df
```

