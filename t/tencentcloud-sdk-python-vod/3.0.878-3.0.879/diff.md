# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.878.tar", last modified: Thu Apr 20 00:55:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.879.tar", last modified: Fri Apr 21 01:09:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.878.tar` & `tencentcloud-sdk-python-vod-3.0.879.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:51.000000 tencentcloud-sdk-python-vod-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:55:50.000000 tencentcloud-sdk-python-vod-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:51.000000 tencentcloud-sdk-python-vod-3.0.878/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:51.000000 tencentcloud-sdk-python-vod-3.0.878/tencentcloud/vod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:51.000000 tencentcloud-sdk-python-vod-3.0.878/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)   172410 2023-04-20 00:55:50.000000 tencentcloud-sdk-python-vod-3.0.878/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)    25016 2023-04-20 00:55:50.000000 tencentcloud-sdk-python-vod-3.0.878/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:55:50.000000 tencentcloud-sdk-python-vod-3.0.878/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1169017 2023-04-20 00:55:50.000000 tencentcloud-sdk-python-vod-3.0.878/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:55:50.000000 tencentcloud-sdk-python-vod-3.0.878/tencentcloud/vod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:55:50.000000 tencentcloud-sdk-python-vod-3.0.878/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:51.000000 tencentcloud-sdk-python-vod-3.0.878/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:55:51.000000 tencentcloud-sdk-python-vod-3.0.878/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:55:51.000000 tencentcloud-sdk-python-vod-3.0.878/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:55:50.000000 tencentcloud-sdk-python-vod-3.0.878/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:55:51.000000 tencentcloud-sdk-python-vod-3.0.878/tencentcloud_sdk_python_vod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:55:51.000000 tencentcloud-sdk-python-vod-3.0.878/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:55:50.000000 tencentcloud-sdk-python-vod-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:55:51.000000 tencentcloud-sdk-python-vod-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)   172410 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)    25016 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1170904 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud_sdk_python_vod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vod-3.0.878/README.rst` & `tencentcloud-sdk-python-vod-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.878/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/vod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.878/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.878/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12535,22 +12535,26 @@
         :type UrlSignatureAuthPolicy: :class:`tencentcloud.vod.v20180717.models.UrlSignatureAuthPolicy`
         :param RefererAuthPolicy: [Referer 防盗链](https://cloud.tencent.com/document/product/266/14046)配置信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type RefererAuthPolicy: :class:`tencentcloud.vod.v20180717.models.RefererAuthPolicy`
         :param CreateTime: 域名添加到腾讯云点播系统中的时间。
 <li>格式按照 ISO 8601标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#iso-.E6.97.A5.E6.9C.9F.E6.A0.BC.E5.BC.8F)。</li>
         :type CreateTime: str
+        :param QUICConfig: 域名 QUIC 配置信息。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type QUICConfig: :class:`tencentcloud.vod.v20180717.models.DomainQUICConfig`
         """
         self.Domain = None
         self.AccelerateAreaInfos = None
         self.DeployStatus = None
         self.HTTPSConfig = None
         self.UrlSignatureAuthPolicy = None
         self.RefererAuthPolicy = None
         self.CreateTime = None
+        self.QUICConfig = None
 
 
     def _deserialize(self, params):
         self.Domain = params.get("Domain")
         if params.get("AccelerateAreaInfos") is not None:
             self.AccelerateAreaInfos = []
             for item in params.get("AccelerateAreaInfos"):
@@ -12564,14 +12568,17 @@
         if params.get("UrlSignatureAuthPolicy") is not None:
             self.UrlSignatureAuthPolicy = UrlSignatureAuthPolicy()
             self.UrlSignatureAuthPolicy._deserialize(params.get("UrlSignatureAuthPolicy"))
         if params.get("RefererAuthPolicy") is not None:
             self.RefererAuthPolicy = RefererAuthPolicy()
             self.RefererAuthPolicy._deserialize(params.get("RefererAuthPolicy"))
         self.CreateTime = params.get("CreateTime")
+        if params.get("QUICConfig") is not None:
+            self.QUICConfig = DomainQUICConfig()
+            self.QUICConfig._deserialize(params.get("QUICConfig"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -12598,14 +12605,40 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DomainQUICConfig(AbstractModel):
+    """域名 QUIC 配置信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Status: QUIC 配置状态，可选值：
+<li>Enabled: 启用；</li>
+<li>Disabled: 禁用。</li>
+        :type Status: str
+        """
+        self.Status = None
+
+
+    def _deserialize(self, params):
+        self.Status = params.get("Status")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DrmStreamingsInfo(AbstractModel):
     """DRM 自适应码流播放信息
 
     """
 
     def __init__(self):
         r"""
@@ -19453,30 +19486,36 @@
         :type Domain: str
         :param SubAppId: <b>点播[子应用](/document/product/266/14574) ID。如果要访问子应用中的资源，则将该字段填写为子应用 ID；否则无需填写该字段。</b>
         :type SubAppId: int
         :param RefererAuthPolicy: [Referer 防盗链](/document/product/266/14046)规则。
         :type RefererAuthPolicy: :class:`tencentcloud.vod.v20180717.models.RefererAuthPolicy`
         :param UrlSignatureAuthPolicy: [Key 防盗链](/document/product/266/14047)规则。
         :type UrlSignatureAuthPolicy: :class:`tencentcloud.vod.v20180717.models.UrlSignatureAuthPolicy`
+        :param QUICConfig: QUIC 配置。
+        :type QUICConfig: :class:`tencentcloud.vod.v20180717.models.DomainQUICConfig`
         """
         self.Domain = None
         self.SubAppId = None
         self.RefererAuthPolicy = None
         self.UrlSignatureAuthPolicy = None
+        self.QUICConfig = None
 
 
     def _deserialize(self, params):
         self.Domain = params.get("Domain")
         self.SubAppId = params.get("SubAppId")
         if params.get("RefererAuthPolicy") is not None:
             self.RefererAuthPolicy = RefererAuthPolicy()
             self.RefererAuthPolicy._deserialize(params.get("RefererAuthPolicy"))
         if params.get("UrlSignatureAuthPolicy") is not None:
             self.UrlSignatureAuthPolicy = UrlSignatureAuthPolicy()
             self.UrlSignatureAuthPolicy._deserialize(params.get("UrlSignatureAuthPolicy"))
+        if params.get("QUICConfig") is not None:
+            self.QUICConfig = DomainQUICConfig()
+            self.QUICConfig._deserialize(params.get("QUICConfig"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -23323,25 +23362,37 @@
 class RemoveWaterMarkTaskOutput(AbstractModel):
     """智能去除水印任务的输出。
 
     """
 
     def __init__(self):
         r"""
-        :param FileId: 视频 ID。
+        :param FileId: 媒体文件 ID。
         :type FileId: str
+        :param FileType: 文件类型，例如 mp4、mp3 等。
+        :type FileType: str
+        :param FileUrl: 媒体文件播放地址。
+        :type FileUrl: str
+        :param MediaName: 文件名称，最长 64 个字符。
+        :type MediaName: str
         :param MetaData: 元信息。包括大小、时长、视频流信息、音频流信息等。
         :type MetaData: :class:`tencentcloud.vod.v20180717.models.MediaMetaData`
         """
         self.FileId = None
+        self.FileType = None
+        self.FileUrl = None
+        self.MediaName = None
         self.MetaData = None
 
 
     def _deserialize(self, params):
         self.FileId = params.get("FileId")
+        self.FileType = params.get("FileType")
+        self.FileUrl = params.get("FileUrl")
+        self.MediaName = params.get("MediaName")
         if params.get("MetaData") is not None:
             self.MetaData = MediaMetaData()
             self.MetaData._deserialize(params.get("MetaData"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
```

### Comparing `tencentcloud-sdk-python-vod-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.879/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vod-3.0.878/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.879/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.879/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.878/setup.py` & `tencentcloud-sdk-python-vod-3.0.879/setup.py`

 * *Files identical despite different names*

