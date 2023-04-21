# Comparing `tmp/skale-checks-1.0.dev8.tar.gz` & `tmp/skale-checks-1.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skale-checks-1.0.dev8.tar", last modified: Mon Apr  4 17:51:19 2022, max compression
+gzip compressed data, was "dist/skale-checks-1.0.dev9.tar", last modified: Wed Apr 13 12:00:14 2022, max compression
```

## Comparing `skale-checks-1.0.dev8.tar` & `skale-checks-1.0.dev9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 17:51:19.000000 skale-checks-1.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-04-04 17:51:19.000000 skale-checks-1.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-04-04 17:50:17.000000 skale-checks-1.0.dev8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-04 17:51:19.000000 skale-checks-1.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-04-04 17:51:19.000000 skale-checks-1.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 17:51:19.000000 skale-checks-1.0.dev8/skale_checks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-04 17:50:17.000000 skale-checks-1.0.dev8/skale_checks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 17:51:19.000000 skale-checks-1.0.dev8/skale_checks/adapters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-04 17:50:17.000000 skale-checks-1.0.dev8/skale_checks/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-04-04 17:50:17.000000 skale-checks-1.0.dev8/skale_checks/adapters/connectors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4797 2022-04-04 17:50:17.000000 skale-checks-1.0.dev8/skale_checks/adapters/watchdog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 17:51:19.000000 skale-checks-1.0.dev8/skale_checks/checks/
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-04-04 17:50:17.000000 skale-checks-1.0.dev8/skale_checks/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4117 2022-04-04 17:50:17.000000 skale-checks-1.0.dev8/skale_checks/checks/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4580 2022-04-04 17:50:17.000000 skale-checks-1.0.dev8/skale_checks/checks/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-04-04 17:50:17.000000 skale-checks-1.0.dev8/skale_checks/checks/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-04-04 17:50:17.000000 skale-checks-1.0.dev8/skale_checks/checks/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6271 2022-04-04 17:50:17.000000 skale-checks-1.0.dev8/skale_checks/checks/watchdog.py
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-04-04 17:50:17.000000 skale-checks-1.0.dev8/skale_checks/requirements.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 17:51:19.000000 skale-checks-1.0.dev8/skale_checks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-04-04 17:51:19.000000 skale-checks-1.0.dev8/skale_checks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-04-04 17:51:19.000000 skale-checks-1.0.dev8/skale_checks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-04 17:51:19.000000 skale-checks-1.0.dev8/skale_checks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-04-04 17:51:19.000000 skale-checks-1.0.dev8/skale_checks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-04 17:51:19.000000 skale-checks-1.0.dev8/skale_checks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 12:00:14.000000 skale-checks-1.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2022-04-13 12:00:14.000000 skale-checks-1.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-04-13 11:59:09.000000 skale-checks-1.0.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-13 12:00:14.000000 skale-checks-1.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-04-13 12:00:14.000000 skale-checks-1.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 12:00:14.000000 skale-checks-1.0.dev9/skale_checks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 11:59:09.000000 skale-checks-1.0.dev9/skale_checks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 12:00:14.000000 skale-checks-1.0.dev9/skale_checks/adapters/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 11:59:09.000000 skale-checks-1.0.dev9/skale_checks/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-04-13 11:59:09.000000 skale-checks-1.0.dev9/skale_checks/adapters/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4797 2022-04-13 11:59:09.000000 skale-checks-1.0.dev9/skale_checks/adapters/watchdog.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 12:00:14.000000 skale-checks-1.0.dev9/skale_checks/checks/
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2022-04-13 11:59:09.000000 skale-checks-1.0.dev9/skale_checks/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4179 2022-04-13 11:59:09.000000 skale-checks-1.0.dev9/skale_checks/checks/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4580 2022-04-13 11:59:09.000000 skale-checks-1.0.dev9/skale_checks/checks/node.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-04-13 11:59:09.000000 skale-checks-1.0.dev9/skale_checks/checks/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-04-13 11:59:09.000000 skale-checks-1.0.dev9/skale_checks/checks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6271 2022-04-13 11:59:09.000000 skale-checks-1.0.dev9/skale_checks/checks/watchdog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-04-13 11:59:09.000000 skale-checks-1.0.dev9/skale_checks/requirements.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 12:00:14.000000 skale-checks-1.0.dev9/skale_checks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2022-04-13 12:00:14.000000 skale-checks-1.0.dev9/skale_checks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      535 2022-04-13 12:00:14.000000 skale-checks-1.0.dev9/skale_checks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-13 12:00:14.000000 skale-checks-1.0.dev9/skale_checks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-04-13 12:00:14.000000 skale-checks-1.0.dev9/skale_checks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-13 12:00:14.000000 skale-checks-1.0.dev9/skale_checks.egg-info/top_level.txt
```

### Comparing `skale-checks-1.0.dev8/PKG-INFO` & `skale-checks-1.0.dev9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale-checks
-Version: 1.0.dev8
+Version: 1.0.dev9
 Summary: Checks for SKALE infrastructure
 Home-page: https://github.com/skalenetwork/skale-checks
 Author: SKALE Labs
 Author-email: support@skalelabs.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: skale,checks
```

### Comparing `skale-checks-1.0.dev8/README.md` & `skale-checks-1.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `skale-checks-1.0.dev8/setup.py` & `skale-checks-1.0.dev9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 extras_require['dev'] = (
     extras_require['linter'] + extras_require['dev']
 )
 
 setup(
     name='skale-checks',
-    version='1.0dev8',
+    version='1.0dev9',
     description='Checks for SKALE infrastructure',
     long_description_markdown_filename='README.md',
     author='SKALE Labs',
     author_email='support@skalelabs.com',
     url='https://github.com/skalenetwork/skale-checks',
     install_requires=[
         "skale.py == 5.7dev7",
```

### Comparing `skale-checks-1.0.dev8/skale_checks/adapters/connectors.py` & `skale-checks-1.0.dev9/skale_checks/adapters/connectors.py`

 * *Files identical despite different names*

### Comparing `skale-checks-1.0.dev8/skale_checks/adapters/watchdog.py` & `skale-checks-1.0.dev9/skale_checks/adapters/watchdog.py`

 * *Files identical despite different names*

### Comparing `skale-checks-1.0.dev8/skale_checks/checks/__init__.py` & `skale-checks-1.0.dev9/skale_checks/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `skale-checks-1.0.dev8/skale_checks/checks/base.py` & `skale-checks-1.0.dev9/skale_checks/checks/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,34 +16,37 @@
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import inspect
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from functools import wraps, partial
+from time import sleep
+
 from skale_checks.checks.types import ChecksDict, CheckStatus, Func, CheckRunners
 from skale_checks.checks.utils import get_requirements
 
 MAX_WORKERS = 3
 
 
 def check(result_headers) -> Func:
     def real_decorator(checker):
         checker.is_check = True
         checker.headers = result_headers
 
         @wraps(checker)
-        def wrapper(*args, retries=1, **kwargs) -> ChecksDict:
+        def wrapper(*args, retries=1, delay=0, **kwargs) -> ChecksDict:
             results = []
             for _ in range(retries):
                 results = checker(*args, **kwargs)
                 if not isinstance(results, tuple):
                     results = [results]
                 if None not in results:
                     break
+                sleep(delay)
             wrapped_results = [
                 CheckStatus.UNKNOWN if result is None else CheckStatus(result)
                 for result in results
             ]
             return dict(zip(result_headers, wrapped_results))
         return wrapper
     return real_decorator
```

### Comparing `skale-checks-1.0.dev8/skale_checks/checks/node.py` & `skale-checks-1.0.dev9/skale_checks/checks/node.py`

 * *Files identical despite different names*

### Comparing `skale-checks-1.0.dev8/skale_checks/checks/types.py` & `skale-checks-1.0.dev9/skale_checks/checks/types.py`

 * *Files identical despite different names*

### Comparing `skale-checks-1.0.dev8/skale_checks/checks/utils.py` & `skale-checks-1.0.dev9/skale_checks/checks/utils.py`

 * *Files identical despite different names*

### Comparing `skale-checks-1.0.dev8/skale_checks/checks/watchdog.py` & `skale-checks-1.0.dev9/skale_checks/checks/watchdog.py`

 * *Files identical despite different names*

### Comparing `skale-checks-1.0.dev8/skale_checks/requirements.yaml` & `skale-checks-1.0.dev9/skale_checks/requirements.yaml`

 * *Files identical despite different names*

### Comparing `skale-checks-1.0.dev8/skale_checks.egg-info/PKG-INFO` & `skale-checks-1.0.dev9/skale_checks.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale-checks
-Version: 1.0.dev8
+Version: 1.0.dev9
 Summary: Checks for SKALE infrastructure
 Home-page: https://github.com/skalenetwork/skale-checks
 Author: SKALE Labs
 Author-email: support@skalelabs.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: skale,checks
```

### Comparing `skale-checks-1.0.dev8/skale_checks.egg-info/SOURCES.txt` & `skale-checks-1.0.dev9/skale_checks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

