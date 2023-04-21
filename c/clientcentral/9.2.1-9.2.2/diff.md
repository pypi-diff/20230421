# Comparing `tmp/clientcentral-9.2.1.tar.gz` & `tmp/clientcentral-9.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clientcentral-9.2.1.tar", last modified: Wed Apr 15 13:41:52 2020, max compression
+gzip compressed data, was "dist/clientcentral-9.2.2.tar", last modified: Wed Apr 15 13:49:47 2020, max compression
```

## Comparing `clientcentral-9.2.1.tar` & `clientcentral-9.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 13:41:52.308857 clientcentral-9.2.1/
--rw-r--r--   0 root         (0) root         (0)     6956 2020-04-15 13:41:52.308857 clientcentral-9.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5221 2020-04-15 13:41:46.000000 clientcentral-9.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 13:41:52.304857 clientcentral-9.2.1/clientcentral/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/Exceptions.py
--rw-r--r--   0 root         (0) root         (0)      167 2020-04-15 13:41:46.000000 clientcentral-9.2.1/clientcentral/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6160 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/clientcentral.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 13:41:52.308857 clientcentral-9.2.1/clientcentral/model/
--rw-rw-rw-   0 root         (0) root         (0)      524 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/model/Button.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/model/Change.py
--rw-rw-rw-   0 root         (0) root         (0)     1061 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/model/ChangeEvent.py
--rw-rw-rw-   0 root         (0) root         (0)      610 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/model/Comment.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/model/Role.py
--rw-rw-rw-   0 root         (0) root         (0)      323 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/model/Status.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/model/TicketEvent.py
--rw-rw-rw-   0 root         (0) root         (0)      212 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/model/TicketType.py
--rw-rw-rw-   0 root         (0) root         (0)     1065 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/model/User.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9387 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/query.py
--rw-rw-rw-   0 root         (0) root         (0)     3716 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/roles.py
--rw-rw-rw-   0 root         (0) root         (0)    29132 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/ticket.py
--rw-rw-rw-   0 root         (0) root         (0)     1231 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/ticketformatting.py
--rw-rw-rw-   0 root         (0) root         (0)     3800 2020-04-15 13:34:36.000000 clientcentral-9.2.1/clientcentral/users_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 13:41:52.308857 clientcentral-9.2.1/clientcentral.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6956 2020-04-15 13:41:52.000000 clientcentral-9.2.1/clientcentral.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      880 2020-04-15 13:41:52.000000 clientcentral-9.2.1/clientcentral.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-04-15 13:41:52.000000 clientcentral-9.2.1/clientcentral.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2020-04-15 13:41:52.000000 clientcentral-9.2.1/clientcentral.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-04-15 13:41:52.000000 clientcentral-9.2.1/clientcentral.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2020-04-15 13:41:52.000000 clientcentral-9.2.1/clientcentral.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2020-04-15 13:41:52.000000 clientcentral-9.2.1/clientcentral.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      944 2020-04-15 13:41:52.308857 clientcentral-9.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1353 2020-04-15 13:41:46.000000 clientcentral-9.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 13:41:52.308857 clientcentral-9.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-15 13:34:36.000000 clientcentral-9.2.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15540 2020-04-15 13:34:36.000000 clientcentral-9.2.1/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)     6288 2020-04-15 13:34:36.000000 clientcentral-9.2.1/tests/test_async_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 13:49:47.557236 clientcentral-9.2.2/
+-rw-r--r--   0 root         (0) root         (0)     6956 2020-04-15 13:49:47.557236 clientcentral-9.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5221 2020-04-15 13:49:44.000000 clientcentral-9.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 13:49:47.553236 clientcentral-9.2.2/clientcentral/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/Exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      167 2020-04-15 13:49:44.000000 clientcentral-9.2.2/clientcentral/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6040 2020-04-15 13:47:14.000000 clientcentral-9.2.2/clientcentral/clientcentral.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 13:49:47.557236 clientcentral-9.2.2/clientcentral/model/
+-rw-rw-rw-   0 root         (0) root         (0)      524 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/model/Button.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/model/Change.py
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/model/ChangeEvent.py
+-rw-rw-rw-   0 root         (0) root         (0)      610 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/model/Comment.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/model/Role.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/model/Status.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/model/TicketEvent.py
+-rw-rw-rw-   0 root         (0) root         (0)      212 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/model/TicketType.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/model/User.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9387 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     3716 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/roles.py
+-rw-rw-rw-   0 root         (0) root         (0)    29132 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1231 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/ticketformatting.py
+-rw-rw-rw-   0 root         (0) root         (0)     3800 2020-04-15 13:34:36.000000 clientcentral-9.2.2/clientcentral/users_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 13:49:47.553236 clientcentral-9.2.2/clientcentral.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6956 2020-04-15 13:49:47.000000 clientcentral-9.2.2/clientcentral.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      880 2020-04-15 13:49:47.000000 clientcentral-9.2.2/clientcentral.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-04-15 13:49:47.000000 clientcentral-9.2.2/clientcentral.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2020-04-15 13:49:47.000000 clientcentral-9.2.2/clientcentral.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-04-15 13:49:47.000000 clientcentral-9.2.2/clientcentral.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2020-04-15 13:49:47.000000 clientcentral-9.2.2/clientcentral.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2020-04-15 13:49:47.000000 clientcentral-9.2.2/clientcentral.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      944 2020-04-15 13:49:47.557236 clientcentral-9.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1353 2020-04-15 13:49:44.000000 clientcentral-9.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 13:49:47.557236 clientcentral-9.2.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-15 13:34:36.000000 clientcentral-9.2.2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15540 2020-04-15 13:34:36.000000 clientcentral-9.2.2/tests/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     6288 2020-04-15 13:34:36.000000 clientcentral-9.2.2/tests/test_async_api.py
```

### Comparing `clientcentral-9.2.1/PKG-INFO` & `clientcentral-9.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: clientcentral
-Version: 9.2.1
+Version: 9.2.2
 Summary: Client Central Python API.
 Home-page: https://github.com/EPI-USE-Labs/client-central-python-api
 Author: Thomas Scholtz
 Author-email: thomas@labs.epiuse.com
 License: UNKNOWN
 Description: # clientcentral-api-python
-        [![version](https://img.shields.io/badge/version-9.2.1-green.svg)]()
+        [![version](https://img.shields.io/badge/version-9.2.2-green.svg)]()
         [![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
         [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
         
         # Install
         ```bash
         pip install clientcentral --user
         ```
         # Upgrading
         ```bash
         pip install --user --upgrade clientcentral
         ```
         
         A specific version can also be installed by adding the tag:
         ```bash
-        pip install --user --upgrade clientcentral==9.2.1
+        pip install --user --upgrade clientcentral==9.2.2
         ```
         
         # Requirements
         This library was built and tested on `Python 3.7.4` a minimal Python version of `Python 3.6.x` is required.
         
         `Python 2` is not supported.
```

### Comparing `clientcentral-9.2.1/README.md` & `clientcentral-9.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # clientcentral-api-python
-[![version](https://img.shields.io/badge/version-9.2.1-green.svg)]()
+[![version](https://img.shields.io/badge/version-9.2.2-green.svg)]()
 [![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
 
 # Install
 ```bash
 pip install clientcentral --user
 ```
 # Upgrading
 ```bash
 pip install --user --upgrade clientcentral
 ```
 
 A specific version can also be installed by adding the tag:
 ```bash
-pip install --user --upgrade clientcentral==9.2.1
+pip install --user --upgrade clientcentral==9.2.2
 ```
 
 # Requirements
 This library was built and tested on `Python 3.7.4` a minimal Python version of `Python 3.6.x` is required.
 
 `Python 2` is not supported.
```

### Comparing `clientcentral-9.2.1/clientcentral/Exceptions.py` & `clientcentral-9.2.2/clientcentral/Exceptions.py`

 * *Files identical despite different names*

### Comparing `clientcentral-9.2.1/clientcentral/clientcentral.py` & `clientcentral-9.2.2/clientcentral/clientcentral.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,27 +39,24 @@
 
         if not self.base_url:
             self.base_url = "https://qa-cc.labs.epiuse.com"
             if production:
                 self.base_url = "https://clientcentral.io"
 
         # Get the token from the environment
-
-        p = re.compile(r'^(?:[A-Za-z0-9+/]{4})*(?:[A-Za-z0-9+/]{2}==|[A-Za-z0-9+/]{3}=)?$')
-
         raw_token = None
 
         if os.environ.get("CC_TOKEN"):
             raw_token = str(os.environ.get("CC_TOKEN"))
 
         if token:
             raw_token = token
             self.token = "token=" + raw_token
 
-        if not raw_token or not len(raw_token) == 32 or not p.match(raw_token):
+        if not raw_token or not len(raw_token) == 32:
             raise NoTokenProvided("Token invalid or not present")
 
         self.token ="token=" + raw_token
 
         self.run_async = run_async
         self._event_loop = self._get_event_loop()
         future = asyncio.ensure_future(self._create_session(), loop=self._event_loop)
```

### Comparing `clientcentral-9.2.1/clientcentral/model/Button.py` & `clientcentral-9.2.2/clientcentral/model/Button.py`

 * *Files identical despite different names*

### Comparing `clientcentral-9.2.1/clientcentral/model/ChangeEvent.py` & `clientcentral-9.2.2/clientcentral/model/ChangeEvent.py`

 * *Files identical despite different names*

### Comparing `clientcentral-9.2.1/clientcentral/model/Comment.py` & `clientcentral-9.2.2/clientcentral/model/Comment.py`

 * *Files identical despite different names*

### Comparing `clientcentral-9.2.1/clientcentral/model/TicketEvent.py` & `clientcentral-9.2.2/clientcentral/model/TicketEvent.py`

 * *Files identical despite different names*

### Comparing `clientcentral-9.2.1/clientcentral/model/User.py` & `clientcentral-9.2.2/clientcentral/model/User.py`

 * *Files identical despite different names*

### Comparing `clientcentral-9.2.1/clientcentral/query.py` & `clientcentral-9.2.2/clientcentral/query.py`

 * *Files identical despite different names*

### Comparing `clientcentral-9.2.1/clientcentral/roles.py` & `clientcentral-9.2.2/clientcentral/roles.py`

 * *Files identical despite different names*

### Comparing `clientcentral-9.2.1/clientcentral/ticket.py` & `clientcentral-9.2.2/clientcentral/ticket.py`

 * *Files identical despite different names*

### Comparing `clientcentral-9.2.1/clientcentral/ticketformatting.py` & `clientcentral-9.2.2/clientcentral/ticketformatting.py`

 * *Files identical despite different names*

### Comparing `clientcentral-9.2.1/clientcentral/users_client.py` & `clientcentral-9.2.2/clientcentral/users_client.py`

 * *Files identical despite different names*

### Comparing `clientcentral-9.2.1/clientcentral.egg-info/PKG-INFO` & `clientcentral-9.2.2/clientcentral.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: clientcentral
-Version: 9.2.1
+Version: 9.2.2
 Summary: Client Central Python API.
 Home-page: https://github.com/EPI-USE-Labs/client-central-python-api
 Author: Thomas Scholtz
 Author-email: thomas@labs.epiuse.com
 License: UNKNOWN
 Description: # clientcentral-api-python
-        [![version](https://img.shields.io/badge/version-9.2.1-green.svg)]()
+        [![version](https://img.shields.io/badge/version-9.2.2-green.svg)]()
         [![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
         [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
         
         # Install
         ```bash
         pip install clientcentral --user
         ```
         # Upgrading
         ```bash
         pip install --user --upgrade clientcentral
         ```
         
         A specific version can also be installed by adding the tag:
         ```bash
-        pip install --user --upgrade clientcentral==9.2.1
+        pip install --user --upgrade clientcentral==9.2.2
         ```
         
         # Requirements
         This library was built and tested on `Python 3.7.4` a minimal Python version of `Python 3.6.x` is required.
         
         `Python 2` is not supported.
```

### Comparing `clientcentral-9.2.1/clientcentral.egg-info/SOURCES.txt` & `clientcentral-9.2.2/clientcentral.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clientcentral-9.2.1/setup.cfg` & `clientcentral-9.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 9.2.1
+current_version = 9.2.2
 commit = True
 tag = False
 message = 'Bump Version: {current_version} → {new_version} [skip-ci]'
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `clientcentral-9.2.1/setup.py` & `clientcentral-9.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,12 +38,12 @@
     keywords=['ClientCentral', 'Client', 'EPI-USE Labs', 'EPI-USE', 'Client-Central'],
     name='clientcentral',
     packages=find_packages(),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/EPI-USE-Labs/client-central-python-api',
-    version='9.2.1',
+    version='9.2.2',
     zip_safe=False,
     data_files=[('.', [])],
     python_requires='>=3.6'
 )
```

### Comparing `clientcentral-9.2.1/tests/test_api.py` & `clientcentral-9.2.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `clientcentral-9.2.1/tests/test_async_api.py` & `clientcentral-9.2.2/tests/test_async_api.py`

 * *Files identical despite different names*

