# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.878.tar", last modified: Thu Apr 20 00:55:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.879.tar", last modified: Fri Apr 21 01:09:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.878.tar` & `tencentcloud-sdk-python-vpc-3.0.879.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:55:58.000000 tencentcloud-sdk-python-vpc-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   327723 2023-04-20 00:55:58.000000 tencentcloud-sdk-python-vpc-3.0.878/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    40141 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   834270 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:55:58.000000 tencentcloud-sdk-python-vpc-3.0.878/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:55:58.000000 tencentcloud-sdk-python-vpc-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:55:59.000000 tencentcloud-sdk-python-vpc-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   327723 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    40141 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   834744 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:09:32.000000 tencentcloud-sdk-python-vpc-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.878/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.879/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.878/README.rst` & `tencentcloud-sdk-python-vpc-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.878/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.878/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.878/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,14 +355,20 @@
 <li><strong>BANDWIDTH_PACKAGE</strong></li>
 <p style="padding-left: 30px;">表示共享带宽包。</p>
 注意：此字段可能返回 null，表示取不到有效值。
         :type InternetChargeType: str
         :param TagSet: 弹性公网IP关联的标签列表。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TagSet: list of Tag
+        :param DeadlineDate: 到期时间。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeadlineDate: str
+        :param InstanceType: EIP绑定的实例类型。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceType: str
         """
         self.AddressId = None
         self.AddressName = None
         self.AddressStatus = None
         self.AddressIp = None
         self.InstanceId = None
         self.CreatedTime = None
@@ -375,14 +381,16 @@
         self.CascadeRelease = None
         self.EipAlgType = None
         self.InternetServiceProvider = None
         self.LocalBgp = None
         self.Bandwidth = None
         self.InternetChargeType = None
         self.TagSet = None
+        self.DeadlineDate = None
+        self.InstanceType = None
 
 
     def _deserialize(self, params):
         self.AddressId = params.get("AddressId")
         self.AddressName = params.get("AddressName")
         self.AddressStatus = params.get("AddressStatus")
         self.AddressIp = params.get("AddressIp")
@@ -404,14 +412,16 @@
         self.InternetChargeType = params.get("InternetChargeType")
         if params.get("TagSet") is not None:
             self.TagSet = []
             for item in params.get("TagSet"):
                 obj = Tag()
                 obj._deserialize(item)
                 self.TagSet.append(obj)
+        self.DeadlineDate = params.get("DeadlineDate")
+        self.InstanceType = params.get("InstanceType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.879/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.879/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.878/setup.py` & `tencentcloud-sdk-python-vpc-3.0.879/setup.py`

 * *Files identical despite different names*

