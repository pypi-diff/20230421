# Comparing `tmp/tencentcloud-sdk-python-es-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-es-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-es-3.0.878.tar", last modified: Thu Apr 20 00:28:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-es-3.0.879.tar", last modified: Fri Apr 21 00:44:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-es-3.0.878.tar` & `tencentcloud-sdk-python-es-3.0.879.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      734 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/tencentcloud/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/tencentcloud/es/v20180416/
--rw-r--r--   0 root         (0) root         (0)    35037 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/tencentcloud/es/v20180416/es_client.py
--rw-r--r--   0 root         (0) root         (0)     3332 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/tencentcloud/es/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/tencentcloud/es/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   177567 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/tencentcloud/es/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/tencentcloud/es/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/tencentcloud_sdk_python_es.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/tencentcloud_sdk_python_es.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/tencentcloud_sdk_python_es.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/tencentcloud_sdk_python_es.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/tencentcloud_sdk_python_es.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1004 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:28:33.000000 tencentcloud-sdk-python-es-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/
+-rw-r--r--   0 root         (0) root         (0)      734 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/tencentcloud/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/tencentcloud/es/v20180416/
+-rw-r--r--   0 root         (0) root         (0)    35037 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/tencentcloud/es/v20180416/es_client.py
+-rw-r--r--   0 root         (0) root         (0)     3332 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/tencentcloud/es/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/tencentcloud/es/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   177567 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/tencentcloud/es/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/tencentcloud/es/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/tencentcloud_sdk_python_es.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/tencentcloud_sdk_python_es.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/tencentcloud_sdk_python_es.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/tencentcloud_sdk_python_es.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/tencentcloud_sdk_python_es.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:44:35.000000 tencentcloud-sdk-python-es-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-es-3.0.878/README.rst` & `tencentcloud-sdk-python-es-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.878/tencentcloud/es/v20180416/es_client.py` & `tencentcloud-sdk-python-es-3.0.879/tencentcloud/es/v20180416/es_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.878/tencentcloud/es/v20180416/errorcodes.py` & `tencentcloud-sdk-python-es-3.0.879/tencentcloud/es/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.878/tencentcloud/es/v20180416/models.py` & `tencentcloud-sdk-python-es-3.0.879/tencentcloud/es/v20180416/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-es-3.0.879/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.878'
+__version__ = '3.0.879'
```

### Comparing `tencentcloud-sdk-python-es-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-es-3.0.879/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-es
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Es SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-es-3.0.878/tencentcloud_sdk_python_es.egg-info/PKG-INFO` & `tencentcloud-sdk-python-es-3.0.879/tencentcloud_sdk_python_es.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-es
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Es SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-es-3.0.878/setup.py` & `tencentcloud-sdk-python-es-3.0.879/setup.py`

 * *Files identical despite different names*

