# Comparing `tmp/tencentcloud-sdk-python-apm-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-apm-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apm-3.0.878.tar", last modified: Thu Apr 20 00:18:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apm-3.0.879.tar", last modified: Fri Apr 21 00:28:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apm-3.0.878.tar` & `tencentcloud-sdk-python-apm-3.0.879.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/tencentcloud/apm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/tencentcloud/apm/v20210622/
--rw-r--r--   0 root         (0) root         (0)     3561 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/tencentcloud/apm/v20210622/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     8295 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/tencentcloud/apm/v20210622/apm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/tencentcloud/apm/v20210622/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43088 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/tencentcloud/apm/v20210622/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/tencentcloud/apm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/tencentcloud_sdk_python_apm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/tencentcloud_sdk_python_apm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/tencentcloud_sdk_python_apm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/tencentcloud_sdk_python_apm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/tencentcloud_sdk_python_apm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:18:23.000000 tencentcloud-sdk-python-apm-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:18:24.000000 tencentcloud-sdk-python-apm-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/tencentcloud/apm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/tencentcloud/apm/v20210622/
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/tencentcloud/apm/v20210622/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     8295 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/tencentcloud/apm/v20210622/apm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/tencentcloud/apm/v20210622/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43549 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/tencentcloud/apm/v20210622/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/tencentcloud/apm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/tencentcloud_sdk_python_apm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/tencentcloud_sdk_python_apm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/tencentcloud_sdk_python_apm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/tencentcloud_sdk_python_apm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/tencentcloud_sdk_python_apm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:28:22.000000 tencentcloud-sdk-python-apm-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-apm-3.0.878/README.rst` & `tencentcloud-sdk-python-apm-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apm-3.0.878/tencentcloud/apm/v20210622/errorcodes.py` & `tencentcloud-sdk-python-apm-3.0.879/tencentcloud/apm/v20210622/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apm-3.0.878/tencentcloud/apm/v20210622/apm_client.py` & `tencentcloud-sdk-python-apm-3.0.879/tencentcloud/apm/v20210622/apm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apm-3.0.878/tencentcloud/apm/v20210622/models.py` & `tencentcloud-sdk-python-apm-3.0.879/tencentcloud/apm/v20210622/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,20 @@
         :type LogTopicID: str
         :param ClientCount: 该实例已上报的客户端应用数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type ClientCount: int
         :param TotalCount: 该实例已上报的总应用数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type TotalCount: int
+        :param LogSet: CLS日志集 | ES集群ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LogSet: str
+        :param MetricDuration: Metric数据保存时长
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MetricDuration: int
         """
         self.AmountOfUsedStorage = None
         self.Name = None
         self.Tags = None
         self.InstanceId = None
         self.CreateUin = None
         self.ServiceCount = None
@@ -285,14 +291,16 @@
         self.SlowRequestSavedThreshold = None
         self.LogRegion = None
         self.LogSource = None
         self.IsRelatedLog = None
         self.LogTopicID = None
         self.ClientCount = None
         self.TotalCount = None
+        self.LogSet = None
+        self.MetricDuration = None
 
 
     def _deserialize(self, params):
         self.AmountOfUsedStorage = params.get("AmountOfUsedStorage")
         self.Name = params.get("Name")
         if params.get("Tags") is not None:
             self.Tags = []
@@ -317,14 +325,16 @@
         self.SlowRequestSavedThreshold = params.get("SlowRequestSavedThreshold")
         self.LogRegion = params.get("LogRegion")
         self.LogSource = params.get("LogSource")
         self.IsRelatedLog = params.get("IsRelatedLog")
         self.LogTopicID = params.get("LogTopicID")
         self.ClientCount = params.get("ClientCount")
         self.TotalCount = params.get("TotalCount")
+        self.LogSet = params.get("LogSet")
+        self.MetricDuration = params.get("MetricDuration")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-apm-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apm-3.0.879/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-apm-3.0.878/tencentcloud_sdk_python_apm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apm-3.0.879/tencentcloud_sdk_python_apm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apm
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Apm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apm-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-apm-3.0.879/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apm
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Apm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apm-3.0.878/setup.py` & `tencentcloud-sdk-python-apm-3.0.879/setup.py`

 * *Files identical despite different names*

