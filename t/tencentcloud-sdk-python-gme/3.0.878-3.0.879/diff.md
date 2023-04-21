# Comparing `tmp/tencentcloud-sdk-python-gme-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-gme-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-gme-3.0.878.tar", last modified: Thu Apr 20 00:32:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-gme-3.0.879.tar", last modified: Fri Apr 21 00:45:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-gme-3.0.878.tar` & `tencentcloud-sdk-python-gme-3.0.879.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/tencentcloud/gme/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/tencentcloud/gme/v20180711/
--rw-r--r--   0 root         (0) root         (0)    33250 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/tencentcloud/gme/v20180711/gme_client.py
--rw-r--r--   0 root         (0) root         (0)     3906 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/tencentcloud/gme/v20180711/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/tencentcloud/gme/v20180711/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104423 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/tencentcloud/gme/v20180711/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/tencentcloud/gme/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/tencentcloud_sdk_python_gme.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/tencentcloud_sdk_python_gme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/tencentcloud_sdk_python_gme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/tencentcloud_sdk_python_gme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/tencentcloud_sdk_python_gme.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:32:54.000000 tencentcloud-sdk-python-gme-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:45:35.000000 tencentcloud-sdk-python-gme-3.0.879/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 00:45:34.000000 tencentcloud-sdk-python-gme-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:45:35.000000 tencentcloud-sdk-python-gme-3.0.879/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:45:34.000000 tencentcloud-sdk-python-gme-3.0.879/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:45:35.000000 tencentcloud-sdk-python-gme-3.0.879/tencentcloud/gme/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:45:35.000000 tencentcloud-sdk-python-gme-3.0.879/tencentcloud/gme/v20180711/
+-rw-r--r--   0 root         (0) root         (0)    33250 2023-04-21 00:45:34.000000 tencentcloud-sdk-python-gme-3.0.879/tencentcloud/gme/v20180711/gme_client.py
+-rw-r--r--   0 root         (0) root         (0)     3906 2023-04-21 00:45:34.000000 tencentcloud-sdk-python-gme-3.0.879/tencentcloud/gme/v20180711/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:45:34.000000 tencentcloud-sdk-python-gme-3.0.879/tencentcloud/gme/v20180711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104900 2023-04-21 00:45:34.000000 tencentcloud-sdk-python-gme-3.0.879/tencentcloud/gme/v20180711/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:45:34.000000 tencentcloud-sdk-python-gme-3.0.879/tencentcloud/gme/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:45:35.000000 tencentcloud-sdk-python-gme-3.0.879/tencentcloud_sdk_python_gme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:45:35.000000 tencentcloud-sdk-python-gme-3.0.879/tencentcloud_sdk_python_gme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 00:45:35.000000 tencentcloud-sdk-python-gme-3.0.879/tencentcloud_sdk_python_gme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:45:35.000000 tencentcloud-sdk-python-gme-3.0.879/tencentcloud_sdk_python_gme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:45:35.000000 tencentcloud-sdk-python-gme-3.0.879/tencentcloud_sdk_python_gme.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:45:35.000000 tencentcloud-sdk-python-gme-3.0.879/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 00:45:34.000000 tencentcloud-sdk-python-gme-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:45:35.000000 tencentcloud-sdk-python-gme-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-gme-3.0.878/README.rst` & `tencentcloud-sdk-python-gme-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-gme-3.0.879/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-gme-3.0.878/tencentcloud/gme/v20180711/gme_client.py` & `tencentcloud-sdk-python-gme-3.0.879/tencentcloud/gme/v20180711/gme_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.878/tencentcloud/gme/v20180711/errorcodes.py` & `tencentcloud-sdk-python-gme-3.0.879/tencentcloud/gme/v20180711/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gme-3.0.878/tencentcloud/gme/v20180711/models.py` & `tencentcloud-sdk-python-gme-3.0.879/tencentcloud/gme/v20180711/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,33 +439,38 @@
     def __init__(self):
         r"""
         :param AppName: 应用名称
         :type AppName: str
         :param ProjectId: 腾讯云项目ID，默认为0，表示默认项目
         :type ProjectId: int
         :param EngineList: 需要支持的引擎列表，默认全选。
+取值：android/ios/unity/cocos/unreal/windows
         :type EngineList: list of str
         :param RegionList: 服务区域列表，默认全选。
+取值：mainland-大陆地区，hmt-港澳台，sea-东南亚，na-北美，eu-欧洲，jpkr-日韩亚太，sa-南美，oc-澳洲，me-中东
         :type RegionList: list of str
         :param RealtimeSpeechConf: 实时语音服务配置数据
         :type RealtimeSpeechConf: :class:`tencentcloud.gme.v20180711.models.RealtimeSpeechConf`
-        :param VoiceMessageConf: 语音消息及转文本服务配置数据
+        :param VoiceMessageConf: 语音消息服务配置数据
         :type VoiceMessageConf: :class:`tencentcloud.gme.v20180711.models.VoiceMessageConf`
         :param VoiceFilterConf: 语音分析服务配置数据
         :type VoiceFilterConf: :class:`tencentcloud.gme.v20180711.models.VoiceFilterConf`
+        :param AsrConf: 语音转文本配置数据
+        :type AsrConf: :class:`tencentcloud.gme.v20180711.models.AsrConf`
         :param Tags: 需要添加的标签列表
         :type Tags: list of Tag
         """
         self.AppName = None
         self.ProjectId = None
         self.EngineList = None
         self.RegionList = None
         self.RealtimeSpeechConf = None
         self.VoiceMessageConf = None
         self.VoiceFilterConf = None
+        self.AsrConf = None
         self.Tags = None
 
 
     def _deserialize(self, params):
         self.AppName = params.get("AppName")
         self.ProjectId = params.get("ProjectId")
         self.EngineList = params.get("EngineList")
@@ -475,14 +480,17 @@
             self.RealtimeSpeechConf._deserialize(params.get("RealtimeSpeechConf"))
         if params.get("VoiceMessageConf") is not None:
             self.VoiceMessageConf = VoiceMessageConf()
             self.VoiceMessageConf._deserialize(params.get("VoiceMessageConf"))
         if params.get("VoiceFilterConf") is not None:
             self.VoiceFilterConf = VoiceFilterConf()
             self.VoiceFilterConf._deserialize(params.get("VoiceFilterConf"))
+        if params.get("AsrConf") is not None:
+            self.AsrConf = AsrConf()
+            self.AsrConf._deserialize(params.get("AsrConf"))
         if params.get("Tags") is not None:
             self.Tags = []
             for item in params.get("Tags"):
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tags.append(obj)
         memeber_set = set(params.keys())
```

### Comparing `tencentcloud-sdk-python-gme-3.0.878/tencentcloud_sdk_python_gme.egg-info/PKG-INFO` & `tencentcloud-sdk-python-gme-3.0.879/tencentcloud_sdk_python_gme.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gme
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Gme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gme-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-gme-3.0.879/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gme
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Gme SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gme-3.0.878/setup.py` & `tencentcloud-sdk-python-gme-3.0.879/setup.py`

 * *Files identical despite different names*

