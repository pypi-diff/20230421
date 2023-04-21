# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.877.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.877.tar", last modified: Wed Apr 19 09:16:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.879.tar", last modified: Fri Apr 21 00:44:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.877.tar` & `tencentcloud-sdk-python-essbasic-3.0.879.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    15377 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    50151 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   228153 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-19 09:16:47.000000 tencentcloud-sdk-python-essbasic-3.0.877/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    15377 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    50151 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   229475 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:44:51.000000 tencentcloud-sdk-python-essbasic-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.877
+Version: 3.0.879
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.877/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.877'
+__version__ = '3.0.879'
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2379,14 +2379,24 @@
 {“ComponentTypeLimit”: [“xxx”]}
 xxx可以为：
 HANDWRITE – 手写签名
 BORDERLESS_ESIGN – 自动生成无边框腾讯体
 OCR_ESIGN -- AI智能识别手写签名
 ESIGN -- 个人印章类型
 如：{“ComponentTypeLimit”: [“BORDERLESS_ESIGN”]}
+
+ComponentType为SIGN_DATE时，支持以下参数：
+1 Font：字符串类型目前只支持"黑体"、"宋体"，如果不填默认为"黑体"
+2 FontSize： 数字类型，范围6-72，默认值为12
+3 FontAlign： 字符串类型，可取Left/Right/Center，对应左对齐/居中/右对齐
+4 Format： 字符串类型，日期格式，必须是以下五种之一 “yyyy m d”，”yyyy年m月d日”，”yyyy/m/d”，”yyyy-m-d”，”yyyy.m.d”。
+5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙钟的空格个数
+如果extra参数为空，默认为”yyyy年m月d日”格式的居中日期
+特别地，如果extra中Format字段为空或无法被识别，则extra参数会被当作默认值处理（Font，FontSize，Gaps和FontAlign都不会起效）
+参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}",
         :type ComponentExtra: str
         :param ComponentValue: 控件填充vaule，ComponentType和传入值类型对应关系：
 TEXT - 文本内容
 MULTI_LINE_TEXT - 文本内容
 CHECK_BOX - true/false
 FILL_IMAGE、ATTACHMENT - 附件的FileId，需要通过UploadFiles接口上传获取
 SELECTOR - 选项值
@@ -4659,17 +4669,17 @@
 class PdfVerifyResult(AbstractModel):
     """合同文件验签单个结果结构体
 
     """
 
     def __init__(self):
         r"""
-        :param VerifyResult: 验签结果
+        :param VerifyResult: 验签结果。0-签名域未签名；1-验签成功； 3-验签失败；4-未找到签名域：文件内没有签名域；5-签名值格式不正确。
         :type VerifyResult: int
-        :param SignPlatform: 签署平台
+        :param SignPlatform: 签署平台，如果文件是在腾讯电子签平台签署，则返回腾讯电子签，如果文件不在腾讯电子签平台签署，则返回其他平台。
         :type SignPlatform: str
         :param SignerName: 签署人名称
         :type SignerName: str
         :param SignTime: 签署时间
         :type SignTime: int
         :param SignAlgorithm: 签名算法
         :type SignAlgorithm: str
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.877/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.879/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.877/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.879/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.877
+Version: 3.0.879
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.877/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.879/setup.py`

 * *Files identical despite different names*

