# Comparing `tmp/tencentcloud-sdk-python-yunsou-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-yunsou-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-yunsou-3.0.878.tar", last modified: Thu Apr 20 00:57:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-yunsou-3.0.879.tar", last modified: Fri Apr 21 01:10:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-yunsou-3.0.878.tar` & `tencentcloud-sdk-python-yunsou-3.0.879.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      746 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20191115/
--rw-r--r--   0 root         (0) root         (0)     2733 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20191115/yunsou_client.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20191115/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20191115/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13973 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20191115/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20180504/
--rw-r--r--   0 root         (0) root         (0)     2727 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20180504/yunsou_client.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20180504/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20180504/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7381 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20180504/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud_sdk_python_yunsou.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud_sdk_python_yunsou.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      648 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud_sdk_python_yunsou.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud_sdk_python_yunsou.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud_sdk_python_yunsou.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:57:03.000000 tencentcloud-sdk-python-yunsou-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:10:46.000000 tencentcloud-sdk-python-yunsou-3.0.879/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-04-21 01:10:45.000000 tencentcloud-sdk-python-yunsou-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:10:46.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:10:46.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:10:46.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20191115/
+-rw-r--r--   0 root         (0) root         (0)     2733 2023-04-21 01:10:45.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20191115/yunsou_client.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-04-21 01:10:45.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20191115/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:10:45.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20191115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13973 2023-04-21 01:10:45.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20191115/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:10:46.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20180504/
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-04-21 01:10:45.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20180504/yunsou_client.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-04-21 01:10:45.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20180504/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:10:45.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20180504/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-04-21 01:10:45.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20180504/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:10:45.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:10:45.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:10:46.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud_sdk_python_yunsou.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:10:46.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud_sdk_python_yunsou.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      648 2023-04-21 01:10:46.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud_sdk_python_yunsou.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-21 01:10:46.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud_sdk_python_yunsou.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:10:46.000000 tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud_sdk_python_yunsou.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-21 01:10:46.000000 tencentcloud-sdk-python-yunsou-3.0.879/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-21 01:10:45.000000 tencentcloud-sdk-python-yunsou-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:10:46.000000 tencentcloud-sdk-python-yunsou-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-yunsou-3.0.878/README.rst` & `tencentcloud-sdk-python-yunsou-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20191115/yunsou_client.py` & `tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20191115/yunsou_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20191115/errorcodes.py` & `tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20191115/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20191115/models.py` & `tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20191115/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20180504/yunsou_client.py` & `tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20180504/yunsou_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20180504/errorcodes.py` & `tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20180504/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/yunsou/v20180504/models.py` & `tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/yunsou/v20180504/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud_sdk_python_yunsou.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud_sdk_python_yunsou.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yunsou-3.0.878/tencentcloud_sdk_python_yunsou.egg-info/PKG-INFO` & `tencentcloud-sdk-python-yunsou-3.0.879/tencentcloud_sdk_python_yunsou.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yunsou
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Yunsou SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yunsou-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-yunsou-3.0.879/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yunsou
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Yunsou SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yunsou-3.0.878/setup.py` & `tencentcloud-sdk-python-yunsou-3.0.879/setup.py`

 * *Files identical despite different names*

