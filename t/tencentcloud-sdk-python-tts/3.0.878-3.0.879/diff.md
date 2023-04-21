# Comparing `tmp/tencentcloud-sdk-python-tts-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-tts-3.0.879.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.878.tar", last modified: Thu Apr 20 00:55:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.879.tar", last modified: Fri Apr 21 01:08:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tts-3.0.878.tar` & `tencentcloud-sdk-python-tts-3.0.879.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/
--rw-r--r--   0 root         (0) root         (0)     5481 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19249 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)     5910 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/tts_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud_sdk_python_tts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/tencentcloud_sdk_python_tts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:55:21.000000 tencentcloud-sdk-python-tts-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/
+-rw-r--r--   0 root         (0) root         (0)     5481 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20734 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)     5910 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/tts_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud_sdk_python_tts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud_sdk_python_tts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tts-3.0.878/README.rst` & `tencentcloud-sdk-python-tts-3.0.879/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/errorcodes.py` & `tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/models.py` & `tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -286,26 +286,56 @@
         :param ModelType: 模型类型，1-默认模型。
         :type ModelType: int
         :param VoiceType: 标准音色<li>10510000-智逍遥，阅读男声</li><li>1001-智瑜，情感女声</li><li>1002-智聆，通用女声</li><li>1003-智美，客服女声</li><li>1004-智云，通用男声</li><li>1005-智莉，通用女声</li><li>1007-智娜，客服女声</li><li>1008-智琪，客服女声</li><li>1009-智芸，知性女声</li><li>1010-智华，通用男声</li><li>1017-智蓉，情感女声</li><li>1018-智靖，情感男声</li><li>1050-WeJack，英文男声</li><li>1051-WeRose，英文女声</li>精品音色<br>精品音色拟真度更高，价格不同于标准音色，查看[购买指南](https://cloud.tencent.com/document/product/1073/34112)<br><li>100510000-智逍遥，阅读男声</li><li>101001-智瑜，情感女声</li><li>101002-智聆，通用女声</li><li>101003-智美，客服女声</li><li>101004-智云，通用男声</li><li>101005-智莉，通用女声</li><li>101006-智言，助手女声</li><li>101007-智娜，客服女声</li><li>101008-智琪，客服女声</li><li>101009-智芸，知性女声</li><li>101010-智华，通用男声</li><li>101011-智燕，新闻女声</li><li>101012-智丹，新闻女声</li><li>101013-智辉，新闻男声</li><li>101014-智宁，新闻男声</li><li>101015-智萌，男童声</li><li>101016-智甜，女童声</li><li>101017-智蓉，情感女声</li><li>101018-智靖，情感男声</li><li>101019-智彤，粤语女声</li><li>101020-智刚，新闻男声</li><li>101021-智瑞，新闻男声</li><li>101022-智虹，新闻女声</li><li>101023-智萱，聊天女声</li><li>101024-智皓，聊天男声</li><li>101025-智薇，聊天女声</li><li>101026-智希，通用女声</li><li>101027-智梅，通用女声</li><li>101028-智洁，通用女声</li><li>101029-智凯，通用男声</li><li>101030-智柯，通用男声</li><li>101031-智奎，通用男声</li><li>101032-智芳，通用女声</li><li>101033-智蓓，客服女声</li><li>101034-智莲，通用女声</li><li>101035-智依，通用女声</li><li>101040-智川，四川女声</li><li>101050-WeJack，英文男声</li><li>101051-WeRose，英文女声</li><li>101052-智味，通用男声</li>
 <li>101053-智方，通用男声</li>
 <li>101054-智友，通用男声</li>
 <li>101055-智付，通用女声</li>
 <li>101056-智林，东北男声</li>
+<li>301000-爱小广，多情感通用男声</li>
+<li>301001-爱小栋，多情感通用男声</li>
+<li>301002-爱小海，多情感通用男声</li>
+<li>301003-爱小霞，多情感通用女声</li>
+<li>301004-爱小玲，多情感通用女声</li>
+<li>301005-爱小章，多情感通用男声</li>
+<li>301006-爱小峰，多情感通用男声</li>
+<li>301007-爱小亮，多情感通用男声</li>
+<li>301008-爱小博，多情感通用男声</li>
+<li>301009-爱小芸，多情感通用女声</li>
+<li>301010-爱小秋，多情感通用女声</li>
+<li>301011-爱小芳，多情感通用女声</li>
+<li>301012-爱小琴，多情感通用女声</li>
+<li>301013-爱小康，多情感通用男声</li>
+<li>301014-爱小辉，多情感通用男声</li>
+<li>301015-爱小璐，多情感通用女声</li>
+<li>301016-爱小阳，多情感通用男声</li>
+<li>301017-爱小泉，多情感通用男声</li>
+<li>301018-爱小昆，多情感通用男声</li>
+<li>301019-爱小诚，多情感通用男声</li>
+<li>301020-爱小岚，多情感通用女声</li>
+<li>301021-爱小茹，多情感通用女声</li>
+<li>301022-爱小蓉，多情感通用女声</li>
+<li>301023-爱小燕，多情感通用女声</li>
+<li>301024-爱小莲，多情感通用女声</li>
+<li>301025-爱小武，多情感通用男声</li>
+<li>301026-爱小雪，多情感通用女声</li>
+<li>301027-爱小媛，多情感通用女声</li>
+<li>301028-爱小娴，多情感通用女声</li>
+<li>301029-爱小涛，多情感通用男声</li>
         :type VoiceType: int
         :param PrimaryLanguage: 主语言类型：<li>1-中文（默认）</li><li>2-英文</li>
         :type PrimaryLanguage: int
         :param SampleRate: 音频采样率：<li>16000：16k（默认）</li><li>8000：8k</li>
         :type SampleRate: int
         :param Codec: 返回音频格式，可取值：wav（默认），mp3，pcm
         :type Codec: str
         :param EnableSubtitle: 是否开启时间戳功能，默认为false。
         :type EnableSubtitle: bool
         :param SegmentRate: 断句敏感阈值，默认值为：0，取值范围：[0,1,2]。该值越大越不容易断句，模型会更倾向于仅按照标点符号断句。此参数建议不要随意调整，可能会影响合成效果。
         :type SegmentRate: int
-        :param EmotionCategory: 控制合成音频的情感，仅支持情绪音色使用。取值: peaceful、exciting、thrill、neutral、sad、angry、cute、fear、poetry、happy、regretful、exciting_strong、aojiao、sajiao、story、raido、call、jieshuo等等；
+        :param EmotionCategory: 控制合成音频的情感，仅支持多情感音色使用。取值: neutral(中性)、sad(悲伤)、happy(高兴)、angry(生气)、fear(恐惧)、news(新闻)、story(故事)、radio(广播)、poetry(诗歌)、call(客服)
         :type EmotionCategory: str
         :param EmotionIntensity: 控制合成音频情感程度，取值范围为[50,200],默认为100，不填写为默认值；只有EmotionCategory不为空时生效；
         :type EmotionIntensity: int
         """
         self.Text = None
         self.SessionId = None
         self.Volume = None
```

### Comparing `tencentcloud-sdk-python-tts-3.0.878/tencentcloud/tts/v20190823/tts_client.py` & `tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/tts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tts-3.0.879/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tts-3.0.878/tencentcloud_sdk_python_tts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.879/tencentcloud_sdk_python_tts.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.879/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.878
+Version: 3.0.879
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.878/setup.py` & `tencentcloud-sdk-python-tts-3.0.879/setup.py`

 * *Files identical despite different names*

