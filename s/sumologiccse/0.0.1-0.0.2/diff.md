# Comparing `tmp/sumologiccse-0.0.1.tar.gz` & `tmp/sumologiccse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumologiccse-0.0.1.tar", last modified: Mon Apr 10 21:36:23 2023, max compression
+gzip compressed data, was "sumologiccse-0.0.2.tar", last modified: Fri Apr 21 04:52:19 2023, max compression
```

## Comparing `sumologiccse-0.0.1.tar` & `sumologiccse-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rjury      (502) staff       (20)        0 2023-04-10 21:36:23.845044 sumologiccse-0.0.1/
--rw-r--r--   0 rjury      (502) staff       (20)     1068 2023-04-10 21:04:30.000000 sumologiccse-0.0.1/LICENSE
--rw-r--r--   0 rjury      (502) staff       (20)     1983 2023-04-10 21:36:23.844878 sumologiccse-0.0.1/PKG-INFO
--rw-r--r--   0 rjury      (502) staff       (20)     1368 2022-11-24 21:13:26.000000 sumologiccse-0.0.1/README.md
--rw-r--r--   0 rjury      (502) staff       (20)      599 2023-04-10 21:02:55.000000 sumologiccse-0.0.1/pyproject.toml
--rw-r--r--   0 rjury      (502) staff       (20)       38 2023-04-10 21:36:23.845098 sumologiccse-0.0.1/setup.cfg
-drwxr-xr-x   0 rjury      (502) staff       (20)        0 2023-04-10 21:36:23.843823 sumologiccse-0.0.1/sumologiccse/
--rw-r--r--   0 rjury      (502) staff       (20)        0 2023-04-10 20:59:21.000000 sumologiccse-0.0.1/sumologiccse/__init__.py
--rw-r--r--   0 rjury      (502) staff       (20)     8633 2023-03-28 02:38:12.000000 sumologiccse-0.0.1/sumologiccse/sumologiccse.py
-drwxr-xr-x   0 rjury      (502) staff       (20)        0 2023-04-10 21:36:23.844465 sumologiccse-0.0.1/sumologiccse.egg-info/
--rw-r--r--   0 rjury      (502) staff       (20)     1983 2023-04-10 21:36:23.000000 sumologiccse-0.0.1/sumologiccse.egg-info/PKG-INFO
--rw-r--r--   0 rjury      (502) staff       (20)      257 2023-04-10 21:36:23.000000 sumologiccse-0.0.1/sumologiccse.egg-info/SOURCES.txt
--rw-r--r--   0 rjury      (502) staff       (20)        1 2023-04-10 21:36:23.000000 sumologiccse-0.0.1/sumologiccse.egg-info/dependency_links.txt
--rw-r--r--   0 rjury      (502) staff       (20)       13 2023-04-10 21:36:23.000000 sumologiccse-0.0.1/sumologiccse.egg-info/top_level.txt
-drwxr-xr-x   0 rjury      (502) staff       (20)        0 2023-04-10 21:36:23.844634 sumologiccse-0.0.1/tests/
--rw-r--r--   0 rjury      (502) staff       (20)     1689 2023-04-10 21:33:13.000000 sumologiccse-0.0.1/tests/test_sumologiccse.py
+drwxr-xr-x   0 rjury      (502) staff       (20)        0 2023-04-21 04:52:19.403558 sumologiccse-0.0.2/
+-rw-r--r--   0 rjury      (502) staff       (20)     1068 2023-04-10 21:04:30.000000 sumologiccse-0.0.2/LICENSE
+-rw-r--r--   0 rjury      (502) staff       (20)     2442 2023-04-21 04:52:19.403318 sumologiccse-0.0.2/PKG-INFO
+-rw-r--r--   0 rjury      (502) staff       (20)     1827 2023-04-10 21:45:16.000000 sumologiccse-0.0.2/README.md
+-rw-r--r--   0 rjury      (502) staff       (20)      599 2023-04-21 04:52:13.000000 sumologiccse-0.0.2/pyproject.toml
+-rw-r--r--   0 rjury      (502) staff       (20)       38 2023-04-21 04:52:19.403690 sumologiccse-0.0.2/setup.cfg
+drwxr-xr-x   0 rjury      (502) staff       (20)        0 2023-04-21 04:52:19.402289 sumologiccse-0.0.2/sumologiccse/
+-rw-r--r--   0 rjury      (502) staff       (20)        0 2023-04-10 20:59:21.000000 sumologiccse-0.0.2/sumologiccse/__init__.py
+-rw-r--r--   0 rjury      (502) staff       (20)     8641 2023-04-21 04:47:05.000000 sumologiccse-0.0.2/sumologiccse/sumologiccse.py
+drwxr-xr-x   0 rjury      (502) staff       (20)        0 2023-04-21 04:52:19.402938 sumologiccse-0.0.2/sumologiccse.egg-info/
+-rw-r--r--   0 rjury      (502) staff       (20)     2442 2023-04-21 04:52:19.000000 sumologiccse-0.0.2/sumologiccse.egg-info/PKG-INFO
+-rw-r--r--   0 rjury      (502) staff       (20)      257 2023-04-21 04:52:19.000000 sumologiccse-0.0.2/sumologiccse.egg-info/SOURCES.txt
+-rw-r--r--   0 rjury      (502) staff       (20)        1 2023-04-21 04:52:19.000000 sumologiccse-0.0.2/sumologiccse.egg-info/dependency_links.txt
+-rw-r--r--   0 rjury      (502) staff       (20)       13 2023-04-21 04:52:19.000000 sumologiccse-0.0.2/sumologiccse.egg-info/top_level.txt
+drwxr-xr-x   0 rjury      (502) staff       (20)        0 2023-04-21 04:52:19.403105 sumologiccse-0.0.2/tests/
+-rw-r--r--   0 rjury      (502) staff       (20)     1689 2023-04-10 21:33:13.000000 sumologiccse-0.0.2/tests/test_sumologiccse.py
```

### Comparing `sumologiccse-0.0.1/LICENSE` & `sumologiccse-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sumologiccse-0.0.1/PKG-INFO` & `sumologiccse-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: sumologiccse
-Version: 0.0.1
+Version: 0.0.2
 Summary: An API client for common use cases for the Sumologic Cloud SIEM API https://api.sumologic.com/docs/sec/#
 Author-email: Rick Jury <rjury@sumologic.com>
 Project-URL: Homepage, https://github.com/rjury-sumo/sumologic-cse-python-sdk
 Project-URL: Bug Tracker, https://github.com/rjury-sumo/sumologic-cse-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sumologic-cse-python-sdk
-https://api.sumologic.com/docs/sec/#
+An api client similar to the official Sumologic python API client but for the CSE api: https://api.sumologic.com/docs/sec/#
+
+This api has many endpoints this project only intends to cover off and provide useful scripts to solve some common use caes rather than support all of them.
+
+
+# install package
+```
+pip install sumologiccse==0.0.1
+```
 
 # Getting Started
 see the scripts section for examples. In general either set env vars:
 - SUMO_ACCESS_ID
 - SUMO_ACCESS_KEY
 or you must privide as arguments.
 
@@ -39,20 +47,24 @@
 ```
 
 There are a lot of API endpoints you can also call them directly for example:
 ```
 statuses = cse.get('/insight-status')
 ```
 
+# Example Use Case Scripts
+You can find these in ./scripts
+
 ## Bulk Resolve Insights Script
-Use the provided script for example from root dir of project. This has a dryrun mode set this to False to make updates.
+For bulk closing insights using various criteria. This can be using the DSL (-q) or using client side filtering such as confidence score or a regex vs the json-ified payload. 
+
+This has a dryrun mode set this to False to make updates.
 The script will add a comment to each insight before changing it's status and resolution using the supplied params.
 
 Assuming you set env vars as per above for key and id:
 ```
-export PYTHONPATH="`pwd`"
 python ./scripts/insights/resolve_insights.py --endpoint 'us2' --dryrun True --limit 5 --query='-status:"closed"'
 ```
 
 # TODOs
 - Add a decent selection of endpoints
-- Write some unit and integration tests
+- Write some more unit and integration tests
```

### Comparing `sumologiccse-0.0.1/README.md` & `sumologiccse-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # sumologic-cse-python-sdk
-https://api.sumologic.com/docs/sec/#
+An api client similar to the official Sumologic python API client but for the CSE api: https://api.sumologic.com/docs/sec/#
+
+This api has many endpoints this project only intends to cover off and provide useful scripts to solve some common use caes rather than support all of them.
+
+
+# install package
+```
+pip install sumologiccse==0.0.1
+```
 
 # Getting Started
 see the scripts section for examples. In general either set env vars:
 - SUMO_ACCESS_ID
 - SUMO_ACCESS_KEY
 or you must privide as arguments.
 
@@ -25,20 +33,24 @@
 ```
 
 There are a lot of API endpoints you can also call them directly for example:
 ```
 statuses = cse.get('/insight-status')
 ```
 
+# Example Use Case Scripts
+You can find these in ./scripts
+
 ## Bulk Resolve Insights Script
-Use the provided script for example from root dir of project. This has a dryrun mode set this to False to make updates.
+For bulk closing insights using various criteria. This can be using the DSL (-q) or using client side filtering such as confidence score or a regex vs the json-ified payload. 
+
+This has a dryrun mode set this to False to make updates.
 The script will add a comment to each insight before changing it's status and resolution using the supplied params.
 
 Assuming you set env vars as per above for key and id:
 ```
-export PYTHONPATH="`pwd`"
 python ./scripts/insights/resolve_insights.py --endpoint 'us2' --dryrun True --limit 5 --query='-status:"closed"'
 ```
 
 # TODOs
 - Add a decent selection of endpoints
-- Write some unit and integration tests
+- Write some more unit and integration tests
```

### Comparing `sumologiccse-0.0.1/pyproject.toml` & `sumologiccse-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sumologiccse"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Rick Jury", email="rjury@sumologic.com" },
 ]
 description = "An API client for common use cases for the Sumologic Cloud SIEM API https://api.sumologic.com/docs/sec/#"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sumologiccse-0.0.1/sumologiccse/sumologiccse.py` & `sumologiccse-0.0.2/sumologiccse/sumologiccse.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,20 +155,20 @@
 
             if nextPageToken == None:
                 logger.debug(str(len(insights))
                              + ' insights at last page: ' + str(pages))
                 break
         return insights
     
-    def get_insights_list(self,q=None,offset=0,limit=10):
+    def get_insights_list(self,q=None,offset=0,limit=20):
         params = {'q': q, 'offset': offset, 'limit': limit}
         response = self.get('/insights', params)
         return json.loads(response.text)
     
-    def query_insights(self, q=None,offset=0,limit=10):
+    def query_insights(self, q=None,offset=0,limit=20):
         insights = []
         pages = 0
         if limit > 20:
             batchsize = 20
         else: 
             batchsize = limit
 
@@ -185,15 +185,15 @@
                 logger.debug("no results")
                 remaining = 0
 
             if i['data']['hasNextPage'] == False:
                 logger.debug(str(len(insights))
                              + ' insights at last page: ' + str(len(i['data']['objects'])))
                 break
-            pages += 1
+            pages += batchsize
             if remaining > 20:
                 batchsize = 20
             else:
                 batchsize = remaining
         return insights
 
     def get_insight(self, insight_id):
```

### Comparing `sumologiccse-0.0.1/sumologiccse.egg-info/PKG-INFO` & `sumologiccse-0.0.2/sumologiccse.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: sumologiccse
-Version: 0.0.1
+Version: 0.0.2
 Summary: An API client for common use cases for the Sumologic Cloud SIEM API https://api.sumologic.com/docs/sec/#
 Author-email: Rick Jury <rjury@sumologic.com>
 Project-URL: Homepage, https://github.com/rjury-sumo/sumologic-cse-python-sdk
 Project-URL: Bug Tracker, https://github.com/rjury-sumo/sumologic-cse-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sumologic-cse-python-sdk
-https://api.sumologic.com/docs/sec/#
+An api client similar to the official Sumologic python API client but for the CSE api: https://api.sumologic.com/docs/sec/#
+
+This api has many endpoints this project only intends to cover off and provide useful scripts to solve some common use caes rather than support all of them.
+
+
+# install package
+```
+pip install sumologiccse==0.0.1
+```
 
 # Getting Started
 see the scripts section for examples. In general either set env vars:
 - SUMO_ACCESS_ID
 - SUMO_ACCESS_KEY
 or you must privide as arguments.
 
@@ -39,20 +47,24 @@
 ```
 
 There are a lot of API endpoints you can also call them directly for example:
 ```
 statuses = cse.get('/insight-status')
 ```
 
+# Example Use Case Scripts
+You can find these in ./scripts
+
 ## Bulk Resolve Insights Script
-Use the provided script for example from root dir of project. This has a dryrun mode set this to False to make updates.
+For bulk closing insights using various criteria. This can be using the DSL (-q) or using client side filtering such as confidence score or a regex vs the json-ified payload. 
+
+This has a dryrun mode set this to False to make updates.
 The script will add a comment to each insight before changing it's status and resolution using the supplied params.
 
 Assuming you set env vars as per above for key and id:
 ```
-export PYTHONPATH="`pwd`"
 python ./scripts/insights/resolve_insights.py --endpoint 'us2' --dryrun True --limit 5 --query='-status:"closed"'
 ```
 
 # TODOs
 - Add a decent selection of endpoints
-- Write some unit and integration tests
+- Write some more unit and integration tests
```

### Comparing `sumologiccse-0.0.1/tests/test_sumologiccse.py` & `sumologiccse-0.0.2/tests/test_sumologiccse.py`

 * *Files identical despite different names*

