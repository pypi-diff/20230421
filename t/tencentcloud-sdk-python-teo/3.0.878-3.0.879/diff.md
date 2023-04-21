# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.878.tar", last modified: Thu Apr 20 00:49:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.879.tar", last modified: Fri Apr 21 01:03:04 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.878.tar` & `tencentcloud-sdk-python-teo-3.0.879.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)     2192 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24724 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)     5379 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)    21320 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   504803 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220901/models.py
--rw-r--r--   0 root         (0) root         (0)    81864 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/tencentcloud_sdk_python_teo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:49:35.000000 tencentcloud-sdk-python-teo-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24724 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)     5379 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)    21320 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   504807 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220901/models.py
+-rw-r--r--   0 root         (0) root         (0)    81864 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:03:04.000000 tencentcloud-sdk-python-teo-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-teo-3.0.878/README.rst` & `tencentcloud-sdk-python-teo-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220901/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5536,31 +5536,31 @@
     def __init__(self):
         r"""
         :param StartTime: 开始时间。
         :type StartTime: str
         :param EndTime: 结束时间。
         :type EndTime: str
         :param MetricName: 查询的指标，取值有：
-<li> l7Flow_outFlux_country：按国家维度统计流量指标；</li>
+<li> l7Flow_outFlux_country：按国家/地区维度统计流量指标；</li>
 <li> l7Flow_outFlux_statusCode：按状态码维度统计流量指标；</li>
 <li> l7Flow_outFlux_domain：按域名维度统计流量指标；</li>
 <li> l7Flow_outFlux_url：按URL维度统计流量指标; </li>
 <li> l7Flow_outFlux_resourceType：按资源类型维度统计流量指标；</li>
 <li> l7Flow_outFlux_sip：按客户端的源IP维度统计流量指标；</li>
 <li> l7Flow_outFlux_referers：按refer信息维度统计流量指标；</li>
 <li> l7Flow_outFlux_ua_device：按设备类型维度统计流量指标; </li>
 <li> l7Flow_outFlux_ua_browser：按浏览器类型维度统计流量指标；</li>
 <li> l7Flow_outFlux_us_os：按操作系统类型维度统计流量指标；</li>
-<li> l7Flow_request_country：按国家维度统计请求数指标；</li>
+<li> l7Flow_request_country：按国家/地区维度统计请求数指标；</li>
 <li> l7Flow_request_statusCode：按状态码维度统计请求数指标；</li>
 <li> l7Flow_request_domain：按域名维度统计请求数指标；</li>
 <li> l7Flow_request_url：按URL维度统计请求数指标; </li>
 <li> l7Flow_request_resourceType：按资源类型维度统计请求数指标；</li>
 <li> l7Flow_request_sip：按客户端的源IP维度统计请求数指标；</li>
-<li> l7Flow_request_refere请求的rs：按refer信息维度统计请求数指标；</li>
+<li> l7Flow_request_referer：按refer信息维度统计请求数指标；</li>
 <li> l7Flow_request_ua_device：按设备类型维度统计请求数指标; </li>
 <li> l7Flow_request_ua_browser：按浏览器类型维度统计请求数指标；</li>
 <li> l7Flow_request_us_os：按操作系统类型维度统计请求数指标。</li>
 
         :type MetricName: str
         :param ZoneIds: 站点集合，此参数必填，不填默认查询为空。
         :type ZoneIds: list of str
```

### Comparing `tencentcloud-sdk-python-teo-3.0.878/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.879/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.879/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.879/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.878/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.879/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.878/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.879/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.878/setup.py` & `tencentcloud-sdk-python-teo-3.0.879/setup.py`

 * *Files identical despite different names*

