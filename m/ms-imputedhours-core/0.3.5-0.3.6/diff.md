# Comparing `tmp/ms_imputedhours_core-0.3.5.tar.gz` & `tmp/ms_imputedhours_core-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_imputedhours_core-0.3.5.tar", max compression
+gzip compressed data, was "ms_imputedhours_core-0.3.6.tar", max compression
```

## Comparing `ms_imputedhours_core-0.3.5.tar` & `ms_imputedhours_core-0.3.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35149 2023-04-20 11:36:24.207517 ms_imputedhours_core-0.3.5/LICENSE
--rw-r--r--   0        0        0     2401 2023-04-20 11:36:24.207517 ms_imputedhours_core-0.3.5/README.md
--rw-r--r--   0        0        0       22 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/__init__.py
--rw-r--r--   0        0        0     3238 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/agreements/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/agreements/__tests__/__init__.py
--rw-r--r--   0        0        0     3228 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/agreements/__tests__/test_agreements.py
--rw-r--r--   0        0        0     4113 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/__tests__/__init__.py
--rw-r--r--   0        0        0     6179 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/__tests__/test_employee.py
--rw-r--r--   0        0        0     6933 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/__tests__/__init__.py
--rw-r--r--   0        0        0     9019 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/__tests__/test_data.py
--rw-r--r--   0        0        0    10444 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/bigquery.py
--rw-r--r--   0        0        0      171 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/constants.py
--rw-r--r--   0        0        0        0 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__tests__/__init__.py
--rw-r--r--   0        0        0     4491 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py
--rw-r--r--   0        0        0     6206 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py
--rw-r--r--   0        0        0      776 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py
--rw-r--r--   0        0        0      654 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/alert.py
--rw-r--r--   0        0        0     3599 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/bigquery.py
--rw-r--r--   0        0        0      423 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/dates.py
--rw-r--r--   0        0        0        0 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/transformers/__init__.py
--rw-r--r--   0        0        0     3828 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/transformers/hours.py
--rw-r--r--   0        0        0      203 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/office/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/office/__tests__/__init__.py
--rw-r--r--   0        0        0      678 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/ms_imputedhours_core/office/__tests__/test_office.py
--rw-r--r--   0        0        0      950 2023-04-20 11:36:24.211517 ms_imputedhours_core-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 ms_imputedhours_core-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-21 15:52:12.605725 ms_imputedhours_core-0.3.6/LICENSE
+-rw-r--r--   0        0        0     2401 2023-04-21 15:52:12.605725 ms_imputedhours_core-0.3.6/README.md
+-rw-r--r--   0        0        0       22 2023-04-21 15:52:12.605725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/__init__.py
+-rw-r--r--   0        0        0     3238 2023-04-21 15:52:12.605725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/agreements/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 15:52:12.605725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/agreements/__tests__/__init__.py
+-rw-r--r--   0        0        0     3228 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/agreements/__tests__/test_agreements.py
+-rw-r--r--   0        0        0     4113 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/__tests__/__init__.py
+-rw-r--r--   0        0        0     6179 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/__tests__/test_employee.py
+-rw-r--r--   0        0        0     6953 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/__tests__/__init__.py
+-rw-r--r--   0        0        0     9019 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/__tests__/test_data.py
+-rw-r--r--   0        0        0    10493 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/bigquery.py
+-rw-r--r--   0        0        0      171 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/constants.py
+-rw-r--r--   0        0        0        0 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__tests__/__init__.py
+-rw-r--r--   0        0        0     4491 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py
+-rw-r--r--   0        0        0     6206 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py
+-rw-r--r--   0        0        0      776 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py
+-rw-r--r--   0        0        0      654 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/alert.py
+-rw-r--r--   0        0        0     3599 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/bigquery.py
+-rw-r--r--   0        0        0      423 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/dates.py
+-rw-r--r--   0        0        0        0 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/transformers/__init__.py
+-rw-r--r--   0        0        0     3828 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/transformers/hours.py
+-rw-r--r--   0        0        0      203 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/office/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/office/__tests__/__init__.py
+-rw-r--r--   0        0        0      678 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/ms_imputedhours_core/office/__tests__/test_office.py
+-rw-r--r--   0        0        0      950 2023-04-21 15:52:12.609725 ms_imputedhours_core-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 ms_imputedhours_core-0.3.6/PKG-INFO
```

### Comparing `ms_imputedhours_core-0.3.5/LICENSE` & `ms_imputedhours_core-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.5/README.md` & `ms_imputedhours_core-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.5/ms_imputedhours_core/agreements/__init__.py` & `ms_imputedhours_core-0.3.6/ms_imputedhours_core/agreements/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.5/ms_imputedhours_core/agreements/__tests__/test_agreements.py` & `ms_imputedhours_core-0.3.6/ms_imputedhours_core/agreements/__tests__/test_agreements.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/__init__.py` & `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/__tests__/test_employee.py` & `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/__tests__/test_employee.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/__init__.py` & `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 def get_all_employees_monthly_data_by_office(date, office_name):
     data = {}
     agreement_hours = Agreements(AGREEMENTS_SPREADSHEET_ID).get_hours_by_month(
         date.month, date.year, office_name
     )
     successfactor_all_data = transform_successfactor_all_data(
-        get_successfactor_all_data(office_name)
+        get_successfactor_all_data(office_name, only_actives=False)
     )
     if successfactor_all_data:
         office_emails = successfactor_all_data.keys()
         current_month_data = group_task_by_email(
             get_all_data(date, office_emails)
         )
         all_employee_ftes = transform_all_capacities(
```

### Comparing `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/__tests__/test_data.py` & `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/__tests__/test_data.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/bigquery.py` & `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/bigquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,16 +66,15 @@
 
 QUERY_SUCCESS_FACTOR_ALL = """
         SELECT
             *
         FROM
             `{BIGQUERY_SUCCESS_FACTOR}`
         WHERE
-            office = '{office_name}' AND
-            status = 'Active'
+            office = '{office_name}'
     """
 
 QUERY_SUCCESS_FACTOR_ALL_DATA = """
         SELECT
             *
         FROM
             `{BIGQUERY_SUCCESS_FACTOR}`
@@ -208,19 +207,23 @@
     query = QUERY_SUCCESS_FACTOR.format(
         email=email, BIGQUERY_SUCCESS_FACTOR=BIGQUERY_SUCCESS_FACTOR
     )
 
     return execute_query(query, error_value=[])
 
 
-def get_successfactor_all_data(office_name):
+def get_successfactor_all_data(office_name, only_actives=True):
     query = QUERY_SUCCESS_FACTOR_ALL.format(
         BIGQUERY_SUCCESS_FACTOR=BIGQUERY_SUCCESS_FACTOR,
         office_name=office_name,
     )
+
+    if only_actives:
+        query += "AND status = 'Active'"
+
     return execute_query(query, error_value=[])
 
 
 def get_successfactor_all_offices():
     query = QUERY_SUCCESS_FACTOR_ALL_DATA.format(
         BIGQUERY_SUCCESS_FACTOR=BIGQUERY_SUCCESS_FACTOR
     )
```

### Comparing `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py` & `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py` & `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py` & `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/alert.py` & `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/alert.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/helpers/bigquery.py` & `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/helpers/bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.5/ms_imputedhours_core/employee/data/transformers/hours.py` & `ms_imputedhours_core-0.3.6/ms_imputedhours_core/employee/data/transformers/hours.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.5/ms_imputedhours_core/office/__tests__/test_office.py` & `ms_imputedhours_core-0.3.6/ms_imputedhours_core/office/__tests__/test_office.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.5/pyproject.toml` & `ms_imputedhours_core-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-imputedhours-core"
-version = "0.3.5"
+version = "0.3.6"
 description = "Python library to collect data about jira imputed hours and employee agreements"
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_imputedhours_core"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_imputedhours_core-0.3.5/PKG-INFO` & `ms_imputedhours_core-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-imputedhours-core
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python library to collect data about jira imputed hours and employee agreements
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

