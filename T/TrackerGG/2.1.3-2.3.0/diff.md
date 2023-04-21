# Comparing `tmp/TrackerGG-2.1.3.tar.gz` & `tmp/TrackerGG-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrackerGG-2.1.3.tar", last modified: Fri Apr  7 09:04:17 2023, max compression
+gzip compressed data, was "TrackerGG-2.3.0.tar", last modified: Fri Apr 21 13:35:00 2023, max compression
```

## Comparing `TrackerGG-2.1.3.tar` & `TrackerGG-2.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 09:04:17.591719 TrackerGG-2.1.3/
--rw-rw-rw-   0        0        0     1085 2023-03-28 13:34:09.000000 TrackerGG-2.1.3/LICENSE
--rw-rw-rw-   0        0        0     1425 2023-04-07 09:04:17.591719 TrackerGG-2.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2023-04-05 02:22:42.000000 TrackerGG-2.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 09:04:17.567718 TrackerGG-2.1.3/TrackerGG/
-drwxrwxrwx   0        0        0        0 2023-04-07 09:04:17.591719 TrackerGG-2.1.3/TrackerGG/Models/
--rw-rw-rw-   0        0        0      621 2023-04-04 05:52:53.000000 TrackerGG-2.1.3/TrackerGG/Models/__init__.py
--rw-rw-rw-   0        0        0     3911 2023-04-05 07:44:54.000000 TrackerGG-2.1.3/TrackerGG/Models/csgo.py
--rw-rw-rw-   0        0        0     1477 2023-03-28 12:55:38.000000 TrackerGG-2.1.3/TrackerGG/Models/platform.py
--rw-rw-rw-   0        0        0     1399 2023-04-03 04:45:05.000000 TrackerGG-2.1.3/TrackerGG/Models/segment.py
--rw-rw-rw-   0        0        0     2059 2023-03-28 23:34:08.000000 TrackerGG-2.1.3/TrackerGG/Models/user.py
--rw-rw-rw-   0        0        0      802 2023-04-04 13:02:49.000000 TrackerGG-2.1.3/TrackerGG/__init__.py
--rw-rw-rw-   0        0        0     2479 2023-04-07 08:50:04.000000 TrackerGG-2.1.3/TrackerGG/client.py
--rw-rw-rw-   0        0        0     3531 2023-04-07 08:57:00.000000 TrackerGG-2.1.3/TrackerGG/httpclient.py
--rw-rw-rw-   0        0        0      833 2023-04-04 13:15:48.000000 TrackerGG-2.1.3/TrackerGG/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:04:17.583719 TrackerGG-2.1.3/TrackerGG.egg-info/
--rw-rw-rw-   0        0        0     1425 2023-04-07 09:04:17.000000 TrackerGG-2.1.3/TrackerGG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-04-07 09:04:17.000000 TrackerGG-2.1.3/TrackerGG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 09:04:17.000000 TrackerGG-2.1.3/TrackerGG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-07 09:04:17.000000 TrackerGG-2.1.3/TrackerGG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-07 09:04:17.000000 TrackerGG-2.1.3/TrackerGG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 09:04:17.591719 TrackerGG-2.1.3/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-04-07 09:03:28.000000 TrackerGG-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:35:00.090427 TrackerGG-2.3.0/
+-rw-rw-rw-   0        0        0     1085 2023-03-28 13:34:09.000000 TrackerGG-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1425 2023-04-21 13:35:00.089427 TrackerGG-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1042 2023-04-05 02:22:42.000000 TrackerGG-2.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 13:35:00.042599 TrackerGG-2.3.0/TrackerGG/
+drwxrwxrwx   0        0        0        0 2023-04-21 13:35:00.087411 TrackerGG-2.3.0/TrackerGG/Models/
+-rw-rw-rw-   0        0        0      652 2023-04-21 13:21:48.000000 TrackerGG-2.3.0/TrackerGG/Models/__init__.py
+-rw-rw-rw-   0        0        0     4464 2023-04-21 13:26:31.000000 TrackerGG-2.3.0/TrackerGG/Models/csgo.py
+-rw-rw-rw-   0        0        0     1477 2023-03-28 12:55:38.000000 TrackerGG-2.3.0/TrackerGG/Models/platform.py
+-rw-rw-rw-   0        0        0     1399 2023-04-03 04:45:05.000000 TrackerGG-2.3.0/TrackerGG/Models/segment.py
+-rw-rw-rw-   0        0        0     2059 2023-03-28 23:34:08.000000 TrackerGG-2.3.0/TrackerGG/Models/user.py
+-rw-rw-rw-   0        0        0      802 2023-04-04 13:02:49.000000 TrackerGG-2.3.0/TrackerGG/__init__.py
+-rw-rw-rw-   0        0        0     3220 2023-04-21 13:26:44.000000 TrackerGG-2.3.0/TrackerGG/client.py
+-rw-rw-rw-   0        0        0     3531 2023-04-07 08:57:00.000000 TrackerGG-2.3.0/TrackerGG/httpclient.py
+-rw-rw-rw-   0        0        0      833 2023-04-04 13:15:48.000000 TrackerGG-2.3.0/TrackerGG/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:35:00.073608 TrackerGG-2.3.0/TrackerGG.egg-info/
+-rw-rw-rw-   0        0        0     1425 2023-04-21 13:34:59.000000 TrackerGG-2.3.0/TrackerGG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-04-21 13:34:59.000000 TrackerGG-2.3.0/TrackerGG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 13:34:59.000000 TrackerGG-2.3.0/TrackerGG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-21 13:34:59.000000 TrackerGG-2.3.0/TrackerGG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 13:34:59.000000 TrackerGG-2.3.0/TrackerGG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 13:35:00.091423 TrackerGG-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      655 2023-04-21 13:34:57.000000 TrackerGG-2.3.0/setup.py
```

### Comparing `TrackerGG-2.1.3/LICENSE` & `TrackerGG-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.1.3/PKG-INFO` & `TrackerGG-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrackerGG
-Version: 2.1.3
+Version: 2.3.0
 Summary: TrackerGG API Wrapper Library
 Home-page: https://github.com/dev-ruby/TrackerGG
 Author: DevRuby
 Author-email: hiveruby@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.3
```

### Comparing `TrackerGG-2.1.3/README.md` & `TrackerGG-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.1.3/TrackerGG/Models/__init__.py` & `TrackerGG-2.3.0/TrackerGG/Models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,7 +14,8 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 """
 
 from .csgo import CSGOProfile
 from .csgo import CSGOMapSegment
+from .csgo import CSGOQueryData
```

### Comparing `TrackerGG-2.1.3/TrackerGG/Models/csgo.py` & `TrackerGG-2.3.0/TrackerGG/Models/csgo.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 """
 from enum import Enum
-from typing import Dict, Any, List, Union
+from typing import Dict, Any, List, Union, Optional
 
 from .platform import PlatformInfo
 from .segment import Stat
 from .user import UserInfo
 
 
 class CSGOStats:
@@ -92,7 +92,18 @@
 
 class CSGOMap:
     def __init__(self, data: Dict[str, Union[str, dict]]):
         self.attributes: dict = data["attributes"]
         self.metadata: dict = data["metadata"]
         self.expiry_date: str = data["expiryDate"]
         self.stats: CSGOMapStats = CSGOMapStats(data["stats"])
+
+
+class CSGOQueryData:
+    def __init__(self, data: Dict[str, Optional[Union[str, int]]]):
+        self.platform_id = int(data["platformId"])
+        self.platform_user_id: Union[str, int] = data["platformUserId"]
+        self.platform_user_handle: str = data["platformUserHandle"]
+        self.platform_user_identifier: Union[str, int] = data["platformUserIdentifier"]
+        self.avatar_url: str = data["avatarUrl"]
+        self.additional_parameters: Any = data["additionalParameters"]
+        self.status: Any = data["status"]
```

### Comparing `TrackerGG-2.1.3/TrackerGG/Models/platform.py` & `TrackerGG-2.3.0/TrackerGG/Models/platform.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.1.3/TrackerGG/Models/segment.py` & `TrackerGG-2.3.0/TrackerGG/Models/segment.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.1.3/TrackerGG/Models/user.py` & `TrackerGG-2.3.0/TrackerGG/Models/user.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.1.3/TrackerGG/__init__.py` & `TrackerGG-2.3.0/TrackerGG/__init__.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.1.3/TrackerGG/client.py` & `TrackerGG-2.3.0/TrackerGG/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 """
 
 import asyncio
 import json
-from typing import List
+from typing import List, Union
 
 from .Models import CSGOProfile
 from .Models import CSGOMapSegment
+from .Models import CSGOQueryData
 from .httpclient import HTTPClient
 from .httpclient import RequestMethod
 from .httpclient import ResponseData
 from .httpclient import Route
 
 
 class TrackerClient:
@@ -73,7 +74,27 @@
 
         segments = []
 
         for segment in json_data["data"]:
             segments.append(CSGOMapSegment(segment))
 
         return segments
+
+    async def search_profile(self, query: str) -> Union[None, List[CSGOQueryData]]:
+        response: ResponseData = await self.http_client.request(
+            Route(RequestMethod.GET, f"/csgo/standard/search", params={"platform":"steam", "query":query})
+        )
+
+        assert response.status == 200, (
+                "HTTP Response Status Code is not 200\nStatus Code : %d" % response.status
+        )
+
+        json_data: dict = json.loads(response.response_data)
+
+        query_data = None
+
+        if json_data["data"]:
+            query_data = []
+            for dat in json_data["data"]:
+                query_data.append(CSGOQueryData(dat))
+
+        return query_data
```

### Comparing `TrackerGG-2.1.3/TrackerGG/httpclient.py` & `TrackerGG-2.3.0/TrackerGG/httpclient.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.1.3/TrackerGG/utils.py` & `TrackerGG-2.3.0/TrackerGG/utils.py`

 * *Files identical despite different names*

### Comparing `TrackerGG-2.1.3/TrackerGG.egg-info/PKG-INFO` & `TrackerGG-2.3.0/TrackerGG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrackerGG
-Version: 2.1.3
+Version: 2.3.0
 Summary: TrackerGG API Wrapper Library
 Home-page: https://github.com/dev-ruby/TrackerGG
 Author: DevRuby
 Author-email: hiveruby@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.3
```

### Comparing `TrackerGG-2.1.3/setup.py` & `TrackerGG-2.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fs:
     long_description = fs.read()
 
 setuptools.setup(
     name="TrackerGG",
-    version="2.1.3",
+    version="2.3.0",
     author="DevRuby",
     author_email="hiveruby@gmail.com",
     description="TrackerGG API Wrapper Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dev-ruby/TrackerGG",
     packages=setuptools.find_packages(),
```

