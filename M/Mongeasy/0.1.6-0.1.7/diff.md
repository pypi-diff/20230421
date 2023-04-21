# Comparing `tmp/Mongeasy-0.1.6.tar.gz` & `tmp/Mongeasy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mongeasy-0.1.6.tar", last modified: Thu Apr 20 12:03:53 2023, max compression
+gzip compressed data, was "Mongeasy-0.1.7.tar", last modified: Thu Apr 20 14:09:11 2023, max compression
```

## Comparing `Mongeasy-0.1.6.tar` & `Mongeasy-0.1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.363582 Mongeasy-0.1.6/
--rw-rw-rw-   0        0        0     1096 2023-04-17 10:50:01.000000 Mongeasy-0.1.6/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.345055 Mongeasy-0.1.6/Mongeasy.egg-info/
--rw-rw-rw-   0        0        0     8684 2023-04-20 12:03:53.000000 Mongeasy-0.1.6/Mongeasy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2023-04-20 12:03:53.000000 Mongeasy-0.1.6/Mongeasy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 12:03:53.000000 Mongeasy-0.1.6/Mongeasy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-20 12:03:53.000000 Mongeasy-0.1.6/Mongeasy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-20 12:03:53.000000 Mongeasy-0.1.6/Mongeasy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-20 12:03:53.000000 Mongeasy-0.1.6/Mongeasy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8684 2023-04-20 12:03:53.363582 Mongeasy-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     7881 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.356061 Mongeasy-0.1.6/mongeasy/
--rw-rw-rw-   0        0        0     2164 2023-04-20 12:03:39.000000 Mongeasy-0.1.6/mongeasy/__init__.py
--rw-rw-rw-   0        0        0     2775 2023-03-03 13:34:30.000000 Mongeasy-0.1.6/mongeasy/base_dict.py
--rw-rw-rw-   0        0        0     2421 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/connection.py
--rw-rw-rw-   0        0        0     1487 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/core.py
--rw-rw-rw-   0        0        0    11815 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/document.py
--rw-rw-rw-   0        0        0     2657 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/dynamics.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.357061 Mongeasy-0.1.6/mongeasy/examples/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/examples/__init__.py
--rw-rw-rw-   0        0        0     1851 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.358061 Mongeasy-0.1.6/mongeasy/extensions/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/extensions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.359061 Mongeasy-0.1.6/mongeasy/plugins/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/plugins/__init__.py
--rw-rw-rw-   0        0        0     4963 2023-04-20 11:49:23.000000 Mongeasy-0.1.6/mongeasy/resultlist.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.360571 Mongeasy-0.1.6/mongeasy/utils/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/utils/__init__.py
--rw-rw-rw-   0        0        0     1803 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/mongeasy/utils/utils.py
--rw-rw-rw-   0        0        0       91 2023-04-17 11:07:53.000000 Mongeasy-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0     1057 2023-04-20 12:03:53.364582 Mongeasy-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1076 2023-04-20 12:03:25.000000 Mongeasy-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:03:53.362577 Mongeasy-0.1.6/tests/
--rw-rw-rw-   0        0        0       39 2023-04-17 07:50:37.000000 Mongeasy-0.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0    10126 2023-04-20 11:53:13.000000 Mongeasy-0.1.6/tests/test_mongeasy.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:09:11.371193 Mongeasy-0.1.7/
+-rw-rw-rw-   0        0        0     1096 2023-04-17 10:50:01.000000 Mongeasy-0.1.7/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-20 14:09:11.356676 Mongeasy-0.1.7/Mongeasy.egg-info/
+-rw-rw-rw-   0        0        0    10733 2023-04-20 14:09:11.000000 Mongeasy-0.1.7/Mongeasy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      599 2023-04-20 14:09:11.000000 Mongeasy-0.1.7/Mongeasy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 14:09:11.000000 Mongeasy-0.1.7/Mongeasy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-20 14:09:11.000000 Mongeasy-0.1.7/Mongeasy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-20 14:09:11.000000 Mongeasy-0.1.7/Mongeasy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-20 14:09:11.000000 Mongeasy-0.1.7/Mongeasy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10733 2023-04-20 14:09:11.371193 Mongeasy-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     9932 2023-04-20 14:08:47.000000 Mongeasy-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 14:09:11.364196 Mongeasy-0.1.7/mongeasy/
+-rw-rw-rw-   0        0        0     2164 2023-04-20 14:08:47.000000 Mongeasy-0.1.7/mongeasy/__init__.py
+-rw-rw-rw-   0        0        0     2775 2023-03-03 13:34:30.000000 Mongeasy-0.1.7/mongeasy/base_dict.py
+-rw-rw-rw-   0        0        0     2421 2023-04-20 11:53:13.000000 Mongeasy-0.1.7/mongeasy/connection.py
+-rw-rw-rw-   0        0        0     2044 2023-04-20 14:08:47.000000 Mongeasy-0.1.7/mongeasy/core.py
+-rw-rw-rw-   0        0        0    12866 2023-04-20 14:08:47.000000 Mongeasy-0.1.7/mongeasy/document.py
+-rw-rw-rw-   0        0        0     2657 2023-04-20 11:53:13.000000 Mongeasy-0.1.7/mongeasy/dynamics.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:09:11.365192 Mongeasy-0.1.7/mongeasy/examples/
+-rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.7/mongeasy/examples/__init__.py
+-rw-rw-rw-   0        0        0     1851 2023-04-20 11:53:13.000000 Mongeasy-0.1.7/mongeasy/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:09:11.366193 Mongeasy-0.1.7/mongeasy/extensions/
+-rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.7/mongeasy/extensions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:09:11.367193 Mongeasy-0.1.7/mongeasy/plugins/
+-rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.7/mongeasy/plugins/__init__.py
+-rw-rw-rw-   0        0        0     4963 2023-04-20 11:49:23.000000 Mongeasy-0.1.7/mongeasy/resultlist.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:09:11.368192 Mongeasy-0.1.7/mongeasy/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.7/mongeasy/utils/__init__.py
+-rw-rw-rw-   0        0        0     1803 2023-04-20 11:53:13.000000 Mongeasy-0.1.7/mongeasy/utils/utils.py
+-rw-rw-rw-   0        0        0       91 2023-04-17 11:07:53.000000 Mongeasy-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1057 2023-04-20 14:09:11.372706 Mongeasy-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2023-04-20 14:08:47.000000 Mongeasy-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:09:11.370193 Mongeasy-0.1.7/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-17 07:50:37.000000 Mongeasy-0.1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0    10126 2023-04-20 11:53:13.000000 Mongeasy-0.1.7/tests/test_mongeasy.py
```

### Comparing `Mongeasy-0.1.6/LICENSE` & `Mongeasy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.6/Mongeasy.egg-info/PKG-INFO` & `Mongeasy-0.1.7/Mongeasy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mongeasy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
 Project-URL: Bug Tracker, https://github.com/artheadsweden/mongeasy/issues
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Mongeasy
 
 Mongeasy is a easy to use library to be used for simple access to a MongoDB database, without any need for schemas or validation. Just store the data as it is used in your application.
 
+### Installation
+Mongoeasy is available on PyPI and can be installed using pip:
+
+```bash
+pip install mongeasy
+```
+
+### What's new in version 0.1.7?
+* Documents now support raw queries using the `raw_query` method. This method will return a pymongo cursor object that can be used to iterate over the documents in the collection.
+* Documents now support raw aggregation using the `raw_aggregate` method. This method will return a pymongo cursor object that can be used to iterate over the documents in the collection.
+* Extended the Query class to support more operators
+
 ### Connection
 Connection to the database is handled automtically for you if you have the conenction information in a configfile or set as environment variables.
 
 #### Connection using configfile
 Create a file called `mongeasy.conf` and place it in your project root folder.
 
 The contents of the file should be:
@@ -231,23 +243,44 @@
 ```python
 query = {'$or': [{'$or': [{'name': {'$eq': 'John'}}, {'age': {'$lt': 40}}]}, {'$and': [{'name': {'$eq': 'Jane'}}, {'age': {'$gt': 20}}]}]}
 ```
 
 you can accomplish the same thing by using the Query object
 
 ```python
+from mongeasy.core import Query
+
+
 query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
 ```
 
 The query can then be used in your queries like this:
 
 ```python
+from mongeasy import create_document_class
+from mongeasy.core import Query
+
+
+User = create_document_class('User', 'users')
+query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
 result = User.find(query)
 ```
 
+Supported operators are:
+* ==
+* !=
+* <
+* >
+* <=
+* >=
+* and
+* or
+* not
+* in
+* not in
 
 ### ResultList
 All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
 
 
 ```python
 from mongeasy import create_document_class
@@ -270,14 +303,33 @@
 * `last_or_none` - Get the last document in the list or None if no document is found, same as last
 * `map` - Apply a given function to each element in the list and return a new ResultList containing the results
 * `filter` - Filter the list using a given function and return a new ResultList containing the results
 * `reduce` - Apply a given function to each element in the list and return a single value
 * `group_by` - Group the list by a given key and return a dict with the results grouped by the key
 * `random` - Get a random document from the list or None if no document is found
 
+### Planned features
+* Enable lazy-loading of query results and support for query chaining
+* Implement a schema plugin system to allow for validation and type checking of documents
+* Add support for transactions using resource management
+* Implement logging and profiling to aid with debugging and performance tuning
+* Enable asynchronous I/O support for improved scalability
+* Implement caching with customizable caching strategies
+* Add support for background tasks using a task queue
+* Implement a paginator utility to allow for pagination of query results
+* Support for MongoDB Atlas search
+* Data migration and seeding utilities
+* Real-time sync feature for monitoring and syncing with another database
+* Automatic data splitting for large documents approaching the 16 MB limit
+* Support for SQL-style auto-increment fields
+* Middleware support for request/response processing
+* Integration with machine learning libraries for data analysis and prediction
+* Built-in analytics to provide insights into database usage and performance
+* Visualization tools to aid with data exploration and presentation
+
 
 ### Contributing
 Contributions are welcome. Please create a pull request with your changes.
 
 ### Issues
 If you find any issues please create an issue on the github page.
```

### Comparing `Mongeasy-0.1.6/Mongeasy.egg-info/SOURCES.txt` & `Mongeasy-0.1.7/Mongeasy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.6/PKG-INFO` & `Mongeasy-0.1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mongeasy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
 Project-URL: Bug Tracker, https://github.com/artheadsweden/mongeasy/issues
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Mongeasy
 
 Mongeasy is a easy to use library to be used for simple access to a MongoDB database, without any need for schemas or validation. Just store the data as it is used in your application.
 
+### Installation
+Mongoeasy is available on PyPI and can be installed using pip:
+
+```bash
+pip install mongeasy
+```
+
+### What's new in version 0.1.7?
+* Documents now support raw queries using the `raw_query` method. This method will return a pymongo cursor object that can be used to iterate over the documents in the collection.
+* Documents now support raw aggregation using the `raw_aggregate` method. This method will return a pymongo cursor object that can be used to iterate over the documents in the collection.
+* Extended the Query class to support more operators
+
 ### Connection
 Connection to the database is handled automtically for you if you have the conenction information in a configfile or set as environment variables.
 
 #### Connection using configfile
 Create a file called `mongeasy.conf` and place it in your project root folder.
 
 The contents of the file should be:
@@ -231,23 +243,44 @@
 ```python
 query = {'$or': [{'$or': [{'name': {'$eq': 'John'}}, {'age': {'$lt': 40}}]}, {'$and': [{'name': {'$eq': 'Jane'}}, {'age': {'$gt': 20}}]}]}
 ```
 
 you can accomplish the same thing by using the Query object
 
 ```python
+from mongeasy.core import Query
+
+
 query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
 ```
 
 The query can then be used in your queries like this:
 
 ```python
+from mongeasy import create_document_class
+from mongeasy.core import Query
+
+
+User = create_document_class('User', 'users')
+query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
 result = User.find(query)
 ```
 
+Supported operators are:
+* ==
+* !=
+* <
+* >
+* <=
+* >=
+* and
+* or
+* not
+* in
+* not in
 
 ### ResultList
 All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
 
 
 ```python
 from mongeasy import create_document_class
@@ -270,14 +303,33 @@
 * `last_or_none` - Get the last document in the list or None if no document is found, same as last
 * `map` - Apply a given function to each element in the list and return a new ResultList containing the results
 * `filter` - Filter the list using a given function and return a new ResultList containing the results
 * `reduce` - Apply a given function to each element in the list and return a single value
 * `group_by` - Group the list by a given key and return a dict with the results grouped by the key
 * `random` - Get a random document from the list or None if no document is found
 
+### Planned features
+* Enable lazy-loading of query results and support for query chaining
+* Implement a schema plugin system to allow for validation and type checking of documents
+* Add support for transactions using resource management
+* Implement logging and profiling to aid with debugging and performance tuning
+* Enable asynchronous I/O support for improved scalability
+* Implement caching with customizable caching strategies
+* Add support for background tasks using a task queue
+* Implement a paginator utility to allow for pagination of query results
+* Support for MongoDB Atlas search
+* Data migration and seeding utilities
+* Real-time sync feature for monitoring and syncing with another database
+* Automatic data splitting for large documents approaching the 16 MB limit
+* Support for SQL-style auto-increment fields
+* Middleware support for request/response processing
+* Integration with machine learning libraries for data analysis and prediction
+* Built-in analytics to provide insights into database usage and performance
+* Visualization tools to aid with data exploration and presentation
+
 
 ### Contributing
 Contributions are welcome. Please create a pull request with your changes.
 
 ### Issues
 If you find any issues please create an issue on the github page.
```

### Comparing `Mongeasy-0.1.6/README.md` & `Mongeasy-0.1.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # Mongeasy
 
 Mongeasy is a easy to use library to be used for simple access to a MongoDB database, without any need for schemas or validation. Just store the data as it is used in your application.
 
+### Installation
+Mongoeasy is available on PyPI and can be installed using pip:
+
+```bash
+pip install mongeasy
+```
+
+### What's new in version 0.1.7?
+* Documents now support raw queries using the `raw_query` method. This method will return a pymongo cursor object that can be used to iterate over the documents in the collection.
+* Documents now support raw aggregation using the `raw_aggregate` method. This method will return a pymongo cursor object that can be used to iterate over the documents in the collection.
+* Extended the Query class to support more operators
+
 ### Connection
 Connection to the database is handled automtically for you if you have the conenction information in a configfile or set as environment variables.
 
 #### Connection using configfile
 Create a file called `mongeasy.conf` and place it in your project root folder.
 
 The contents of the file should be:
@@ -211,23 +223,44 @@
 ```python
 query = {'$or': [{'$or': [{'name': {'$eq': 'John'}}, {'age': {'$lt': 40}}]}, {'$and': [{'name': {'$eq': 'Jane'}}, {'age': {'$gt': 20}}]}]}
 ```
 
 you can accomplish the same thing by using the Query object
 
 ```python
+from mongeasy.core import Query
+
+
 query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
 ```
 
 The query can then be used in your queries like this:
 
 ```python
+from mongeasy import create_document_class
+from mongeasy.core import Query
+
+
+User = create_document_class('User', 'users')
+query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
 result = User.find(query)
 ```
 
+Supported operators are:
+* ==
+* !=
+* <
+* >
+* <=
+* >=
+* and
+* or
+* not
+* in
+* not in
 
 ### ResultList
 All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
 
 
 ```python
 from mongeasy import create_document_class
@@ -250,16 +283,35 @@
 * `last_or_none` - Get the last document in the list or None if no document is found, same as last
 * `map` - Apply a given function to each element in the list and return a new ResultList containing the results
 * `filter` - Filter the list using a given function and return a new ResultList containing the results
 * `reduce` - Apply a given function to each element in the list and return a single value
 * `group_by` - Group the list by a given key and return a dict with the results grouped by the key
 * `random` - Get a random document from the list or None if no document is found
 
+### Planned features
+* Enable lazy-loading of query results and support for query chaining
+* Implement a schema plugin system to allow for validation and type checking of documents
+* Add support for transactions using resource management
+* Implement logging and profiling to aid with debugging and performance tuning
+* Enable asynchronous I/O support for improved scalability
+* Implement caching with customizable caching strategies
+* Add support for background tasks using a task queue
+* Implement a paginator utility to allow for pagination of query results
+* Support for MongoDB Atlas search
+* Data migration and seeding utilities
+* Real-time sync feature for monitoring and syncing with another database
+* Automatic data splitting for large documents approaching the 16 MB limit
+* Support for SQL-style auto-increment fields
+* Middleware support for request/response processing
+* Integration with machine learning libraries for data analysis and prediction
+* Built-in analytics to provide insights into database usage and performance
+* Visualization tools to aid with data exploration and presentation
+
 
 ### Contributing
 Contributions are welcome. Please create a pull request with your changes.
 
 ### Issues
 If you find any issues please create an issue on the github page.
 
 ### License
-This project is licensed under the MIT License - see the LICENSE file for details
+This project is licensed under the MIT License - see the LICENSE file for details
```

### Comparing `Mongeasy-0.1.6/mongeasy/__init__.py` & `Mongeasy-0.1.7/mongeasy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Mongeasy."""
 
 __author__ = """Joakim Wassberg"""
 __email__ = 'joakim.wassberg@arthead.se'
-__version__ = '0.1.6'
+__version__ = '0.1.7'
 
 from mongeasy.connection import MongeasyConnection
 from mongeasy.exceptions import MongeasyDBConnectionError
 from mongeasy.dynamics import create_document_class
 
 connection = MongeasyConnection()
```

### Comparing `Mongeasy-0.1.6/mongeasy/base_dict.py` & `Mongeasy-0.1.7/mongeasy/base_dict.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.6/mongeasy/connection.py` & `Mongeasy-0.1.7/mongeasy/connection.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.6/mongeasy/core.py` & `Mongeasy-0.1.7/mongeasy/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,17 +24,28 @@
             op_map = {
                 ast.Eq: '$eq',
                 ast.NotEq: '$ne',
                 ast.Lt: '$lt',
                 ast.LtE: '$lte',
                 ast.Gt: '$gt',
                 ast.GtE: '$gte',
+                ast.In: '$regex',
+                ast.NotIn: '$nin'
             }
             op = op_map[type(node.ops[0])]
-            return {left: {op: right}}
+            if op == '$regex':
+                return {left: {op: f'.*{right}.*'}}
+            elif isinstance(node, ast.Compare) and isinstance(node.ops[0], ast.NotIn):
+                left = self._transform(node.left)
+                #right = [self._transform(value) for value in node.comparators]
+                return {right: {'$not': {'$regex': '|'.join(left)}}}
+            elif isinstance(right, list):
+                return {left: {op: right}}
+            else:
+                return {left: {op: [right]}}
         elif isinstance(node, ast.Name):
             return node.id
         elif isinstance(node, ast.Str):
             return node.s
         elif isinstance(node, ast.Num):
             return node.n
         else:
```

### Comparing `Mongeasy-0.1.6/mongeasy/document.py` & `Mongeasy-0.1.7/mongeasy/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,14 +177,40 @@
             elif isinstance(value, datetime):
                 json_dict[key] = value.strftime('%Y-%m-%dT%H:%M:%S.%fZ')
             else:
                 json_dict[key] = value
         return json.dumps(json_dict)
 
     @classmethod
+    def raw_query(cls, query: Union[Dict, Query], *args, **kwargs) -> pymongo.cursor.Cursor:
+        """
+        Performs a raw query on the collection
+        :param query: The query to perform
+        :return: Cursor, the cursor to the query results
+        """
+        if isinstance(query, Query):
+            query = query.to_mongo_query()
+        if cls.collection is None:
+            raise MongeasyDBCollectionError('The collection does not exist')
+
+        return cls.collection.find(query, *args, **kwargs)
+
+    @classmethod
+    def raw_aggregate(cls, pipeline: List[Dict], *args, **kwargs) -> pymongo.cursor.Cursor:
+        """
+        Performs a raw aggregation on the collection
+        :param pipeline: The aggregation pipeline to perform
+        :return: Cursor, the cursor to the aggregation results
+        """
+        if cls.collection is None:
+            raise MongeasyDBCollectionError('The collection does not exist')
+
+        return cls.collection.aggregate(pipeline, *args, **kwargs)
+
+    @classmethod
     def create_index(cls, keys: List[str], index_type: str = 'asc', unique: bool = False, name: Union[str, None] = None) -> None:
         """
         Creates an index on the specified keys
         :param keys: The keys to index on
         :param index_type: The index type, either 'asc' (default) or 'desc'
         :param unique: Whether the index should be unique
         :param name: The name of the index
```

### Comparing `Mongeasy-0.1.6/mongeasy/dynamics.py` & `Mongeasy-0.1.7/mongeasy/dynamics.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.6/mongeasy/exceptions.py` & `Mongeasy-0.1.7/mongeasy/exceptions.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.6/mongeasy/resultlist.py` & `Mongeasy-0.1.7/mongeasy/resultlist.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.6/mongeasy/utils/utils.py` & `Mongeasy-0.1.7/mongeasy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.6/setup.cfg` & `Mongeasy-0.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f6e 6765 6173 790d 0a76 6572   = mongeasy..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e36 0d0a 6175  sion = 0.1.6..au
+00000020: 7369 6f6e 203d 2030 2e31 2e37 0d0a 6175  sion = 0.1.7..au
 00000030: 7468 6f72 203d 204a 6f61 6b69 6d20 5761  thor = Joakim Wa
 00000040: 7373 6265 7267 0d0a 6175 7468 6f72 5f65  ssberg..author_e
 00000050: 6d61 696c 203d 206a 6f61 6b69 6d2e 7761  mail = joakim.wa
 00000060: 7373 6265 7267 4061 7274 6865 6164 2e73  ssberg@arthead.s
 00000070: 650d 0a64 6573 6372 6970 7469 6f6e 203d  e..description =
 00000080: 2045 6173 7920 746f 2075 7365 2077 7261   Easy to use wra
 00000090: 7070 6572 2061 726f 756e 6420 7079 6d6f  pper around pymo
```

### Comparing `Mongeasy-0.1.6/setup.py` & `Mongeasy-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     readme = f.read()
 
 with open("LICENSE", encoding="utf8") as f:
     license = f.read()
 
 setup(
     name="Mongeasy",
-    version="0.1.6",
+    version="0.1.7",
     author="Joakim Wassberg",
     author_email="joakim.wassberg@arthead.se",
     description="Easy to use wrapper around pymongo for easy access to MongoDB.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/artheadsweden/mongeasy",
     license="MIT",
```

### Comparing `Mongeasy-0.1.6/tests/test_mongeasy.py` & `Mongeasy-0.1.7/tests/test_mongeasy.py`

 * *Files identical despite different names*

