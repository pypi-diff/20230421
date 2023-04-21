# Comparing `tmp/macrometa-source-mongo-0.0.33.tar.gz` & `tmp/macrometa-source-mongo-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mongo-0.0.33.tar", max compression
+gzip compressed data, was "macrometa-source-mongo-0.0.34.tar", max compression
```

## Comparing `macrometa-source-mongo-0.0.33.tar` & `macrometa-source-mongo-0.0.34.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10765 2023-04-17 09:51:24.291643 macrometa-source-mongo-0.0.33/LICENSE
--rw-r--r--   0        0        0    21337 2023-04-17 09:51:24.291643 macrometa-source-mongo-0.0.33/macrometa_source_mongo/__init__.py
--rw-r--r--   0        0        0     6470 2023-04-17 09:51:24.291643 macrometa-source-mongo-0.0.33/macrometa_source_mongo/connection.py
--rw-r--r--   0        0        0     1151 2023-04-17 09:51:24.291643 macrometa-source-mongo-0.0.33/macrometa_source_mongo/exceptions.py
--rw-r--r--   0        0        0     8097 2023-04-17 09:51:24.291643 macrometa-source-mongo-0.0.33/macrometa_source_mongo/helper.py
--rw-r--r--   0        0        0    10251 2023-04-17 09:51:24.291643 macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/common.py
--rw-r--r--   0        0        0     3647 2023-04-17 09:51:24.295642 macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/full_table.py
--rw-r--r--   0        0        0     6267 2023-04-17 09:51:24.295642 macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/log_based.py
--rw-r--r--   0        0        0     2292 2023-04-17 09:51:24.295642 macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1548 2023-04-17 09:51:24.531543 macrometa-source-mongo-0.0.33/pyproject.toml
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.33/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.33/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-04-21 07:14:10.411421 macrometa-source-mongo-0.0.34/LICENSE
+-rw-r--r--   0        0        0    21337 2023-04-21 07:14:10.411421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/__init__.py
+-rw-r--r--   0        0        0     6470 2023-04-21 07:14:10.411421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/connection.py
+-rw-r--r--   0        0        0     1151 2023-04-21 07:14:10.411421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/exceptions.py
+-rw-r--r--   0        0        0     8097 2023-04-21 07:14:10.411421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/helper.py
+-rw-r--r--   0        0        0    10251 2023-04-21 07:14:10.415421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/common.py
+-rw-r--r--   0        0        0     3647 2023-04-21 07:14:10.415421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/full_table.py
+-rw-r--r--   0        0        0     6267 2023-04-21 07:14:10.415421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     2292 2023-04-21 07:14:10.415421 macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1548 2023-04-21 07:14:10.699438 macrometa-source-mongo-0.0.34/pyproject.toml
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.34/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.34/PKG-INFO
```

### Comparing `macrometa-source-mongo-0.0.33/LICENSE` & `macrometa-source-mongo-0.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.33/macrometa_source_mongo/__init__.py` & `macrometa-source-mongo-0.0.34/macrometa_source_mongo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                            placeholder_value='mongodb_host'),
             ConfigProperty('port', 'Port', ConfigAttributeType.INT, True, False,
                            description='MongoDB port.',
                            default_value='27017'),
             ConfigProperty('user', 'Username', ConfigAttributeType.STRING, True, False,
                            description='MongoDB user.',
                            placeholder_value='mongo'),
-            ConfigProperty('password', 'Password', ConfigAttributeType.STRING, True, False,
+            ConfigProperty('password', 'Password', ConfigAttributeType.PASSWORD, True, False,
                            description='MongoDB password.',
                            placeholder_value='password'),
             ConfigProperty('auth_database', 'Auth Database', ConfigAttributeType.STRING, True, False,
                            description='MongoDB authentication database.',
                            default_value='admin'),
             ConfigProperty('database', 'Database', ConfigAttributeType.STRING, True, False,
                            description='MongoDB database name.',
@@ -175,23 +175,23 @@
                            description='[LOG_BASED] The maximum amount of time in milliseconds the log_based method '
                                        'waits for new data changes before exiting.',
                            default_value='900000'),
             ConfigProperty('direct_connection', 'Direct Connection', ConfigAttributeType.BOOLEAN, False, False,
                            description='Specifies whether to connect directly to the specified MongoDB host as a '
                                        'standalone or connect to the entire replica set of which the given MongoDB host is a part.',
                            default_value="false"),
-            ConfigProperty('tls_ca_file', 'SSL/TLS CA Certificate', ConfigAttributeType.STRING, False, False,
+            ConfigProperty('tls_ca_file', 'SSL/TLS CA Certificate', ConfigAttributeType.FILE, False, False,
                            description='Specific CA certificate in PEM string format. This is most often the case '
                                        'when using `self-signed` server certificate.',
                            placeholder_value="my_ca_certificate"),
-            ConfigProperty('tls_certificate_key_file', 'SSL/TLS Client Certificate', ConfigAttributeType.STRING, False, False,
+            ConfigProperty('tls_certificate_key_file', 'SSL/TLS Client Certificate', ConfigAttributeType.FILE, False, False,
                            description='Specific client certificate in PEM string format. If the private key for the client '
                                        'certificate is stored in a separate file, it should be concatenated with the certificate file.',
                            placeholder_value="my_client_certificate"),
-            ConfigProperty('tls_certificate_key_file_password', 'SSL/TLS Client Key Password', ConfigAttributeType.STRING, False, False,
+            ConfigProperty('tls_certificate_key_file_password', 'SSL/TLS Client Key Password', ConfigAttributeType.PASSWORD, False, False,
                            description='If the private key contained in the certificate keyfile is encrypted, users can provide a '
                                        'password or passphrase to decrypt the encrypted private keys.',
                            placeholder_value="my_client_key_password"),
         ]
 
     def capabilities(self) -> list[str]:
         """Return the capabilities[1] of the connector.
```

### Comparing `macrometa-source-mongo-0.0.33/macrometa_source_mongo/connection.py` & `macrometa-source-mongo-0.0.34/macrometa_source_mongo/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.33/macrometa_source_mongo/exceptions.py` & `macrometa-source-mongo-0.0.34/macrometa_source_mongo/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.33/macrometa_source_mongo/helper.py` & `macrometa-source-mongo-0.0.34/macrometa_source_mongo/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/common.py` & `macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/full_table.py` & `macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/log_based.py` & `macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/sample_data.py` & `macrometa-source-mongo-0.0.34/macrometa_source_mongo/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.33/pyproject.toml` & `macrometa-source-mongo-0.0.34/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mongo"
-version='0.0.33'
+version='0.0.34'
 description = "Macrometa Source for extracting data from MongoDB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mongo-0.0.33/setup.py` & `macrometa-source-mongo-0.0.34/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'tzlocal>=2.1.0,<2.2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mongo = macrometa_source_mongo:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mongo',
-    'version': '0.0.33',
+    'version': '0.0.34',
     'description': 'Macrometa Source for extracting data from MongoDB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mongo-0.0.33/PKG-INFO` & `macrometa-source-mongo-0.0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mongo
-Version: 0.0.33
+Version: 0.0.34
 Summary: Macrometa Source for extracting data from MongoDB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MongoDB,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

