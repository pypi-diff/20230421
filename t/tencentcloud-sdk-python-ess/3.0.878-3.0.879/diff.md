# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.878.tar", last modified: Thu Apr 20 00:28:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.879.tar", last modified: Fri Apr 21 00:44:43 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.878.tar` & `tencentcloud-sdk-python-ess-3.0.879.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    49192 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23577 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   218030 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:28:40.000000 tencentcloud-sdk-python-ess-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    49192 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23577 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   219062 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:44:43.000000 tencentcloud-sdk-python-ess-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.878/README.rst` & `tencentcloud-sdk-python-ess-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.879/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.878/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.879/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -653,14 +653,24 @@
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
         :param IsFormType: 是否是表单域类型，默认不存在
         :type IsFormType: bool
         :param ComponentValue: 控件填充vaule，ComponentType和传入值类型对应关系：
 TEXT - 文本内容
 MULTI_LINE_TEXT - 文本内容
 CHECK_BOX - true/false
```

### Comparing `tencentcloud-sdk-python-ess-3.0.878/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.879/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.879/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.878/setup.py` & `tencentcloud-sdk-python-ess-3.0.879/setup.py`

 * *Files identical despite different names*

