# Comparing `tmp/dequeai-0.742.tar.gz` & `tmp/dequeai-0.744.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.742.tar", last modified: Thu Apr 20 23:15:09 2023, max compression
+gzip compressed data, was "dequeai-0.744.tar", last modified: Thu Apr 20 23:27:02 2023, max compression
```

## Comparing `dequeai-0.742.tar` & `dequeai-0.744.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 23:15:09.029185 dequeai-0.742/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 23:15:09.029185 dequeai-0.742/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 23:15:09.029185 dequeai-0.742/dequeai/
--rw-r--r--   0 root         (0) root         (0)      398 2023-04-20 21:04:18.000000 dequeai-0.742/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.742/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.742/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.742/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-04-20 20:33:33.000000 dequeai-0.742/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    28332 2023-04-20 23:14:54.000000 dequeai-0.742/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.742/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.742/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.742/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.742/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 23:15:09.029185 dequeai-0.742/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 23:15:08.000000 dequeai-0.742/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 23:15:09.000000 dequeai-0.742/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 23:15:08.000000 dequeai-0.742/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 23:15:08.000000 dequeai-0.742/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 23:15:08.000000 dequeai-0.742/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 23:15:09.029185 dequeai-0.742/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 23:14:54.000000 dequeai-0.742/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 23:27:02.134645 dequeai-0.744/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 23:27:02.134645 dequeai-0.744/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 23:27:02.134645 dequeai-0.744/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      398 2023-04-20 21:04:18.000000 dequeai-0.744/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.744/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.744/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.744/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      864 2023-04-20 20:33:33.000000 dequeai-0.744/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    27826 2023-04-20 23:26:49.000000 dequeai-0.744/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.744/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.744/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.744/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.744/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 23:27:02.134645 dequeai-0.744/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 23:27:01.000000 dequeai-0.744/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 23:27:02.000000 dequeai-0.744/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 23:27:01.000000 dequeai-0.744/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 23:27:01.000000 dequeai-0.744/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 23:27:02.000000 dequeai-0.744/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 23:27:02.134645 dequeai-0.744/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 23:26:49.000000 dequeai-0.744/setup.py
```

### Comparing `dequeai-0.742/dequeai/datatypes.py` & `dequeai-0.744/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.742/dequeai/dequeai.py` & `dequeai-0.744/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.742/dequeai/dequeai_run.py` & `dequeai-0.744/dequeai/dequeai_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -421,53 +421,49 @@
         for run in data_list['runs']:
             best_metric = self._get_nested_value(run['best_experiment_data']['data'], metric_key)
             row = [run['run_id'], metric_key, best_metric]
             for key in first_run_data_keys:
                 row.extend(run['best_experiment_data']['data'][key].values())
             rows.append(row)
 
+
         # Use tabulate to generate the HTML table
-        html_table = tabulate(rows, headers=headers, tablefmt="html")
+        table_styles = """
+        <style>
+            table {
+                border-collapse: collapse;
+                font-family: Arial, sans-serif;
+            }
+            th {
+                background-color: #29213C;
+                color: #D953A8;
+                font-weight: bold;
+                padding: 8px;
+                text-align: left;
+                border: 1px solid #C3B5DD;
+            }
+            td {
+                background-color: #60507D;
+                color: #C3B5DD;
+                padding: 8px;
+                text-align: left;
+                border: 1px solid #C3B5DD;
+            }
+        </style>
+        """
 
-        # Style the table with your color palette
-        styled_table = f"""
-            <style>
-                table {{
-                    border-collapse: collapse;
-                    font-family: Arial, sans-serif;
-                    background-color: #29213C;
-                    color: #D953A8;
-                    width: 100%;
-                }}
-                th {{
-                    background-color: #60507D;
-                    color: #D953A8;
-                    padding: 8px;
-                    text-align: left;
-                }}
-                td {{
-                    background-color: #C3B5DD;
-                    color: #7E5BEC;
-                    padding: 8px;
-                    text-align: left;
-                }}
-                tr:nth-child(even) td {{
-                    background-color: #60507D;
-                    color: #7E5BEC;
-                }}
-            </style>
-            {html_table}
-            """
+        html_table = tabulate(data_list, headers="keys", tablefmt="html")
 
         # Wrap the table in a scrollable div
-        scrollable_table = f'<div style="width: 100%; height: 200px; overflow: auto;">{styled_table}</div>'
+        scrollable_table = f'<div style="width: 100%; height: 200px; overflow: auto;">{table_styles}{html_table}</div>'
 
         # Display the scrollable table in the notebook
         display(HTML(scrollable_table))
 
+
     def read_best_run(self, project_name, metric_key):
 
         if self.user_name is None:
             raise ValueError("Please initialize using dequeai.init() before calling compare_runs")
 
         if project_name is None:
             project_name = self._project_name
@@ -492,49 +488,46 @@
         for run in data_list['run']:
             best_metric = self._get_nested_value(run['best_experiment_data']['data'], metric_key)
             row = [run['run_id'], metric_key, best_metric]
             for key in first_run_data_keys:
                 row.extend(run['best_experiment_data']['data'][key].values())
             rows.append(row)
 
-        # Use tabulate to generate the HTML table
-        html_table = tabulate(rows, headers=headers, tablefmt="html")
 
         # Style the table with your color palette
-        styled_table = f"""
-            <style>
-                table {{
-                    border-collapse: collapse;
-                    font-family: Arial, sans-serif;
-                    background-color: #29213C;
-                    color: #D953A8;
-                    width: 100%;
-                }}
-                th {{
-                    background-color: #60507D;
-                    color: #D953A8;
-                    padding: 8px;
-                    text-align: left;
-                }}
-                td {{
-                    background-color: #C3B5DD;
-                    color: #7E5BEC;
-                    padding: 8px;
-                    text-align: left;
-                }}
-                tr:nth-child(even) td {{
-                    background-color: #60507D;
-                    color: #7E5BEC;
-                }}
-            </style>
-            {html_table}
-            """
+        # Use tabulate to generate the HTML table
+        table_styles = """
+        <style>
+            table {
+                border-collapse: collapse;
+                font-family: Arial, sans-serif;
+            }
+            th {
+                background-color: #29213C;
+                color: #D953A8;
+                font-weight: bold;
+                padding: 8px;
+                text-align: left;
+                border: 1px solid #C3B5DD;
+            }
+            td {
+                background-color: #60507D;
+                color: #C3B5DD;
+                padding: 8px;
+                text-align: left;
+                border: 1px solid #C3B5DD;
+            }
+        </style>
+        """
+
+        html_table = tabulate(data_list, headers="keys", tablefmt="html")
 
         # Wrap the table in a scrollable div
-        scrollable_table = f'<div style="width: 100%; height: 200px; overflow: auto;">{styled_table}</div>'
+        scrollable_table = f'<div style="width: 100%; height: 200px; overflow: auto;">{table_styles}{html_table}</div>'
+
 
         # Display the scrollable table in the notebook
         display(HTML(scrollable_table))
 
 
     def search_runs(self,filter_dict):
         if self.user_name is None:
```

### Comparing `dequeai-0.742/dequeai/parsing_service.py` & `dequeai-0.744/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.742/dequeai/rest_connect.py` & `dequeai-0.744/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.742/dequeai/util.py` & `dequeai-0.744/dequeai/util.py`

 * *Files identical despite different names*

