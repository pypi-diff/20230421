# Comparing `tmp/tencentcloud-sdk-python-ssl-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-ssl-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.878.tar", last modified: Thu Apr 20 00:41:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.879.tar", last modified: Fri Apr 21 00:59:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssl-3.0.878.tar` & `tencentcloud-sdk-python-ssl-3.0.879.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/tencentcloud/ssl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/tencentcloud/ssl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/tencentcloud/ssl/v20191205/
--rw-r--r--   0 root         (0) root         (0)     6749 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/tencentcloud/ssl/v20191205/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/tencentcloud/ssl/v20191205/__init__.py
--rw-r--r--   0 root         (0) root         (0)   130814 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/tencentcloud/ssl/v20191205/models.py
--rw-r--r--   0 root         (0) root         (0)    27702 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/tencentcloud/ssl/v20191205/ssl_client.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/tencentcloud_sdk_python_ssl.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:41:59.000000 tencentcloud-sdk-python-ssl-3.0.878/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/tencentcloud/ssl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/tencentcloud/ssl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/tencentcloud/ssl/v20191205/
+-rw-r--r--   0 root         (0) root         (0)     6749 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/tencentcloud/ssl/v20191205/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/tencentcloud/ssl/v20191205/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   132644 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/tencentcloud/ssl/v20191205/models.py
+-rw-r--r--   0 root         (0) root         (0)    28567 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/tencentcloud/ssl/v20191205/ssl_client.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/tencentcloud_sdk_python_ssl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:59:58.000000 tencentcloud-sdk-python-ssl-3.0.879/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.878/README.rst` & `tencentcloud-sdk-python-ssl-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssl-3.0.879/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssl-3.0.878/tencentcloud/ssl/v20191205/errorcodes.py` & `tencentcloud-sdk-python-ssl-3.0.879/tencentcloud/ssl/v20191205/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.878/tencentcloud/ssl/v20191205/models.py` & `tencentcloud-sdk-python-ssl-3.0.879/tencentcloud/ssl/v20191205/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1493,14 +1493,76 @@
             for item in params.get("Certificates"):
                 obj = Certificates()
                 obj._deserialize(item)
                 self.Certificates.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeCompaniesRequest(AbstractModel):
+    """DescribeCompanies请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Offset: 分页偏移量
+        :type Offset: int
+        :param Limit: 分页每页限制数
+        :type Limit: int
+        :param CompanyId: 公司ID
+        :type CompanyId: int
+        """
+        self.Offset = None
+        self.Limit = None
+        self.CompanyId = None
+
+
+    def _deserialize(self, params):
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        self.CompanyId = params.get("CompanyId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeCompaniesResponse(AbstractModel):
+    """DescribeCompanies返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Companies: 公司列表
+        :type Companies: list of CompanyInfo
+        :param TotalCount: 公司总数
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Companies = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Companies") is not None:
+            self.Companies = []
+            for item in params.get("Companies"):
+                obj = CompanyInfo()
+                obj._deserialize(item)
+                self.Companies.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeDeployedResourcesRequest(AbstractModel):
     """DescribeDeployedResources请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.878/tencentcloud/ssl/v20191205/ssl_client.py` & `tencentcloud-sdk-python-ssl-3.0.879/tencentcloud/ssl/v20191205/ssl_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,14 +298,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeCompanies(self, request):
+        """查询公司列表
+
+        :param request: Request instance for DescribeCompanies.
+        :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeCompaniesRequest`
+        :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeCompaniesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeCompanies", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeCompaniesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeDeployedResources(self, request):
         """证书查询关联资源
 
         :param request: Request instance for DescribeDeployedResources.
         :type request: :class:`tencentcloud.ssl.v20191205.models.DescribeDeployedResourcesRequest`
         :rtype: :class:`tencentcloud.ssl.v20191205.models.DescribeDeployedResourcesResponse`
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.879/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.878/setup.py` & `tencentcloud-sdk-python-ssl-3.0.879/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.878/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.879/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

